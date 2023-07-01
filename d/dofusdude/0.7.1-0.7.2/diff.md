# Comparing `tmp/dofusdude-0.7.1.tar.gz` & `tmp/dofusdude-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dofusdude-0.7.1.tar", last modified: Sat Dec 10 14:55:30 2022, max compression
+gzip compressed data, was "dofusdude-0.7.2.tar", last modified: Sat Jul  1 18:25:42 2023, max compression
```

## Comparing `dofusdude-0.7.1.tar` & `dofusdude-0.7.2.tar`

### file list

```diff
@@ -1,410 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.863485 dofusdude-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2022-12-10 14:55:30.863485 dofusdude-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26825 2022-12-10 14:55:20.000000 dofusdude-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.807485 dofusdude-0.7.1/dofusdude/
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62489 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.807485 dofusdude-0.7.1/dofusdude/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/path_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.819485 dofusdude-0.7.1/dofusdude/apis/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/dofus2_language_almanax.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/dofus2_language_almanax_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/dofus2_meta_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/dofus2_meta_language_almanax_bonuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_consumables.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_consumables_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_consumables_ankama_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_consumables_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_cosmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_cosmetics_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_cosmetics_ankama_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_cosmetics_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_equipment.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_equipment_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_equipment_ankama_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_equipment_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_quest.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_quest_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_quest_ankama_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_quest_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_resources_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_resources_ankama_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_resources_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_items_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_mounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_mounts_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_mounts_ankama_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_mounts_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_sets_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_sets_ankama_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/game_language_sets_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/meta_webhooks_almanax.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/meta_webhooks_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/meta_webhooks_twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/webhooks_almanax.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/webhooks_almanax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/webhooks_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/webhooks_rss_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/webhooks_twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/paths/webhooks_twitter_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tag_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.823485 dofusdude-0.7.1/dofusdude/apis/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/all_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/almanax_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/consumables_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/cosmetics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/equipment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/meta_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/mounts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/quest_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/sets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/apis/tags/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19187 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.831485 dofusdude-0.7.1/dofusdude/model/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22087 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/almanax_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    31306 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/almanax_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/condition_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16145 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/cosmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32497 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/create_almanax_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/create_rss_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/create_twitter_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/effects_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    20218 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/equipment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/equipment_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/image_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/item_list_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11407 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/items_list_entry_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/items_list_paged.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/links_paged.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/mount_list_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/mounts_list_paged.py
--rw-r--r--   0 runner    (1001) docker     (123)    31299 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/put_almanax_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/put_rss_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/put_twitter_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/recipe_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16145 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    14594 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/rss_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/set_list_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/sets_list_paged.py
--rw-r--r--   0 runner    (1001) docker     (123)    14613 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/twitter_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    26782 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/model/weapon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.831485 dofusdude-0.7.1/dofusdude/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.831485 dofusdude-0.7.1/dofusdude/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.831485 dofusdude-0.7.1/dofusdude/paths/dofus2_language_almanax/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/dofus2_language_almanax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/dofus2_language_almanax/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.831485 dofusdude-0.7.1/dofusdude/paths/dofus2_language_almanax_date/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/dofus2_language_almanax_date/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/dofus2_language_almanax_date/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/dofus2_meta_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/dofus2_meta_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/dofus2_meta_elements/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/dofus2_meta_language_almanax_bonuses/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/dofus2_meta_language_almanax_bonuses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13438 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/dofus2_meta_language_almanax_bonuses/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_all/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_all/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_ankama_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_search/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16183 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_consumables_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17626 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_all/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17371 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_all/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_ankama_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_search/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16094 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_cosmetics_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19355 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_all/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17502 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_all/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_ankama_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_search/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16159 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_equipment_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.835485 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17899 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_all/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17644 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_all/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_ankama_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_search/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_quest_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17941 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_all/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_all/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_ankama_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_search/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_resources_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_items_search/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16136 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_items_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_mounts/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_mounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15789 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_mounts/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_all/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16024 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_all/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.839485 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_ankama_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_search/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_mounts_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/game_language_sets/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_sets/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/game_language_sets_all/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_sets_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_sets_all/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/game_language_sets_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_sets_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_sets_ankama_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/game_language_sets_search/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_sets_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15925 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/game_language_sets_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_almanax/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_almanax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_almanax/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_rss/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_rss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_rss/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_twitter/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/meta_webhooks_twitter/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/webhooks_almanax/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_almanax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_almanax/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/webhooks_almanax_id/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_almanax_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_almanax_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_almanax_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_almanax_id/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.843485 dofusdude-0.7.1/dofusdude/paths/webhooks_rss/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_rss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_rss/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.847485 dofusdude-0.7.1/dofusdude/paths/webhooks_rss_id/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_rss_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_rss_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_rss_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_rss_id/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.847485 dofusdude-0.7.1/dofusdude/paths/webhooks_twitter/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_twitter/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.847485 dofusdude-0.7.1/dofusdude/paths/webhooks_twitter_id/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_twitter_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_twitter_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_twitter_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/paths/webhooks_twitter_id/put.py
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)   101660 2022-12-10 14:55:20.000000 dofusdude-0.7.1/dofusdude/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.807485 dofusdude-0.7.1/dofusdude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2022-12-10 14:55:30.000000 dofusdude-0.7.1/dofusdude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15608 2022-12-10 14:55:30.000000 dofusdude-0.7.1/dofusdude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 14:55:30.000000 dofusdude-0.7.1/dofusdude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-10 14:55:30.000000 dofusdude-0.7.1/dofusdude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-10 14:55:30.000000 dofusdude-0.7.1/dofusdude.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-10 14:55:30.863485 dofusdude-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9191 2022-12-10 14:55:20.000000 dofusdude-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.795485 dofusdude-0.7.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.851485 dofusdude-0.7.1/test/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_almanax_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_almanax_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_condition_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_cosmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_create_almanax_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_create_rss_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_create_twitter_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_effects_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_equipment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_equipment_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_image_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_item_list_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_items_list_entry_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_items_list_paged.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_links_paged.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_mount_list_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_mounts_list_paged.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_put_almanax_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_put_rss_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_put_twitter_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_recipe_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_rss_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_set_list_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_sets_list_paged.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_twitter_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_models/test_weapon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.851485 dofusdude-0.7.1/test/test_paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.851485 dofusdude-0.7.1/test/test_paths/test_dofus2_language_almanax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_dofus2_language_almanax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_dofus2_language_almanax/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.851485 dofusdude-0.7.1/test/test_paths/test_dofus2_language_almanax_date/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_dofus2_language_almanax_date/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_dofus2_language_almanax_date/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.851485 dofusdude-0.7.1/test/test_paths/test_dofus2_meta_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_dofus2_meta_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_dofus2_meta_elements/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.851485 dofusdude-0.7.1/test/test_paths/test_dofus2_meta_language_almanax_bonuses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_dofus2_meta_language_almanax_bonuses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_dofus2_meta_language_almanax_bonuses/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.851485 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.851485 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_all/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_ankama_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_consumables_search/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_all/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_ankama_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_cosmetics_search/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_all/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_ankama_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_equipment_search/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_all/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_ankama_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_quest_search/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_all/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.855485 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_ankama_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_resources_search/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_items_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_items_search/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_mounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_mounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_mounts/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_all/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_ankama_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_mounts_search/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_sets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_sets/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_sets_all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_sets_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_sets_all/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_sets_ankama_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_sets_ankama_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_sets_ankama_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_game_language_sets_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_sets_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_game_language_sets_search/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_almanax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_almanax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_almanax/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_rss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_rss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_rss/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_twitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_meta_webhooks_twitter/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.859485 dofusdude-0.7.1/test/test_paths/test_webhooks_almanax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_almanax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_almanax/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.863485 dofusdude-0.7.1/test/test_paths/test_webhooks_almanax_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_almanax_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_almanax_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_almanax_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_almanax_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.863485 dofusdude-0.7.1/test/test_paths/test_webhooks_rss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_rss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_rss/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.863485 dofusdude-0.7.1/test/test_paths/test_webhooks_rss_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_rss_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_rss_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_rss_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_rss_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.863485 dofusdude-0.7.1/test/test_paths/test_webhooks_twitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_twitter/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:30.863485 dofusdude-0.7.1/test/test_paths/test_webhooks_twitter_id/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_twitter_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_twitter_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_twitter_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-10 14:55:20.000000 dofusdude-0.7.1/test/test_paths/test_webhooks_twitter_id/test_put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:25:42.660950 dofusdude-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-01 18:25:42.660950 dofusdude-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16458 2023-07-01 18:25:30.000000 dofusdude-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:25:42.644949 dofusdude-0.7.2/dofusdude/
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:25:42.648949 dofusdude-0.7.2/dofusdude/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/all_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22950 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/almanax_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45631 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/consumables_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45365 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/cosmetics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45593 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/equipment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17261 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/meta_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39292 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/mounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45583 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/quest_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45718 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45327 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/sets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95878 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:25:42.652949 dofusdude-0.7.2/dofusdude/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/almanax_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/almanax_entry_bonus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/almanax_entry_tribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/almanax_entry_tribute_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/almanax_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/almanax_webhook_daily_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/condition_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/condition_entry_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/cosmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/cosmetic_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/create_almanax_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/create_almanax_webhook_daily_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/create_almanax_webhook_mentions_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/create_rss_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/create_twitter_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/effects_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/effects_entry_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/equipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/equipment_parent_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/equipment_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/get_meta_almanax_bonuses200_response_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/get_meta_webhooks_twitter200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/image_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/item_list_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/items_list_entry_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/items_list_entry_typed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/items_list_paged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/links_paged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/mount_list_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/mounts_list_paged.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/put_almanax_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/put_rss_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/put_twitter_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/recipe_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/rss_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/set_list_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/sets_list_paged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/twitter_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/weapon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/models/weapon_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-07-01 18:25:30.000000 dofusdude-0.7.2/dofusdude/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:25:42.644949 dofusdude-0.7.2/dofusdude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-01 18:25:42.000000 dofusdude-0.7.2/dofusdude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-01 18:25:42.000000 dofusdude-0.7.2/dofusdude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:25:42.000000 dofusdude-0.7.2/dofusdude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-01 18:25:42.000000 dofusdude-0.7.2/dofusdude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 18:25:42.000000 dofusdude-0.7.2/dofusdude.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-01 18:25:30.000000 dofusdude-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 18:25:42.660950 dofusdude-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-07-01 18:25:30.000000 dofusdude-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:25:42.660950 dofusdude-0.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_all_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_almanax_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_almanax_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_almanax_entry_bonus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_almanax_entry_tribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_almanax_entry_tribute_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_almanax_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_almanax_webhook_daily_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_condition_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_condition_entry_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_consumables_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_cosmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_cosmetic_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_cosmetics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_create_almanax_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_create_almanax_webhook_daily_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_create_almanax_webhook_mentions_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_create_rss_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_create_twitter_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_effects_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_effects_entry_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_equipment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_equipment_parent_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_equipment_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_get_meta_almanax_bonuses200_response_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_get_meta_webhooks_twitter200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_image_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_item_list_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_items_list_entry_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_items_list_entry_typed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_items_list_paged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_links_paged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_meta_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_mount_list_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_mounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_mounts_list_paged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_put_almanax_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_put_rss_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_put_twitter_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_quest_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_recipe_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_rss_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_set_list_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_sets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_sets_list_paged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_twitter_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_weapon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_weapon_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-01 18:25:30.000000 dofusdude-0.7.2/test/test_webhooks_api.py
```

### Comparing `dofusdude-0.7.1/PKG-INFO` & `dofusdude-0.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dofusdude
-Version: 0.7.1
+Version: 0.7.2
 Summary: Dofusdude
 Home-page: https://github.com/dofusdude/dofusdude-py
 Author: Survival
 Author-email: stelzo@steado.de
 Keywords: OpenAPI,OpenAPI-Generator,Dofusdude
-Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don&#x27;t write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don&#39;t write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
```

### Comparing `dofusdude-0.7.1/dofusdude/__init__.py` & `dofusdude-0.7.2/dofusdude.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-# coding: utf-8
+Metadata-Version: 2.1
+Name: dofusdude
+Version: 0.7.2
+Summary: Dofusdude
+Home-page: https://github.com/dofusdude/dofusdude-py
+Author: Survival
+Author-email: stelzo@steado.de
+Keywords: OpenAPI,OpenAPI-Generator,Dofusdude
+Description-Content-Type: text/markdown
 
-# flake8: noqa
-
-"""
-    Dofusdude
-
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
-
-    The version of the OpenAPI document: 0.7.1
-    Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
-
-__version__ = "0.7.1"
-
-# import ApiClient
-from dofusdude.api_client import ApiClient
-
-# import Configuration
-from dofusdude.configuration import Configuration
-
-# import exceptions
-from dofusdude.exceptions import OpenApiException
-from dofusdude.exceptions import ApiAttributeError
-from dofusdude.exceptions import ApiTypeError
-from dofusdude.exceptions import ApiValueError
-from dofusdude.exceptions import ApiKeyError
-from dofusdude.exceptions import ApiException
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don&#39;t write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/all_items_api.py` & `dofusdude-0.7.2/test/test_all_items_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.game_language_items_search.get import GetItemsAllSearch
 
+import unittest
 
-class AllItemsApi(
-    GetItemsAllSearch,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.api.all_items_api import AllItemsApi  # noqa: E501
+from dofusdude.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestAllItemsApi(unittest.TestCase):
+    """AllItemsApi unit test stubs"""
+
+    def setUp(self):
+        self.api = dofusdude.api.all_items_api.AllItemsApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_get_items_all_search(self):
+        """Test case for get_items_all_search
+
+        Search All Items  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/almanax_api.py` & `dofusdude-0.7.2/test/test_almanax_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,48 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.dofus2_language_almanax_date.get import GetAlmanaxDate
-from dofusdude.paths.dofus2_language_almanax.get import GetAlmanaxRange
 
+import unittest
 
