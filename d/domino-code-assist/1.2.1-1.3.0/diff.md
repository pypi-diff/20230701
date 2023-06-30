# Comparing `tmp/domino_code_assist-1.2.1.tar.gz` & `tmp/domino_code_assist-1.3.0.tar.gz`

## Comparing `domino_code_assist-1.2.1.tar` & `domino_code_assist-1.3.0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/DominoLogoGrey.svg
--rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/DominoLogoWhite.svg
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/__init__.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/action.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/action_ui.py
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/actions_store.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/app.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/app_entrypoint.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/code.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/code.vue
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/components.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/crossfilter_widgets.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/css.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/css.vue
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/df_select.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/df_select.vue
--rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/domino_api.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/domino_lab_mock.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/express.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/hooks.py
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/layout.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/logging_workaround.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/nb_app.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/py36.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/sample_project_md.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/serialize.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/settings.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/thumbnail.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/util.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/widgets.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/__init__.py
--rw-r--r--   0        0        0    25812 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/assistant.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/assistant.vue
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/drawer.py
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/drawer.vue
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/handle_user_install.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/menu.vue
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/mixpanel.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/mixpanel.vue
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/notebook.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/__init__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/above_output.vue
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/code.py
--rw-r--r--   0        0        0    29157 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/drawer.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/experiment_search.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/experiment_search.vue
--rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/flaml_api.py
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/hyper_parameters.py
--rw-r--r--   0        0        0    13789 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/icon_classification.svg
--rw-r--r--   0        0        0    18124 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/icon_forecasting.svg
--rw-r--r--   0        0        0    16613 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/icon_regression.svg
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/open_experiment.py
--rw-r--r--   0        0        0    14661 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/placeholder.png
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/select_description.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/select_description.vue
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/store.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/data/__init__.py
--rw-r--r--   0        0        0    19263 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/data/penguins.csv
--rw-r--r--   0        0        0   239436 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/data/small_molecule_drugbank.csv
--rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/data/stocks_long.parquet
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/app_checker.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/app_checker.vue
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/button_clipboard.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/button_clipboard.vue
--rw-r--r--   0        0        0    91330 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/deploy-sync.png
--rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/deployer.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/filesystem_watcher.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/filesystem_watcher.vue
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/jupyter/__init__.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/jupyter/mixpanel_handler.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/jupyter/server_extension.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/__init__.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/big_query.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/data_source.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/drawer.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/object_store.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/panel.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/quick_start.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/snowflake_redshift.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/state.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/app.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/assistant.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/load_data.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/notebook.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/__init__.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/snippet_drawer.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/snippets.py
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/snippets_ui.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/tree.vue
--rw-r--r--   0        0        0  1192947 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/app.png
--rw-r--r--   0        0        0   530421 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/code_inserted.png
--rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/hover_cell.png
--rw-r--r--   0        0        0    35728 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/hover_icon.png
--rw-r--r--   0        0        0   357737 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/load_data.png
--rw-r--r--   0        0        0    93452 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/menu.png
--rw-r--r--   0        0        0    60379 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/menu_app.png
--rw-r--r--   0        0        0    61042 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/menu_transform.png
--rw-r--r--   0        0        0    60333 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/menu_visualizations.png
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/tour.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/tour.vue
--rw-r--r--   0        0        0   634871 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/transform.png
--rw-r--r--   0        0        0   587193 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/visualizations.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/column_description.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/column_description.vue
--rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/transform_action_ui.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/transform_drawer.py
--rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/transform_panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/viz/__init__.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/viz/drawer.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/viz/plot_builder.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/viz/state.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/app.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/app_entrypoint.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/deploy.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/express.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/layout.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/widgets.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/LICENSE.md
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/DominoLogoGrey.svg
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/DominoLogoWhite.svg
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/__init__.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/action.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/action_ui.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/actions_store.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/app.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/app_entrypoint.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/code.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/code.vue
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/components.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/crossfilter_widgets.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/css.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/css.vue
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/df_select.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/df_select.vue
+-rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/domino_api.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/domino_lab_mock.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/express.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/hooks.py
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/layout.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/logging_workaround.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/nb_app.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/py36.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/sample_project_md.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/serialize.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/settings.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/thumbnail.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/util.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/widgets.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/__init__.py
+-rw-r--r--   0        0        0    25812 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/assistant.py
+-rw-r--r--   0        0        0     7948 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/assistant.vue
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/drawer.py
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/drawer.vue
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/handle_user_install.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/menu.vue
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/mixpanel.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/mixpanel.vue
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/assistant/notebook.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/__init__.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/above_output.vue
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/code.py
+-rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/drawer.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/experiment_search.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/experiment_search.vue
+-rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/flaml_api.py
+-rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/hyper_parameters.py
+-rw-r--r--   0        0        0    13789 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/icon_classification.svg
+-rw-r--r--   0        0        0    18124 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/icon_forecasting.svg
+-rw-r--r--   0        0        0    16613 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/icon_regression.svg
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/open_experiment.py
+-rw-r--r--   0        0        0    14661 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/placeholder.png
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/select_description.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/select_description.vue
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/automl/store.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/data/__init__.py
+-rw-r--r--   0        0        0    19263 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/data/penguins.csv
+-rw-r--r--   0        0        0   239436 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/data/small_molecule_drugbank.csv
+-rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/data/stocks_long.parquet
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/app_checker.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/app_checker.vue
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/button_clipboard.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/button_clipboard.vue
+-rw-r--r--   0        0        0    91330 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/deploy-sync.png
+-rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/deployer.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/filesystem_watcher.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/deploy/filesystem_watcher.vue
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/jupyter/__init__.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/jupyter/mixpanel_handler.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/jupyter/server_extension.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/__init__.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/big_query.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/data_source.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/drawer.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/object_store.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/panel.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/quick_start.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/snowflake_redshift.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/load_data/state.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/playwright/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/playwright/app.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/playwright/assistant.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/playwright/load_data.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/playwright/notebook.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/playwright/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/snippets/__init__.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/snippets/snippet_drawer.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/snippets/snippets.py
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/snippets/snippets_ui.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/snippets/tree.vue
+-rw-r--r--   0        0        0  1192947 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/app.png
+-rw-r--r--   0        0        0   530421 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/code_inserted.png
+-rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/hover_cell.png
+-rw-r--r--   0        0        0    35728 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/hover_icon.png
+-rw-r--r--   0        0        0   357737 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/load_data.png
+-rw-r--r--   0        0        0    93452 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/menu.png
+-rw-r--r--   0        0        0    60379 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/menu_app.png
+-rw-r--r--   0        0        0    61042 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/menu_transform.png
+-rw-r--r--   0        0        0    60333 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/menu_visualizations.png
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/tour.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/tour.vue
+-rw-r--r--   0        0        0   634871 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/transform.png
+-rw-r--r--   0        0        0   587193 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/tour/visualizations.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/transform/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/transform/column_description.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/transform/column_description.vue
+-rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/transform/transform_action_ui.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/transform/transform_drawer.py
+-rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/transform/transform_panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/viz/__init__.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/viz/drawer.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/viz/plot_builder.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/domino_code_assist/viz/state.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/low_code_assistant/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/low_code_assistant/app.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/low_code_assistant/app_entrypoint.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/low_code_assistant/deploy.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/low_code_assistant/express.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/low_code_assistant/layout.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/low_code_assistant/widgets.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 domino_code_assist-1.3.0/PKG-INFO
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/DominoLogoGrey.svg` & `domino_code_assist-1.3.0/domino_code_assist/DominoLogoGrey.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/DominoLogoWhite.svg` & `domino_code_assist-1.3.0/domino_code_assist/DominoLogoWhite.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/__init__.py` & `domino_code_assist-1.3.0/domino_code_assist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Dominocode"""
 
-__version__ = "1.2.1"
+__version__ = "1.3.0"
 
 import os
 
 # isort: skip_file
 
 import domino_code_assist.logging_workaround
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/action.py` & `domino_code_assist-1.3.0/domino_code_assist/action.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/action_ui.py` & `domino_code_assist-1.3.0/domino_code_assist/action_ui.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/actions_store.py` & `domino_code_assist-1.3.0/domino_code_assist/actions_store.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/app.py` & `domino_code_assist-1.3.0/domino_code_assist/app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/app_entrypoint.py` & `domino_code_assist-1.3.0/domino_code_assist/app_entrypoint.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/code.py` & `domino_code_assist-1.3.0/domino_code_assist/code.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/code.vue` & `domino_code_assist-1.3.0/domino_code_assist/code.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/components.py` & `domino_code_assist-1.3.0/domino_code_assist/components.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/crossfilter_widgets.py` & `domino_code_assist-1.3.0/domino_code_assist/crossfilter_widgets.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/css.vue` & `domino_code_assist-1.3.0/domino_code_assist/css.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/df_select.py` & `domino_code_assist-1.3.0/domino_code_assist/df_select.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,25 @@
     template_file = (__file__, "df_select.vue")
 
     label = traitlets.Unicode("").tag(sync=True)
     items = traitlets.List().tag(sync=True)
     value = traitlets.Unicode(allow_none=True).tag(sync=True)
     hide_details = traitlets.Any(False).tag(sync=True)
     error_messages = traitlets.List(allow_none=True).tag(sync=True)
+    messages = traitlets.List(allow_none=True).tag(sync=True)
+    error = traitlets.Bool(False).tag(sync=True)
 
 
 @reacton.component
 def DfSelect(
     label: str,
     items: List,
     value: Optional[str],
     on_value: Callable[[Optional[str]], None],
     hide_details: bool = False,
     error_messages: Optional[List[str]] = None,
+    messages: Optional[List[str]] = [],
+    error: bool = False,
 ):
-    return DfSelectWidget.element(label=label, items=items, value=value, on_value=on_value, hide_details=hide_details, error_messages=error_messages)
+    return DfSelectWidget.element(
+        label=label, items=items, value=value, on_value=on_value, hide_details=hide_details, error_messages=error_messages, messages=messages, error=error
+    )
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/domino_api.py` & `domino_code_assist-1.3.0/domino_code_assist/domino_api.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/domino_lab_mock.py` & `domino_code_assist-1.3.0/domino_code_assist/domino_lab_mock.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/layout.py` & `domino_code_assist-1.3.0/domino_code_assist/layout.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/nb_app.py` & `domino_code_assist-1.3.0/domino_code_assist/nb_app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/py36.py` & `domino_code_assist-1.3.0/domino_code_assist/py36.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/sample_project_md.py` & `domino_code_assist-1.3.0/domino_code_assist/sample_project_md.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/serialize.py` & `domino_code_assist-1.3.0/domino_code_assist/serialize.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/settings.py` & `domino_code_assist-1.3.0/domino_code_assist/settings.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/thumbnail.py` & `domino_code_assist-1.3.0/domino_code_assist/thumbnail.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/util.py` & `domino_code_assist-1.3.0/domino_code_assist/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
 from keyword import iskeyword
-from typing import Any, Callable, Dict, List
+from typing import Any, Callable, Dict, List, Optional
 
 import nbformat as nbf
 import reacton
 import reacton.ipyvuetify as v
 import solara.util as sutil
 from IPython import get_ipython
 
@@ -136,7 +136,25 @@
 
     try:
         from mlflow import log_artifact
 
         log_artifact(file_name)
     finally:
         os.remove(file_name)
+
+
+def to_float(s: Optional[str]):
+    if s is None:
+        return None
+    try:
+        return float(s)
+    except ValueError:
+        return None
+
+
+def to_int(s: Optional[str]):
+    if s is None:
+        return None
+    try:
+        return int(s)
+    except ValueError:
+        return None
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/assistant/assistant.py` & `domino_code_assist-1.3.0/domino_code_assist/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/assistant/assistant.vue` & `domino_code_assist-1.3.0/domino_code_assist/assistant/assistant.vue`

 * *Files 4% similar despite different names*

```diff
@@ -43,31 +43,40 @@
     }
   },
   mounted() {
     window.lastLcaAsistant = this
     this.assistantDOM = this.$refs.domino_code_assistAssistantMenu;
     this.notebookId = test = DCA.getNotebookId(this.$el);
 
+    const [major, minor] = DCA.getFormatVersion(this.notebookId);
+    this.hasRequiredNbVersion = major > 4 || (major === 4 && minor >= 5);
+    if (!this.hasRequiredNbVersion) {
+      console.warn("Domino Code Assist requires notebook format version 4.5 or higher. Please upgrade your notebook.")
+    }
+
     this.cleanUpDOM()
 
     this.cleanups = [];
     DCA.assistants[this.notebookId] = this;
     this.isAttached = true;
 
     const update = () => {
       if (this.isAttached) {
         this.injectCells();
         this.notebook_path = DCA.getNotebookPath(this.notebookId);
-        const cells = DCA.getCells(this.notebookId);
-        cells.filter(cell => cell.model.type === "markdown" && cell.model.id == null)
-             .forEach(cell => cell.model.id = this.generate_id())
+
+        if (this.hasRequiredNbVersion) {
+          const cells = DCA.getCells(this.notebookId);
+          cells.filter(cell => cell.model.type === "markdown" && cell.model.id == null)
+               .forEach(cell => cell.model.id = this.generate_id())
           this.markdown_cells = Object.fromEntries(
               cells.filter(cell => cell.model.type === "markdown")
                    .map(cell => [cell.model.id, cell.model.value.text])
               )
+        }
         if (this._cell && this.snippet_edit_mode && this._cell.model.type === "code") {
           this.syncStyle(this._cell);
         }
         setTimeout(update, 1000);
       }
     }
     update();
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/assistant/drawer.py` & `domino_code_assist-1.3.0/domino_code_assist/assistant/drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/assistant/drawer.vue` & `domino_code_assist-1.3.0/domino_code_assist/assistant/drawer.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/assistant/handle_user_install.py` & `domino_code_assist-1.3.0/domino_code_assist/assistant/handle_user_install.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/assistant/menu.vue` & `domino_code_assist-1.3.0/domino_code_assist/assistant/menu.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/assistant/mixpanel.py` & `domino_code_assist-1.3.0/domino_code_assist/assistant/mixpanel.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/assistant/mixpanel.vue` & `domino_code_assist-1.3.0/domino_code_assist/assistant/mixpanel.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/above_output.vue` & `domino_code_assist-1.3.0/domino_code_assist/automl/above_output.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/code.py` & `domino_code_assist-1.3.0/domino_code_assist/automl/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 mlflow.autolog(disable=True)
 
 with mlflow.start_run() as run:
     run_name = run.data.tags["mlflow.runName"]
     print("Run name: ", run_name)
     display(dca.automl.OpenExperiment(experiment_name))
     automl = AutoML(metric="___optimization_metric___")
-    automl.fit(dataframe=df_automl, label=label, task="___ml_task___", period=___period___, time_budget=___time_budget___, max_iter=___max_iterations___, custom_hp=custom_hp, estimator_list=estimator_list)
+    automl.fit(dataframe=df_automl, label=label, task="___ml_task___", period=___period___, time_budget=___time_budget___, max_iter=___max_iterations___, custom_hp=custom_hp, estimator_list=estimator_list, eval_method=None)
     # Log the best model
     train = df_automl.drop(label, axis=1)[:5]
     predictions = pd.DataFrame({label: automl.predict(train)})
     mlflow.sklearn.log_model(automl, "model", signature=infer_signature(train, predictions), input_example=train)
     # Find the best run
     best_run = mlflow.search_runs(
         experiment_ids=[experiment.experiment_id],
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/drawer.py` & `domino_code_assist-1.3.0/domino_code_assist/automl/drawer.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from typing import Any, Callable, Dict, List, Optional, cast
 
 import mlflow
 import pandas as pd
 import reacton.ipyvuetify as v
 import solara
 from mlflow.utils.name_utils import _generate_random_name
+from reacton import use_effect
 from reacton.ipyvue import use_event
 from solara.components.input import _use_input_numeric
 from solara.lab import Ref
 
 from domino_code_assist import util
-from domino_code_assist.assistant import drawer
+from domino_code_assist.assistant import drawer, mixpanel
 from domino_code_assist.automl.experiment_search import ExperimentSearch
 from domino_code_assist.automl.store import (
     AVAILABLE_TASKS,
     MLTask,
     TaskConfig,
     get_task_arg_for_name,
     ml_task,
@@ -96,14 +97,25 @@
                 code = code.replace("estimator_list = ___estimator_list___\ncustom_hp = ___custom_hp___\n\n", "")
                 code = code.replace(", custom_hp=custom_hp, estimator_list=estimator_list", "")
             else:
                 code = code.replace("___estimator_list___", str(config.custom_learners_enabled).replace("'", '"'))
                 code = code.replace(
                     "___custom_hp___", hyper_parameters.get_hyper_parameters_string(config.custom_learners or {}, config.custom_learners_enabled or [])
                 )
+
+            if config.resampling_strategy != "Auto":
+                if config.resampling_strategy == "Holdout":
+                    method = "holdout"
+                    arg = f"split_ratio={config.split_ratio}"
+                else:
+                    method = "cv"
+                    arg = f"n_splits={config.folds}"
+                code = code.replace(", eval_method=None", f', eval_method="{method}", {arg}')
+            else:
+                code = code.replace(", eval_method=None", "")
     else:
         code = f"# TODO: insert {task.task_type} code. {task.task_config}"
 
     return code
 
 
 @solara.component
@@ -115,27 +127,32 @@
             solara.Image(os.path.join(os.path.dirname(__file__), task_info.image), width="120px")
         with solara.Div():
             solara.Div(children=task_info.name, style_="font-size: 20px")
             solara.Div(children=task_info.description, style_="font-size: 14px")
             if task_info.soon:
                 v.Chip(children="Coming soon", color="green", small=True, style_="margin-top: 8px", dark=True)
 
-    v.use_event(tile, "click", lambda *args: on_task_info(task_info) if not task_info.soon else None)
+    def on_click(*args):
+        if not task_info.soon:
+            on_task_info(task_info)
+        mixpanel.api.track_with_defaults("interaction", {"section": "automl", "type": "select_task", "task": task_info.name})
+
+    v.use_event(tile, "click", on_click)
 
 
 @solara.component
 def FixHorizontalScrollingInDialog(children):
     # See: https://github.com/vuetifyjs/vuetify/issues/3765
     assert len(children) == 1
     use_event(children[0], "wheel.stop", lambda *args: None)
     return children[0]
 
 
 @solara.component
-def MlTaskConfigUI(dfs: List[str], task_type, edit: bool, on_load_own_data: Callable[[], None]):
+def MlTaskConfigUI(dfs: List[str], task_type, edit: bool, on_load_own_data: Callable[[], None], emphasize_errors: bool):
     ml_task.use()
     task_config_store.use()
 
     expanded, set_expanded = solara.use_state([0])
     column_menu_open, set_column_menu_open = solara.use_state(cast(Optional[str], None))
 
     extended_dfs: List[Any] = dfs
@@ -177,15 +194,19 @@
             return None
         Ref(task_config_store.fields.time_column).set(date_time_columns[0])
 
     solara.use_memo(pre_select_time_column, [date_time_columns])
 
     int_period, set_int_period = solara.use_state(cast(Optional[int], task_config_store.value.period))
     period, set_period, period_error = _use_input_numeric(int, optional=True, value=int_period, on_value=set_int_period)
-    Ref(task_config_store.fields.period).set(period if not period_error else None)
+
+    def set_value():
+        Ref(task_config_store.fields.period).set(period if not period_error else None)
+
+    use_effect(set_value, [period, period_error])
 
     def available_items(used_items: Optional[List[Optional[str]]], used_description: str):
         if available_columns is None or df is None:
             return None
         return [
             {
                 "text": col + (f" ({used_description})" if col in (used_items or []) else ""),
@@ -231,36 +252,39 @@
                             with v.Col(class_="py-1").key("df"):
                                 DfSelect(
                                     value=task_config_store.value.df_var_name,
                                     label="Data frame",
                                     on_value=set_df_var_name,
                                     items=extended_dfs or [],
                                     hide_details=bool(task_config_store.value.df_var_name),
-                                    error_messages=["required"] if not task_config_store.value.df_var_name else None,
+                                    error=emphasize_errors and not bool(task_config_store.value.df_var_name),
+                                    messages=["required"] if not task_config_store.value.df_var_name else None,
                                 )
                             if task_type and task_type.startswith("Forecasting"):
                                 with v.Col(class_="py-1").key("time"):
                                     v.Select(
                                         label="Time column",
                                         items=date_time_columns,
                                         hide_details=bool(task_config_store.value.target),
                                         v_model=task_config_store.value.time_column,
                                         on_v_model=Ref(task_config_store.fields.time_column).set,
-                                        error_messages=["required"] if not task_config_store.value.time_column else None,
+                                        error=emphasize_errors and not bool(task_config_store.value.time_column),
+                                        messages=["required"] if not task_config_store.value.time_column else None,
                                         no_data_text="No date/time columns found",
-                                    )
+                                    ).meta(ref="TimeColumnSelect")
                             with v.Col(class_="py-1").key("predict"):
                                 v.Select(
                                     label="Predict value",
                                     items=available_columns,
                                     clearable=True,
                                     hide_details=bool(task_config_store.value.target),
                                     v_model=task_config_store.value.target,
                                     on_v_model=task_config_store.set_target,
-                                    error_messages=["required"] if not task_config_store.value.target else None,
+                                    error=emphasize_errors and not bool(task_config_store.value.target),
+                                    messages=["required"] if not task_config_store.value.target else None,
                                 )
                         with v.Row():
 
                             def on_features(v: List[str]):
                                 Ref(task_config_store.fields.exclude_features).set(
                                     [c for c in (available_columns or []) if c not in v and c != task_config_store.value.target]
                                 )
@@ -269,15 +293,16 @@
                                 v.Select(
                                     label="Features",
                                     items=available_items([task_config_store.value.target], "Predict value"),
                                     multiple=True,
                                     chips=True,
                                     deletable_chips=True,
                                     hide_details=bool(features),
-                                    error_messages=["required"] if not features else None,
+                                    error=emphasize_errors and not bool(features),
+                                    messages=["required"] if not features else None,
                                     v_model=features,
                                     on_v_model=on_features,
                                 )
                         if task_type and task_type.startswith("Forecasting"):
                             with v.Row():
                                 with v.Col(class_="py-1", sm=2):
                                     period_error_message = None
@@ -287,15 +312,16 @@
                                         period_error_message = "invalid"
 
                                     v.TextField(
                                         label="Period",
                                         clearable=True,
                                         v_model=period,
                                         on_v_model=set_period,
-                                        error_messages=period_error_message,
+                                        error=emphasize_errors and bool(period_error_message),
+                                        messages=period_error_message,
                                         hide_details=bool(not period_error_message),
                                     )
                                 with v.Col(class_="py-1", sm=2):
                                     with solara.ToggleButtonsSingle(
                                         value="regression" if ml_task.value.task_type == "Forecasting" else "classification",  # type: ignore
                                         on_value=lambda val: Ref(ml_task.fields.task_type).set(
                                             "Forecasting" if val == "regression" else "Forecasting (classification)"
@@ -371,15 +397,64 @@
                             with v.Col(class_="py-1"):
                                 v.Select(
                                     label="Unit",
                                     items=["Seconds", "Minutes", "Hours"],
                                     hide_details=True,
                                 ).connect(Ref(task_config_store.fields.time_unit))
                 hyper_parameters.Hyperparameters(task)
-
+                with v.ExpansionPanel():
+                    with v.ExpansionPanelHeader():
+                        with solara.Div(style_="display: flex; flex-direction: row;"):
+                            with solara.Div(style_="min-width: 140px"):
+                                v.Html(tag="strong", children=["Resampling"])
+                            if 3 in expanded or (task_config_store.value.resampling_strategy == "Auto"):
+                                solara.Text("Customize the resampling method")
+                            else:
+                                with solara.ColumnsResponsive([6, 6], gutters=False, classes=["pa-0"]):
+                                    with solara.Row(gap="8px"):
+                                        solara.Text("Resampling strategy:", style="font-weight: bold; color: var(--jp-border-color1);")
+                                        solara.Text(task_config_store.value.resampling_strategy)
+                                    with solara.Row(gap="8px", classes=["pt-2"]):
+                                        if task_config_store.value.resampling_strategy == "Holdout":
+                                            solara.Text(
+                                                "Split ratio:",
+                                                style="font-weight: bold; color: var(--jp-border-color1);",
+                                            )
+                                            solara.Text(task_config_store.value.split_ratio)
+                                        else:
+                                            solara.Text(
+                                                "Folds:",
+                                                style="font-weight: bold; color: var(--jp-border-color1);",
+                                            )
+                                            solara.Text(task_config_store.value.folds)
+                    with v.ExpansionPanelContent():
+                        with v.Row():
+                            with v.Col(class_="py-1"):
+                                v.Select(label="Validation method", items=["Auto", "Holdout", "Cross validation"]).connect(
+                                    Ref(task_config_store.fields.resampling_strategy)
+                                )
+                            with v.Col(class_="py-1"):
+                                if task_config_store.value.resampling_strategy == "Holdout":
+                                    messages = None
+                                    if not task_config_store.value.split_ratio:
+                                        messages = ["required"]
+                                    elif util.to_float(task_config_store.value.split_ratio) is None:
+                                        messages = ["invalid"]
+                                    v.TextField(label="Split ratio", error_messages=messages).connect(Ref(task_config_store.fields.split_ratio)).key(
+                                        "split_ratio"
+                                    )
+                                elif task_config_store.value.resampling_strategy == "Cross validation":
+                                    messages = None
+                                    if not task_config_store.value.folds:
+                                        messages = ["required"]
+                                    elif util.to_int(task_config_store.value.folds) is None:
+                                        messages = ["invalid"]
+                                    v.TextField(label="Folds", error=emphasize_errors and bool(messages), messages=messages).key("folds").connect(
+                                        Ref(task_config_store.fields.folds)
+                                    )
         with FixHorizontalScrollingInDialog():
             with v.Col(style_="overflow: hidden;"):
                 if df is not None:
                     solara.DataFrame(
                         df,
                         items_per_page=10,
                         scrollable=True,
@@ -402,34 +477,52 @@
     on_close: Callable[[], None],
     on_load_own_data: Callable[[], None],
     overwrite_warning=None,
 ):
     ml_task.use()
     task_config_store.use()
 
+    emphasize_errors, set_emphasize_errors = solara.use_state(False)
+
+    def is_valid():
+        return (
+            ml_task.value.task_type in ["Regression", "Classification"]
+            or (
+                ml_task.value.task_type
+                and ml_task.value.task_type.startswith("Forecasting")
+                and task_config_store.value.period is not None
+                and task_config_store.value.time_column is not None
+            )
+        ) and task_config_store.is_valid()
+
     def on_apply():
-        complete_task = ml_task.value
-        if complete_task.task_type in ["Classification", "Regression", "Forecasting", "Forecasting (classification)"]:
-            task_config = replace(
-                task_config_store.value,
-                auto=hyper_parameters.auto.value,
-                custom_learners=hyper_parameters.learner_params.value,
-                custom_learners_enabled=hyper_parameters.selected_learners.value,
+        if is_valid():
+            complete_task = ml_task.value
+            if complete_task.task_type in ["Classification", "Regression", "Forecasting", "Forecasting (classification)"]:
+                task_config = replace(
+                    task_config_store.value,
+                    auto=hyper_parameters.auto.value,
+                    custom_learners=hyper_parameters.learner_params.value,
+                    custom_learners_enabled=hyper_parameters.selected_learners.value,
+                )
+                complete_task = replace(complete_task, task_config=task_config)
+            set_code(
+                {
+                    "code": generate_code(complete_task),
+                    "meta": dumps(complete_task),
+                }
             )
-            complete_task = replace(complete_task, task_config=task_config)
-        set_code(
-            {
-                "code": generate_code(complete_task),
-                "meta": dumps(complete_task),
-            }
-        )
-        on_close()
+            mixpanel.api.track_with_defaults("inserted code", {"section": "automl", "task_type": complete_task.task_type})
+            on_close()
+        else:
+            set_emphasize_errors(True)
 
     def init():
         hyper_param_scratchpad.set({})
+        set_emphasize_errors(False)
         if is_open and edit_data and edit:
             ml_task.set(edit_data)
             assert edit_data.task_config
             task_config_store.set(edit_data.task_config)
 
             assert edit_data.task_config
             hyper_parameters.auto.value = edit_data.task_config.auto
@@ -470,41 +563,30 @@
                 hyper_parameters.learner_params.value = current["learner_params"]
                 hyper_parameters.selected_learners.value = current["selected_learners"]
             else:
                 hyper_parameters.auto.value = True
                 hyper_parameters.learner_params.value = {}
                 hyper_parameters.selected_learners.value = flaml_api.get_estimator_ids_for_task(get_task_arg_for_name(ml_task.value.task_type))
 
-        if hyper_parameters.selected_learners.value is None:
+        if hyper_parameters.selected_learners.value is None and ml_task.value.task_type:
             hyper_parameters.selected_learners.value = flaml_api.get_estimator_ids_for_task(get_task_arg_for_name(ml_task.value.task_type))
 
     solara.use_effect(on_ml_task, [ml_task.value.task_type])
 
     def load_own_data():
         on_close()
         on_load_own_data()
 
     with drawer.RightDrawer(
         open=is_open,
         on_open=lambda v: on_close() if not v else None,
         title="AutoML" + (" - " + ml_task.value.task_type if ml_task.value.task_type else ""),
         edit=bool(edit),
         on_apply=on_apply,
-        apply_disabled=not (
-            (
-                ml_task.value.task_type in ["Regression", "Classification"]
-                or (
-                    ml_task.value.task_type
-                    and ml_task.value.task_type.startswith("Forecasting")
-                    and task_config_store.value.period is not None
-                    and task_config_store.value.time_column is not None
-                )
-            )
-            and task_config_store.is_valid()
-        ),
+        apply_disabled=not ml_task.value.task_type,
         show_var_out=False,
         width="1024px" if not ml_task.value.task_type else "100vw",
         warning_widget=overwrite_warning,
         class_="dca-ml-task-selection",
     ):
         with v.Stepper(v_model=1 if not ml_task.value.task_type else 2, elevation=0, class_="elevation-0", style_="margin: 0"):
             with v.StepperItems():
@@ -539,10 +621,10 @@
                             ),
                             ".",
                         ],
                     )
                     with solara.Div(style_="padding: 32px"):
                         if ml_task.value.task_type:
                             if ml_task.value.task_type in ["Classification", "Regression", "Forecasting", "Forecasting (classification)"]:
-                                MlTaskConfigUI(dfs, ml_task.value.task_type, edit, load_own_data)
+                                MlTaskConfigUI(dfs, ml_task.value.task_type, edit, load_own_data, emphasize_errors)
                             else:
                                 v.Chip(children=[ml_task.value.task_type])
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/experiment_search.py` & `domino_code_assist-1.3.0/domino_code_assist/automl/experiment_search.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/experiment_search.vue` & `domino_code_assist-1.3.0/domino_code_assist/automl/experiment_search.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/flaml_api.py` & `domino_code_assist-1.3.0/domino_code_assist/automl/flaml_api.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/hyper_parameters.py` & `domino_code_assist-1.3.0/domino_code_assist/automl/hyper_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,17 @@
                             solara.Text("Hyper-parameters: ", style="color: var(--jp-border-color1);")
                             solara.Text(
                                 f" {len(get_enabled_hyper_params(estimator))}/{len(flaml_api.get_hyper_parameters_for_task(estimator, task))} configured"
                             )
                         with solara.Row():
                             solara.Button(icon_name="mdi-pencil", icon=True, on_click=lambda estimator=estimator: on_open_params(estimator))
         if opened_estimator:
-            with v.Dialog(v_model=bool(opened_estimator), on_v_model=lambda on: set_opened_estimator(None) if not on else None, max_width="800px"):
+            with v.Dialog(v_model=bool(opened_estimator), on_v_model=lambda on: set_opened_estimator(None) if not on else None, max_width="800px").key(
+                "dialog"
+            ):
                 with v.Card(class_="dca-hyperparameters-dialog"):
                     with v.CardTitle():
                         solara.Text("Edit hyper-parameters for ", style="white-space: pre;")
                         solara.Text(opened_estimator.get("readable_name", opened_estimator["id"]), style="font-weight: bold;")
                     with v.CardText():
                         HyperParametersPanel(task, opened_estimator["id"])
                     with v.CardActions():
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/icon_classification.svg` & `domino_code_assist-1.3.0/domino_code_assist/automl/icon_classification.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/icon_forecasting.svg` & `domino_code_assist-1.3.0/domino_code_assist/automl/icon_forecasting.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/icon_regression.svg` & `domino_code_assist-1.3.0/domino_code_assist/automl/icon_regression.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/open_experiment.py` & `domino_code_assist-1.3.0/domino_code_assist/automl/open_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,19 @@
         else:
             finished = experiments_result.state == solara.ResultState.FINISHED
 
             if not experiments_result.value:
                 solara.Error("Could not find experiment.")
             else:
                 with solara.Div().key("found"):
-                    href = f"/experiments/integration-test/{settings.domino_project_name}/{experiments_result.value['experiment_id']}" if finished else ""
+                    href = (
+                        f"/experiments/{settings.domino_project_owner}/{settings.domino_project_name}/{experiments_result.value['experiment_id']}"
+                        if finished
+                        else ""
+                    )
                     solara.Button(
                         f"open experiment: {name}",
                         disabled=not finished,
                         color="primary",
                         icon_name="mdi-open-in-new",
                         href=href,
                         target="_blank",
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/placeholder.png` & `domino_code_assist-1.3.0/domino_code_assist/automl/placeholder.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/automl/store.py` & `domino_code_assist-1.3.0/domino_code_assist/automl/store.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dataclasses import asdict, dataclass
 from typing import Dict, List, Optional
 
 import solara
 from solara.lab import Ref
 
+from domino_code_assist import util
+
 
 @dataclass(frozen=True)
 class TaskInfo:
     name: str
     arg: str
     description: str
     image: str = "placeholder.png"
@@ -60,19 +62,31 @@
     max_time: Optional[int] = None
     time_unit: str = "Minutes"
     period: Optional[int] = None
     auto: bool = True
     custom_learners: Optional[Dict] = None
     custom_learners_enabled: Optional[List[str]] = None
     time_column: Optional[str] = None
+    resampling_strategy: str = "Auto"
+    split_ratio: str = "0.1"
+    folds: str = "5"
 
 
 class ReactiveTaskConfig(solara.lab.Reactive[TaskConfig]):
     def is_valid(self):
-        return bool(self.value.df_var_name and self.value.target and self.value.experiment_name)
+        return bool(
+            self.value.df_var_name
+            and self.value.target
+            and self.value.experiment_name
+            and (
+                self.value.resampling_strategy == "Auto"
+                or (self.value.resampling_strategy == "Holdout" and util.to_float(self.value.split_ratio) is not None)
+                or (self.value.resampling_strategy == "Cross validation" and util.to_int(self.value.folds) is not None)
+            )
+        )
 
     def get_features(self, all_columns):
         return [c for c in all_columns if c not in (self.value.exclude_features or []) and c != self.value.target] if all_columns is not None else None
 
     def set_target(self, target):
         if target in (self.value.exclude_features or []):
             Ref(self.fields.exclude_features).set([f for f in (self.value.exclude_features or []) if f != target])
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/data/penguins.csv` & `domino_code_assist-1.3.0/domino_code_assist/data/penguins.csv`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/data/small_molecule_drugbank.csv` & `domino_code_assist-1.3.0/domino_code_assist/data/small_molecule_drugbank.csv`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/data/stocks_long.parquet` & `domino_code_assist-1.3.0/domino_code_assist/data/stocks_long.parquet`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/deploy/app_checker.py` & `domino_code_assist-1.3.0/domino_code_assist/deploy/app_checker.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/deploy/app_checker.vue` & `domino_code_assist-1.3.0/domino_code_assist/deploy/app_checker.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/deploy/button_clipboard.vue` & `domino_code_assist-1.3.0/domino_code_assist/deploy/button_clipboard.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/deploy/deploy-sync.png` & `domino_code_assist-1.3.0/domino_code_assist/deploy/deploy-sync.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/deploy/deployer.py` & `domino_code_assist-1.3.0/domino_code_assist/deploy/deployer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/deploy/filesystem_watcher.py` & `domino_code_assist-1.3.0/domino_code_assist/deploy/filesystem_watcher.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/deploy/filesystem_watcher.vue` & `domino_code_assist-1.3.0/domino_code_assist/deploy/filesystem_watcher.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/jupyter/mixpanel_handler.py` & `domino_code_assist-1.3.0/domino_code_assist/jupyter/mixpanel_handler.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/jupyter/server_extension.py` & `domino_code_assist-1.3.0/domino_code_assist/jupyter/server_extension.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/load_data/big_query.py` & `domino_code_assist-1.3.0/domino_code_assist/load_data/big_query.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/load_data/data_source.py` & `domino_code_assist-1.3.0/domino_code_assist/load_data/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,10 +82,10 @@
                 object_store.Panel(ds)
             elif ds.datasource_type in snowflake_redshift.supported_types:
                 snowflake_redshift.Panel(ds)
             elif ds.datasource_type == "BigQueryConfig":
                 BigQueryPanel(ds=ds).key("bq" + data_source.value.name)  # type: ignore
             if data_source.value.sample:
                 with solara.Div(class_="ml-4"):
-                    solara.Warning("This table has to many rows. A sample of this table will be loaded.")
+                    solara.Warning("This table has too many rows. A sample of this table will be loaded.")
 
     return main
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/load_data/drawer.py` & `domino_code_assist-1.3.0/domino_code_assist/load_data/drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/load_data/object_store.py` & `domino_code_assist-1.3.0/domino_code_assist/load_data/object_store.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/load_data/panel.py` & `domino_code_assist-1.3.0/domino_code_assist/load_data/panel.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/load_data/quick_start.py` & `domino_code_assist-1.3.0/domino_code_assist/load_data/quick_start.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/load_data/snowflake_redshift.py` & `domino_code_assist-1.3.0/domino_code_assist/load_data/snowflake_redshift.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,21 @@
                 return pd.concat([df_tables, views])
         if ds.datasource_type == "RedshiftConfig":
             res = ds.query(
                 textwrap.dedent(
                     """\
                 select tab.table_schema as schema_name,
                        tab.table_name as name,
