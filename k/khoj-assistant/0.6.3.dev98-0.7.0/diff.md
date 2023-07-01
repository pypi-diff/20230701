# Comparing `tmp/khoj_assistant-0.6.3.dev98.tar.gz` & `tmp/khoj_assistant-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jun 26 19:38:00 2023, max compression
+gzip compressed data, last modified: Sat Jul  1 12:44:22 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev98.tar` & `khoj_assistant-0.7.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/__init__.py
--rw-r--r--   0        0        0    10868 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17819 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3435 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0     9894 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     6222 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     4572 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6799 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    12798 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3644 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1828 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0   205167 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     6985 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    13690 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4001 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3070 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4158 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/LICENSE
--rw-r--r--   0        0        0    22944 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/README.md
--rw-r--r--   0        0        0     2801 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/pyproject.toml
--rw-r--r--   0        0        0    25306 2023-06-26 19:38:00.000000 khoj_assistant-0.6.3.dev98/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11337 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/configure.py
+-rw-r--r--   0        0        0     4956 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17819 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3532 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    14414 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     6212 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6990 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6799 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    19296 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3644 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0   205167 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6056 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13768 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7338 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5193 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    18153 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4394 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7560 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2112 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2510 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2995 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6852 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4215 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/LICENSE
+-rw-r--r--   0        0        0    23224 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/README.md
+-rw-r--r--   0        0        0     2841 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    25625 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/configure.py` & `khoj_assistant-0.7.0/src/khoj/configure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Standard Packages
 import sys
 import logging
 import json
 from enum import Enum
+from typing import Optional
 import requests
 
 # External Packages
 import schedule
 from fastapi.staticfiles import StaticFiles
 
 # Internal Packages
@@ -32,15 +33,15 @@
 
 def configure_server(args, required=False):
     if args.config is None:
         if required:
             logger.error(f"Exiting as Khoj is not configured.\nConfigure it via GUI or by editing {state.config_file}.")
             sys.exit(1)
         else:
-            logger.warn(
+            logger.warning(
                 f"Khoj is not configured.\nConfigure it via khoj GUI, plugins or by editing {state.config_file}."
             )
             return
     else:
         state.config = args.config
 
     # Initialize Processor from Config
@@ -74,91 +75,95 @@
 
 
 def configure_search_types(config: FullConfig):
     # Extract core search types
     core_search_types = {e.name: e.value for e in SearchType}
     # Extract configured plugin search types
     plugin_search_types = {}
-    if config.content_type.plugins:
+    if config.content_type and config.content_type.plugins:
         plugin_search_types = {plugin_type: plugin_type for plugin_type in config.content_type.plugins.keys()}
 
     # Dynamically generate search type enum by merging core search types with configured plugin search types
     return Enum("SearchType", merge_dicts(core_search_types, plugin_search_types))
 
 
-def configure_search(model: SearchModels, config: FullConfig, regenerate: bool, t: state.SearchType = None):
+def configure_search(model: SearchModels, config: FullConfig, regenerate: bool, t: Optional[state.SearchType] = None):
+    if config is None or config.content_type is None or config.search_type is None:
+        logger.warning("🚨 No Content or Search type is configured.")
+        return
+
     # Initialize Org Notes Search
-    if (t == state.SearchType.Org or t == None) and config.content_type.org:
+    if (t == state.SearchType.Org or t == None) and config.content_type.org and config.search_type.asymmetric:
         logger.info("🦄 Setting up search for orgmode notes")
         # Extract Entries, Generate Notes Embeddings
         model.org_search = text_search.setup(
             OrgToJsonl,
             config.content_type.org,
             search_config=config.search_type.asymmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter(), FileFilter()],
         )
 
     # Initialize Org Music Search
-    if (t == state.SearchType.Music or t == None) and config.content_type.music:
+    if (t == state.SearchType.Music or t == None) and config.content_type.music and config.search_type.asymmetric:
         logger.info("🎺 Setting up search for org-music")
         # Extract Entries, Generate Music Embeddings
         model.music_search = text_search.setup(
             OrgToJsonl,
             config.content_type.music,
             search_config=config.search_type.asymmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter()],
         )
 
     # Initialize Markdown Search
-    if (t == state.SearchType.Markdown or t == None) and config.content_type.markdown:
+    if (t == state.SearchType.Markdown or t == None) and config.content_type.markdown and config.search_type.asymmetric:
         logger.info("💎 Setting up search for markdown notes")
         # Extract Entries, Generate Markdown Embeddings
         model.markdown_search = text_search.setup(
             MarkdownToJsonl,
             config.content_type.markdown,
             search_config=config.search_type.asymmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter(), FileFilter()],
         )
 
     # Initialize Ledger Search
-    if (t == state.SearchType.Ledger or t == None) and config.content_type.ledger:
+    if (t == state.SearchType.Ledger or t == None) and config.content_type.ledger and config.search_type.symmetric:
         logger.info("💸 Setting up search for ledger")
         # Extract Entries, Generate Ledger Embeddings
         model.ledger_search = text_search.setup(
             BeancountToJsonl,
             config.content_type.ledger,
             search_config=config.search_type.symmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter(), FileFilter()],
         )
 
     # Initialize PDF Search
-    if (t == state.SearchType.Pdf or t == None) and config.content_type.pdf:
+    if (t == state.SearchType.Pdf or t == None) and config.content_type.pdf and config.search_type.asymmetric:
         logger.info("🖨️ Setting up search for pdf")
         # Extract Entries, Generate PDF Embeddings
         model.pdf_search = text_search.setup(
             PdfToJsonl,
             config.content_type.pdf,
             search_config=config.search_type.asymmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter(), FileFilter()],
         )
 
     # Initialize Image Search
-    if (t == state.SearchType.Image or t == None) and config.content_type.image:
+    if (t == state.SearchType.Image or t == None) and config.content_type.image and config.search_type.image:
         logger.info("🌄 Setting up search for images")
         # Extract Entries, Generate Image Embeddings
         model.image_search = image_search.setup(
             config.content_type.image, search_config=config.search_type.image, regenerate=regenerate
         )
 
-    if (t == state.SearchType.Github or t == None) and config.content_type.github:
+    if (t == state.SearchType.Github or t == None) and config.content_type.github and config.search_type.asymmetric:
         logger.info("🐙 Setting up search for github")
         # Extract Entries, Generate Github Embeddings
         model.github_search = text_search.setup(
             GithubToJsonl,
             config.content_type.github,
             search_config=config.search_type.asymmetric,
             regenerate=regenerate,
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/main.py` & `khoj_assistant-0.7.0/src/khoj/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 
 def set_state(args):
     state.config_file = args.config_file
     state.config = args.config
     state.verbose = args.verbose
     state.host = args.host
     state.port = args.port
+    state.demo = args.demo
 
 
 def start_server(app, host=None, port=None, socket=None):
     logger.info("🌖 Khoj is ready to use")
     if socket:
         uvicorn.run(app, proxy_headers=True, uds=socket, log_level="debug", use_colors=True, log_config=None)
     else:
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.7.0/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.7.0/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.0/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.0/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.0/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.0/src/khoj/interface/web/base_config.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 <!DOCTYPE html>
 <html data-theme="light">
     <head>
         <meta charset="utf-8">
+        <meta name="viewport" content="width=device-width, initial-scale=1.0 maximum-scale=1.0">
         <link rel="icon" type="image/png" sizes="128x128" href="/static/assets/icons/favicon-128x128.png">
         <title>Khoj - Settings</title>
         <link rel="stylesheet" href="/static/assets/pico.min.css">
         <link rel="stylesheet" href="/static/assets/khoj.css">
     </head>
     <body class="khoj-configure">
         <div class="khoj-header">
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
 
 
+
 [Khoj]  Chat Search Settings
 {% block content %} {% endblock %}
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.0/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.0/src/khoj/interface/web/chat.html`

 * *Files 22% similar despite different names*

```diff
@@ -80,41 +80,72 @@
                 chat();
             }
         }
 
         window.onload = function () {
             fetch('/api/chat?client=web')
                 .then(response => response.json())
-                .then(data => data.response)
-                .then(chat_logs => {
+                .then(data => {
+                    if (data.detail) {
+                        // If the server returns a 500 error with detail, render it as a message.
+                        renderMessage(data.detail + " You can configure Khoj chat in your <a class='inline-chat-link' href='/config'>settings</a>.", "khoj");
+                    }
+                    return data.response;
+                })
+                .then(response => {
                     // Render conversation history, if any
-                    chat_logs.forEach(chat_log => {
+                    response.forEach(chat_log => {
                         renderMessageWithReference(chat_log.message, chat_log.by, chat_log.context, new Date(chat_log.created));
                     });
+                })
+                .catch(err => {
+                    return;
                 });
 
              // Set welcome message on load
             renderMessage("Hey, what's up?", "khoj");
 
             // Fill query field with value passed in URL query parameters, if any.
             var query_via_url = new URLSearchParams(window.location.search).get("q");
             if (query_via_url) {
                 document.getElementById("chat-input").value = query_via_url;
                 chat();
             }
         }
     </script>
     <body>
-       <!--Add Header Logo and Nav Pane-->
+        <!--Add Header Logo and Nav Pane-->
         <div class="khoj-header">
-            <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+            {% if demo %}
+                <!-- Banner linking to https://khoj.dev -->
+                <div class="khoj-banner-container">
+                    <a class="khoj-banner" href="https://khoj.dev" target="_blank">
+                        <p id="khoj-banner" class="khoj-banner">
+                            Enroll in Khoj cloud to get your own Github assistant
+                        </p>
+                    </a>
+                    <input type="text" id="khoj-banner-email" placeholder="email" class="khoj-banner-email"></input>
+                    <button id="khoj-banner-submit" class="khoj-banner-button">Submit</button>
+                </div>
+            {% endif %}
+            {% if demo %}
+                <a href="https://khoj.dev" target="_blank">
+                    <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+                </a>
+            {% else %}
+                <a href="https://lantern.khoj.dev" target="_blank">
+                    <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+                </a>
+            {% endif %}
             <nav class="khoj-nav">
                 <a class="khoj-nav-selected" href="/chat">Chat</a>
                 <a href="/">Search</a>
-                <a href="/config">Settings</a>
+                {% if not demo %}
+                    <a href="/config">Settings</a>
+                {% endif %}
             </nav>
         </div>
 
         <!-- Chat Body -->
         <div id="chat-body"></div>
 
         <!-- Chat Footer -->
@@ -231,14 +262,20 @@
         .option:hover {
             box-shadow: 0 0 11px #aaa;
         }
         #chat-input {
             font-size: medium;
         }
 
+        a.inline-chat-link {
+            color: #475569;
+            text-decoration: none;
+            border-bottom: 1px dotted #475569;
+        }
+
         @media (pointer: coarse), (hover: none) {
             abbr[title] {
                 position: relative;
                 padding-left: 4px;  /* space references out to ease tapping */
             }
             abbr[title]:focus:after {
                 content: attr(title);
@@ -267,19 +304,107 @@
                 grid-column: 1;
             }
             #chat-footer {
                 padding: 0;
                 margin: 4px;
                 grid-template-columns: auto;
             }
+            a.khoj-banner {
+                display: block;
+            }
         }
         @media only screen and (min-width: 600px) {
             body {
                 grid-template-columns: auto min(70vw, 100%) auto;
                 grid-template-rows: auto minmax(80px, 100%) auto;
             }
             body > * {
                 grid-column: 2;
             }
         }
+
+        div.khoj-banner-container {
+            background: linear-gradient(-45deg, #FFC107, #FF9800, #FF5722, #FF9800, #FFC107);
+            background-size: 400% 400%;
+            animation: gradient 15s ease infinite;
+            text-align: center;
+            padding: 10px;
+        }
+
+        @keyframes gradient {
+            0% {
+                background-position: 0% 50%;
+            }
+            50% {
+                background-position: 100% 50%;
+            }
+            100% {
+                background-position: 0% 50%;
+            }
+        }
+
+        a.khoj-banner {
+            color: black;
+        }
+
+        a.khoj-logo {
+            text-align: center;
+        }
+
+        p.khoj-banner {
+            margin: 0;
+            padding: 10px;
+        }
+
+        button#khoj-banner-submit,
+        input#khoj-banner-email {
+            padding: 10px;
+            border-radius: 5px;
+            border: 1px solid #475569;
+            background: #f9fafc;
+        }
+
+        button#khoj-banner-submit:hover,
+        input#khoj-banner-email:hover {
+            box-shadow: 0 0 11px #aaa;
+        }
+
+        p#khoj-banner {
+            display: inline;
+        }
+
+        a.khoj-banner {
+            color: black;
+            text-decoration: none;
+        }
     </style>