-class AlmanaxApi(
-    GetAlmanaxDate,
-    GetAlmanaxRange,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.api.almanax_api import AlmanaxApi  # noqa: E501
+from dofusdude.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestAlmanaxApi(unittest.TestCase):
+    """AlmanaxApi unit test stubs"""
+
+    def setUp(self):
+        self.api = dofusdude.api.almanax_api.AlmanaxApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_get_almanax_date(self):
+        """Test case for get_almanax_date
+
+        Single Almanax Date  # noqa: E501
+        """
+        pass
+
+    def test_get_almanax_range(self):
+        """Test case for get_almanax_range
+
+        Almanax Range  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/consumables_api.py` & `dofusdude-0.7.2/test/test_meta_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.game_language_items_consumables_all.get import GetAllItemsConsumablesList
-from dofusdude.paths.game_language_items_consumables.get import GetItemsConsumablesList
-from dofusdude.paths.game_language_items_consumables_search.get import GetItemsConsumablesSearch
-from dofusdude.paths.game_language_items_consumables_ankama_id.get import GetItemsConsumablesSingle
 
+import unittest
 
-class ConsumablesApi(
-    GetAllItemsConsumablesList,
-    GetItemsConsumablesList,
-    GetItemsConsumablesSearch,
-    GetItemsConsumablesSingle,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.api.meta_api import MetaApi  # noqa: E501
+from dofusdude.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestMetaApi(unittest.TestCase):
+    """MetaApi unit test stubs"""
+
+    def setUp(self):
+        self.api = dofusdude.api.meta_api.MetaApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_get_meta_almanax_bonuses(self):
+        """Test case for get_meta_almanax_bonuses
+
+        Available Almanax Bonuses  # noqa: E501
+        """
+        pass
+
+    def test_get_meta_elements(self):
+        """Test case for get_meta_elements
+
+        Effects and Condition Elements  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/cosmetics_api.py` & `dofusdude-0.7.2/test/test_cosmetics_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,62 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.game_language_items_cosmetics_all.get import GetAllCosmeticsList
-from dofusdude.paths.game_language_items_cosmetics.get import GetCosmeticsList
-from dofusdude.paths.game_language_items_cosmetics_search.get import GetCosmeticsSearch
-from dofusdude.paths.game_language_items_cosmetics_ankama_id.get import GetCosmeticsSingle
 
+import unittest
 
-class CosmeticsApi(
-    GetAllCosmeticsList,
-    GetCosmeticsList,
-    GetCosmeticsSearch,
-    GetCosmeticsSingle,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.api.cosmetics_api import CosmeticsApi  # noqa: E501
+from dofusdude.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestCosmeticsApi(unittest.TestCase):
+    """CosmeticsApi unit test stubs"""
+
+    def setUp(self):
+        self.api = dofusdude.api.cosmetics_api.CosmeticsApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_get_all_cosmetics_list(self):
+        """Test case for get_all_cosmetics_list
+
+        List All Cosmetics  # noqa: E501
+        """
+        pass
+
+    def test_get_cosmetics_list(self):
+        """Test case for get_cosmetics_list
+
+        List Cosmetics  # noqa: E501
+        """
+        pass
+
+    def test_get_cosmetics_search(self):
+        """Test case for get_cosmetics_search
+
+        Search Cosmetics  # noqa: E501
+        """
+        pass
+
+    def test_get_cosmetics_single(self):
+        """Test case for get_cosmetics_single
+
+        Single Cosmetics  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/equipment_api.py` & `dofusdude-0.7.2/test/test_image_urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,58 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.game_language_items_equipment_all.get import GetAllItemsEquipmentList
-from dofusdude.paths.game_language_items_equipment.get import GetItemsEquipmentList
-from dofusdude.paths.game_language_items_equipment_search.get import GetItemsEquipmentSearch
-from dofusdude.paths.game_language_items_equipment_ankama_id.get import GetItemsEquipmentSingle
 
+import unittest
+import datetime
 
-class EquipmentApi(
-    GetAllItemsEquipmentList,
-    GetItemsEquipmentList,
-    GetItemsEquipmentSearch,
-    GetItemsEquipmentSingle,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.models.image_urls import ImageUrls  # noqa: E501
+from dofusdude.rest import ApiException
+
+class TestImageUrls(unittest.TestCase):
+    """ImageUrls unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ImageUrls
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ImageUrls`
+        """
+        model = dofusdude.models.image_urls.ImageUrls()  # noqa: E501
+        if include_optional :
+            return ImageUrls(
+                icon = '', 
+                sd = '', 
+                hq = '', 
+                hd = ''
+            )
+        else :
+            return ImageUrls(
+        )
+        """
+
+    def testImageUrls(self):
+        """Test ImageUrls"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
-    Do not edit the class manually.
-    """
-    pass
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/meta_api.py` & `dofusdude-0.7.2/test/test_resources_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,62 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.dofus2_meta_language_almanax_bonuses.get import GetMetaAlmanaxBonuses
-from dofusdude.paths.dofus2_meta_elements.get import GetMetaElements
 
+import unittest
 
-class MetaApi(
-    GetMetaAlmanaxBonuses,
-    GetMetaElements,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.api.resources_api import ResourcesApi  # noqa: E501
+from dofusdude.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestResourcesApi(unittest.TestCase):
+    """ResourcesApi unit test stubs"""
+
+    def setUp(self):
+        self.api = dofusdude.api.resources_api.ResourcesApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_get_all_items_resources_list(self):
+        """Test case for get_all_items_resources_list
+
+        List All Resources  # noqa: E501
+        """
+        pass
+
+    def test_get_items_resource_search(self):
+        """Test case for get_items_resource_search
+
+        Search Resources  # noqa: E501
+        """
+        pass
+
+    def test_get_items_resources_list(self):
+        """Test case for get_items_resources_list
+
+        List Resources  # noqa: E501
+        """
+        pass
+
+    def test_get_items_resources_single(self):
+        """Test case for get_items_resources_single
+
+        Single Resources  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/mounts_api.py` & `dofusdude-0.7.2/test/test_quest_items_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,62 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.game_language_mounts_all.get import GetAllMountsList
-from dofusdude.paths.game_language_mounts.get import GetMountsList
-from dofusdude.paths.game_language_mounts_search.get import GetMountsSearch
-from dofusdude.paths.game_language_mounts_ankama_id.get import GetMountsSingle
 
+import unittest
 
-class MountsApi(
-    GetAllMountsList,
-    GetMountsList,
-    GetMountsSearch,
-    GetMountsSingle,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.api.quest_items_api import QuestItemsApi  # noqa: E501
+from dofusdude.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestQuestItemsApi(unittest.TestCase):
+    """QuestItemsApi unit test stubs"""
+
+    def setUp(self):
+        self.api = dofusdude.api.quest_items_api.QuestItemsApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_get_all_items_quest_list(self):
+        """Test case for get_all_items_quest_list
+
+        List All Quest Items  # noqa: E501
+        """
+        pass
+
+    def test_get_item_quest_single(self):
+        """Test case for get_item_quest_single
+
+        Single Quest Items  # noqa: E501
+        """
+        pass
+
+    def test_get_items_quest_list(self):
+        """Test case for get_items_quest_list
+
+        List Quest Items  # noqa: E501
+        """
+        pass
+
+    def test_get_items_quest_search(self):
+        """Test case for get_items_quest_search
+
+        Search Quest Items  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/quest_items_api.py` & `dofusdude-0.7.2/test/test_links_paged.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,58 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.game_language_items_quest_all.get import GetAllItemsQuestList
-from dofusdude.paths.game_language_items_quest_ankama_id.get import GetItemQuestSingle
-from dofusdude.paths.game_language_items_quest.get import GetItemsQuestList
-from dofusdude.paths.game_language_items_quest_search.get import GetItemsQuestSearch
 
+import unittest
+import datetime
 
-class QuestItemsApi(
-    GetAllItemsQuestList,
-    GetItemQuestSingle,
-    GetItemsQuestList,
-    GetItemsQuestSearch,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.models.links_paged import LinksPaged  # noqa: E501
+from dofusdude.rest import ApiException
+
+class TestLinksPaged(unittest.TestCase):
+    """LinksPaged unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test LinksPaged
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `LinksPaged`
+        """
+        model = dofusdude.models.links_paged.LinksPaged()  # noqa: E501
+        if include_optional :
+            return LinksPaged(
+                first = '', 
+                prev = '', 
+                next = '', 
+                last = ''
+            )
+        else :
+            return LinksPaged(
+        )
+        """
+
+    def testLinksPaged(self):
+        """Test LinksPaged"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
-    Do not edit the class manually.
-    """
-    pass
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/resources_api.py` & `dofusdude-0.7.2/test/test_recipe_entry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,57 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.game_language_items_resources_all.get import GetAllItemsResourcesList
-from dofusdude.paths.game_language_items_resources_search.get import GetItemsResourceSearch
-from dofusdude.paths.game_language_items_resources.get import GetItemsResourcesList
-from dofusdude.paths.game_language_items_resources_ankama_id.get import GetItemsResourcesSingle
 
+import unittest
+import datetime
 
-class ResourcesApi(
-    GetAllItemsResourcesList,
-    GetItemsResourceSearch,
-    GetItemsResourcesList,
-    GetItemsResourcesSingle,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.models.recipe_entry import RecipeEntry  # noqa: E501
+from dofusdude.rest import ApiException
+
+class TestRecipeEntry(unittest.TestCase):
+    """RecipeEntry unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test RecipeEntry
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RecipeEntry`
+        """
+        model = dofusdude.models.recipe_entry.RecipeEntry()  # noqa: E501
+        if include_optional :
+            return RecipeEntry(
+                item_ankama_id = 56, 
+                item_subtype = '', 
+                quantity = 56
+            )
+        else :
+            return RecipeEntry(
+        )
+        """
+
+    def testRecipeEntry(self):
+        """Test RecipeEntry"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
-    Do not edit the class manually.
-    """
-    pass
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/sets_api.py` & `dofusdude-0.7.2/test/test_weapon_range.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,56 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.game_language_sets_all.get import GetAllSetsList
-from dofusdude.paths.game_language_sets.get import GetSetsList
-from dofusdude.paths.game_language_sets_search.get import GetSetsSearch
-from dofusdude.paths.game_language_sets_ankama_id.get import GetSetsSingle
 
+import unittest
+import datetime
 
-class SetsApi(
-    GetAllSetsList,
-    GetSetsList,
-    GetSetsSearch,
-    GetSetsSingle,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import dofusdude
+from dofusdude.models.weapon_range import WeaponRange  # noqa: E501
+from dofusdude.rest import ApiException
+
+class TestWeaponRange(unittest.TestCase):
+    """WeaponRange unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test WeaponRange
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `WeaponRange`
+        """
+        model = dofusdude.models.weapon_range.WeaponRange()  # noqa: E501
+        if include_optional :
+            return WeaponRange(
+                min = 56, 
+                max = 56
+            )
+        else :
+            return WeaponRange(
+        )
+        """
+
+    def testWeaponRange(self):
+        """Test WeaponRange"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
-    Do not edit the class manually.
-    """
-    pass
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/apis/tags/webhooks_api.py` & `dofusdude-0.7.2/test/test_items_list_entry_typed_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from dofusdude.paths.webhooks_almanax_id.delete import DeleteWebhooksAlmanaxId
-from dofusdude.paths.webhooks_rss_id.delete import DeleteWebhooksRssId
-from dofusdude.paths.webhooks_twitter_id.delete import DeleteWebhooksTwitterId
-from dofusdude.paths.meta_webhooks_almanax.get import GetMetaWebhooksAlmanax
-from dofusdude.paths.meta_webhooks_rss.get import GetMetaWebhooksRss
-from dofusdude.paths.meta_webhooks_twitter.get import GetMetaWebhooksTwitter
-from dofusdude.paths.webhooks_almanax_id.get import GetWebhooksAlmanaxId
-from dofusdude.paths.webhooks_rss_id.get import GetWebhooksRssId
-from dofusdude.paths.webhooks_twitter_id.get import GetWebhooksTwitterId
-from dofusdude.paths.webhooks_almanax.post import PostWebhooksAlmanax
-from dofusdude.paths.webhooks_rss.post import PostWebhooksRss
-from dofusdude.paths.webhooks_twitter.post import PostWebhooksTwitter
-from dofusdude.paths.webhooks_almanax_id.put import PutWebhooksAlmanaxId
-from dofusdude.paths.webhooks_rss_id.put import PutWebhooksRssId
-from dofusdude.paths.webhooks_twitter_id.put import PutWebhooksTwitterId
-
-
-class WebhooksApi(
-    DeleteWebhooksAlmanaxId,
-    DeleteWebhooksRssId,
-    DeleteWebhooksTwitterId,
-    GetMetaWebhooksAlmanax,
-    GetMetaWebhooksRss,
-    GetMetaWebhooksTwitter,
-    GetWebhooksAlmanaxId,
-    GetWebhooksRssId,
-    GetWebhooksTwitterId,
-    PostWebhooksAlmanax,
-    PostWebhooksRss,
-    PostWebhooksTwitter,
-    PutWebhooksAlmanaxId,
-    PutWebhooksRssId,
-    PutWebhooksTwitterId,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
-    """
-    pass
+import unittest
+import datetime
+
+import dofusdude
+from dofusdude.models.items_list_entry_typed_type import ItemsListEntryTypedType  # noqa: E501
+from dofusdude.rest import ApiException
+
+class TestItemsListEntryTypedType(unittest.TestCase):
+    """ItemsListEntryTypedType unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ItemsListEntryTypedType
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ItemsListEntryTypedType`
+        """
+        model = dofusdude.models.items_list_entry_typed_type.ItemsListEntryTypedType()  # noqa: E501
+        if include_optional :
+            return ItemsListEntryTypedType(
+                name = '', 
+                id = 56
+            )
+        else :
+            return ItemsListEntryTypedType(
+        )
+        """
+
+    def testItemsListEntryTypedType(self):
+        """Test ItemsListEntryTypedType"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/dofusdude/configuration.py` & `dofusdude-0.7.2/dofusdude/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,100 +1,75 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
+import http.client as httplib
 from dofusdude.exceptions import ApiValueError
 
-
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems',
-    'uniqueItems', 'maxProperties', 'minProperties',
+    'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
+    """This class contains various settings of the API client.
 
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
+    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+      in PEM format.
 
     """
 
     _default = None
 
-    def __init__(
-        self,
-        host=None,
-        discard_unknown_keys=False,
-        disabled_client_side_validations="",
-        server_index=None,
-        server_variables=None,
-        server_operation_index=None,
-        server_operation_variables=None,
-    ):
+    def __init__(self, host=None,
+                 api_key=None, api_key_prefix=None,
+                 username=None, password=None,
+                 access_token=None,
+                 server_index=None, server_variables=None,
+                 server_operation_index=None, server_operation_variables=None,
+                 ssl_ca_cert=None,
+                 ):
         """Constructor
         """
         self._base_path = "https://api.dofusdu.de" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -104,15 +79,36 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.api_key = {}
+        if api_key:
+            self.api_key = api_key
+        """dict to store API key(s)
+        """
+        self.api_key_prefix = {}
+        if api_key_prefix:
+            self.api_key_prefix = api_key_prefix
+        """dict to store API prefix (e.g. Bearer)
+        """
+        self.refresh_api_key_hook = None
+        """function hook to refresh API key if expired
+        """
+        self.username = username
+        """Username for HTTP basic authentication
+        """
+        self.password = password
+        """Password for HTTP basic authentication
+        """
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("dofusdude")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -131,26 +127,30 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = None
+        self.ssl_ca_cert = ssl_ca_cert
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
@@ -167,16 +167,25 @@
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -186,46 +195,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -271,23 +283,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -352,16 +364,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.7.1\n"\
-               "SDK Package Version: 0.7.1".\
+               "Version of the API: 0.7.2\n"\
+               "SDK Package Version: 0.7.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `dofusdude-0.7.1/dofusdude/exceptions.py` & `dofusdude-0.7.2/dofusdude/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
-import dataclasses
-import typing
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from urllib3._collections import HTTPHeaderDict
+    Do not edit the class manually.
+"""
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
@@ -98,48 +96,69 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-T = typing.TypeVar("T")
+class ApiException(OpenApiException):
 
-
-@dataclasses.dataclass
-class ApiException(OpenApiException, typing.Generic[T]):
-    status: int
-    reason: str
-    api_response: typing.Optional[T] = None
-
-    @property
-    def body(self) -> typing.Union[str, bytes, None]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.data
-
-    @property
-    def headers(self) -> typing.Optional[HTTPHeaderDict]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.getheaders()
+    def __init__(self, status=None, reason=None, http_resp=None):
+        if http_resp:
+            self.status = http_resp.status
+            self.reason = http_resp.reason
+            self.body = http_resp.data
+            self.headers = http_resp.getheaders()
+        else:
+            self.status = status
+            self.reason = reason
+            self.body = None
+            self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
                 self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
+class BadRequestException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(BadRequestException, self).__init__(status, reason, http_resp)
+
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
 
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
```

### Comparing `dofusdude-0.7.1/dofusdude/model/image_urls.py` & `dofusdude-0.7.2/dofusdude/models/resource.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,168 +1,136 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from dofusdude import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class ImageUrls(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import List, Optional
+from pydantic import BaseModel, StrictInt, StrictStr, conlist
+from dofusdude.models.condition_entry import ConditionEntry
+from dofusdude.models.cosmetic_type import CosmeticType
+from dofusdude.models.effects_entry import EffectsEntry
+from dofusdude.models.image_urls import ImageUrls
+from dofusdude.models.recipe_entry import RecipeEntry
 
-    All images except icon are rendered in the background which can take some time (up to hours if all data is completely generated from scratch). Because of this, they can be null if they are not yet rendered.
+class Resource(BaseModel):
     """
+    Resource
+    """
+    ankama_id: Optional[StrictInt] = None
+    name: Optional[StrictStr] = None
+    description: Optional[StrictStr] = None
+    type: Optional[CosmeticType] = None
+    level: Optional[StrictInt] = None
+    pods: Optional[StrictInt] = None
+    image_urls: Optional[ImageUrls] = None
+    effects: Optional[conlist(EffectsEntry)] = None
+    conditions: Optional[conlist(ConditionEntry)] = None
+    recipe: Optional[conlist(RecipeEntry)] = None
+    __properties = ["ankama_id", "name", "description", "type", "level", "pods", "image_urls", "effects", "conditions", "recipe"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Resource:
+        """Create an instance of Resource from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of type
+        if self.type:
+            _dict['type'] = self.type.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of image_urls
+        if self.image_urls:
+            _dict['image_urls'] = self.image_urls.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in effects (list)
+        _items = []
+        if self.effects:
+            for _item in self.effects:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['effects'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in conditions (list)
+        _items = []
+        if self.conditions:
+            for _item in self.conditions:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['conditions'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in recipe (list)
+        _items = []
+        if self.recipe:
+            for _item in self.recipe:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['recipe'] = _items
+        # set to None if effects (nullable) is None
+        # and __fields_set__ contains the field
+        if self.effects is None and "effects" in self.__fields_set__:
+            _dict['effects'] = None
+
+        # set to None if conditions (nullable) is None
+        # and __fields_set__ contains the field
+        if self.conditions is None and "conditions" in self.__fields_set__:
+            _dict['conditions'] = None
+
+        # set to None if recipe (nullable) is None
+        # and __fields_set__ contains the field
+        if self.recipe is None and "recipe" in self.__fields_set__:
+            _dict['recipe'] = None
+
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> Resource:
+        """Create an instance of Resource from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return Resource.parse_obj(obj)
+
+        _obj = Resource.parse_obj({
+            "ankama_id": obj.get("ankama_id"),
+            "name": obj.get("name"),
+            "description": obj.get("description"),
+            "type": CosmeticType.from_dict(obj.get("type")) if obj.get("type") is not None else None,
+            "level": obj.get("level"),
+            "pods": obj.get("pods"),
+            "image_urls": ImageUrls.from_dict(obj.get("image_urls")) if obj.get("image_urls") is not None else None,
+            "effects": [EffectsEntry.from_dict(_item) for _item in obj.get("effects")] if obj.get("effects") is not None else None,
+            "conditions": [ConditionEntry.from_dict(_item) for _item in obj.get("conditions")] if obj.get("conditions") is not None else None,
+            "recipe": [RecipeEntry.from_dict(_item) for _item in obj.get("recipe")] if obj.get("recipe") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            icon = schemas.StrSchema
-            
-            
-            class sd(
-                schemas.StrBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneStrMixin
-            ):
-            
-            
-                def __new__(
-                    cls,
-                    *_args: typing.Union[None, str, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'sd':
-                    return super().__new__(
-                        cls,
-                        *_args,
-                        _configuration=_configuration,
-                    )
-            
-            
-            class hq(
-                schemas.StrBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneStrMixin
-            ):
-            
-            
-                def __new__(
-                    cls,
-                    *_args: typing.Union[None, str, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'hq':
-                    return super().__new__(
-                        cls,
-                        *_args,
-                        _configuration=_configuration,
-                    )
-            
-            
-            class hd(
-                schemas.StrBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneStrMixin
-            ):
-            
-            
-                def __new__(
-                    cls,
-                    *_args: typing.Union[None, str, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'hd':
-                    return super().__new__(
-                        cls,
-                        *_args,
-                        _configuration=_configuration,
-                    )
-            __annotations__ = {
-                "icon": icon,
-                "sd": sd,
-                "hq": hq,
-                "hd": hd,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["icon"]) -> MetaOapg.properties.icon: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sd"]) -> MetaOapg.properties.sd: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["hq"]) -> MetaOapg.properties.hq: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["hd"]) -> MetaOapg.properties.hd: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["icon", "sd", "hq", "hd", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["icon"]) -> typing.Union[MetaOapg.properties.icon, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sd"]) -> typing.Union[MetaOapg.properties.sd, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["hq"]) -> typing.Union[MetaOapg.properties.hq, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["hd"]) -> typing.Union[MetaOapg.properties.hd, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["icon", "sd", "hq", "hd", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        icon: typing.Union[MetaOapg.properties.icon, str, schemas.Unset] = schemas.unset,
-        sd: typing.Union[MetaOapg.properties.sd, None, str, schemas.Unset] = schemas.unset,
-        hq: typing.Union[MetaOapg.properties.hq, None, str, schemas.Unset] = schemas.unset,
-        hd: typing.Union[MetaOapg.properties.hd, None, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ImageUrls':
-        return super().__new__(
-            cls,
-            *_args,
-            icon=icon,
-            sd=sd,
-            hq=hq,
-            hd=hd,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `dofusdude-0.7.1/dofusdude/model/items_list_paged.py` & `dofusdude-0.7.2/dofusdude/models/sets_list_paged.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,85 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from dofusdude import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class ItemsListPaged(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from typing import List, Optional
+from pydantic import BaseModel, Field, conlist
+from dofusdude.models.links_paged import LinksPaged
+from dofusdude.models.set_list_entry import SetListEntry
 
-    Do not edit the class manually.
+class SetsListPaged(BaseModel):
     """
+    SetsListPaged
+    """
+    links: Optional[LinksPaged] = Field(None, alias="_links")
+    items: Optional[conlist(SetListEntry)] = None
+    __properties = ["_links", "items"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> SetsListPaged:
+        """Create an instance of SetsListPaged from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of links
+        if self.links:
+            _dict['_links'] = self.links.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in items (list)
+        _items = []
+        if self.items:
+            for _item in self.items:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['items'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> SetsListPaged:
+        """Create an instance of SetsListPaged from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return SetsListPaged.parse_obj(obj)
+
+        _obj = SetsListPaged.parse_obj({
+            "links": LinksPaged.from_dict(obj.get("_links")) if obj.get("_links") is not None else None,
+            "items": [SetListEntry.from_dict(_item) for _item in obj.get("items")] if obj.get("items") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-        
-            @staticmethod
-            def _links() -> typing.Type['LinksPaged']:
-                return LinksPaged
-            
-            
-            class items(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ItemListEntry']:
-                        return ItemListEntry
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['ItemListEntry'], typing.List['ItemListEntry']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'items':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ItemListEntry':
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "_links": _links,
-                "items": items,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["_links"]) -> 'LinksPaged': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["items"]) -> MetaOapg.properties.items: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["_links", "items", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["_links"]) -> typing.Union['LinksPaged', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["items"]) -> typing.Union[MetaOapg.properties.items, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["_links", "items", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        _links: typing.Union['LinksPaged', schemas.Unset] = schemas.unset,
-        items: typing.Union[MetaOapg.properties.items, list, tuple, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ItemsListPaged':
-        return super().__new__(
-            cls,
-            *_args,
-            _links=_links,
-            items=items,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from dofusdude.model.item_list_entry import ItemListEntry
-from dofusdude.model.links_paged import LinksPaged
```

### Comparing `dofusdude-0.7.1/dofusdude/model/mount_list_entry.py` & `dofusdude-0.7.2/dofusdude/models/item_list_entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,102 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from dofusdude import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class MountListEntry(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from typing import List, Optional
+from pydantic import BaseModel, StrictInt, StrictStr, conlist
+from dofusdude.models.image_urls import ImageUrls
+from dofusdude.models.items_list_entry_typed_type import ItemsListEntryTypedType
+from dofusdude.models.recipe_entry import RecipeEntry
 
-    Do not edit the class manually.
+class ItemListEntry(BaseModel):
     """
+    ItemListEntry
+    """
+    ankama_id: Optional[StrictInt] = None
+    name: Optional[StrictStr] = None
+    type: Optional[ItemsListEntryTypedType] = None
+    level: Optional[StrictInt] = None
+    image_urls: Optional[ImageUrls] = None
+    recipe: Optional[conlist(RecipeEntry)] = None
+    __properties = ["ankama_id", "name", "type", "level", "image_urls", "recipe"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> ItemListEntry:
+        """Create an instance of ItemListEntry from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of type
+        if self.type:
+            _dict['type'] = self.type.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of image_urls
+        if self.image_urls:
+            _dict['image_urls'] = self.image_urls.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in recipe (list)
+        _items = []
+        if self.recipe:
+            for _item in self.recipe:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['recipe'] = _items
+        # set to None if recipe (nullable) is None
+        # and __fields_set__ contains the field
+        if self.recipe is None and "recipe" in self.__fields_set__:
+            _dict['recipe'] = None
+
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> ItemListEntry:
+        """Create an instance of ItemListEntry from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return ItemListEntry.parse_obj(obj)
+
+        _obj = ItemListEntry.parse_obj({
+            "ankama_id": obj.get("ankama_id"),
+            "name": obj.get("name"),
+            "type": ItemsListEntryTypedType.from_dict(obj.get("type")) if obj.get("type") is not None else None,
+            "level": obj.get("level"),
+            "image_urls": ImageUrls.from_dict(obj.get("image_urls")) if obj.get("image_urls") is not None else None,
+            "recipe": [RecipeEntry.from_dict(_item) for _item in obj.get("recipe")] if obj.get("recipe") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            ankama_id = schemas.IntSchema
-            name = schemas.StrSchema
-            family_name = schemas.StrSchema
-        
-            @staticmethod
-            def image_urls() -> typing.Type['ImageUrls']:
-                return ImageUrls
-            __annotations__ = {
-                "ankama_id": ankama_id,
-                "name": name,
-                "family_name": family_name,
-                "image_urls": image_urls,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ankama_id"]) -> MetaOapg.properties.ankama_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["family_name"]) -> MetaOapg.properties.family_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["image_urls"]) -> 'ImageUrls': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["ankama_id", "name", "family_name", "image_urls", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ankama_id"]) -> typing.Union[MetaOapg.properties.ankama_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["family_name"]) -> typing.Union[MetaOapg.properties.family_name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["image_urls"]) -> typing.Union['ImageUrls', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["ankama_id", "name", "family_name", "image_urls", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        ankama_id: typing.Union[MetaOapg.properties.ankama_id, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
-        family_name: typing.Union[MetaOapg.properties.family_name, str, schemas.Unset] = schemas.unset,
-        image_urls: typing.Union['ImageUrls', schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'MountListEntry':
-        return super().__new__(
-            cls,
-            *_args,
-            ankama_id=ankama_id,
-            name=name,
-            family_name=family_name,
-            image_urls=image_urls,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from dofusdude.model.image_urls import ImageUrls
```

### Comparing `dofusdude-0.7.1/dofusdude/model/mounts_list_paged.py` & `dofusdude-0.7.2/dofusdude/models/items_list_paged.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,120 +1,85 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from dofusdude import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class MountsListPaged(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from typing import List, Optional
+from pydantic import BaseModel, Field, conlist
+from dofusdude.models.item_list_entry import ItemListEntry
+from dofusdude.models.links_paged import LinksPaged
 
-    Do not edit the class manually.
+class ItemsListPaged(BaseModel):
     """
+    ItemsListPaged
+    """
+    links: Optional[LinksPaged] = Field(None, alias="_links")
+    items: Optional[conlist(ItemListEntry)] = None
+    __properties = ["_links", "items"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> ItemsListPaged:
+        """Create an instance of ItemsListPaged from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of links
+        if self.links:
+            _dict['_links'] = self.links.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in items (list)
+        _items = []
+        if self.items:
+            for _item in self.items:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['items'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> ItemsListPaged:
+        """Create an instance of ItemsListPaged from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return ItemsListPaged.parse_obj(obj)
+
+        _obj = ItemsListPaged.parse_obj({
+            "links": LinksPaged.from_dict(obj.get("_links")) if obj.get("_links") is not None else None,
+            "items": [ItemListEntry.from_dict(_item) for _item in obj.get("items")] if obj.get("items") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-        
-            @staticmethod
-            def _links() -> typing.Type['LinksPaged']:
-                return LinksPaged
-            
-            
-            class items(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['MountListEntry']:
-                        return MountListEntry
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['MountListEntry'], typing.List['MountListEntry']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'items':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'MountListEntry':
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "_links": _links,
-                "items": items,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["_links"]) -> 'LinksPaged': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["items"]) -> MetaOapg.properties.items: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["_links", "items", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["_links"]) -> typing.Union['LinksPaged', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["items"]) -> typing.Union[MetaOapg.properties.items, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["_links", "items", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        _links: typing.Union['LinksPaged', schemas.Unset] = schemas.unset,
-        items: typing.Union[MetaOapg.properties.items, list, tuple, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'MountsListPaged':
-        return super().__new__(
-            cls,
-            *_args,
-            _links=_links,
-            items=items,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from dofusdude.model.links_paged import LinksPaged
-from dofusdude.model.mount_list_entry import MountListEntry
```

### Comparing `dofusdude-0.7.1/dofusdude/model/recipe_entry.py` & `dofusdude-0.7.2/dofusdude/models/items_list_entry_typed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,89 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from dofusdude import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class RecipeEntry(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from typing import Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+from dofusdude.models.image_urls import ImageUrls
+from dofusdude.models.items_list_entry_typed_type import ItemsListEntryTypedType
 
-    Do not edit the class manually.
+class ItemsListEntryTyped(BaseModel):
     """
+    ItemsListEntryTyped
+    """
+    ankama_id: Optional[StrictInt] = None
+    name: Optional[StrictStr] = None
+    type: Optional[ItemsListEntryTypedType] = None
+    item_subtype: Optional[StrictStr] = Field(None, description="The API item category. Can be used to build the request URL for this particular item. Always english.")
+    level: Optional[StrictInt] = None
+    image_urls: Optional[ImageUrls] = None
+    __properties = ["ankama_id", "name", "type", "item_subtype", "level", "image_urls"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> ItemsListEntryTyped:
+        """Create an instance of ItemsListEntryTyped from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of type
+        if self.type:
+            _dict['type'] = self.type.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of image_urls
+        if self.image_urls:
+            _dict['image_urls'] = self.image_urls.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> ItemsListEntryTyped:
+        """Create an instance of ItemsListEntryTyped from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return ItemsListEntryTyped.parse_obj(obj)
+
+        _obj = ItemsListEntryTyped.parse_obj({
+            "ankama_id": obj.get("ankama_id"),
+            "name": obj.get("name"),
+            "type": ItemsListEntryTypedType.from_dict(obj.get("type")) if obj.get("type") is not None else None,
+            "item_subtype": obj.get("item_subtype"),
+            "level": obj.get("level"),
+            "image_urls": ImageUrls.from_dict(obj.get("image_urls")) if obj.get("image_urls") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            item_ankama_id = schemas.IntSchema
-            item_subtype = schemas.StrSchema
-            quantity = schemas.IntSchema
-            __annotations__ = {
-                "item_ankama_id": item_ankama_id,
-                "item_subtype": item_subtype,
-                "quantity": quantity,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["item_ankama_id"]) -> MetaOapg.properties.item_ankama_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["item_subtype"]) -> MetaOapg.properties.item_subtype: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["quantity"]) -> MetaOapg.properties.quantity: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["item_ankama_id", "item_subtype", "quantity", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["item_ankama_id"]) -> typing.Union[MetaOapg.properties.item_ankama_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["item_subtype"]) -> typing.Union[MetaOapg.properties.item_subtype, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["quantity"]) -> typing.Union[MetaOapg.properties.quantity, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["item_ankama_id", "item_subtype", "quantity", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        item_ankama_id: typing.Union[MetaOapg.properties.item_ankama_id, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        item_subtype: typing.Union[MetaOapg.properties.item_subtype, str, schemas.Unset] = schemas.unset,
-        quantity: typing.Union[MetaOapg.properties.quantity, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'RecipeEntry':
-        return super().__new__(
-            cls,
-            *_args,
-            item_ankama_id=item_ankama_id,
-            item_subtype=item_subtype,
-            quantity=quantity,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `dofusdude-0.7.1/dofusdude/model/set_list_entry.py` & `dofusdude-0.7.2/dofusdude/models/create_almanax_webhook_mentions_value_inner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,80 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from dofusdude import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class SetListEntry(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, conint
 
-    Do not edit the class manually.
+class CreateAlmanaxWebhookMentionsValueInner(BaseModel):
     """
+    Mention
+    """
+    discord_id: Optional[StrictInt] = Field(None, description="User or role ID directly from Discord. Activate developer mode and right click a user or role to get them.")
+    is_role: Optional[StrictBool] = Field(None, description="Whether an ID describes a role (true) or user (false). This is needed for formatting the mention command so Discord understands it.")
+    ping_days_before: Optional[conint(strict=True, le=31, ge=1)] = Field(None, description="Get a mention days before the bonus comes up. It will post on the specified time. Also works when the interval is not daily.")
+    __properties = ["discord_id", "is_role", "ping_days_before"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> CreateAlmanaxWebhookMentionsValueInner:
+        """Create an instance of CreateAlmanaxWebhookMentionsValueInner from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # set to None if ping_days_before (nullable) is None
+        # and __fields_set__ contains the field
+        if self.ping_days_before is None and "ping_days_before" in self.__fields_set__:
+            _dict['ping_days_before'] = None
+
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> CreateAlmanaxWebhookMentionsValueInner:
+        """Create an instance of CreateAlmanaxWebhookMentionsValueInner from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return CreateAlmanaxWebhookMentionsValueInner.parse_obj(obj)
+
+        _obj = CreateAlmanaxWebhookMentionsValueInner.parse_obj({
+            "discord_id": obj.get("discord_id"),
+            "is_role": obj.get("is_role"),
+            "ping_days_before": obj.get("ping_days_before")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            ankama_id = schemas.IntSchema
-            name = schemas.StrSchema
-            items = schemas.IntSchema
-            level = schemas.IntSchema
-            __annotations__ = {
-                "ankama_id": ankama_id,
-                "name": name,
-                "items": items,
-                "level": level,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ankama_id"]) -> MetaOapg.properties.ankama_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["items"]) -> MetaOapg.properties.items: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["level"]) -> MetaOapg.properties.level: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["ankama_id", "name", "items", "level", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ankama_id"]) -> typing.Union[MetaOapg.properties.ankama_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["items"]) -> typing.Union[MetaOapg.properties.items, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["level"]) -> typing.Union[MetaOapg.properties.level, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["ankama_id", "name", "items", "level", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        ankama_id: typing.Union[MetaOapg.properties.ankama_id, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
-        items: typing.Union[MetaOapg.properties.items, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        level: typing.Union[MetaOapg.properties.level, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SetListEntry':
-        return super().__new__(
-            cls,
-            *_args,
-            ankama_id=ankama_id,
-            name=name,
-            items=items,
-            level=level,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `dofusdude-0.7.1/dofusdude/model/sets_list_paged.py` & `dofusdude-0.7.2/dofusdude/models/mount.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,120 +1,96 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from dofusdude import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class SetsListPaged(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from typing import List, Optional
+from pydantic import BaseModel, StrictInt, StrictStr, conlist
+from dofusdude.models.effects_entry import EffectsEntry
+from dofusdude.models.image_urls import ImageUrls
 
-    Do not edit the class manually.
+class Mount(BaseModel):
     """
+    Mount
+    """
+    ankama_id: Optional[StrictInt] = None
+    name: Optional[StrictStr] = None
+    family_name: Optional[StrictStr] = None
+    image_urls: Optional[ImageUrls] = None
+    effects: Optional[conlist(EffectsEntry)] = None
+    __properties = ["ankama_id", "name", "family_name", "image_urls", "effects"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Mount:
+        """Create an instance of Mount from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of image_urls
+        if self.image_urls:
+            _dict['image_urls'] = self.image_urls.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in effects (list)
+        _items = []
+        if self.effects:
+            for _item in self.effects:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['effects'] = _items
+        # set to None if effects (nullable) is None
+        # and __fields_set__ contains the field
+        if self.effects is None and "effects" in self.__fields_set__:
+            _dict['effects'] = None
+
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> Mount:
+        """Create an instance of Mount from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return Mount.parse_obj(obj)
+
+        _obj = Mount.parse_obj({
+            "ankama_id": obj.get("ankama_id"),
+            "name": obj.get("name"),
+            "family_name": obj.get("family_name"),
+            "image_urls": ImageUrls.from_dict(obj.get("image_urls")) if obj.get("image_urls") is not None else None,
+            "effects": [EffectsEntry.from_dict(_item) for _item in obj.get("effects")] if obj.get("effects") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-        
-            @staticmethod
-            def _links() -> typing.Type['LinksPaged']:
-                return LinksPaged
-            
-            
-            class items(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['SetListEntry']:
-                        return SetListEntry
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['SetListEntry'], typing.List['SetListEntry']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'items':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'SetListEntry':
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "_links": _links,
-                "items": items,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["_links"]) -> 'LinksPaged': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["items"]) -> MetaOapg.properties.items: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["_links", "items", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["_links"]) -> typing.Union['LinksPaged', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["items"]) -> typing.Union[MetaOapg.properties.items, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["_links", "items", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        _links: typing.Union['LinksPaged', schemas.Unset] = schemas.unset,
-        items: typing.Union[MetaOapg.properties.items, list, tuple, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SetsListPaged':
-        return super().__new__(
-            cls,
-            *_args,
-            _links=_links,
-            items=items,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from dofusdude.model.links_paged import LinksPaged
-from dofusdude.model.set_list_entry import SetListEntry
```

### Comparing `dofusdude-0.7.1/dofusdude/rest.py` & `dofusdude-0.7.2/dofusdude/rest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,54 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
+import io
+import json
 import logging
+import re
 import ssl
-from urllib.parse import urlencode
-import typing
 
-import certifi
+from urllib.parse import urlencode, quote_plus
 import urllib3
-from urllib3._collections import HTTPHeaderDict
 
-from dofusdude.exceptions import ApiException, ApiValueError
+from dofusdude.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError, BadRequestException
 
 
 logger = logging.getLogger(__name__)
 
 
+class RESTResponse(io.IOBase):
+
+    def __init__(self, resp):
+        self.urllib3_response = resp
+        self.status = resp.status
+        self.reason = resp.reason
+        self.data = resp.data
+
+    def getheaders(self):
+        """Returns a dictionary of the response headers."""
+        return self.urllib3_response.headers
+
+    def getheader(self, name, default=None):
+        """Returns a given response header."""
+        return self.urllib3_response.headers.get(name, default)
+
+
 class RESTClientObject(object):
 
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
         # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
@@ -36,28 +56,25 @@
 
         # cert_reqs
         if configuration.verify_ssl:
             cert_reqs = ssl.CERT_REQUIRED
         else:
             cert_reqs = ssl.CERT_NONE
 
-        # ca_certs
-        if configuration.ssl_ca_cert:
-            ca_certs = configuration.ssl_ca_cert
-        else:
-            # if not set certificate file, use Mozilla's root certificates.
-            ca_certs = certifi.where()
-
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.tls_server_name:
+            addition_pool_args['server_hostname'] = configuration.tls_server_name
+
+
         if configuration.socket_options is not None:
             addition_pool_args['socket_options'] = configuration.socket_options
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
@@ -65,191 +82,223 @@
 
         # https pool manager
         if configuration.proxy:
             self.pool_manager = urllib3.ProxyManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
+                ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
                 proxy_headers=configuration.proxy_headers,
                 **addition_pool_args
             )
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
+                ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 **addition_pool_args
             )
 
-    def request(
-        self,
-        method: str,
-        url: str,
-        headers: typing.Optional[HTTPHeaderDict] = None,
-        fields: typing.Optional[typing.Tuple[typing.Tuple[str, typing.Any], ...]] = None,
-        body: typing.Optional[typing.Union[str, bytes]] = None,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> urllib3.HTTPResponse:
+    def request(self, method, url, query_params=None, headers=None,
+                body=None, post_params=None, _preload_content=True,
+                _request_timeout=None):
         """Perform requests.
 
         :param method: http request method
         :param url: http request url
+        :param query_params: query parameters in the url
         :param headers: http request headers
-        :param body: request body, for other types
-        :param fields: request parameters for
-                                `application/x-www-form-urlencoded`
-                                or `multipart/form-data`
-        :param stream: if True, the urllib3.HTTPResponse object will
-                                be returned without reading/decoding response
-                                data. Default is False.
-        :param timeout: timeout setting for this request. If one
-                                number provided, it will be total request
-                                timeout. It can also be a pair (tuple) of
-                                (connection, read) timeouts.
+        :param body: request json body, for `application/json`
+        :param post_params: request post parameters,
+                            `application/x-www-form-urlencoded`
+                            and `multipart/form-data`
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
         """
         method = method.upper()
         assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
                           'PATCH', 'OPTIONS']
 
-        if fields and body:
+        if post_params and body:
             raise ApiValueError(
-                "body parameter cannot be used with fields parameter."
+                "body parameter cannot be used with post_params parameter."
             )
 
-        fields = fields or {}
+        post_params = post_params or {}
         headers = headers or {}
-
-        if timeout:
-            if isinstance(timeout, (int, float)):  # noqa: E501,F821
-                timeout = urllib3.Timeout(total=timeout)
-            elif (isinstance(timeout, tuple) and
-                  len(timeout) == 2):
-                timeout = urllib3.Timeout(connect=timeout[0], read=timeout[1])
+        # url already contains the URL query string
+        # so reset query_params to empty dict
+        query_params = {}
+
+        timeout = None
+        if _request_timeout:
+            if isinstance(_request_timeout, (int,float)):  # noqa: E501,F821
+                timeout = urllib3.Timeout(total=_request_timeout)
+            elif (isinstance(_request_timeout, tuple) and
+                  len(_request_timeout) == 2):
+                timeout = urllib3.Timeout(
+                    connect=_request_timeout[0], read=_request_timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-                if 'Content-Type' not in headers and body is None:
+
+                # no content type provided or payload is json
+                if not headers.get('Content-Type') or re.search('json', headers['Content-Type'], re.IGNORECASE):
+                    request_body = None
+                    if body is not None:
+                        request_body = json.dumps(body)
                     r = self.pool_manager.request(
-                        method,
-                        url,
-                        preload_content=not stream,
+                        method, url,
+                        body=request_body,
+                        preload_content=_preload_content,
                         timeout=timeout,
-                        headers=headers
-                    )
+                        headers=headers)
                 elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
                     r = self.pool_manager.request(
                         method, url,
-                        body=body,
-                        fields=fields,
+                        fields=post_params,
                         encode_multipart=False,
-                        preload_content=not stream,
+                        preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers)
                 elif headers['Content-Type'] == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
                     r = self.pool_manager.request(
                         method, url,
-                        fields=fields,
+                        fields=post_params,
                         encode_multipart=True,
-                        preload_content=not stream,
+                        preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers)
                 # Pass a `string` parameter directly in the body to support
                 # other content types than Json when `body` argument is
                 # provided in serialized form
                 elif isinstance(body, str) or isinstance(body, bytes):
                     request_body = body
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
-                        preload_content=not stream,
+                        preload_content=_preload_content,
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
                 r = self.pool_manager.request(method, url,
-                                              preload_content=not stream,
+                                              fields={},
+                                              preload_content=_preload_content,
                                               timeout=timeout,
                                               headers=headers)
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
-        if not stream:
+        if _preload_content:
+            r = RESTResponse(r)
+
             # log response body
             logger.debug("response body: %s", r.data)
 
+        if not 200 <= r.status <= 299:
+            if r.status == 400:
+                raise BadRequestException(http_resp=r)
+
+            if r.status == 401:
+                raise UnauthorizedException(http_resp=r)
+
+            if r.status == 403:
+                raise ForbiddenException(http_resp=r)
+
+            if r.status == 404:
+                raise NotFoundException(http_resp=r)
+
+            if 500 <= r.status <= 599:
+                raise ServiceException(http_resp=r)
+
+            raise ApiException(http_resp=r)
+
         return r
 
-    def GET(self, url, headers=None, stream=False,
-            timeout=None, fields=None) -> urllib3.HTTPResponse:
+    def get_request(self, url, headers=None, query_params=None, _preload_content=True,
+            _request_timeout=None):
         return self.request("GET", url,
                             headers=headers,
-                            stream=stream,
-                            timeout=timeout,
-                            fields=fields)
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
 
-    def HEAD(self, url, headers=None, stream=False,
-             timeout=None, fields=None) -> urllib3.HTTPResponse:
+    def head_request(self, url, headers=None, query_params=None, _preload_content=True,
+             _request_timeout=None):
         return self.request("HEAD", url,
                             headers=headers,
-                            stream=stream,
-                            timeout=timeout,
-                            fields=fields)
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            query_params=query_params)
 
-    def OPTIONS(self, url, headers=None,
-                body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+    def options_request(self, url, headers=None, query_params=None, post_params=None,
+                body=None, _preload_content=True, _request_timeout=None):
         return self.request("OPTIONS", url,
                             headers=headers,
-                            stream=stream,
-                            timeout=timeout,
-                            body=body, fields=fields)
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
 
-    def DELETE(self, url, headers=None, body=None,
-               stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+    def delete_request(self, url, headers=None, query_params=None, body=None,
+               _preload_content=True, _request_timeout=None):
         return self.request("DELETE", url,
                             headers=headers,
-                            stream=stream,
-                            timeout=timeout,
-                            body=body, fields=fields)
+                            query_params=query_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
 
-    def POST(self, url, headers=None,
-             body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+    def post_request(self, url, headers=None, query_params=None, post_params=None,
+             body=None, _preload_content=True, _request_timeout=None):
         return self.request("POST", url,
                             headers=headers,
-                            stream=stream,
-                            timeout=timeout,
-                            body=body, fields=fields)
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
 
-    def PUT(self, url, headers=None,
-            body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+    def put_request(self, url, headers=None, query_params=None, post_params=None,
+            body=None, _preload_content=True, _request_timeout=None):
         return self.request("PUT", url,
                             headers=headers,
-                            stream=stream,
-                            timeout=timeout,
-                            body=body, fields=fields)
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
 
-    def PATCH(self, url, headers=None,
-              body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+    def patch_request(self, url, headers=None, query_params=None, post_params=None,
+              body=None, _preload_content=True, _request_timeout=None):
         return self.request("PATCH", url,
                             headers=headers,
-                            stream=stream,
-                            timeout=timeout,
-                            body=body, fields=fields)
+                            query_params=query_params,
+                            post_params=post_params,
+                            _preload_content=_preload_content,
+                            _request_timeout=_request_timeout,
+                            body=body)
```

### Comparing `dofusdude-0.7.1/dofusdude.egg-info/PKG-INFO` & `dofusdude-0.7.2/test/test_put_rss_webhook.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,64 @@
-Metadata-Version: 2.1
-Name: dofusdude
-Version: 0.7.1
-Summary: Dofusdude
-Home-page: https://github.com/dofusdude/dofusdude-py
-Author: Survival
-Author-email: stelzo@steado.de
-Keywords: OpenAPI,OpenAPI-Generator,Dofusdude
-Requires-Python: >=3.7
+# coding: utf-8
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don&#x27;t write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
-    
+"""
+    Dofusdude
+
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+
+    The version of the OpenAPI document: 0.7.2
+    Contact: stelzo@steado.de
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""
+
+
+import unittest
+import datetime
+
+import dofusdude
+from dofusdude.models.put_rss_webhook import PutRSSWebhook  # noqa: E501
+from dofusdude.rest import ApiException
+
+class TestPutRSSWebhook(unittest.TestCase):
+    """PutRSSWebhook unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test PutRSSWebhook
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `PutRSSWebhook`
+        """
+        model = dofusdude.models.put_rss_webhook.PutRSSWebhook()  # noqa: E501
+        if include_optional :
+            return PutRSSWebhook(
+                whitelist = [
+                    ''
+                    ], 
+                blacklist = [
+                    ''
+                    ], 
+                subscriptions = [
+                    ''
+                    ], 
+                preview_length = 2000
+            )
+        else :
+            return PutRSSWebhook(
+        )
+        """
+
+    def testPutRSSWebhook(self):
+        """Test PutRSSWebhook"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dofusdude-0.7.1/setup.py` & `dofusdude-0.7.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 from setuptools import setup, find_packages  # noqa: H301
 
-NAME = "dofusdude"
-VERSION = "0.7.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
-
+NAME = "dofusdude"
+VERSION = "0.7.2"
+PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
-    "certifi >= 14.5.14",
-    "frozendict ~= 2.3.4",
-    "python-dateutil ~= 2.7.0",
-    "setuptools >= 21.0.0",
-    "typing_extensions ~= 4.3.0",
-    "urllib3 ~= 1.26.7",
+    "urllib3 >= 1.25.3, < 2.1.0",
+    "python-dateutil",
+    "pydantic >= 1.10.5, < 2",
+    "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Dofusdude",
     author="Survival",
     author_email="stelzo@steado.de",
     url="https://github.com/dofusdude/dofusdude-py",
     keywords=["OpenAPI", "OpenAPI-Generator", "Dofusdude"],
-    python_requires=">=3.7",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
+    long_description_content_type='text/markdown',
     long_description="""\
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don&#x27;t write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
-    """
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don&#39;t write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    """,
+    package_data={"dofusdude": ["py.typed"]},
 )
```

### Comparing `dofusdude-0.7.1/test/test_models/test_almanax_entry.py` & `dofusdude-0.7.2/test/test_create_almanax_webhook_mentions_value_inner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,57 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.almanax_entry import AlmanaxEntry
-from dofusdude import configuration
+from dofusdude.models.create_almanax_webhook_mentions_value_inner import CreateAlmanaxWebhookMentionsValueInner  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestCreateAlmanaxWebhookMentionsValueInner(unittest.TestCase):
+    """CreateAlmanaxWebhookMentionsValueInner unit test stubs"""
 
-class TestAlmanaxEntry(unittest.TestCase):
-    """AlmanaxEntry unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test CreateAlmanaxWebhookMentionsValueInner
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `CreateAlmanaxWebhookMentionsValueInner`
+        """
+        model = dofusdude.models.create_almanax_webhook_mentions_value_inner.CreateAlmanaxWebhookMentionsValueInner()  # noqa: E501
+        if include_optional :
+            return CreateAlmanaxWebhookMentionsValueInner(
+                discord_id = 1234, 
+                is_role = True, 
+                ping_days_before = 1
+            )
+        else :
+            return CreateAlmanaxWebhookMentionsValueInner(
+        )
+        """
+
+    def testCreateAlmanaxWebhookMentionsValueInner(self):
+        """Test CreateAlmanaxWebhookMentionsValueInner"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_almanax_webhook.py` & `dofusdude-0.7.2/test/test_almanax_webhook_daily_settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,56 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.almanax_webhook import AlmanaxWebhook
-from dofusdude import configuration
+from dofusdude.models.almanax_webhook_daily_settings import AlmanaxWebhookDailySettings  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestAlmanaxWebhookDailySettings(unittest.TestCase):
+    """AlmanaxWebhookDailySettings unit test stubs"""
 
-class TestAlmanaxWebhook(unittest.TestCase):
-    """AlmanaxWebhook unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test AlmanaxWebhookDailySettings
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `AlmanaxWebhookDailySettings`
+        """
+        model = dofusdude.models.almanax_webhook_daily_settings.AlmanaxWebhookDailySettings()  # noqa: E501
+        if include_optional :
+            return AlmanaxWebhookDailySettings(
+                timezone = 'Europe/Paris', 
+                midnight_offset = 0
+            )
+        else :
+            return AlmanaxWebhookDailySettings(
+        )
+        """
+
+    def testAlmanaxWebhookDailySettings(self):
+        """Test AlmanaxWebhookDailySettings"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_condition_entry.py` & `dofusdude-0.7.2/test/test_condition_entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,60 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.condition_entry import ConditionEntry
-from dofusdude import configuration
-
+from dofusdude.models.condition_entry import ConditionEntry  # noqa: E501
+from dofusdude.rest import ApiException
 
 class TestConditionEntry(unittest.TestCase):
     """ConditionEntry unit test stubs"""
-    _configuration = configuration.Configuration()
 
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ConditionEntry
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ConditionEntry`
+        """
+        model = dofusdude.models.condition_entry.ConditionEntry()  # noqa: E501
+        if include_optional :
+            return ConditionEntry(
+                operator = '', 
+                int_value = 56, 
+                element = dofusdude.models.condition_entry_element.Condition_Entry_element(
+                    name = '', 
+                    id = 56, 
+                    is_meta = True, )
+            )
+        else :
+            return ConditionEntry(
+        )
+        """
+
+    def testConditionEntry(self):
+        """Test ConditionEntry"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_cosmetic.py` & `dofusdude-0.7.2/test/test_mount_list_entry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,62 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.cosmetic import Cosmetic
-from dofusdude import configuration
+from dofusdude.models.mount_list_entry import MountListEntry  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestMountListEntry(unittest.TestCase):
+    """MountListEntry unit test stubs"""
 
-class TestCosmetic(unittest.TestCase):
-    """Cosmetic unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test MountListEntry
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `MountListEntry`
+        """
+        model = dofusdude.models.mount_list_entry.MountListEntry()  # noqa: E501
+        if include_optional :
+            return MountListEntry(
+                ankama_id = 56, 
+                name = '', 
+                family_name = '', 
+                image_urls = dofusdude.models.image_urls.Image-Urls(
+                    icon = '', 
+                    sd = '', 
+                    hq = '', 
+                    hd = '', )
+            )
+        else :
+            return MountListEntry(
+        )
+        """
+
+    def testMountListEntry(self):
+        """Test MountListEntry"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_create_almanax_webhook.py` & `dofusdude-0.7.2/test/test_mounts_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,62 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
 
 import dofusdude
-from dofusdude.model.create_almanax_webhook import CreateAlmanaxWebhook
-from dofusdude import configuration
+from dofusdude.api.mounts_api import MountsApi  # noqa: E501
+from dofusdude.rest import ApiException
+
+
+class TestMountsApi(unittest.TestCase):
+    """MountsApi unit test stubs"""
+
+    def setUp(self):
+        self.api = dofusdude.api.mounts_api.MountsApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_get_all_mounts_list(self):
+        """Test case for get_all_mounts_list
+
+        List All Mounts  # noqa: E501
+        """
+        pass
+
+    def test_get_mounts_list(self):
+        """Test case for get_mounts_list
+
+        List Mounts  # noqa: E501
+        """
+        pass
+
+    def test_get_mounts_search(self):
+        """Test case for get_mounts_search
+
+        Search Mounts  # noqa: E501
+        """
+        pass
 
+    def test_get_mounts_single(self):
+        """Test case for get_mounts_single
 
-class TestCreateAlmanaxWebhook(unittest.TestCase):
-    """CreateAlmanaxWebhook unit test stubs"""
-    _configuration = configuration.Configuration()
+        Single Mounts  # noqa: E501
+        """
+        pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_create_rss_webhook.py` & `dofusdude-0.7.2/test/test_twitter_webhook.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,69 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.create_rss_webhook import CreateRSSWebhook
-from dofusdude import configuration
+from dofusdude.models.twitter_webhook import TwitterWebhook  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestTwitterWebhook(unittest.TestCase):
+    """TwitterWebhook unit test stubs"""
 
-class TestCreateRSSWebhook(unittest.TestCase):
-    """CreateRSSWebhook unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test TwitterWebhook
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TwitterWebhook`
+        """
+        model = dofusdude.models.twitter_webhook.TwitterWebhook()  # noqa: E501
+        if include_optional :
+            return TwitterWebhook(
+                id = '', 
+                whitelist = [
+                    ''
+                    ], 
+                blacklist = [
+                    ''
+                    ], 
+                subscriptions = [
+                    ''
+                    ], 
+                format = 'discord', 
+                preview_length = 280, 
+                created_at = '2022-10-25T15:32:37.406281+02:00', 
+                last_fired_at = '2022-10-25T15:35:37.103240+02:00', 
+                updated_at = '2022-10-25T15:32:37.406281+02:00'
+            )
+        else :
+            return TwitterWebhook(
+        )
+        """
+
+    def testTwitterWebhook(self):
+        """Test TwitterWebhook"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_create_twitter_webhook.py` & `dofusdude-0.7.2/test/test_effects_entry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,64 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.create_twitter_webhook import CreateTwitterWebhook
-from dofusdude import configuration
+from dofusdude.models.effects_entry import EffectsEntry  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestEffectsEntry(unittest.TestCase):
+    """EffectsEntry unit test stubs"""
 
-class TestCreateTwitterWebhook(unittest.TestCase):
-    """CreateTwitterWebhook unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test EffectsEntry
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `EffectsEntry`
+        """
+        model = dofusdude.models.effects_entry.EffectsEntry()  # noqa: E501
+        if include_optional :
+            return EffectsEntry(
+                int_minimum = 56, 
+                int_maximum = 56, 
+                type = dofusdude.models.effects_entry_type.Effects_Entry_type(
+                    name = '', 
+                    id = 56, 
+                    is_meta = True, 
+                    is_active = True, ), 
+                ignore_int_min = True, 
+                ignore_int_max = True, 
+                formatted = ''
+            )
+        else :
+            return EffectsEntry(
+        )
+        """
+
+    def testEffectsEntry(self):
+        """Test EffectsEntry"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_effects_entry.py` & `dofusdude-0.7.2/test/test_almanax_entry_tribute_item.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,62 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.effects_entry import EffectsEntry
-from dofusdude import configuration
+from dofusdude.models.almanax_entry_tribute_item import AlmanaxEntryTributeItem  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestAlmanaxEntryTributeItem(unittest.TestCase):
+    """AlmanaxEntryTributeItem unit test stubs"""
 
-class TestEffectsEntry(unittest.TestCase):
-    """EffectsEntry unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test AlmanaxEntryTributeItem
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `AlmanaxEntryTributeItem`
+        """
+        model = dofusdude.models.almanax_entry_tribute_item.AlmanaxEntryTributeItem()  # noqa: E501
+        if include_optional :
+            return AlmanaxEntryTributeItem(
+                ankama_id = 56, 
+                image_urls = dofusdude.models.image_urls.Image-Urls(
+                    icon = '', 
+                    sd = '', 
+                    hq = '', 
+                    hd = '', ), 
+                name = '', 
+                subtype = ''
+            )
+        else :
+            return AlmanaxEntryTributeItem(
+        )
+        """
+
+    def testAlmanaxEntryTributeItem(self):
+        """Test AlmanaxEntryTributeItem"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_equipment.py` & `dofusdude-0.7.2/test/test_almanax_entry_tribute.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,64 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.equipment import Equipment
-from dofusdude import configuration
+from dofusdude.models.almanax_entry_tribute import AlmanaxEntryTribute  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestAlmanaxEntryTribute(unittest.TestCase):
+    """AlmanaxEntryTribute unit test stubs"""
 
-class TestEquipment(unittest.TestCase):
-    """Equipment unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test AlmanaxEntryTribute
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `AlmanaxEntryTribute`
+        """
+        model = dofusdude.models.almanax_entry_tribute.AlmanaxEntryTribute()  # noqa: E501
+        if include_optional :
+            return AlmanaxEntryTribute(
+                item = dofusdude.models.almanax_entry_tribute_item.Almanax_Entry_tribute_item(
+                    ankama_id = 56, 
+                    image_urls = dofusdude.models.image_urls.Image-Urls(
+                        icon = '', 
+                        sd = '', 
+                        hq = '', 
+                        hd = '', ), 
+                    name = '', 
+                    subtype = '', ), 
+                quantity = 56
+            )
+        else :
+            return AlmanaxEntryTribute(
+        )
+        """
+
+    def testAlmanaxEntryTribute(self):
+        """Test AlmanaxEntryTribute"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_equipment_set.py` & `dofusdude-0.7.2/test/test_almanax_entry_bonus.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,58 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.equipment_set import EquipmentSet
-from dofusdude import configuration
+from dofusdude.models.almanax_entry_bonus import AlmanaxEntryBonus  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestAlmanaxEntryBonus(unittest.TestCase):
+    """AlmanaxEntryBonus unit test stubs"""
 
-class TestEquipmentSet(unittest.TestCase):
-    """EquipmentSet unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test AlmanaxEntryBonus
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `AlmanaxEntryBonus`
+        """
+        model = dofusdude.models.almanax_entry_bonus.AlmanaxEntryBonus()  # noqa: E501
+        if include_optional :
+            return AlmanaxEntryBonus(
+                description = '', 
+                type = dofusdude.models.get_meta_almanax_bonuses_200_response_inner.get_meta_almanax_bonuses_200_response_inner(
+                    id = '', 
+                    name = '', )
+            )
+        else :
+            return AlmanaxEntryBonus(
+        )
+        """
+
+    def testAlmanaxEntryBonus(self):
+        """Test AlmanaxEntryBonus"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_image_urls.py` & `dofusdude-0.7.2/test/test_create_twitter_webhook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,71 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.image_urls import ImageUrls
-from dofusdude import configuration
+from dofusdude.models.create_twitter_webhook import CreateTwitterWebhook  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestCreateTwitterWebhook(unittest.TestCase):
+    """CreateTwitterWebhook unit test stubs"""
 
-class TestImageUrls(unittest.TestCase):
-    """ImageUrls unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test CreateTwitterWebhook
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `CreateTwitterWebhook`
+        """
+        model = dofusdude.models.create_twitter_webhook.CreateTwitterWebhook()  # noqa: E501
+        if include_optional :
+            return CreateTwitterWebhook(
+                whitelist = [
+                    ''
+                    ], 
+                blacklist = [
+                    ''
+                    ], 
+                subscriptions = [
+                    ''
+                    ], 
+                format = 'discord', 
+                preview_length = 280, 
+                callback = 'https://discord.com/api/webhooks/XYZ'
+            )
+        else :
+            return CreateTwitterWebhook(
+                subscriptions = [
+                    ''
+                    ],
+                format = 'discord',
+                callback = 'https://discord.com/api/webhooks/XYZ',
+        )
+        """
+
+    def testCreateTwitterWebhook(self):
+        """Test CreateTwitterWebhook"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_item_list_entry.py` & `dofusdude-0.7.2/test/test_put_twitter_webhook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,64 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.item_list_entry import ItemListEntry
-from dofusdude import configuration
+from dofusdude.models.put_twitter_webhook import PutTwitterWebhook  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestPutTwitterWebhook(unittest.TestCase):
+    """PutTwitterWebhook unit test stubs"""
 
-class TestItemListEntry(unittest.TestCase):
-    """ItemListEntry unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test PutTwitterWebhook
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `PutTwitterWebhook`
+        """
+        model = dofusdude.models.put_twitter_webhook.PutTwitterWebhook()  # noqa: E501
+        if include_optional :
+            return PutTwitterWebhook(
+                whitelist = [
+                    ''
+                    ], 
+                blacklist = [
+                    ''
+                    ], 
+                subscriptions = [
+                    ''
+                    ], 
+                preview_length = 280
+            )
+        else :
+            return PutTwitterWebhook(
+        )
+        """
+
+    def testPutTwitterWebhook(self):
+        """Test PutTwitterWebhook"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_items_list_entry_typed.py` & `dofusdude-0.7.2/test/test_condition_entry_element.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,57 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.items_list_entry_typed import ItemsListEntryTyped
-from dofusdude import configuration
+from dofusdude.models.condition_entry_element import ConditionEntryElement  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestConditionEntryElement(unittest.TestCase):
+    """ConditionEntryElement unit test stubs"""
 
-class TestItemsListEntryTyped(unittest.TestCase):
-    """ItemsListEntryTyped unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ConditionEntryElement
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ConditionEntryElement`
+        """
+        model = dofusdude.models.condition_entry_element.ConditionEntryElement()  # noqa: E501
+        if include_optional :
+            return ConditionEntryElement(
+                name = '', 
+                id = 56, 
+                is_meta = True
+            )
+        else :
+            return ConditionEntryElement(
+        )
+        """
+
+    def testConditionEntryElement(self):
+        """Test ConditionEntryElement"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_links_paged.py` & `dofusdude-0.7.2/test/test_cosmetic_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,56 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.links_paged import LinksPaged
-from dofusdude import configuration
+from dofusdude.models.cosmetic_type import CosmeticType  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestCosmeticType(unittest.TestCase):
+    """CosmeticType unit test stubs"""
 
-class TestLinksPaged(unittest.TestCase):
-    """LinksPaged unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test CosmeticType
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `CosmeticType`
+        """
+        model = dofusdude.models.cosmetic_type.CosmeticType()  # noqa: E501
+        if include_optional :
+            return CosmeticType(
+                name = '', 
+                id = 0
+            )
+        else :
+            return CosmeticType(
+        )
+        """
+
+    def testCosmeticType(self):
+        """Test CosmeticType"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_put_almanax_webhook.py` & `dofusdude-0.7.2/test/test_effects_entry_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,58 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.put_almanax_webhook import PutAlmanaxWebhook
-from dofusdude import configuration
+from dofusdude.models.effects_entry_type import EffectsEntryType  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestEffectsEntryType(unittest.TestCase):
+    """EffectsEntryType unit test stubs"""
 
-class TestPutAlmanaxWebhook(unittest.TestCase):
-    """PutAlmanaxWebhook unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test EffectsEntryType
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `EffectsEntryType`
+        """
+        model = dofusdude.models.effects_entry_type.EffectsEntryType()  # noqa: E501
+        if include_optional :
+            return EffectsEntryType(
+                name = '', 
+                id = 56, 
+                is_meta = True, 
+                is_active = True
+            )
+        else :
+            return EffectsEntryType(
+        )
+        """
+
+    def testEffectsEntryType(self):
+        """Test EffectsEntryType"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_put_rss_webhook.py` & `dofusdude-0.7.2/test/test_create_rss_webhook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,71 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import dofusdude
-from dofusdude.model.put_rss_webhook import PutRSSWebhook
-from dofusdude import configuration
+from dofusdude.models.create_rss_webhook import CreateRSSWebhook  # noqa: E501
+from dofusdude.rest import ApiException
 
+class TestCreateRSSWebhook(unittest.TestCase):
+    """CreateRSSWebhook unit test stubs"""
 
-class TestPutRSSWebhook(unittest.TestCase):
-    """PutRSSWebhook unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test CreateRSSWebhook
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `CreateRSSWebhook`
+        """
+        model = dofusdude.models.create_rss_webhook.CreateRSSWebhook()  # noqa: E501
+        if include_optional :
+            return CreateRSSWebhook(
+                whitelist = [
+                    ''
+                    ], 
+                blacklist = [
+                    ''
+                    ], 
+                subscriptions = [
+                    ''
+                    ], 
+                format = 'discord', 
+                preview_length = 2000, 
+                callback = 'https://discord.com/api/webhooks/XYZ'
+            )
+        else :
+            return CreateRSSWebhook(
+                subscriptions = [
+                    ''
+                    ],
+                format = 'discord',
+                callback = 'https://discord.com/api/webhooks/XYZ',
+        )
+        """
+
+    def testCreateRSSWebhook(self):
+        """Test CreateRSSWebhook"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_put_twitter_webhook.py` & `dofusdude-0.7.2/dofusdude/models/items_list_entry_typed_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,73 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-
-import dofusdude
-from dofusdude.model.put_twitter_webhook import PutTwitterWebhook
-from dofusdude import configuration
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""
 
-class TestPutTwitterWebhook(unittest.TestCase):
-    """PutTwitterWebhook unit test stubs"""
-    _configuration = configuration.Configuration()
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import Optional
+from pydantic import BaseModel, StrictInt, StrictStr
+
+class ItemsListEntryTypedType(BaseModel):
+    """
+    ItemsListEntryTypedType
+    """
+    name: Optional[StrictStr] = None
+    id: Optional[StrictInt] = None
+    __properties = ["name", "id"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> ItemsListEntryTypedType:
+        """Create an instance of ItemsListEntryTypedType from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> ItemsListEntryTypedType:
+        """Create an instance of ItemsListEntryTypedType from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return ItemsListEntryTypedType.parse_obj(obj)
+
+        _obj = ItemsListEntryTypedType.parse_obj({
+            "name": obj.get("name"),
+            "id": obj.get("id")
+        })
+        return _obj
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `dofusdude-0.7.1/test/test_models/test_set_list_entry.py` & `dofusdude-0.7.2/dofusdude/models/mount_list_entry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,81 @@
 # coding: utf-8
 
 """
     Dofusdude
 
-    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina  I highly recommend using the SDKs for quick results. I use them myself for microservices for the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
+    # A project for you - the developer. The free, always-up-to-date, low-latency, insert-buzzword-here Ankama API for your next cool project!  ## Client SDKs Don't write types or functions yourself - I already (kinda) did! 😉 - [Javascript](https://github.com/dofusdude/dofusdude-js) npm i dofusdude-js --save - [Typescript](https://github.com/dofusdude/dofusdude-ts) npm i dofusdude-ts --save - [Go](https://github.com/dofusdude/dodugo) go get -u github.com/dofusdude/dodugo - [Python](https://github.com/dofusdude/dofusdude-py) pip install dofusdude - [PHP](https://github.com/dofusdude/dofusdude-php)  Everything, including this site, is generated out of the [Docs Repo](https://github.com/dofusdude/api-docs). Consider it the Single Source of Truth. If there is a problem with the SDKs, create an issue there.  Your favorite language is missing? Please let me know!  # Main Features - 🥷 **Seamless Auto-Update** load data in the background when a new Dofus version is released and serving it within 2 minutes with atomic data source switching. No downtime and no effects for the user, just always up-to-date.  - ⚡ **Blazingly Fast** all data in-memory, aggressive caching over short time spans, HTTP/2 multiplexing, written in Go, optimized for low latency, hosted on bare metal in 🇩🇪.  - 📨 **Discord Integration** Ankama related Twitter, RSS and Almanax feeds to post to Discord servers with advanced features like filters or mentions. Use the endpoints as a dev or the official [Web Client](https://discord.dofusdude.com) as a user.  - 🩸 **Dofus 2 Beta** from stable to bleeding edge by replacing /dofus2 with /dofus2beta.  - 🗣️ **Multilingual** supporting _en_, _fr_, _es_, _pt_ including the dropped languages from the Dofus website _de_ and _it_.  - 🧠 **Search by Relevance** allowing typos in name and description, handled by language specific text analysis and indexing by the powerful [Meilisearch](https://www.meilisearch.com) written in Rust.  - 🕵️ **Complete** actual data from the game including items invisible to the encyclopedia like quest items.  - 🖼️ **HD Images** rendering vector graphics into PNGs up to 800x800 px in the background.   ## Current state - Weapons ✅ - Equipment ✅ - Sets ✅ - Resources ✅ - Consumables ✅ - Pets ✅ - Mounts ✅ - Cosmetics/Ceremonial Items ✅ - Harnesses ✅ - Quest Items ✅ - Almanax ✅ - Monsters ❌ - Spells ❌  ... and much more on the Roadmap on my Discord.   ## Deploy now. Use forever. Everything you see here on this site, you can use now and forever. Updates could introduce new fields, new paths or parameter but never break backwards compatibility, so no field or parameter will be deleted.  There is one exception! **The API will _always_ choose being up-to-date over everything else**. So if Ankama decides to drop languages from the game like they did with their website, the API will loose support for them, too.  ## Only the beginning... 🤯 I want this project to be useful and not just add plain GET-categories no one needs.  There is a long list of features I want to add (see the Roadmap on my [Discord](https://discord.gg/3EtHskZD8h)). But they are all focussed on you, the developers. So please let me know what you need. I will change the list based on demand.  # Get started! 🥳 Scroll down and try it for yourself!  Or see how these other awesome projects use it: - [KaellyBot](https://github.com/Kaysoro/KaellyBot) by Kaysoro - [Dofus Craftlist](https://dofuscraftlist-dev.netlify.app) by Lystina - [AlmanaxApp](https://almanaxapp.netlify.app) by Lystina - [DofuStuffSimulator](https://dofusstuffsimulator.netlify.app/)  I highly recommend using the SDKs for quick results. I use them myself for parts of the API.  ## Thank you! I highly welcome everyone on my [Discord](https://discord.gg/3EtHskZD8h) to just talk about projects and use cases or give feedback of any kind.  The servers have a fixed monthly cost to provide very fast responses. If you want to help me keeping them running or simply  donate, consider becoming a [GitHub Sponsor](https://github.com/sponsors/dofusdude).   # noqa: E501
 
-    The version of the OpenAPI document: 0.7.1
+    The version of the OpenAPI document: 0.7.2
     Contact: stelzo@steado.de
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-
-import dofusdude
-from dofusdude.model.set_list_entry import SetListEntry
-from dofusdude import configuration
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""
 
-class TestSetListEntry(unittest.TestCase):
-    """SetListEntry unit test stubs"""
-    _configuration = configuration.Configuration()
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import Optional
+from pydantic import BaseModel, StrictInt, StrictStr
+from dofusdude.models.image_urls import ImageUrls
+
+class MountListEntry(BaseModel):
+    """
+    MountListEntry
+    """
+    ankama_id: Optional[StrictInt] = None
+    name: Optional[StrictStr] = None
+    family_name: Optional[StrictStr] = None
+    image_urls: Optional[ImageUrls] = None
+    __properties = ["ankama_id", "name", "family_name", "image_urls"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> MountListEntry:
+        """Create an instance of MountListEntry from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of image_urls
+        if self.image_urls:
+            _dict['image_urls'] = self.image_urls.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> MountListEntry:
+        """Create an instance of MountListEntry from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return MountListEntry.parse_obj(obj)
+
+        _obj = MountListEntry.parse_obj({
+            "ankama_id": obj.get("ankama_id"),
+            "name": obj.get("name"),
+            "family_name": obj.get("family_name"),
+            "image_urls": ImageUrls.from_dict(obj.get("image_urls")) if obj.get("image_urls") is not None else None
+        })
+        return _obj
 
-if __name__ == '__main__':
-    unittest.main()
```