-                       tinf.tbl_rows as rows
+                       class.reltuples as rows
                 from svv_tables tab
-                         join svv_table_info tinf
-                              on tab.table_schema = tinf.schema
-                                  and tab.table_name = tinf.table
+                         join pg_class class
+                              on tab.table_name = class.relname
                 where tab.table_type = 'BASE TABLE'
                   and tab.table_schema not in('pg_catalog','information_schema')
-                  and tinf.tbl_rows > 1
+                  and class.reltuples > 1
                 """
                 )
             )
             return res.to_pandas()
         raise RuntimeError(f"Unknown datasource: {ds.datasource_type}")
 
     tables_result: solara.Result = solara.hooks.use_thread(get_tables, [ds])
```

### Comparing `domino_code_assist-1.2.1/domino_code_assist/load_data/state.py` & `domino_code_assist-1.3.0/domino_code_assist/load_data/state.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/playwright/app.py` & `domino_code_assist-1.3.0/domino_code_assist/playwright/app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/playwright/assistant.py` & `domino_code_assist-1.3.0/domino_code_assist/playwright/assistant.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/playwright/load_data.py` & `domino_code_assist-1.3.0/domino_code_assist/playwright/load_data.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/playwright/notebook.py` & `domino_code_assist-1.3.0/domino_code_assist/playwright/notebook.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/playwright/transform.py` & `domino_code_assist-1.3.0/domino_code_assist/playwright/transform.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/snippets/snippet_drawer.py` & `domino_code_assist-1.3.0/domino_code_assist/snippets/snippet_drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/snippets/snippets.py` & `domino_code_assist-1.3.0/domino_code_assist/snippets/snippets.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/snippets/snippets_ui.py` & `domino_code_assist-1.3.0/domino_code_assist/snippets/snippets_ui.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/snippets/tree.vue` & `domino_code_assist-1.3.0/domino_code_assist/snippets/tree.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/app.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/app.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/code_inserted.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/code_inserted.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/hover_cell.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/hover_cell.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/hover_icon.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/hover_icon.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/load_data.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/load_data.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/menu.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/menu.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/menu_app.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/menu_app.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/menu_transform.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/menu_transform.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/menu_visualizations.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/menu_visualizations.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/tour.py` & `domino_code_assist-1.3.0/domino_code_assist/tour/tour.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/tour.vue` & `domino_code_assist-1.3.0/domino_code_assist/tour/tour.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/transform.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/transform.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/tour/visualizations.png` & `domino_code_assist-1.3.0/domino_code_assist/tour/visualizations.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/transform/column_description.py` & `domino_code_assist-1.3.0/domino_code_assist/transform/column_description.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/transform/column_description.vue` & `domino_code_assist-1.3.0/domino_code_assist/transform/column_description.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/transform/transform_action_ui.py` & `domino_code_assist-1.3.0/domino_code_assist/transform/transform_action_ui.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/transform/transform_drawer.py` & `domino_code_assist-1.3.0/domino_code_assist/transform/transform_drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/transform/transform_panel.py` & `domino_code_assist-1.3.0/domino_code_assist/transform/transform_panel.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/viz/drawer.py` & `domino_code_assist-1.3.0/domino_code_assist/viz/drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/viz/plot_builder.py` & `domino_code_assist-1.3.0/domino_code_assist/viz/plot_builder.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/domino_code_assist/viz/state.py` & `domino_code_assist-1.3.0/domino_code_assist/viz/state.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.1/pyproject.toml` & `domino_code_assist-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "nbformat>=4.5",  # to support cell ids
     "notebook>=4.6",  # to support cell ids
     "openpyxl",
     "xlrd",
     "vaex-core",
     "flaml",
     "mlflow",
+    "flaml[catboost]",
     "lightgbm",
     "hcrystalball",
     "statsmodels",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

### Comparing `domino_code_assist-1.2.1/PKG-INFO` & `domino_code_assist-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: domino-code-assist
-Version: 1.2.1
+Version: 1.3.0
 Project-URL: Home, https://github.com/cerebrotech/domino-code-assist
 License-File: LICENSE.md
 Requires-Dist: dominodatalab; python_version >= '3.8'
 Requires-Dist: flaml
+Requires-Dist: flaml[catboost]
 Requires-Dist: hcrystalball
 Requires-Dist: humanize
 Requires-Dist: ipyvue
 Requires-Dist: ipyvuetify>=1.8.5
 Requires-Dist: ipywidgets<8
 Requires-Dist: lightgbm
 Requires-Dist: mlflow
```