+    <script>
+        var khojBannerSubmit = document.getElementById("khoj-banner-submit");
+
+        khojBannerSubmit.addEventListener("click", function(event) {
+            event.preventDefault();
+            var email = document.getElementById("khoj-banner-email").value;
+            fetch("https://lantern.khoj.dev/beta/users/", {
+                    method: "POST",
+                    body: JSON.stringify({
+                        email: email
+                    }),
+                    headers: {
+                        "Content-Type": "application/json"
+                    }
+                }).then(function(response) {
+                    return response.json();
+                }).then(function(data) {
+                    console.log(data);
+                    if (data.user != null) {
+                        document.getElementById("khoj-banner").innerHTML = "Thanks for signing up. We'll be in touch soon! 🚀";
+                        document.getElementById("khoj-banner-submit").remove();
+                    } else {
+                        document.getElementById("khoj-banner").innerHTML = "There was an error signing up. Please contact team@khoj.dev";
+                    }
+                }).catch(function(error) {
+                    console.log(error);
+                    document.getElementById("khoj-banner").innerHTML = "There was an error signing up. Please contact team@khoj.dev";
+                });
+            });
+    </script>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,9 @@
 
 
 
-[Khoj]  Chat Search Settings
+{% if demo %}
+Enroll_in_Khoj_cloud_to_get_your_own_Github_assistant
+ [                    ] Submit
+{% endif %} {% if demo %} [Khoj] {% else %} [Khoj] {% endif %}  Chat Search {%
+if not demo %} Settings {% endif %}
 [                    ]
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.0/src/khoj/interface/web/config.html`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 <script>
     var configure = document.getElementById("configure");
     configure.addEventListener("click", function(event) {
         event.preventDefault();
         configure.disabled = true;
         configure.innerHTML = "Configuring...";
         const csrfToken = document.cookie.split('; ').find(row => row.startsWith('csrftoken'))?.split('=')[1];
-        fetch('/api/update?force=true&client=web', {
+        fetch('/api/update?&client=web', {
             method: 'GET',
             headers: {
                 'Content-Type': 'application/json',
                 'X-CSRFToken': csrfToken
             }
         })
         .then(response => response.json())
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.0/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.0/src/khoj/interface/web/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -10,77 +10,116 @@
     </head>
     <script type="text/javascript" src="/static/assets/org.min.js"></script>
     <script type="text/javascript" src="/static/assets/markdown-it.min.js"></script>
 
     <script>
         function render_image(item) {
             return `
+            <div class="results-image">
             <a href="${item.entry}" class="image-link">
                 <img id=${item.score} src="${item.entry}?${Math.random()}"
                     title="Effective Score: ${item.score}, Meta: ${item.additional.metadata_score}, Image: ${item.additional.image_score}"
                     class="image">
-            </a>`
+            </a>
+            </div>`;
         }
 
         function render_org(query, data, classPrefix="") {
-            var orgCode = data.map(function (item) {
-                return `${item.entry}`
-            }).join("\n")
-            var orgParser = new Org.Parser();
-            var orgDocument = orgParser.parse(orgCode);
-            var orgHTMLDocument = orgDocument.convert(Org.ConverterHTML, { htmlClassPrefix: classPrefix });
-            return orgHTMLDocument.toString();
+            return data.map(function (item) {
+                var orgParser = new Org.Parser();
+                var orgDocument = orgParser.parse(item.entry);
+                var orgHTMLDocument = orgDocument.convert(Org.ConverterHTML, { htmlClassPrefix: classPrefix });
+                return `<div class="results-org">` + orgHTMLDocument.toString() + `</div>`;
+            }).join("\n");
         }
 
         function render_markdown(query, data) {
             var md = window.markdownit();
-            return md.render(data.map(function (item) {
+            return data.map(function (item) {
+                let rendered = "";
                 if (item.additional.file.startsWith("http")) {
                     lines = item.entry.split("\n");
-                    return `${lines[0]}\t[*](${item.additional.file})\n${lines.slice(1).join("\n")}`;
+                    rendered = md.render(`${lines[0]}\t[*](${item.additional.file})\n${lines.slice(1).join("\n")}`);
                 }
-                return `${item.entry}`;
-            }).join("\n"));
+                else {
+                    rendered = md.render(`${item.entry}`);
+                }
+                return `<div class="results-markdown">` + rendered + `</div>`;
+            }).join("\n");
         }
 
         function render_ledger(query, data) {
-            return `<div id="results-ledger">` + data.map(function (item) {
-                return `<p>${item.entry}</p>`
-            }).join("\n") + `</div>`;
+            return data.map(function (item) {
+                return `<div class="results-ledger">` + `<p>${item.entry}</p>` + `</div>`;
+            }).join("\n");
         }
 
         function render_pdf(query, data) {
-            return `<div id="results-pdf">` + data.map(function (item) {
+            return data.map(function (item) {
                 let compiled_lines = item.additional.compiled.split("\n");
                 let filename = compiled_lines.shift();
                 let text_match = compiled_lines.join("\n")
-                return `<h2>${filename}</h2>\n<p>${text_match}</p>`
-            }).join("\n") + `</div>`;
+                return `<div class="results-pdf">` + `<h2>${filename}</h2>\n<p>${text_match}</p>` + `</div>`;
+            }).join("\n");
+        }
+
+        function render_multiple(query, data, type) {
+            let html = "";
+            data.forEach(item => {
+                if (item.additional.file.endsWith(".org")) {
+                    html += render_org(query, [item], "org-");
+                } else if (
+                    item.additional.file.endsWith(".md") ||
+                    item.additional.file.endsWith(".markdown") ||
+                        (item.additional.file.includes("issues") && item.additional.file.includes("github.com")) ||
+                        (item.additional.file.includes("commit") && item.additional.file.includes("github.com"))
+                    )
+                {
+                    html += render_markdown(query, [item]);
+                } else if (item.additional.file.endsWith(".pdf")) {
+                    html += render_pdf(query, [item]);
+                }
+            });
+            return html;
         }
 
-        function render_json(data, query, type) {
+        function render_results(data, query, type) {
+            let results = "";
             if (type === "markdown") {
-                return render_markdown(query, data);
+                results = render_markdown(query, data);
             } else if (type === "org") {
-                return render_org(query, data);
+                results = render_org(query, data, "org-");
             } else if (type === "music") {
-                return render_org(query, data, "music-");
+                results = render_org(query, data, "music-");
             } else if (type === "image") {
-                return data.map(render_image).join('');
+                results = data.map(render_image).join('');
             } else if (type === "ledger") {
-                return render_ledger(query, data);
+                results = render_ledger(query, data);
             } else if (type === "pdf") {
-                return render_pdf(query, data);
-            } else if (type == "github") {
-                return render_markdown(query, data);
+                results = render_pdf(query, data);
+            } else if (type === "github" || type === "all") {
+                results = render_multiple(query, data, type);
             } else {
-                return `<div id="results-plugin">`
-                    + data.map((item) => `<p>${item.entry}</p>`).join("\n")
-                    + `</div>`;
+                results = data.map((item) => `<div class="results-plugin">` + `<p>${item.entry}</p>` + `</div>`).join("\n")
             }
+
+            // Any POST rendering goes here.
+
+            let renderedResults = document.createElement("div");
+            renderedResults.id = `results-${type}`;
+            renderedResults.innerHTML = results;
+
+            // For all elements that are of type img in the results html and have a src with 'avatar' in the URL, add the class 'avatar'
+            // This is used to make the avatar images round
+            let images = renderedResults.querySelectorAll("img[src*='avatar']");
+            for (let i = 0; i < images.length; i++) {
+                images[i].classList.add("avatar");
+            }
+
+            return renderedResults.outerHTML;
         }
 
         function search(rerank=false) {
             // Extract required fields for search from form
             query = document.getElementById("query").value.trim();
             type = document.getElementById("type").value;
             results_count = document.getElementById("results-count").value || 6;
@@ -90,39 +129,32 @@
             if (query.length === 0)
                 return;
 
             // If set query field in url query param on rerank
             if (rerank)
                 setQueryFieldInUrl(query);
 
-            // Generate Backend API URL to execute Search
-            url = type === "image"
-                ? `/api/search?q=${encodeURIComponent(query)}&t=${type}&n=${results_count}&client=web`
-                : `/api/search?q=${encodeURIComponent(query)}&t=${type}&n=${results_count}&r=${rerank}&client=web`;
-
             // Execute Search and Render Results
+            url = createRequestUrl(query, type, results_count, rerank);
             fetch(url)
                 .then(response => response.json())
                 .then(data => {
                     console.log(data);
-                    document.getElementById("results").innerHTML =
-                        `<div id=results-${type}>`
-                        + render_json(data, query, type)
-                        + `</div>`;
+                    document.getElementById("results").innerHTML = render_results(data, query, type);
                 });
         }
 
         function updateIndex() {
             type = document.getElementById("type").value;
             fetch(`/api/update?t=${type}&client=web`)
                 .then(response => response.json())
                 .then(data => {
                     console.log(data);
                     document.getElementById("results").innerHTML =
-                        render_json(data);
+                        render_results(data);
                 });
         }
 
         function incrementalSearch(event) {
             type = document.getElementById("type").value;
             // Search with reranking on 'Enter'
             if (event.key === 'Enter') {
@@ -150,14 +182,26 @@
                     // Set type field to content type passed in URL query parameter, if valid
                     var type_via_url = new URLSearchParams(window.location.search).get("t");
                     if (type_via_url && enabled_types.includes(type_via_url))
                         document.getElementById("type").value = type_via_url;
                 });
         }
 
+        function createRequestUrl(query, type, results_count, rerank) {
+            // Generate Backend API URL to execute Search
+            let url = `/api/search?q=${encodeURIComponent(query)}&n=${results_count}&client=web`;
+            // If type is not 'all', append type to URL
+            if (type !== 'all')
+                url += `&t=${type}`;
+            // Rerank is only supported by text types
+            if (type !== "image")
+                url += `&r=${rerank}`;
+            return url;
+        }
+
         function setTypeFieldInUrl(type) {
             var url = new URL(window.location.href);
             url.searchParams.set("t", type.value);
             window.history.pushState({}, "", url.href);
         }
 
         function setCountFieldInUrl(results_count) {
@@ -187,19 +231,39 @@
                 document.getElementById("query").value = query_via_url;
         }
     </script>
 
     <body>
         <!--Add Header Logo and Nav Pane-->
         <div class="khoj-header">
-            <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+            {% if demo %}
+                <!-- Banner linking to https://khoj.dev -->
+                <div class="khoj-banner-container">
+                    <a class="khoj-banner" href="https://khoj.dev" target="_blank">
+                        <p id="khoj-banner" class="khoj-banner">
+                            Enroll in Khoj cloud to get your own Github assistant
+                        </p>
+                    </a>
+                    <input type="text" id="khoj-banner-email" placeholder="email" class="khoj-banner-email"></input>
+                    <button id="khoj-banner-submit" class="khoj-banner-button">Submit</button>
+                </div>
+                <a class="khoj-logo" href="https://khoj.dev" target="_blank">
+                    <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+                </a>
+            {% else %}
+                <a class="khoj-logo" href="https://lantern.khoj.dev" target="_blank">
+                    <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+                </a>
+            {% endif %}
             <nav class="khoj-nav">
                 <a href="/chat">Chat</a>
                 <a class="khoj-nav-selected" href="/">Search</a>
-                <a href="/config">Settings</a>
+                {% if not demo %}
+                    <a href="/config">Settings</a>
+                {% endif %}
             </nav>
         </div>
 
         <!--Add Text Box To Enter Query, Trigger Incremental Search OnChange -->
         <input type="text" id="query" class="option" onkeyup=incrementalSearch(event) autofocus="autofocus" placeholder="What is the meaning of life?">
 
         <div id="options">
@@ -240,15 +304,14 @@
             }
         }
         body {
             padding: 0px;
             margin: 0px;
             background: #f8fafc;
             color: #475569;
-            text-align: center;
             font-family: roboto, karma, segoe ui, sans-serif;
             font-size: 20px;
             font-weight: 300;
             line-height: 1.5em;
         }
         body > * {
             padding: 10px;
@@ -279,76 +342,189 @@
             font-size: larger;
         }
         #results {
             font-size: medium;
             margin: 0px;
             line-height: 20px;
         }
-        #results-image {
+        .results-image {
             display: grid;
             grid-template-columns: repeat(3, 1fr);
         }
         .image-link {
             place-self: center;
         }
         .image {
             width: 20vw;
             border-radius: 10px;
             border: 1px solid #475569;
         }
         #json {
             white-space: pre-wrap;
         }
-        #results-pdf,
-        #results-plugin,
-        #results-ledger {
+        .results-pdf,
+        .results-plugin,
+        .results-ledger {
             text-align: left;
             white-space: pre-line;
         }
-        #results-markdown, #results-github {
+        .results-markdown,
+        .results-github {
             text-align: left;
         }
-        #results-music,
-        #results-org {
+        .results-music,
+        .results-org {
             text-align: left;
             white-space: pre-line;
         }
-        #results-music h3,
-        #results-org h3 {
+        .results-music h3,
+        .results-org h3 {
             margin: 20px 0 0 0;
             font-size: larger;
         }
         span.music-task-status,
-        span.task-status {
+        span.org-task-status {
             color: white;
             padding: 3.5px 3.5px 0;
             margin-right: 5px;
             border-radius: 5px;
             background-color: #eab308;
             font-size: medium;
         }
         span.music-task-status.todo,
-        span.task-status.todo {
+        span.org-task-status.todo {
             background-color: #3b82f6
         }
         span.music-task-status.done,
-        span.task-status.done {
+        span.org-task-status.done {
             background-color: #22c55e;
         }
         span.music-task-tag,
-        span.task-tag {
+        span.org-task-tag {
             color: white;
             padding: 3.5px 3.5px 0;
             margin-right: 5px;
             border-radius: 5px;
             border: 1px solid #475569;
             background-color: #ef4444;
             font-size: small;
         }
 
         pre {
             max-width: 100;
         }
 
+        a {
+            color: #3b82f6;
+            text-decoration: none;
+        }
+
+        img.avatar {
+            width: 20px;
+            height: 20px;
+            border-radius: 50%;
+        }
+
+        div.results-markdown,
+        div.results-org,
+        div.results-pdf {
+            text-align: left;
+            box-shadow: 2px 2px 2px var(--primary-hover);
+            border-radius: 5px;
+            padding: 10px;
+            margin: 10px 0;
+            border: 4px solid rgb(229, 229, 229);
+        }
+
+        img {
+            max-width: 90%;
+        }
+
+        div.khoj-banner-container {
+            background: linear-gradient(-45deg, #FFC107, #FF9800, #FF5722, #FF9800, #FFC107);
+            background-size: 400% 400%;
+            animation: gradient 15s ease infinite;
+            text-align: center;
+            padding: 10px;
+        }
+
+        @keyframes gradient {
+            0% {
+                background-position: 0% 50%;
+            }
+            50% {
+                background-position: 100% 50%;
+            }
+            100% {
+                background-position: 0% 50%;
+            }
+        }
+
+        a.khoj-banner {
+            color: black;
+        }
+
+        a.khoj-logo {
+            text-align: center;
+        }
+
+        p.khoj-banner {
+            margin: 0;
+            padding: 10px;
+        }
+
+        button#khoj-banner-submit,
+        input#khoj-banner-email {
+            padding: 10px;
+            border-radius: 5px;
+            border: 1px solid #475569;
+            background: #f9fafc;
+        }
+
+        button#khoj-banner-submit:hover,
+        input#khoj-banner-email:hover {
+            box-shadow: 0 0 11px #aaa;
+        }
+
+        p#khoj-banner {
+            display: inline;
+        }
+
+        @media only screen and (max-width: 600px) {
+            a.khoj-banner {
+                display: block;
+            }
+        }
+
     </style>
+    <script>
+        var khojBannerSubmit = document.getElementById("khoj-banner-submit");
+
+        khojBannerSubmit.addEventListener("click", function(event) {
+            event.preventDefault();
+            var email = document.getElementById("khoj-banner-email").value;
+            fetch("https://lantern.khoj.dev/beta/users/", {
+                    method: "POST",
+                    body: JSON.stringify({
+                        email: email
+                    }),
+                    headers: {
+                        "Content-Type": "application/json"
+                    }
+                }).then(function(response) {
+                    return response.json();
+                }).then(function(data) {
+                    console.log(data);
+                    if (data.user != null) {
+                        document.getElementById("khoj-banner").innerHTML = "Thanks for signing up. We'll be in touch soon! 🚀";
+                        document.getElementById("khoj-banner-submit").remove();
+                    } else {
+                        document.getElementById("khoj-banner").innerHTML = "There was an error signing up. Please contact team@khoj.dev";
+                    }
+                }).catch(function(error) {
+                    console.log(error);
+                    document.getElementById("khoj-banner").innerHTML = "There was an error signing up. Please contact team@khoj.dev";
+                });
+            });
+    </script>
 
 </html>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,6 +1,10 @@
 
 
 
-[Khoj]  Chat Search Settings
+{% if demo %}
+Enroll_in_Khoj_cloud_to_get_your_own_Github_assistant
+ [                    ] Submit
+[Khoj] {% else %} [Khoj] {% endif %}  Chat Search {% if not demo %} Settings {%
+endif %}
  [                    ]
   Update  [Unknown INPUT type]
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.0/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/khoj.css`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     grid-auto-flow: row;
     gap: 20px;
     padding: 16px 0;
     margin: 0 0 16px 0;
 }
 .khoj-nav {
     display: grid;
-    grid-template-columns: repeat(3, 1fr);
+    grid-auto-flow: column;
     grid-gap: 32px;
     justify-self: center;
 }
 .khoj-nav a {
     color: #333;
     text-decoration: none;
     font-size: 20px;
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/org.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -611,16 +611,18 @@
                 var blankToken = this.skipBlank();
                 if (!this.lexer.hasNext())
                     break;
 
                 var notBlankNextToken = this.lexer.peekNextToken();
                 if (blankToken && !notBlankNextToken.isListElement())
                     this.lexer.pushToken(blankToken); // Recover blank token only when next line is not listElement.
-                if (notBlankNextToken.indentation <= rootIndentation)
-                    break; // end of the list
+                // End of the list if hit less indented line or end of directive
+                if (notBlankNextToken.indentation <= rootIndentation ||
+                    (notBlankNextToken.type === Lexer.tokens.directive && notBlankNextToken.endDirective))
+                    break;
 
                 var element = this.parseElement(); // recursive
                 if (element)
                     listElement.appendChild(element);
             }
 
             return listElement;
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.0/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.0/src/khoj/processor/conversation/gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             # Clean response to increase likelihood of valid JSON. E.g replace ' with " to enclose strings
             response.strip(empty_escape_sequences)
             .replace("['", '["')
             .replace("']", '"]')
             .replace("', '", '", "')
         )
     except json.decoder.JSONDecodeError:
-        logger.warn(f"GPT returned invalid JSON. Falling back to using user message as search query.\n{response}")
+        logger.warning(f"GPT returned invalid JSON. Falling back to using user message as search query.\n{response}")
         questions = [text]
     logger.debug(f"Extracted Questions by GPT: {questions}")
     return questions
 
 
 def extract_search_type(text, model, api_key=None, temperature=0.5, max_tokens=100, verbose=0):
     """
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.0/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.0/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.0/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,166 +1,174 @@
 # Standard Packages
+import glob
 import logging
-import time
-from typing import Dict, List
-
-# External Packages
-import requests
+import re
+from pathlib import Path
+from typing import List
 
 # Internal Packages
-from khoj.utils.helpers import timer
-from khoj.utils.rawconfig import Entry, GithubContentConfig
-from khoj.processor.markdown.markdown_to_jsonl import MarkdownToJsonl
 from khoj.processor.text_to_jsonl import TextToJsonl
+from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
+from khoj.utils.constants import empty_escape_sequences
 from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
+from khoj.utils.rawconfig import Entry, TextContentConfig
 
 
 logger = logging.getLogger(__name__)
 
 
-class GithubToJsonl(TextToJsonl):
-    def __init__(self, config: GithubContentConfig):
+class MarkdownToJsonl(TextToJsonl):
+    def __init__(self, config: TextContentConfig):
         super().__init__(config)
         self.config = config
-        self.repo_url = f"https://api.github.com/repos/{self.config.repo_owner}/{self.config.repo_name}"
-
-    @staticmethod
-    def wait_for_rate_limit_reset(response, func, *args, **kwargs):
-        if response.status_code != 200 and response.headers.get("X-RateLimit-Remaining") == "0":
-            wait_time = int(response.headers.get("X-RateLimit-Reset")) - int(time.time())
-            logger.info(f"Github Rate limit reached. Waiting for {wait_time} seconds")
-            time.sleep(wait_time)
-            return func(*args, **kwargs)
-        else:
-            return
 
+    # Define Functions
     def process(self, previous_entries=None):
-        with timer("Download markdown files from github repo", logger):
-            try:
-                docs = self.get_markdown_files()
-            except Exception as e:
-                logger.error(f"Unable to download github repo {self.config.repo_owner}/{self.config.repo_name}")
-                raise e
+        # Extract required fields from config
+        markdown_files, markdown_file_filter, output_file = (
+            self.config.input_files,
+            self.config.input_filter,
+            self.config.compressed_jsonl,
+        )
+
+        # Input Validation
+        if is_none_or_empty(markdown_files) and is_none_or_empty(markdown_file_filter):
+            print("At least one of markdown-files or markdown-file-filter is required to be specified")
+            exit(1)
 
-        logger.info(f"Found {len(docs)} documents in github repo {self.config.repo_owner}/{self.config.repo_name}")
+        # Get Markdown Files to Process
+        markdown_files = MarkdownToJsonl.get_markdown_files(markdown_files, markdown_file_filter)
 
-        with timer("Extract markdown entries from github repo", logger):
+        # Extract Entries from specified Markdown files
+        with timer("Parse entries from Markdown files into dictionaries", logger):
             current_entries = MarkdownToJsonl.convert_markdown_entries_to_maps(
-                *GithubToJsonl.extract_markdown_entries(docs)
+                *MarkdownToJsonl.extract_markdown_entries(markdown_files)
             )
 
-        with timer("Extract commit messages from github repo", logger):
-            current_entries += self.convert_commits_to_entries(self.get_commits())
-
+        # Split entries by max tokens supported by model
         with timer("Split entries by max token size supported by model", logger):
-            current_entries = TextToJsonl.split_entries_by_max_tokens(current_entries, max_tokens=256)
+            current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
             if not previous_entries:
                 entries_with_ids = list(enumerate(current_entries))
             else:
                 entries_with_ids = TextToJsonl.mark_entries_for_update(
                     current_entries, previous_entries, key="compiled", logger=logger
                 )
 
-        with timer("Write github entries to JSONL file", logger):
+        with timer("Write markdown entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = MarkdownToJsonl.convert_markdown_maps_to_jsonl(entries)
 
             # Compress JSONL formatted Data
-            if self.config.compressed_jsonl.suffix == ".gz":
-                compress_jsonl_data(jsonl_data, self.config.compressed_jsonl)
-            elif self.config.compressed_jsonl.suffix == ".jsonl":
-                dump_jsonl(jsonl_data, self.config.compressed_jsonl)
+            if output_file.suffix == ".gz":
+                compress_jsonl_data(jsonl_data, output_file)
+            elif output_file.suffix == ".jsonl":
+                dump_jsonl(jsonl_data, output_file)
 
         return entries_with_ids
 
-    def get_markdown_files(self):
-        # Get the contents of the repository
-        repo_content_url = f"{self.repo_url}/git/trees/{self.config.repo_branch}"
-        headers = {"Authorization": f"token {self.config.pat_token}"}
-        params = {"recursive": "true"}
-        response = requests.get(repo_content_url, headers=headers, params=params)
-        contents = response.json()
-
-        # Wait for rate limit reset if needed
-        result = self.wait_for_rate_limit_reset(response, self.get_markdown_files)
-        if result is not None:
-            return result
-
-        # Extract markdown files from the repository
-        markdown_files = []
-        for item in contents["tree"]:
-            # Find all markdown files in the repository
-            if item["type"] == "blob" and item["path"].endswith(".md"):
-                # Create URL for each markdown file on Github
-                url_path = f'https://github.com/{self.config.repo_owner}/{self.config.repo_name}/blob/{self.config.repo_branch}/{item["path"]}'
-
-                # Add markdown file contents and URL to list
-                markdown_files += [{"content": self.get_file_contents(item["url"]), "path": url_path}]
-
-        return markdown_files
-
-    def get_file_contents(self, file_url):
-        # Get text from each markdown file
-        headers = {"Authorization": f"token {self.config.pat_token}", "Accept": "application/vnd.github.v3.raw"}
-        response = requests.get(file_url, headers=headers)
-
-        # Wait for rate limit reset if needed
-        result = self.wait_for_rate_limit_reset(response, self.get_file_contents, file_url)
-        if result is not None:
-            return result
-
-        return response.content.decode("utf-8")
-
-    def get_commits(self) -> List[Dict]:
-        # Get commit messages from the repository using the Github API
-        commits_url = f"{self.repo_url}/commits"
-        headers = {"Authorization": f"token {self.config.pat_token}"}
-        params = {"per_page": 100}
-        commits = []
-
-        while commits_url is not None:
-            # Get the next page of commits
-            response = requests.get(commits_url, headers=headers, params=params)
-            raw_commits = response.json()
-
-            # Wait for rate limit reset if needed
-            result = self.wait_for_rate_limit_reset(response, self.get_commits)
-            if result is not None:
-                return result
-
-            # Extract commit messages from the response
-            for commit in raw_commits:
-                commits += [{"content": commit["commit"]["message"], "path": commit["html_url"]}]
-
-            # Get the URL for the next page of commits, if any
-            commits_url = response.links.get("next", {}).get("url")
-
-        return commits
-
-    def convert_commits_to_entries(self, commits) -> List[Entry]:
-        entries: List[Entry] = []
-        for commit in commits:
-            compiled = f'Commit message from {self.config.repo_owner}/{self.config.repo_name}:\n{commit["content"]}'
-            entries.append(
-                Entry(
-                    compiled=compiled,
-                    raw=f'### {commit["content"]}',
-                    heading=commit["content"].split("\n")[0],
-                    file=commit["path"],
-                )
+    @staticmethod
+    def get_markdown_files(markdown_files=None, markdown_file_filters=None):
+        "Get Markdown files to process"
+        absolute_markdown_files, filtered_markdown_files = set(), set()
+        if markdown_files:
+            absolute_markdown_files = {get_absolute_path(markdown_file) for markdown_file in markdown_files}
+        if markdown_file_filters:
+            filtered_markdown_files = {
+                filtered_file
+                for markdown_file_filter in markdown_file_filters
+                for filtered_file in glob.glob(get_absolute_path(markdown_file_filter), recursive=True)
+            }
+
+        all_markdown_files = sorted(absolute_markdown_files | filtered_markdown_files)
+
+        files_with_non_markdown_extensions = {
+            md_file
+            for md_file in all_markdown_files
+            if not md_file.endswith(".md") and not md_file.endswith(".markdown")
+        }
+
+        if any(files_with_non_markdown_extensions):
+            logger.warning(
+                f"[Warning] There maybe non markdown-mode files in the input set: {files_with_non_markdown_extensions}"
             )
 
-        return entries
+        logger.debug(f"Processing files: {all_markdown_files}")
+
+        return all_markdown_files
 
     @staticmethod
     def extract_markdown_entries(markdown_files):
+        "Extract entries by heading from specified Markdown files"
+
+        # Regex to extract Markdown Entries by Heading
+
         entries = []
         entry_to_file_map = []
-        for doc in markdown_files:
-            entries, entry_to_file_map = MarkdownToJsonl.process_single_markdown_file(
-                doc["content"], doc["path"], entries, entry_to_file_map
-            )
+        for markdown_file in markdown_files:
+            with open(markdown_file, "r", encoding="utf8") as f:
+                markdown_content = f.read()
+                entries, entry_to_file_map = MarkdownToJsonl.process_single_markdown_file(
+                    markdown_content, markdown_file, entries, entry_to_file_map
+                )
+
         return entries, dict(entry_to_file_map)
+
+    @staticmethod
+    def process_single_markdown_file(
+        markdown_content: str, markdown_file: Path, entries: List, entry_to_file_map: List
+    ):
+        markdown_heading_regex = r"^#"
+
+        markdown_entries_per_file = []
+        any_headings = re.search(markdown_heading_regex, markdown_content, flags=re.MULTILINE)
+        for entry in re.split(markdown_heading_regex, markdown_content, flags=re.MULTILINE):
+            # Add heading level as the regex split removed it from entries with headings
+            prefix = "#" if entry.startswith("#") else "# " if any_headings else ""
+            stripped_entry = entry.strip(empty_escape_sequences)
+            if stripped_entry != "":
+                markdown_entries_per_file.append(f"{prefix}{stripped_entry}")
+
+        entry_to_file_map += zip(markdown_entries_per_file, [markdown_file] * len(markdown_entries_per_file))
+        entries.extend(markdown_entries_per_file)
+        return entries, entry_to_file_map
+
+    @staticmethod
+    def convert_markdown_entries_to_maps(parsed_entries: List[str], entry_to_file_map) -> List[Entry]:
+        "Convert each Markdown entries into a dictionary"
+        entries = []
+        for parsed_entry in parsed_entries:
+            raw_filename = entry_to_file_map[parsed_entry]
+
+            # Check if raw_filename is a URL. If so, save it as is. If not, convert it to a Path.
+            if type(raw_filename) == str and re.search(r"^https?://", raw_filename):
+                entry_filename = raw_filename
+            else:
+                entry_filename = str(Path(raw_filename))
+            stem = Path(raw_filename).stem
+
+            heading = parsed_entry.splitlines()[0] if re.search("^#+\s", parsed_entry) else ""
+            # Append base filename to compiled entry for context to model
+            # Increment heading level for heading entries and make filename as its top level heading
+            prefix = f"# {stem}\n#" if heading else f"# {stem}\n"
+            compiled_entry = f"{prefix}{parsed_entry}"
+            entries.append(
+                Entry(
+                    compiled=compiled_entry,
+                    raw=parsed_entry,
+                    heading=f"{prefix}{heading}",
+                    file=f"{entry_filename}",
+                )
+            )
+
+        logger.debug(f"Converted {len(parsed_entries)} markdown entries to dictionaries")
+
+        return entries
+
+    @staticmethod
+    def convert_markdown_maps_to_jsonl(entries: List[Entry]):
+        "Convert each Markdown entry to JSON and collate as JSONL"
+        return "".join([f"{entry.to_json()}\n" for entry in entries])
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.0/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.7.0/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.0/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 from typing import Iterable, List
 
 # Internal Packages
 from khoj.processor.org_mode import orgnode
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
 from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
-from khoj.utils.rawconfig import Entry
+from khoj.utils.rawconfig import Entry, TextContentConfig
 from khoj.utils import state
 
 
 logger = logging.getLogger(__name__)
 
 
 class OrgToJsonl(TextToJsonl):
+    def __init__(self, config: TextContentConfig):
+        super().__init__(config)
+        self.config = config
+
     # Define Functions
     def process(self, previous_entries: List[Entry] = None):
         # Extract required fields from config
         org_files, org_file_filter, output_file = (
             self.config.input_files,
             self.config.input_filter,
             self.config.compressed_jsonl,
@@ -80,33 +84,41 @@
                 for filtered_file in glob.glob(get_absolute_path(org_file_filter), recursive=True)
             }
 
         all_org_files = sorted(absolute_org_files | filtered_org_files)
 
         files_with_non_org_extensions = {org_file for org_file in all_org_files if not org_file.endswith(".org")}
         if any(files_with_non_org_extensions):
-            logger.warn(f"There maybe non org-mode files in the input set: {files_with_non_org_extensions}")
+            logger.warning(f"There maybe non org-mode files in the input set: {files_with_non_org_extensions}")
 
         logger.debug(f"Processing files: {all_org_files}")
 
         return all_org_files
 
     @staticmethod
     def extract_org_entries(org_files):
         "Extract entries from specified Org files"
         entries = []
         entry_to_file_map = []
         for org_file in org_files:
-            org_file_entries = orgnode.makelist(str(org_file))
+            org_file_entries = orgnode.makelist_with_filepath(str(org_file))
             entry_to_file_map += zip(org_file_entries, [org_file] * len(org_file_entries))
             entries.extend(org_file_entries)
 
         return entries, dict(entry_to_file_map)
 
     @staticmethod
+    def process_single_org_file(org_content: str, org_file: str, entries: List, entry_to_file_map: List):
+        # Process single org file. The org parser assumes that the file is a single org file and reads it from a buffer. We'll split the raw conetnt of this file by new line to mimic the same behavior.
+        org_file_entries = orgnode.makelist(org_content.split("\n"), org_file)
+        entry_to_file_map += zip(org_file_entries, [org_file] * len(org_file_entries))
+        entries.extend(org_file_entries)
+        return entries, entry_to_file_map
+
+    @staticmethod
     def convert_org_nodes_to_entries(
         parsed_entries: List[orgnode.Orgnode], entry_to_file_map, index_heading_entries=False
     ) -> List[Entry]:
         "Convert Org-Mode nodes into list of Entry objects"
         entries: List[Entry] = []
         for parsed_entry in parsed_entries:
             if not parsed_entry.hasBody and not index_heading_entries:
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.0/src/khoj/processor/org_mode/orgnode.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,22 +49,27 @@
         normalized_filename = f"~/{relpath(filename, start=Path.home())}"
     else:
         normalized_filename = filename
     escaped_filename = f"{normalized_filename}".replace("[", "\[").replace("]", "\]")
     return escaped_filename
 
 
-def makelist(filename):
+def makelist_with_filepath(filename):
+    f = open(filename, "r")
+    return makelist(f, filename)
+
+
+def makelist(file, filename):
     """
     Read an org-mode file and return a list of Orgnode objects
     created from this file.
     """
     ctr = 0
 
-    f = open(filename, "r")
+    f = file
 
     todos = {
         "TODO": "",
         "WAITING": "",
         "ACTIVE": "",
         "DONE": "",
         "CANCELLED": "",
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.0/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,17 @@
             }
 
         all_pdf_files = sorted(absolute_pdf_files | filtered_pdf_files)
 
         files_with_non_pdf_extensions = {pdf_file for pdf_file in all_pdf_files if not pdf_file.endswith(".pdf")}
 
         if any(files_with_non_pdf_extensions):
-            logger.warn(f"[Warning] There maybe non pdf-mode files in the input set: {files_with_non_pdf_extensions}")
+            logger.warning(
+                f"[Warning] There maybe non pdf-mode files in the input set: {files_with_non_pdf_extensions}"
+            )
 
         logger.debug(f"Processing files: {all_pdf_files}")
 
         return all_pdf_files
 
     @staticmethod
     def extract_pdf_entries(pdf_files):
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/routers/api_beta.py` & `khoj_assistant-0.7.0/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.0/src/khoj/routers/web_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,99 +17,98 @@
 templates = Jinja2Templates(directory=constants.web_directory)
 
 VALID_CONTENT_TYPES = ["org", "ledger", "markdown", "pdf"]
 
 
 # Create Routes
 @web_client.get("/", response_class=FileResponse)
-def index():
-    return FileResponse(constants.web_directory / "index.html")
+def index(request: Request):
+    return templates.TemplateResponse("index.html", context={"request": request, "demo": state.demo})
 
 
-@web_client.get("/config", response_class=HTMLResponse)
-def config_page(request: Request):
-    return templates.TemplateResponse("config.html", context={"request": request})
-
-
-@web_client.get("/config/content_type/github", response_class=HTMLResponse)
-def github_config_page(request: Request):
-    default_copy = constants.default_config.copy()
-    default_github = default_copy["content-type"]["github"]  # type: ignore
-
-    default_config = TextContentConfig(
-        compressed_jsonl=default_github["compressed-jsonl"],
-        embeddings_file=default_github["embeddings-file"],
-    )
-
-    current_config = (
-        state.config.content_type.github
-        if state.config and state.config.content_type and state.config.content_type.github
-        else default_config
-    )
-
-    current_config = json.loads(current_config.json())
+@web_client.get("/chat", response_class=FileResponse)
+def chat_page(request: Request):
+    return templates.TemplateResponse("chat.html", context={"request": request, "demo": state.demo})
 
-    return templates.TemplateResponse(
-        "content_type_github_input.html", context={"request": request, "current_config": current_config}
-    )
 
+if not state.demo:
 
-@web_client.get("/config/content_type/{content_type}", response_class=HTMLResponse)
-def content_config_page(request: Request, content_type: str):
-    if content_type not in VALID_CONTENT_TYPES:
+    @web_client.get("/config", response_class=HTMLResponse)
+    def config_page(request: Request):
         return templates.TemplateResponse("config.html", context={"request": request})
 
-    default_copy = constants.default_config.copy()
-    default_content_type = default_copy["content-type"][content_type]  # type: ignore
-
-    default_config = TextContentConfig(
-        compressed_jsonl=default_content_type["compressed-jsonl"],
-        embeddings_file=default_content_type["embeddings-file"],
-    )
-
-    current_config = (
-        state.config.content_type[content_type]
-        if state.config and state.config.content_type and state.config.content_type[content_type]  # type: ignore
-        else default_config
-    )
-    current_config = json.loads(current_config.json())
-
-    return templates.TemplateResponse(
-        "content_type_input.html",
-        context={
-            "request": request,
-            "current_config": current_config,
-            "content_type": content_type,
-        },
-    )
-
-
-@web_client.get("/config/processor/conversation", response_class=HTMLResponse)
-def conversation_processor_config_page(request: Request):
-    default_copy = constants.default_config.copy()
-    default_processor_config = default_copy["processor"]["conversation"]  # type: ignore
-    default_processor_config = ConversationProcessorConfig(
-        openai_api_key="",
-        model=default_processor_config["model"],
-        conversation_logfile=default_processor_config["conversation-logfile"],
-        chat_model=default_processor_config["chat-model"],
-    )
-
-    current_processor_conversation_config = (
-        state.config.processor.conversation
-        if state.config and state.config.processor and state.config.processor.conversation
-        else default_processor_config
-    )
-    current_processor_conversation_config = json.loads(current_processor_conversation_config.json())
-
-    return templates.TemplateResponse(
-        "processor_conversation_input.html",
-        context={
-            "request": request,
-            "current_config": current_processor_conversation_config,
-        },
-    )
-
-
-@web_client.get("/chat", response_class=FileResponse)
-def chat_page():
-    return FileResponse(constants.web_directory / "chat.html")
+    @web_client.get("/config/content_type/github", response_class=HTMLResponse)
+    def github_config_page(request: Request):
+        default_copy = constants.default_config.copy()
+        default_github = default_copy["content-type"]["github"]  # type: ignore
+
+        default_config = TextContentConfig(
+            compressed_jsonl=default_github["compressed-jsonl"],
+            embeddings_file=default_github["embeddings-file"],
+        )
+
+        current_config = (
+            state.config.content_type.github
+            if state.config and state.config.content_type and state.config.content_type.github
+            else default_config
+        )
+
+        current_config = json.loads(current_config.json())
+
+        return templates.TemplateResponse(
+            "content_type_github_input.html", context={"request": request, "current_config": current_config}
+        )
+
+    @web_client.get("/config/content_type/{content_type}", response_class=HTMLResponse)
+    def content_config_page(request: Request, content_type: str):
+        if content_type not in VALID_CONTENT_TYPES:
+            return templates.TemplateResponse("config.html", context={"request": request})
+
+        default_copy = constants.default_config.copy()
+        default_content_type = default_copy["content-type"][content_type]  # type: ignore
+
+        default_config = TextContentConfig(
+            compressed_jsonl=default_content_type["compressed-jsonl"],
+            embeddings_file=default_content_type["embeddings-file"],
+        )
+
+        current_config = (
+            state.config.content_type[content_type]
+            if state.config and state.config.content_type and state.config.content_type[content_type]  # type: ignore
+            else default_config
+        )
+        current_config = json.loads(current_config.json())
+
+        return templates.TemplateResponse(
+            "content_type_input.html",
+            context={
+                "request": request,
+                "current_config": current_config,
+                "content_type": content_type,
+            },
+        )
+
+    @web_client.get("/config/processor/conversation", response_class=HTMLResponse)
+    def conversation_processor_config_page(request: Request):
+        default_copy = constants.default_config.copy()
+        default_processor_config = default_copy["processor"]["conversation"]  # type: ignore
+        default_processor_config = ConversationProcessorConfig(
+            openai_api_key="",
+            model=default_processor_config["model"],
+            conversation_logfile=default_processor_config["conversation-logfile"],
+            chat_model=default_processor_config["chat-model"],
+        )
+
+        current_processor_conversation_config = (
+            state.config.processor.conversation
+            if state.config and state.config.processor and state.config.processor.conversation
+            else default_processor_config
+        )
+        current_processor_conversation_config = json.loads(current_processor_conversation_config.json())
+
+        return templates.TemplateResponse(
+            "processor_conversation_input.html",
+            context={
+                "request": request,
+                "current_config": current_processor_conversation_config,
+            },
+        )
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.0/src/khoj/search_filter/date_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,27 +45,31 @@
                         continue
                     self.date_to_entry_ids[date_in_entry].add(id)
 
     def can_filter(self, raw_query):
         "Check if query contains date filters"
         return self.extract_date_range(raw_query) is not None
 
+    def defilter(self, query):
+        # remove date range filter from query
+        query = re.sub(rf"\s+{self.date_regex}", " ", query)
+        query = re.sub(r"\s{2,}", " ", query).strip()  # remove multiple spaces
+        return query
+
     def apply(self, query, entries):
         "Find entries containing any dates that fall within date range specified in query"
         # extract date range specified in date filter of query
         with timer("Extract date range to filter from query", logger):
             query_daterange = self.extract_date_range(query)
 
         # if no date in query, return all entries
         if query_daterange is None:
             return query, set(range(len(entries)))
 
-        # remove date range filter from query
-        query = re.sub(rf"\s+{self.date_regex}", " ", query)
-        query = re.sub(r"\s{2,}", " ", query).strip()  # remove multiple spaces
+        query = self.defilter(query)
 
         # return results from cache if exists
         cache_key = tuple(query_daterange)
         if cache_key in self.cache:
             logger.debug(f"Return date filter results from cache")
             entries_to_include = self.cache[cache_key]
             return query, entries_to_include
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.0/src/khoj/search_filter/file_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         with timer("Created file filter index", logger):
             for id, entry in enumerate(entries):
                 self.file_to_entry_map[getattr(entry, self.entry_key)].add(id)
 
     def can_filter(self, raw_query):
         return re.search(self.file_filter_regex, raw_query) is not None
 
+    def defilter(self, query: str) -> str:
+        return re.sub(self.file_filter_regex, "", query).strip()
+
     def apply(self, query, entries):
         # Extract file filters from raw query
         with timer("Extract files_to_search from query", logger):
             raw_files_to_search = re.findall(self.file_filter_regex, query)
             if not raw_files_to_search:
                 return query, set(range(len(entries)))
 
@@ -40,16 +43,18 @@
             files_to_search = []
             for file in sorted(raw_files_to_search):
                 if "/" not in file and "\\" not in file and "*" not in file:
                     files_to_search += [f"*{file}"]
                 else:
                     files_to_search += [file]
 
+        # Remove filter terms from original query
+        query = self.defilter(query)
+
         # Return item from cache if exists
-        query = re.sub(self.file_filter_regex, "", query).strip()
         cache_key = tuple(files_to_search)
         if cache_key in self.cache:
             logger.debug(f"Return file filter results from cache")
             included_entry_indices = self.cache[cache_key]
             return query, included_entry_indices
 
         if not self.file_to_entry_map:
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.0/src/khoj/search_filter/word_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,24 @@
     def can_filter(self, raw_query):
         "Check if query contains word filters"
         required_words = re.findall(self.required_regex, raw_query)
         blocked_words = re.findall(self.blocked_regex, raw_query)
 
         return len(required_words) != 0 or len(blocked_words) != 0
 
+    def defilter(self, query: str) -> str:
+        return re.sub(self.blocked_regex, "", re.sub(self.required_regex, "", query)).strip()
+
     def apply(self, query, entries):
         "Find entries containing required and not blocked words specified in query"
         # Separate natural query from required, blocked words filters
         with timer("Extract required, blocked filters from query", logger):
             required_words = set([word.lower() for word in re.findall(self.required_regex, query)])
             blocked_words = set([word.lower() for word in re.findall(self.blocked_regex, query)])
-            query = re.sub(self.blocked_regex, "", re.sub(self.required_regex, "", query)).strip()
+            query = self.defilter(query)
 
         if len(required_words) == 0 and len(blocked_words) == 0:
             return query, set(range(len(entries)))
 
         # Return item from cache if exists
         cache_key = tuple(sorted(required_words)), tuple(sorted(blocked_words))
         if cache_key in self.cache:
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.0/src/khoj/search_type/image_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         image_processed_metadata += ". " + ", ".join(image_metadata_subjects)
 
     logger.debug(f"{image_name}:\t{image_processed_metadata}")
 
     return image_processed_metadata
 
 
-def query(raw_query, count, model: ImageSearchModel, score_threshold: float = -math.inf):
+async def query(raw_query, count, model: ImageSearchModel, score_threshold: float = -math.inf):
     # Set query to image content if query is of form file:/path/to/file.png
     if raw_query.startswith("file:") and pathlib.Path(raw_query[5:]).is_file():
         query_imagepath = resolve_absolute_path(pathlib.Path(raw_query[5:]), strict=True)
         query = copy.deepcopy(Image.open(query_imagepath))
         query.thumbnail((640, query.height))  # scale down image for faster processing
         logger.info(f"🔎 Find Images by Image: {query_imagepath}")
     else:
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.0/src/khoj/search_type/text_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Standard Packages
 import logging
 import math
 from pathlib import Path
-from typing import List, Tuple, Type
+from typing import List, Tuple, Type, Union
 
 # External Packages
 import torch
 from sentence_transformers import SentenceTransformer, CrossEncoder, util
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.search_filter.base_filter import BaseFilter
 
@@ -98,17 +98,18 @@
         corpus_embeddings = util.normalize_embeddings(corpus_embeddings)
         torch.save(corpus_embeddings, embeddings_file)
         logger.info(f"📩 Saved computed text embeddings to {embeddings_file}")
 
     return corpus_embeddings
 
 
-def query(
+async def query(
     raw_query: str,
     model: TextSearchModel,
+    question_embedding: Union[torch.Tensor, None] = None,
     rank_results: bool = False,
     score_threshold: float = -math.inf,
     dedupe: bool = True,
 ) -> Tuple[List[dict], List[Entry]]:
     "Search for entries that answer the query"
     query, entries, corpus_embeddings = raw_query, model.entries, model.corpus_embeddings
 
@@ -120,17 +121,18 @@
         return [], []
     # If query only had filters it'll be empty now. So short-circuit and return results.
     if query.strip() == "":
         hits = [{"corpus_id": id, "score": 1.0} for id, _ in enumerate(entries)]
         return hits, entries
 
     # Encode the query using the bi-encoder
-    with timer("Query Encode Time", logger, state.device):
-        question_embedding = model.bi_encoder.encode([query], convert_to_tensor=True, device=state.device)
-        question_embedding = util.normalize_embeddings(question_embedding)
+    if question_embedding is None:
+        with timer("Query Encode Time", logger, state.device):
+            question_embedding = model.bi_encoder.encode([query], convert_to_tensor=True, device=state.device)
+            question_embedding = util.normalize_embeddings(question_embedding)
 
     # Find relevant entries for the query
     with timer("Search Time", logger, state.device):
         hits = util.semantic_search(
             question_embedding, corpus_embeddings, top_k=model.top_k, score_function=util.dot_score
         )[0]
 
@@ -175,15 +177,15 @@
     bi_encoder, cross_encoder, top_k = initialize_model(search_config)
 
     # Map notes in text files to (compressed) JSONL formatted file
     config.compressed_jsonl = resolve_absolute_path(config.compressed_jsonl)
     previous_entries = (
         extract_entries(config.compressed_jsonl) if config.compressed_jsonl.exists() and not regenerate else None
     )
-    entries_with_indices = text_to_jsonl(config).process(previous_entries)
+    entries_with_indices = text_to_jsonl(config).process(previous_entries or [])
 
     # Extract Updated Entries
     entries = extract_entries(config.compressed_jsonl)
     if is_none_or_empty(entries):
         raise ValueError(f"No valid entries found in specified files: {config.input_files} or {config.input_filter}")
     top_k = min(len(entries), top_k)  # top_k hits can't be more than the total entries in corpus
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/cli.py` & `khoj_assistant-0.7.0/src/khoj/utils/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     parser.add_argument("--port", "-p", type=int, default=8000, help="Port of the server. Default: 8000")
     parser.add_argument(
         "--socket",
         type=pathlib.Path,
         help="Path to UNIX socket for server. Use to run server behind reverse proxy. Default: /tmp/uvicorn.sock",
     )
     parser.add_argument("--version", "-V", action="store_true", help="Print the installed Khoj version and exit")
+    parser.add_argument("--demo", action="store_true", default=False, help="Run Khoj in demo mode")
 
     args = parser.parse_args(args)
 
     if args.version:
         # Show version of khoj installed and exit
         print(version("khoj-assistant"))
         exit(0)
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/config.py` & `khoj_assistant-0.7.0/src/khoj/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     from sentence_transformers import CrossEncoder
     from khoj.search_filter.base_filter import BaseFilter
     from khoj.utils.models import BaseEncoder
     from khoj.utils.rawconfig import ConversationProcessorConfig, Entry
 
 
 class SearchType(str, Enum):
+    All = "all"
     Org = "org"
     Ledger = "ledger"
     Music = "music"
     Markdown = "markdown"
     Image = "image"
     Pdf = "pdf"
     Github = "github"
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/constants.py` & `khoj_assistant-0.7.0/src/khoj/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,15 @@
             "input-files": None,
             "input-filter": None,
             "compressed-jsonl": "~/.khoj/content/music/music.jsonl.gz",
             "embeddings-file": "~/.khoj/content/music/music_embeddings.pt",
         },
         "github": {
             "pat-token": None,
-            "repo-name": None,
-            "repo-owner": None,
-            "repo-branch": "master",
+            "repos": [],
             "compressed-jsonl": "~/.khoj/content/github/github.jsonl.gz",
             "embeddings-file": "~/.khoj/content/github/github_embeddings.pt",
         },
     },
     "search-type": {
         "symmetric": {
             "encoder": "sentence-transformers/all-MiniLM-L6-v2",
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.0/src/khoj/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,28 +170,31 @@
         # Write the server_id to the env file
         with open(app_env_filename, "w") as f:
             f.write("server_id=" + server_id + "\n")
 
     return server_id
 
 
-def log_telemetry(telemetry_type: str, api: str = None, client: str = None, app_config: AppConfig = None):
+def log_telemetry(
+    telemetry_type: str, api: str = None, client: str = None, app_config: AppConfig = None, properties: dict = None
+):
     """Log basic app usage telemetry like client, os, api called"""
     # Do not log usage telemetry, if telemetry is disabled via app config
     if not app_config or not app_config.should_log_telemetry:
         return []
 
     # Populate telemetry data to log
     request_body = {
         "telemetry_type": telemetry_type,
         "server_id": get_server_id(),
         "server_version": version("khoj-assistant"),
         "os": platform.system(),
         "timestamp": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
     }
+    request_body.update(properties or {})
     if api:
         # API endpoint on server called by client
         request_body["api"] = api
     if client:
         # Client from which the API was called. E.g Emacs, Obsidian
         request_body["client"] = client
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.0/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/models.py` & `khoj_assistant-0.7.0/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.0/src/khoj/utils/rawconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,19 +37,23 @@
         if is_none_or_empty(input_filter) and ("input_files" not in values or values["input_files"] is None):
             raise ValueError(
                 "Either input_filter or input_files required in all content-type.<text_search> section of Khoj config file"
             )
         return input_filter
 
 
+class GithubRepoConfig(ConfigBase):
+    name: str
+    owner: str
+    branch: Optional[str] = "master"
+
+
 class GithubContentConfig(TextConfigBase):
     pat_token: str
-    repo_name: str
-    repo_owner: str
-    repo_branch: Optional[str] = "master"
+    repos: List[GithubRepoConfig]
 
 
 class ImageContentConfig(ConfigBase):
     input_directories: Optional[List[Path]]
     input_filter: Optional[List[str]]
     embeddings_file: Path
     use_xmp_metadata: bool
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/state.py` & `khoj_assistant-0.7.0/src/khoj/utils/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 port: int = None
 cli_args: List[str] = None
 query_cache = LRU()
 search_index_lock = threading.Lock()
 SearchType = utils_config.SearchType
 telemetry: List[Dict[str, str]] = []
 previous_query: str = None
+demo: bool = False
 
 if torch.cuda.is_available():
     # Use CUDA GPU
     device = torch.device("cuda:0")
 elif version.parse(torch.__version__) >= version.parse("1.13.0.dev") and torch.backends.mps.is_available():
     # Use Apple M1 Metal Acceleration
     device = torch.device("mps")
```

### Comparing `khoj_assistant-0.6.3.dev98/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.0/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/.gitignore` & `khoj_assistant-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/LICENSE` & `khoj_assistant-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev98/README.md` & `khoj_assistant-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 ## Architecture
 
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_architecture.png?)
 
 ## Setup
 These are the general setup instructions for Khoj.
 
-- Make sure [python](https://realpython.com/installing-python/) (version 3.10 or lower) and [pip](https://pip.pypa.io/en/stable/installation/) are installed on your machine
+- Make sure [python](https://realpython.com/installing-python/) and [pip](https://pip.pypa.io/en/stable/installation/) are installed on your machine
 - Check the [Khoj.el Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#Setup) to setup Khoj with Emacs<br />
   Its simpler as it can skip the server *install*, *run* and *configure* step below.
 - Check the [Khoj Obsidian Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#Setup) to setup Khoj with Obsidian<br />
   Its simpler as it can skip the *configure* step below.
 
 ### 1. Install
 - On Linux/MacOS
@@ -325,19 +325,24 @@
 ### GPT API
 - The [chat](http://localhost:8000/api/chat), [answer](http://localhost:8000/api/beta/answer) and [search](http://localhost:8000/api/beta/search) API endpoints use [OpenAI API](https://openai.com/api/)
 - They are disabled by default
 - To use them:
   1. [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
   2. Interact with them from the [Khoj Swagger docs](http://locahost:8000/docs)[^2]
 
-### Use a Github Repository as a source
-Note that this plugin is currently *only* indexing Markdown files. It will ignore all other files in the repository. This is because Khoj, as it stands, is a semantic search engine. Eventually, we hope to get to a state where you can search for any file in your repository and even explain code.
+### Index Github Repository for Search, Chat
+The Khoj Github plugin can index issues, commit messages and markdown, org-mode and PDF files from any repositories you have access to. This allows you to chat or search with these repositories. Get answers, resolve issues or just explore a repo with the help of your AI personal assistant.
 
+See the [Khoj FAQ](https://faq.khoj.dev) for a demo of Khoj search and chat. It makes the Khoj github repo available for exploring.
+
+Note: *Khoj will ignore code files in the repository for now as the default AI model used works best with natural language text, not code.*
+
+#### Setup Khoj Github plugin
 1. Get a [pat token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token) with `repo` and `read:org` scopes in the classic flow.
-2. Configure your settings to include the `owner` and `repo_name`. The `owner` will be the organization name if the repo is in an organization. The `repo_name` will be the name of the repository. Optionally, you can also supply a branch name. If no branch name is supplied, the `master` branch will be used.
+2. Configure Khoj settings to include the `owner` and `repo_name`. The `owner` will be the organization name if the repo is in an organization. The `repo_name` will be the name of the repository. Optionally, you can also supply a branch name. If no branch name is supplied, the `master` branch will be used.
 
 ## Performance
 
 ### Query performance
 
 - Semantic search using the bi-encoder is fairly fast at \<50 ms
 - Reranking using the cross-encoder is slower at \<2s on 15 results. Tweak `top_k` to tradeoff speed for accuracy of results
```

### Comparing `khoj_assistant-0.6.3.dev98/pyproject.toml` & `khoj_assistant-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "khoj-assistant"
 description = "A natural language search engine for your personal notes, transactions and images"
 readme = "README.md"
 license = "GPL-3.0-or-later"
-requires-python = ">=3.8, <3.11"
+requires-python = ">=3.8"
 authors = [
     { name = "Debanjum Singh Solanky, Saba Imran" },
 ]
 keywords = [
     "search",
     "semantic-search",
     "productivity",
@@ -27,14 +27,15 @@
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Topic :: Text Processing :: Linguistic",
 ]
 dependencies = [
     "dateparser == 1.1.1",
@@ -47,15 +48,15 @@
     "pillow == 9.3.0",
     "pydantic >= 1.9.1",
     "pyqt6 == 6.3.1",
     "pyyaml == 6.0",
     "rich >= 13.3.1",
     "schedule == 1.1.0",
     "sentence-transformers == 2.2.2",
-    "torch == 1.13.1",
+    "torch >= 2.0.1",
     "uvicorn == 0.17.6",
     "aiohttp == 3.8.4",
     "langchain >= 0.0.187",
     "pypdf >= 3.9.0",
     "requests >= 2.26.0",
     "bs4 >= 0.0.1",
 ]
@@ -69,23 +70,23 @@
 
 [project.scripts]
 khoj = "khoj.main:run"
 
 [project.optional-dependencies]
 test = [
     "pytest >= 7.1.2",
+    "freezegun >= 1.2.0",
+    "factory-boy >= 3.2.1",
+    "trio >= 0.22.0",
 ]
 dev = [
     "khoj-assistant[test]",
     "mypy >= 1.0.1",
     "black >= 23.1.0",
     "pre-commit >= 3.0.4",
-    "freezegun >= 1.2.0",
-    "factory-boy==3.2.1",
-    "Faker==18.10.1",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 raw-options.local_scheme = "no-local-version"  # PEP440 compliant version for PyPi
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `khoj_assistant-0.6.3.dev98/PKG-INFO` & `khoj_assistant-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev98
+Version: 0.7.0
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -13,19 +13,20 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: dateparser==1.1.1
 Requires-Dist: defusedxml==0.7.1
 Requires-Dist: fastapi==0.77.1
 Requires-Dist: jinja2==3.1.2
 Requires-Dist: langchain>=0.0.187
@@ -37,26 +38,26 @@
 Requires-Dist: pyyaml==6.0
 Requires-Dist: requests>=2.26.0
 Requires-Dist: rich>=13.3.1
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentence-transformers==2.2.2
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: tiktoken>=0.3.0
-Requires-Dist: torch==1.13.1
+Requires-Dist: torch>=2.0.1
 Requires-Dist: uvicorn==0.17.6
 Provides-Extra: dev
 Requires-Dist: black>=23.1.0; extra == 'dev'
-Requires-Dist: factory-boy==3.2.1; extra == 'dev'
-Requires-Dist: faker==18.10.1; extra == 'dev'
-Requires-Dist: freezegun>=1.2.0; extra == 'dev'
 Requires-Dist: khoj-assistant[test]; extra == 'dev'
 Requires-Dist: mypy>=1.0.1; extra == 'dev'
 Requires-Dist: pre-commit>=3.0.4; extra == 'dev'
 Provides-Extra: test
+Requires-Dist: factory-boy>=3.2.1; extra == 'test'
+Requires-Dist: freezegun>=1.2.0; extra == 'test'
 Requires-Dist: pytest>=7.1.2; extra == 'test'
+Requires-Dist: trio>=0.22.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 <h1><img src="src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg" width="330" alt="Khoj Logo"></h1>
 
 [![test](https://github.com/khoj-ai/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/khoj-ai/khoj/actions/workflows/test.yml)
 [![dockerize](https://github.com/khoj-ai/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/khoj-ai/khoj/pkgs/container/khoj)
 [![pypi](https://github.com/khoj-ai/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
@@ -166,15 +167,15 @@
 ## Architecture
 
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_architecture.png?)
 
 ## Setup
 These are the general setup instructions for Khoj.
 
-- Make sure [python](https://realpython.com/installing-python/) (version 3.10 or lower) and [pip](https://pip.pypa.io/en/stable/installation/) are installed on your machine
+- Make sure [python](https://realpython.com/installing-python/) and [pip](https://pip.pypa.io/en/stable/installation/) are installed on your machine
 - Check the [Khoj.el Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/emacs#Setup) to setup Khoj with Emacs<br />
   Its simpler as it can skip the server *install*, *run* and *configure* step below.
 - Check the [Khoj Obsidian Readme](https://github.com/khoj-ai/khoj/tree/master/src/interface/obsidian#Setup) to setup Khoj with Obsidian<br />
   Its simpler as it can skip the *configure* step below.
 
 ### 1. Install
 - On Linux/MacOS
@@ -382,19 +383,24 @@
 ### GPT API
 - The [chat](http://localhost:8000/api/chat), [answer](http://localhost:8000/api/beta/answer) and [search](http://localhost:8000/api/beta/search) API endpoints use [OpenAI API](https://openai.com/api/)
 - They are disabled by default
 - To use them:
   1. [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
   2. Interact with them from the [Khoj Swagger docs](http://locahost:8000/docs)[^2]
 
-### Use a Github Repository as a source
-Note that this plugin is currently *only* indexing Markdown files. It will ignore all other files in the repository. This is because Khoj, as it stands, is a semantic search engine. Eventually, we hope to get to a state where you can search for any file in your repository and even explain code.
+### Index Github Repository for Search, Chat
+The Khoj Github plugin can index issues, commit messages and markdown, org-mode and PDF files from any repositories you have access to. This allows you to chat or search with these repositories. Get answers, resolve issues or just explore a repo with the help of your AI personal assistant.
 
+See the [Khoj FAQ](https://faq.khoj.dev) for a demo of Khoj search and chat. It makes the Khoj github repo available for exploring.
+
+Note: *Khoj will ignore code files in the repository for now as the default AI model used works best with natural language text, not code.*
+
+#### Setup Khoj Github plugin
 1. Get a [pat token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token) with `repo` and `read:org` scopes in the classic flow.
-2. Configure your settings to include the `owner` and `repo_name`. The `owner` will be the organization name if the repo is in an organization. The `repo_name` will be the name of the repository. Optionally, you can also supply a branch name. If no branch name is supplied, the `master` branch will be used.
+2. Configure Khoj settings to include the `owner` and `repo_name`. The `owner` will be the organization name if the repo is in an organization. The `repo_name` will be the name of the repository. Optionally, you can also supply a branch name. If no branch name is supplied, the `master` branch will be used.
 
 ## Performance
 
 ### Query performance
 
 - Semantic search using the bi-encoder is fairly fast at \<50 ms
 - Reranking using the cross-encoder is slower at \<2s on 15 results. Tweak `top_k` to tradeoff speed for accuracy of results
```

