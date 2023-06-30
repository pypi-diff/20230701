# Comparing `tmp/requests_cache-1.0.1.tar.gz` & `tmp/requests_cache-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_cache-1.0.1.tar", max compression
+gzip compressed data, was "requests_cache-1.1.0.tar", max compression
```

## Comparing `requests_cache-1.0.1.tar` & `requests_cache-1.1.0.tar`

### file list

```diff
@@ -1,201 +1,201 @@
--rw-r--r--   0        0        0      272 2023-03-25 01:13:40.391311 requests_cache-1.0.1/.readthedocs.yml
--rw-r--r--   0        0        0     7501 2023-03-25 01:13:40.391311 requests_cache-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    41353 2023-03-25 01:13:40.391311 requests_cache-1.0.1/CONTRIBUTORS.md
--rw-r--r--   0        0        0    33439 2023-03-25 01:13:40.391311 requests_cache-1.0.1/HISTORY.md
--rw-r--r--   0        0        0     1357 2023-03-25 01:13:40.391311 requests_cache-1.0.1/LICENSE
--rw-r--r--   0        0        0     7054 2023-03-25 01:13:40.391311 requests_cache-1.0.1/README.md
--rw-r--r--   0        0        0      957 2023-03-25 01:13:40.391311 requests_cache-1.0.1/docker-compose.yml
--rw-r--r--   0        0        0      191 2023-03-25 01:13:40.391311 requests_cache-1.0.1/docs/404.rst
--rw-r--r--   0        0        0      176 2023-03-25 01:13:40.391311 requests_cache-1.0.1/docs/Dockerfile
--rw-r--r--   0        0        0     4389 2023-03-25 01:13:40.391311 requests_cache-1.0.1/docs/_static/dynamodb.png
--rw-r--r--   0        0        0     3754 2023-03-25 01:13:40.391311 requests_cache-1.0.1/docs/_static/dynamodb_32px.png
--rw-r--r--   0        0        0    51196 2023-03-25 01:13:40.391311 requests_cache-1.0.1/docs/_static/dynamodb_create_table.png
--rw-r--r--   0        0        0    37675 2023-03-25 01:13:40.391311 requests_cache-1.0.1/docs/_static/dynamodb_items.png
--rw-r--r--   0        0        0   102427 2023-03-25 01:13:40.391311 requests_cache-1.0.1/docs/_static/dynamodb_response.png
--rw-r--r--   0        0        0     4166 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0        0        0     3888 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-json.png
--rw-r--r--   0        0        0     3291 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-json_32px.png
--rw-r--r--   0        0        0      989 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-pickle.png
--rw-r--r--   0        0        0     2399 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-pickle_32px.png
--rw-r--r--   0        0        0     5620 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-toml.png
--rw-r--r--   0        0        0     2811 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-toml_32px.png
--rw-r--r--   0        0        0     1907 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-yaml.png
--rw-r--r--   0        0        0     2582 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-yaml_32px.png
--rw-r--r--   0        0        0     2719 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/file-yaml_32px.png.png
--rw-r--r--   0        0        0     7663 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/files-generic.png
--rw-r--r--   0        0        0     6029 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/files-generic_32px.png
--rw-r--r--   0        0        0     9754 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/files-json.png
--rw-r--r--   0        0        0     3823 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/files-json_32px.png
--rw-r--r--   0        0        0    32890 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/memcached.png
--rw-r--r--   0        0        0     3790 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/memcached_32px.png
--rw-r--r--   0        0        0     5923 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/memory_32px.png
--rw-r--r--   0        0        0     5158 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/mongodb.png
--rw-r--r--   0        0        0     2980 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/mongodb_32px.png
--rw-r--r--   0        0        0   216933 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/mongodb_vscode.png
--rw-r--r--   0        0        0     9031 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/redis.png
--rw-r--r--   0        0        0     4998 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/redis_32px.png
--rw-r--r--   0        0        0    49524 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/requests-cache-gh-preview.png
--rw-r--r--   0        0        0    30478 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/requests-cache-icon.png
--rw-r--r--   0        0        0    21674 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/requests-cache-logo-dark.webp
--rw-r--r--   0        0        0    21385 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/requests-cache-logo-header.png
--rw-r--r--   0        0        0    21144 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/requests-cache-logo-light.webp
--rw-r--r--   0        0        0     5525 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/sqlite.png
--rw-r--r--   0        0        0     3309 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/sqlite_32px.png
--rw-r--r--   0        0        0      463 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/table.css
--rw-r--r--   0        0        0     1404 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_static/toml.png
--rw-r--r--   0        0        0      291 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_templates/module.rst_t
--rw-r--r--   0        0        0      214 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/_templates/package.rst_t
--rw-r--r--   0        0        0      309 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/api/requests_cache.session.md
--rw-r--r--   0        0        0     5370 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/conf.py
--rw-r--r--   0        0        0      275 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/docker-compose.yml
--rw-r--r--   0        0        0     7288 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/examples.md
--rw-r--r--   0        0        0      897 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/index.md
--rw-r--r--   0        0        0     3317 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/project_info/code_of_conduct.md
--rw-r--r--   0        0        0      805 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/project_info/codeshelter.md
--rw-r--r--   0        0        0      142 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/project_info/contributing.md
--rw-r--r--   0        0        0       82 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/project_info/contributors.md
--rw-r--r--   0        0        0       87 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/project_info/history.md
--rw-r--r--   0        0        0     2240 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/project_info/related_projects.md
--rw-r--r--   0        0        0      198 2023-03-25 01:13:40.395311 requests_cache-1.0.1/docs/project_info.md
--rw-r--r--   0        0        0     1017 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/reference.md
--rw-r--r--   0        0        0     1312 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/sample_data/sample_response_binary.json
--rw-r--r--   0        0        0     1178 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/sample_data/sample_response_binary.yaml
--rw-r--r--   0        0        0     1397 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/sample_data/sample_response_json.json
--rw-r--r--   0        0        0      970 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/sample_data/sample_response_json.yaml
--rw-r--r--   0        0        0     1967 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/advanced_requests.md
--rw-r--r--   0        0        0     4208 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/backends/dynamodb.md
--rw-r--r--   0        0        0     2148 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/backends/filesystem.md
--rw-r--r--   0        0        0      617 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/backends/gridfs.md
--rw-r--r--   0        0        0     3609 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/backends/mongodb.md
--rw-r--r--   0        0        0     2731 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/backends/redis.md
--rw-r--r--   0        0        0     3697 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/backends/sqlite.md
--rw-r--r--   0        0        0     7088 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/backends.md
--rw-r--r--   0        0        0     7394 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/compatibility.md
--rw-r--r--   0        0        0    10951 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/expiration.md
--rw-r--r--   0        0        0     3200 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/files.md
--rw-r--r--   0        0        0     2875 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/filtering.md
--rw-r--r--   0        0        0     3820 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/general.md
--rw-r--r--   0        0        0     4026 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/headers.md
--rw-r--r--   0        0        0     3848 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/inspection.md
--rw-r--r--   0        0        0     1550 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/installation.md
--rw-r--r--   0        0        0     7727 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/matching.md
--rw-r--r--   0        0        0     3159 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/security.md
--rw-r--r--   0        0        0     7143 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/serializers.md
--rw-r--r--   0        0        0     6069 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide/troubleshooting.md
--rw-r--r--   0        0        0      508 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/user_guide.md
--rw-r--r--   0        0        0    16051 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/vector/requests-cache-logo-header.svg
--rw-r--r--   0        0        0    15895 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/vector/requests-cache-logo.svg
--rw-r--r--   0        0        0     6035 2023-03-25 01:13:40.399311 requests_cache-1.0.1/docs/vector/requests_cache_icon.svg
--rw-r--r--   0        0        0      241 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/README.md
--rwxr-xr-x   0        0        0     1188 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/basic_patching.py
--rwxr-xr-x   0        0        0      994 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/basic_sessions.py
--rwxr-xr-x   0        0        0     3345 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/benchmark.py
--rw-r--r--   0        0        0      974 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/cloudformation.yml
--rwxr-xr-x   0        0        0     1382 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/convert_cache.py
--rwxr-xr-x   0        0        0     2295 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/custom_request_matcher.py
--rwxr-xr-x   0        0        0     1419 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/expiration.py
--rwxr-xr-x   0        0        0      803 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/external_config.py
--rw-r--r--   0        0        0      291 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/external_config.yml
--rwxr-xr-x   0        0        0     4414 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/generate_test_db.py
--rw-r--r--   0        0        0      729 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/github_actions.yml
--rwxr-xr-x   0        0        0     1524 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/log_requests.py
--rwxr-xr-x   0        0        0     4602 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/pygithub.py
--rw-r--r--   0        0        0    36120 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/rps_graph.png
--rw-r--r--   0        0        0     4144 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/rps_graph.py
--rwxr-xr-x   0        0        0     1261 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/threads.py
--rwxr-xr-x   0        0        0     1336 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/time_machine_backtesting.py
--rwxr-xr-x   0        0        0     1583 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/url_patterns.py
--rwxr-xr-x   0        0        0     3697 2023-03-25 01:13:40.399311 requests_cache-1.0.1/examples/vcr.py
--rw-r--r--   0        0        0     5542 2023-03-25 01:13:40.403311 requests_cache-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      342 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/__init__.py
--rw-r--r--   0        0        0     2940 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/_utils.py
--rw-r--r--   0        0        0     3417 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/backends/__init__.py
--rw-r--r--   0        0        0    17188 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/backends/base.py
--rw-r--r--   0        0        0     6228 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/backends/dynamodb.py
--rw-r--r--   0        0        0     5029 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/backends/filesystem.py
--rw-r--r--   0        0        0     3844 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/backends/gridfs.py
--rw-r--r--   0        0        0     5694 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/backends/mongodb.py
--rw-r--r--   0        0        0     6429 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/backends/redis.py
--rw-r--r--   0        0        0    15965 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/backends/sqlite.py
--rw-r--r--   0        0        0     8448 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/cache_keys.py
--rw-r--r--   0        0        0      507 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/models/__init__.py
--rw-r--r--   0        0        0     1268 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/models/base.py
--rw-r--r--   0        0        0     4093 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/models/raw_response.py
--rw-r--r--   0        0        0     2132 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/models/request.py
--rwxr-xr-x   0        0        0     8330 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/models/response.py
--rw-r--r--   0        0        0     3773 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/patcher.py
--rw-r--r--   0        0        0      866 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/policy/__init__.py
--rw-r--r--   0        0        0    14239 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/policy/actions.py
--rw-r--r--   0        0        0     3239 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/policy/directives.py
--rw-r--r--   0        0        0     4397 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/policy/expiration.py
--rw-r--r--   0        0        0     2548 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/policy/settings.py
--rw-r--r--   0        0        0        0 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/py.typed
--rw-r--r--   0        0        0     2555 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/serializers/__init__.py
--rw-r--r--   0        0        0     7047 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/serializers/cattrs.py
--rw-r--r--   0        0        0     2507 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/serializers/pipeline.py
--rw-r--r--   0        0        0     5165 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/serializers/preconf.py
--rw-r--r--   0        0        0    16216 2023-03-25 01:13:40.403311 requests_cache-1.0.1/requests_cache/session.py
--rw-r--r--   0        0        0      151 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/README.md
--rw-r--r--   0        0        0        0 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2902 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/benchmark_serializers.py
--rw-r--r--   0        0        0      170 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/compat/README.md
--rw-r--r--   0        0        0    24576 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/compat/httpbin_sample.test-db
--rw-r--r--   0        0        0     1044 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/compat/test_requests_mock_combine_cache.py
--rw-r--r--   0        0        0      732 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/compat/test_requests_mock_disable_cache.py
--rw-r--r--   0        0        0     2198 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/compat/test_requests_mock_load_cache.py
--rw-r--r--   0        0        0     2110 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/compat/test_responses_load_cache.py
--rw-r--r--   0        0        0     9880 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/conftest.py
--rwxr-xr-x   0        0        0      624 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/generate_test_db.py
--rw-r--r--   0        0        0        0 2023-03-25 01:13:40.403311 requests_cache-1.0.1/tests/integration/__init__.py
--rw-r--r--   0        0        0    17539 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/base_cache_test.py
--rw-r--r--   0        0        0     6501 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/base_storage_test.py
--rw-r--r--   0        0        0     3516 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/test_dynamodb.py
--rw-r--r--   0        0        0     4661 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/test_filesystem.py
--rw-r--r--   0        0        0      579 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/test_memory.py
--rw-r--r--   0        0        0     5051 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/test_mongodb.py
--rw-r--r--   0        0        0     2288 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/test_redis.py
--rw-r--r--   0        0        0    12698 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/test_sqlite.py
--rw-r--r--   0        0        0      905 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/integration/test_upgrade.py
--rw-r--r--   0        0        0   131072 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.3.0
--rw-r--r--   0        0        0   131072 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.4.0
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.4.13
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.5.0
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.5.1
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.5.2
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.6.0
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.6.1
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.6.2
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.407311 requests_cache-1.0.1/tests/sample_data/sample.db.0.6.3
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.6.4
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.7.0
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.7.1
--rw-r--r--   0        0        0   122880 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.7.2
--rw-r--r--   0        0        0   122880 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.7.3
--rw-r--r--   0        0        0   122880 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.7.4
--rw-r--r--   0        0        0   147456 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.7.5
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.8.0
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.8.1
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.0
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.1
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.2
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.3
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.4
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.5
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.6
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.411311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.7
--rw-r--r--   0        0        0   118784 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/sample_data/sample.db.0.9.8
--rw-r--r--   0        0        0   122880 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/sample_data/sample.db.1.0.0
--rw-r--r--   0        0        0     1301 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/sample_data/vcr_requests_cache.yaml
--rw-r--r--   0        0        0     1777 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/sample_data/vcr_vcrpy.yaml
--rw-r--r--   0        0        0      931 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/models/test_base.py
--rw-r--r--   0        0        0     1980 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/models/test_raw_response.py
--rw-r--r--   0        0        0      827 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/models/test_request.py
--rw-r--r--   0        0        0     4888 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/models/test_response.py
--rw-r--r--   0        0        0    18127 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/policy/test_actions.py
--rw-r--r--   0        0        0     3454 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/policy/test_expiration.py
--rw-r--r--   0        0        0    15200 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/test_base_cache.py
--rw-r--r--   0        0        0     5721 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/test_cache_keys.py
--rw-r--r--   0        0        0     3482 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/test_patcher.py
--rw-r--r--   0        0        0     4609 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/test_serializers.py
--rw-r--r--   0        0        0    38198 2023-03-25 01:13:40.415311 requests_cache-1.0.1/tests/unit/test_session.py
--rw-r--r--   0        0        0     9918 1970-01-01 00:00:00.000000 requests_cache-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      272 2023-06-30 23:03:53.995100 requests_cache-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0     7501 2023-06-30 23:03:53.995100 requests_cache-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    41830 2023-06-30 23:03:53.995100 requests_cache-1.1.0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0    34641 2023-06-30 23:03:53.995100 requests_cache-1.1.0/HISTORY.md
+-rw-r--r--   0        0        0     1357 2023-06-30 23:03:53.995100 requests_cache-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7054 2023-06-30 23:03:53.995100 requests_cache-1.1.0/README.md
+-rw-r--r--   0        0        0      957 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docker-compose.yml
+-rw-r--r--   0        0        0      191 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/404.rst
+-rw-r--r--   0        0        0      176 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/Dockerfile
+-rw-r--r--   0        0        0     4389 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/dynamodb.png
+-rw-r--r--   0        0        0     3754 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/dynamodb_32px.png
+-rw-r--r--   0        0        0    51196 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/dynamodb_create_table.png
+-rw-r--r--   0        0        0    37675 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/dynamodb_items.png
+-rw-r--r--   0        0        0   102427 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/dynamodb_response.png
+-rw-r--r--   0        0        0     4166 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0        0        0     3888 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-json.png
+-rw-r--r--   0        0        0     3291 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-json_32px.png
+-rw-r--r--   0        0        0      989 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-pickle.png
+-rw-r--r--   0        0        0     2399 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-pickle_32px.png
+-rw-r--r--   0        0        0     5620 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-toml.png
+-rw-r--r--   0        0        0     2811 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-toml_32px.png
+-rw-r--r--   0        0        0     1907 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-yaml.png
+-rw-r--r--   0        0        0     2582 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-yaml_32px.png
+-rw-r--r--   0        0        0     2719 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/file-yaml_32px.png.png
+-rw-r--r--   0        0        0     7663 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/files-generic.png
+-rw-r--r--   0        0        0     6029 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/files-generic_32px.png
+-rw-r--r--   0        0        0     9754 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/files-json.png
+-rw-r--r--   0        0        0     3823 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/files-json_32px.png
+-rw-r--r--   0        0        0    32890 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/memcached.png
+-rw-r--r--   0        0        0     3790 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/memcached_32px.png
+-rw-r--r--   0        0        0     5923 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/memory_32px.png
+-rw-r--r--   0        0        0     5158 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/mongodb.png
+-rw-r--r--   0        0        0     2980 2023-06-30 23:03:53.995100 requests_cache-1.1.0/docs/_static/mongodb_32px.png
+-rw-r--r--   0        0        0   216933 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/mongodb_vscode.png
+-rw-r--r--   0        0        0     9031 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/redis.png
+-rw-r--r--   0        0        0     4998 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/redis_32px.png
+-rw-r--r--   0        0        0    49524 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/requests-cache-gh-preview.png
+-rw-r--r--   0        0        0    30478 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/requests-cache-icon.png
+-rw-r--r--   0        0        0    21674 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/requests-cache-logo-dark.webp
+-rw-r--r--   0        0        0    21385 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/requests-cache-logo-header.png
+-rw-r--r--   0        0        0    21144 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/requests-cache-logo-light.webp
+-rw-r--r--   0        0        0     5525 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/sqlite.png
+-rw-r--r--   0        0        0     3309 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/sqlite_32px.png
+-rw-r--r--   0        0        0      463 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/table.css
+-rw-r--r--   0        0        0     1404 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_static/toml.png
+-rw-r--r--   0        0        0      291 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_templates/module.rst_t
+-rw-r--r--   0        0        0      214 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/_templates/package.rst_t
+-rw-r--r--   0        0        0      309 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/api/requests_cache.session.md
+-rw-r--r--   0        0        0     5370 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0      275 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/docker-compose.yml
+-rw-r--r--   0        0        0     7288 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/examples.md
+-rw-r--r--   0        0        0      897 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/index.md
+-rw-r--r--   0        0        0     3317 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/project_info/code_of_conduct.md
+-rw-r--r--   0        0        0      805 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/project_info/codeshelter.md
+-rw-r--r--   0        0        0      142 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/project_info/contributing.md
+-rw-r--r--   0        0        0       82 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/project_info/contributors.md
+-rw-r--r--   0        0        0       87 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/project_info/history.md
+-rw-r--r--   0        0        0     2577 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/project_info/related_projects.md
+-rw-r--r--   0        0        0      198 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/project_info.md
+-rw-r--r--   0        0        0     1017 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/reference.md
+-rw-r--r--   0        0        0     1312 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/sample_data/sample_response_binary.json
+-rw-r--r--   0        0        0     1178 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/sample_data/sample_response_binary.yaml
+-rw-r--r--   0        0        0     1397 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/sample_data/sample_response_json.json
+-rw-r--r--   0        0        0      970 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/sample_data/sample_response_json.yaml
+-rw-r--r--   0        0        0     1967 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/advanced_requests.md
+-rw-r--r--   0        0        0     4208 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/backends/dynamodb.md
+-rw-r--r--   0        0        0     2148 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/backends/filesystem.md
+-rw-r--r--   0        0        0      617 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/backends/gridfs.md
+-rw-r--r--   0        0        0     3609 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/backends/mongodb.md
+-rw-r--r--   0        0        0     2731 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/backends/redis.md
+-rw-r--r--   0        0        0     4535 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/backends/sqlite.md
+-rw-r--r--   0        0        0     7088 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/backends.md
+-rw-r--r--   0        0        0     7394 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/compatibility.md
+-rw-r--r--   0        0        0    10951 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/expiration.md
+-rw-r--r--   0        0        0     3200 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/files.md
+-rw-r--r--   0        0        0     2875 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/filtering.md
+-rw-r--r--   0        0        0     3820 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/general.md
+-rw-r--r--   0        0        0     4026 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/headers.md
+-rw-r--r--   0        0        0     3848 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/inspection.md
+-rw-r--r--   0        0        0     1550 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/installation.md
+-rw-r--r--   0        0        0     7703 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/matching.md
+-rw-r--r--   0        0        0     3159 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/security.md
+-rw-r--r--   0        0        0     7143 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide/serializers.md
+-rw-r--r--   0        0        0     6069 2023-06-30 23:03:54.003100 requests_cache-1.1.0/docs/user_guide/troubleshooting.md
+-rw-r--r--   0        0        0      508 2023-06-30 23:03:53.999100 requests_cache-1.1.0/docs/user_guide.md
+-rw-r--r--   0        0        0    16051 2023-06-30 23:03:54.003100 requests_cache-1.1.0/docs/vector/requests-cache-logo-header.svg
+-rw-r--r--   0        0        0    15895 2023-06-30 23:03:54.003100 requests_cache-1.1.0/docs/vector/requests-cache-logo.svg
+-rw-r--r--   0        0        0     6035 2023-06-30 23:03:54.003100 requests_cache-1.1.0/docs/vector/requests_cache_icon.svg
+-rw-r--r--   0        0        0      241 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/README.md
+-rwxr-xr-x   0        0        0     1188 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/basic_patching.py
+-rwxr-xr-x   0        0        0      994 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/basic_sessions.py
+-rwxr-xr-x   0        0        0     3345 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/benchmark.py
+-rw-r--r--   0        0        0      974 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/cloudformation.yml
+-rwxr-xr-x   0        0        0     1382 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/convert_cache.py
+-rwxr-xr-x   0        0        0     2295 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/custom_request_matcher.py
+-rwxr-xr-x   0        0        0     1419 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/expiration.py
+-rwxr-xr-x   0        0        0      803 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/external_config.py
+-rw-r--r--   0        0        0      291 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/external_config.yml
+-rwxr-xr-x   0        0        0     4414 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/generate_test_db.py
+-rw-r--r--   0        0        0      729 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/github_actions.yml
+-rwxr-xr-x   0        0        0     1524 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/log_requests.py
+-rwxr-xr-x   0        0        0     4602 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/pygithub.py
+-rw-r--r--   0        0        0    36120 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/rps_graph.png
+-rw-r--r--   0        0        0     4144 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/rps_graph.py
+-rwxr-xr-x   0        0        0     1261 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/threads.py
+-rwxr-xr-x   0        0        0     1336 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/time_machine_backtesting.py
+-rwxr-xr-x   0        0        0     1583 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/url_patterns.py
+-rwxr-xr-x   0        0        0     3697 2023-06-30 23:03:54.003100 requests_cache-1.1.0/examples/vcr.py
+-rw-r--r--   0        0        0     5729 2023-06-30 23:03:54.003100 requests_cache-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      342 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/__init__.py
+-rw-r--r--   0        0        0     3467 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/_utils.py
+-rw-r--r--   0        0        0     3417 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/backends/__init__.py
+-rw-r--r--   0        0        0    17729 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/backends/base.py
+-rw-r--r--   0        0        0     6228 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/backends/dynamodb.py
+-rw-r--r--   0        0        0     5030 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/backends/filesystem.py
+-rw-r--r--   0        0        0     3851 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/backends/gridfs.py
+-rw-r--r--   0        0        0     5694 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/backends/mongodb.py
+-rw-r--r--   0        0        0     6429 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/backends/redis.py
+-rw-r--r--   0        0        0    18115 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/backends/sqlite.py
+-rw-r--r--   0        0        0     8897 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/cache_keys.py
+-rw-r--r--   0        0        0      507 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/models/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/models/base.py
+-rw-r--r--   0        0        0     4598 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/models/raw_response.py
+-rw-r--r--   0        0        0     2132 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/models/request.py
+-rwxr-xr-x   0        0        0     8336 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/models/response.py
+-rw-r--r--   0        0        0     3795 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/patcher.py
+-rw-r--r--   0        0        0      866 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/policy/__init__.py
+-rw-r--r--   0        0        0    14872 2023-06-30 23:03:54.003100 requests_cache-1.1.0/requests_cache/policy/actions.py
+-rw-r--r--   0        0        0     3239 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/policy/directives.py
+-rw-r--r--   0        0        0     4397 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/policy/expiration.py
+-rw-r--r--   0        0        0     2548 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/policy/settings.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/py.typed
+-rw-r--r--   0        0        0     2555 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/serializers/__init__.py
+-rw-r--r--   0        0        0     7567 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/serializers/cattrs.py
+-rw-r--r--   0        0        0     2507 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/serializers/pipeline.py
+-rw-r--r--   0        0        0     5165 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/serializers/preconf.py
+-rw-r--r--   0        0        0    15792 2023-06-30 23:03:54.007100 requests_cache-1.1.0/requests_cache/session.py
+-rw-r--r--   0        0        0      151 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2902 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/benchmark_serializers.py
+-rw-r--r--   0        0        0      170 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/compat/README.md
+-rw-r--r--   0        0        0    24576 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/compat/httpbin_sample.test-db
+-rw-r--r--   0        0        0     1044 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/compat/test_requests_mock_combine_cache.py
+-rw-r--r--   0        0        0      732 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/compat/test_requests_mock_disable_cache.py
+-rw-r--r--   0        0        0     2198 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/compat/test_requests_mock_load_cache.py
+-rw-r--r--   0        0        0     2110 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/compat/test_responses_load_cache.py
+-rw-r--r--   0        0        0    11196 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/conftest.py
+-rwxr-xr-x   0        0        0      624 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/generate_test_db.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0    17715 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/base_cache_test.py
+-rw-r--r--   0        0        0     6508 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/base_storage_test.py
+-rw-r--r--   0        0        0     3516 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/test_dynamodb.py
+-rw-r--r--   0        0        0     4661 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/test_filesystem.py
+-rw-r--r--   0        0        0      579 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/test_memory.py
+-rw-r--r--   0        0        0     5051 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/test_mongodb.py
+-rw-r--r--   0        0        0     2288 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/test_redis.py
+-rw-r--r--   0        0        0    15423 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/test_sqlite.py
+-rw-r--r--   0        0        0      894 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/integration/test_upgrade.py
+-rw-r--r--   0        0        0   131072 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.3.0
+-rw-r--r--   0        0        0   131072 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.4.0
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.4.13
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.5.0
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.5.1
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.5.2
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.6.0
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.6.1
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.6.2
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.007100 requests_cache-1.1.0/tests/sample_data/sample.db.0.6.3
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.6.4
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.7.0
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.7.1
+-rw-r--r--   0        0        0   122880 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.7.2
+-rw-r--r--   0        0        0   122880 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.7.3
+-rw-r--r--   0        0        0   122880 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.7.4
+-rw-r--r--   0        0        0   147456 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.7.5
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.8.0
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.8.1
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.0
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.1
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.2
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.3
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.4
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.5
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.6
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.7
+-rw-r--r--   0        0        0   118784 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.0.9.8
+-rw-r--r--   0        0        0   122880 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/sample.db.1.0.0
+-rw-r--r--   0        0        0     1301 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/vcr_requests_cache.yaml
+-rw-r--r--   0        0        0     1777 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/sample_data/vcr_vcrpy.yaml
+-rw-r--r--   0        0        0      931 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/unit/models/test_base.py
+-rw-r--r--   0        0        0     1930 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/unit/models/test_raw_response.py
+-rw-r--r--   0        0        0      827 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/unit/models/test_request.py
+-rw-r--r--   0        0        0     4882 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/unit/models/test_response.py
+-rw-r--r--   0        0        0    18127 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/unit/policy/test_actions.py
+-rw-r--r--   0        0        0     3454 2023-06-30 23:03:54.011100 requests_cache-1.1.0/tests/unit/policy/test_expiration.py
+-rw-r--r--   0        0        0    17000 2023-06-30 23:03:54.015101 requests_cache-1.1.0/tests/unit/test_base_cache.py
+-rw-r--r--   0        0        0     6298 2023-06-30 23:03:54.015101 requests_cache-1.1.0/tests/unit/test_cache_keys.py
+-rw-r--r--   0        0        0     3482 2023-06-30 23:03:54.015101 requests_cache-1.1.0/tests/unit/test_patcher.py
+-rw-r--r--   0        0        0     4609 2023-06-30 23:03:54.015101 requests_cache-1.1.0/tests/unit/test_serializers.py
+-rw-r--r--   0        0        0    42304 2023-06-30 23:03:54.015101 requests_cache-1.1.0/tests/unit/test_session.py
+-rw-r--r--   0        0        0     9913 1970-01-01 00:00:00.000000 requests_cache-1.1.0/PKG-INFO
```

### Comparing `requests_cache-1.0.1/CONTRIBUTING.md` & `requests_cache-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/CONTRIBUTORS.md` & `requests_cache-1.1.0/CONTRIBUTORS.md`

 * *Files 0% similar despite different names*

```diff
@@ -71,66 +71,67 @@
       <td align="center" valign="top" width="14.28%"><a href="https://gedmin.as/"><img src="https://avatars.githubusercontent.com/u/159967?v=4?s=100" width="100px;" alt="Marius Gedminas"/><br /><sub><b>Marius Gedminas</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=mgedmin" title="Code">💻</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Amgedmin" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.zopatista.com/"><img src="https://avatars.githubusercontent.com/u/46775?v=4?s=100" width="100px;" alt="Martijn Pieters"/><br /><sub><b>Martijn Pieters</b></sub></a><br /><a href="#ideas-mjpieters" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://lab.ar90n.net/"><img src="https://avatars.githubusercontent.com/u/2285892?v=4?s=100" width="100px;" alt="Masahiro Wada"/><br /><sub><b>Masahiro Wada</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=ar90n" title="Code">💻</a> <a href="#feature-ar90n" title="New features">✨</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://santini.di.unimi.it/"><img src="https://avatars.githubusercontent.com/u/612826?v=4?s=100" width="100px;" alt="Massimo Santini"/><br /><sub><b>Massimo Santini</b></sub></a><br /><a href="#ideas-mapio" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.mherman.org/"><img src="https://avatars.githubusercontent.com/u/2018167?v=4?s=100" width="100px;" alt="Michael Herman"/><br /><sub><b>Michael Herman</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=mjhea0" title="Code">💻</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=mjhea0" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mportesdev"><img src="https://avatars.githubusercontent.com/u/43098013?v=4?s=100" width="100px;" alt="Michal Porteš"/><br /><sub><b>Michal Porteš</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Amportesdev" title="Bug reports">🐛</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=mportesdev" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://mgorny.pl/"><img src="https://avatars.githubusercontent.com/u/110765?v=4?s=100" width="100px;" alt="Michał Górny"/><br /><sub><b>Michał Górny</b></sub></a><br /><a href="#infra-mgorny" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mnowotka"><img src="https://avatars.githubusercontent.com/u/837119?v=4?s=100" width="100px;" alt="Michał Nowotka"/><br /><sub><b>Michał Nowotka</b></sub></a><br /><a href="#ideas-mnowotka" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://beaumont.dev/"><img src="https://avatars.githubusercontent.com/u/2266568?v=4?s=100" width="100px;" alt="Mike"/><br /><sub><b>Mike</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=michaelbeaumont" title="Code">💻</a> <a href="#feature-michaelbeaumont" title="New features">✨</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/n-a-t-e"><img src="https://avatars.githubusercontent.com/u/26209011?v=4?s=100" width="100px;" alt="Nate"/><br /><sub><b>Nate</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3An-a-t-e" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://nathancahill.com/"><img src="https://avatars.githubusercontent.com/u/1383872?v=4?s=100" width="100px;" alt="Nathan Cahill"/><br /><sub><b>Nathan Cahill</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Anathancahill" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://nathancahill.com/"><img src="https://avatars.githubusercontent.com/u/1383872?v=4?s=100" width="100px;" alt="Nathan Cahill"/><br /><sub><b>Nathan Cahill</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Anathancahill" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://gitlab.com/kousu"><img src="https://avatars.githubusercontent.com/u/987487?v=4?s=100" width="100px;" alt="Nick"/><br /><sub><b>Nick</b></sub></a><br /><a href="#ideas-kousu" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/olivierdalang"><img src="https://avatars.githubusercontent.com/u/1894106?v=4?s=100" width="100px;" alt="Olivier Dalang"/><br /><sub><b>Olivier Dalang</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=olivierdalang" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/carlosal1015"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Acarlosal1015" title="Bug reports">🐛</a> <a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/parkerhancock"><img src="https://avatars.githubusercontent.com/u/633163?v=4?s=100" width="100px;" alt="Parker Hancock"/><br /><sub><b>Parker Hancock</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=parkerhancock" title="Code">💻</a> <a href="#feature-parkerhancock" title="New features">✨</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Aparkerhancock" title="Bug reports">🐛</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=parkerhancock" title="Tests">⚠️</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=parkerhancock" title="Documentation">📖</a> <a href="#security-parkerhancock" title="Security">🛡️</a> <a href="#ideas-parkerhancock" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pfmoore"><img src="https://avatars.githubusercontent.com/u/1110419?v=4?s=100" width="100px;" alt="Paul Moore"/><br /><sub><b>Paul Moore</b></sub></a><br /><a href="#ideas-pfmoore" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pkrefta"><img src="https://avatars.githubusercontent.com/u/565487?v=4?s=100" width="100px;" alt="Paweł Krefta"/><br /><sub><b>Paweł Krefta</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Apkrefta" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://phil.red/"><img src="https://avatars.githubusercontent.com/u/291575?v=4?s=100" width="100px;" alt="Philipp A."/><br /><sub><b>Philipp A.</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Aflying-sheep" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://phil.red/"><img src="https://avatars.githubusercontent.com/u/291575?v=4?s=100" width="100px;" alt="Philipp A."/><br /><sub><b>Philipp A.</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Aflying-sheep" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://rasmuse.github.io/"><img src="https://avatars.githubusercontent.com/u/1210973?v=4?s=100" width="100px;" alt="Rasmus Einarsson"/><br /><sub><b>Rasmus Einarsson</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Arasmuse" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://roderic.ca/"><img src="https://avatars.githubusercontent.com/u/6867226?v=4?s=100" width="100px;" alt="Roderic Day"/><br /><sub><b>Roderic Day</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3ARodericDay" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/reclosedev"><img src="https://avatars.githubusercontent.com/u/660112?v=4?s=100" width="100px;" alt="Roman Haritonov"/><br /><sub><b>Roman Haritonov</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=reclosedev" title="Code">💻</a> <a href="#maintenance-reclosedev" title="Maintenance">🚧</a> <a href="#feature-reclosedev" title="New features">✨</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Areclosedev" title="Bug reports">🐛</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=reclosedev" title="Tests">⚠️</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=reclosedev" title="Documentation">📖</a> <a href="#infra-reclosedev" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.facebook.com/avasamdev"><img src="https://avatars.githubusercontent.com/u/1350584?v=4?s=100" width="100px;" alt="Samuel T."/><br /><sub><b>Samuel T.</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3AAvasam" title="Bug reports">🐛</a> <a href="#ideas-Avasam" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sebastian-hoeffner.de/"><img src="https://avatars.githubusercontent.com/u/1836815?v=4?s=100" width="100px;" alt="Sebastian Höffner"/><br /><sub><b>Sebastian Höffner</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=shoeffner" title="Code">💻</a> <a href="#feature-shoeffner" title="New features">✨</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=shoeffner" title="Tests">⚠️</a> <a href="#ideas-shoeffner" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/grubberr"><img src="https://avatars.githubusercontent.com/u/195743?v=4?s=100" width="100px;" alt="Serhii Chvaliuk"/><br /><sub><b>Serhii Chvaliuk</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Agrubberr" title="Bug reports">🐛</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=grubberr" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://sbiewald.de/"><img src="https://avatars.githubusercontent.com/u/5983372?v=4?s=100" width="100px;" alt="Simon Biewald"/><br /><sub><b>Simon Biewald</b></sub></a><br /><a href="#security-Varbin" title="Security">🛡️</a> <a href="#ideas-Varbin" title="Ideas, Planning, & Feedback">🤔</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://sbiewald.de/"><img src="https://avatars.githubusercontent.com/u/5983372?v=4?s=100" width="100px;" alt="Simon Biewald"/><br /><sub><b>Simon Biewald</b></sub></a><br /><a href="#security-Varbin" title="Security">🛡️</a> <a href="#ideas-Varbin" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sleiner"><img src="https://avatars.githubusercontent.com/u/6379313?v=4?s=100" width="100px;" alt="Simon Leiner"/><br /><sub><b>Simon Leiner</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=sleiner" title="Code">💻</a> <a href="#feature-sleiner" title="New features">✨</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jseabold"><img src="https://avatars.githubusercontent.com/u/296164?v=4?s=100" width="100px;" alt="Skipper Seabold"/><br /><sub><b>Skipper Seabold</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Ajseabold" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://pathmind.com/"><img src="https://avatars.githubusercontent.com/u/1197406?v=4?s=100" width="100px;" alt="Slin Lee"/><br /><sub><b>Slin Lee</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=slinlee" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.stavros.io/"><img src="https://avatars.githubusercontent.com/u/23648?v=4?s=100" width="100px;" alt="Stavros Korokithakis"/><br /><sub><b>Stavros Korokithakis</b></sub></a><br /><a href="#infra-skorokithakis" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#tool-skorokithakis" title="Tools">🔧</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=skorokithakis" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://cheginit.github.io/"><img src="https://avatars.githubusercontent.com/u/13016644?v=4?s=100" width="100px;" alt="Taher Chegini"/><br /><sub><b>Taher Chegini</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Acheginit" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/TheTechromancer"><img src="https://avatars.githubusercontent.com/u/20261699?v=4?s=100" width="100px;" alt="TheTechromancer"/><br /><sub><b>TheTechromancer</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3ATheTechromancer" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ValueRaider"><img src="https://avatars.githubusercontent.com/u/96923577?v=4?s=100" width="100px;" alt="ValueRaider"/><br /><sub><b>ValueRaider</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=ValueRaider" title="Documentation">📖</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ValueRaider"><img src="https://avatars.githubusercontent.com/u/96923577?v=4?s=100" width="100px;" alt="ValueRaider"/><br /><sub><b>ValueRaider</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=ValueRaider" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://vladimir.panteleev.md/"><img src="https://avatars.githubusercontent.com/u/160894?v=4?s=100" width="100px;" alt="Vladimir Panteleev"/><br /><sub><b>Vladimir Panteleev</b></sub></a><br /><a href="#ideas-CyberShadow" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sansec.io/"><img src="https://avatars.githubusercontent.com/u/1145479?v=4?s=100" width="100px;" alt="Willem de Groot"/><br /><sub><b>Willem de Groot</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=gwillem" title="Code">💻</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Agwillem" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/WouterVH"><img src="https://avatars.githubusercontent.com/u/469509?v=4?s=100" width="100px;" alt="Wouter Vanden Hove"/><br /><sub><b>Wouter Vanden Hove</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3AWouterVH" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/YetAnotherNerd"><img src="https://avatars.githubusercontent.com/u/320738?v=4?s=100" width="100px;" alt="YetAnotherNerd"/><br /><sub><b>YetAnotherNerd</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=YetAnotherNerd" title="Code">💻</a> <a href="#feature-YetAnotherNerd" title="New features">✨</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3AYetAnotherNerd" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aaron-mf1"><img src="https://avatars.githubusercontent.com/u/65560918?v=4?s=100" width="100px;" alt="aaron-mf1"/><br /><sub><b>aaron-mf1</b></sub></a><br /><a href="#ideas-aaron-mf1" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/coryairbhb"><img src="https://avatars.githubusercontent.com/u/50755629?v=4?s=100" width="100px;" alt="coryairbhb"/><br /><sub><b>coryairbhb</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Acoryairbhb" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/craigls"><img src="https://avatars.githubusercontent.com/u/972350?v=4?s=100" width="100px;" alt="craig"/><br /><sub><b>craig</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=craigls" title="Code">💻</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Acraigls" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/craigls"><img src="https://avatars.githubusercontent.com/u/972350?v=4?s=100" width="100px;" alt="craig"/><br /><sub><b>craig</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=craigls" title="Code">💻</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Acraigls" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://stackoverflow.com/users/86643/denis"><img src="https://avatars.githubusercontent.com/u/1280390?v=4?s=100" width="100px;" alt="denis-bz"/><br /><sub><b>denis-bz</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Adenis-bz" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/eserdk"><img src="https://avatars.githubusercontent.com/u/16106844?v=4?s=100" width="100px;" alt="eserdk"/><br /><sub><b>eserdk</b></sub></a><br /><a href="#ideas-eserdk" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://gir.st/"><img src="https://avatars.githubusercontent.com/u/11820748?v=4?s=100" width="100px;" alt="girst"/><br /><sub><b>girst</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Agirst" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/gorogoroumaru"><img src="https://avatars.githubusercontent.com/u/30716350?v=4?s=100" width="100px;" alt="gorogoroumaru"/><br /><sub><b>gorogoroumaru</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=gorogoroumaru" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/gsalvatella"><img src="https://avatars.githubusercontent.com/u/42438361?v=4?s=100" width="100px;" alt="gsalvatella "/><br /><sub><b>gsalvatella </b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Agsalvatella" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/harvey251"><img src="https://avatars.githubusercontent.com/u/33844174?v=4?s=100" width="100px;" alt="harvey251"/><br /><sub><b>harvey251</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Aharvey251" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/masavini"><img src="https://avatars.githubusercontent.com/u/6315187?v=4?s=100" width="100px;" alt="masavini"/><br /><sub><b>masavini</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=masavini" title="Documentation">📖</a></td>
     </tr>
     <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/masavini"><img src="https://avatars.githubusercontent.com/u/6315187?v=4?s=100" width="100px;" alt="masavini"/><br /><sub><b>masavini</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=masavini" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mbarkhau"><img src="https://avatars.githubusercontent.com/u/446561?v=4?s=100" width="100px;" alt="mbarkhau"/><br /><sub><b>mbarkhau</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=mbarkhau" title="Code">💻</a> <a href="https://github.com/requests-cache/requests-cache/commits?author=mbarkhau" title="Tests">⚠️</a> <a href="#infra-mbarkhau" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Ambarkhau" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shiftinv"><img src="https://avatars.githubusercontent.com/u/8530778?v=4?s=100" width="100px;" alt="shiftinv"/><br /><sub><b>shiftinv</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=shiftinv" title="Code">💻</a> <a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Ashiftinv" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.witionstheme.com/"><img src="https://avatars.githubusercontent.com/u/55755139?v=4?s=100" width="100px;" alt="witionstheme"/><br /><sub><b>witionstheme</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3Awitionstheme" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/hlYassine"><img src="https://avatars.githubusercontent.com/u/3386466?v=4?s=100" width="100px;" alt="yassine"/><br /><sub><b>yassine</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/issues?q=author%3AhlYassine" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.zhihu.com/people/tan-jiu-ding"><img src="https://avatars.githubusercontent.com/u/24759802?v=4?s=100" width="100px;" alt="谭九鼎"/><br /><sub><b>谭九鼎</b></sub></a><br /><a href="https://github.com/requests-cache/requests-cache/commits?author=imba-tjd" title="Documentation">📖</a></td>
     </tr>
   </tbody>
```

#### html2text {}

```diff
@@ -1,50 +1,50 @@
 # Contributors Thanks to the following individuals for providing pull requests,
 feedback, and other contributions that have helped to improve requests-cache: -
 --
-                   ) Steers"/>                          [Al_Johri]                                           [Alex_Morega]                                                       [Alex_Sinitsin]                              [Andrew_Kittredge]                                         [Andrew_Stone]                     [Antonio_Lima]
-               Aaron ("AJ") Steers                       Al_Johri                                             Alex_Morega                                                         Alex_Sinitsin                                Andrew_Kittredge                                           Andrew_Stone                       Antonio_Lima
-                                                           ð¤                                            ð ð                                                    ð» ð                                ð                                              ð ð»                ð» â¨ ð¤
-                      ð¤
-             [Boris_Danilovich]                          [Charles]                                           [Chris_Wesseling]                                                    [Chris_de_Graaf]                          [Christoph_Reiter]                                             [Daniel_Holth]                   [Daniel_Rech]
-              Boris_Danilovich                            Charles                                             Chris_Wesseling                                                      Chris_de_Graaf                            Christoph_Reiter                                               Daniel_Holth                     Daniel_Rech
-                  ð» ð                        ð                                                 ð¤                                                          ð» â¨                            ð ð¤                                              ð»                      ð» ð
-                     [David_GIS]                   [David_Schmidt]                                             [David_Stosik]                                                    [Dragon_Dave_McKee]                          [Edward_Betts]                                     [Elan_RuusamÃ¤e]                         [Erik_KÃ¶rner]
-                      David_GIS                     David_Schmidt                                               David_Stosik                                                      Dragon_Dave_McKee                            Edward_Betts                                       Elan_RuusamÃ¤e                           Erik_KÃ¶rner
-                        ð                      ð ð»                                             ð                                                             ð»                                ð» ð                             ð ð ð¤ ð»            ð ð¤
-                      [Evan_D]                    [FemtoTrader]                                             [Florian_Demmer]                                                             [GDR!]                               [Garrett_Reynolds]                                            [Greg_Dingle]                  [Guangnan_Cheng]
-                       Evan_D                      FemtoTrader                                               Florian_Demmer                                                               GDR!                                 Garrett_Reynolds                                              Greg_Dingle                    Guangnan_Cheng
-                        ð               ð» ð ð¤ â¨                               ð» ð                                                          ð                                   ð»                                                    ð¤                      ð» â¨
-               [Honza_Javorek]                         [Iftah]                                                      [Ilya]                                                         [J_Rob_Gant]                               [Jace_Browning]                                           [Jakub_SemriÄ]                     [Jeff_O'Neill]
-                Honza_Javorek                           Iftah                                                        Ilya                                                           J_Rob_Gant                                 Jace_Browning                                             Jakub_SemriÄ                       Jeff_O'Neill
-                  ð ð¤                   ð ð»                                              ð»                                                       ð» ð                            ð» ð                                         ð» ð¤                       ð
-                [Jeremy_Douglass]               [Jessy_Williams]                                      [John_Vandenberg]                                                            [Jonathan_Liuti]                      [JonÃ¡Å¡_JanÄaÅÃ­                         [Jordan_Cook]                              [JÃ¼rgen_Hermann]
-                 Jeremy_Douglass                 Jessy_Williams                                        John_Vandenberg                                                              Jonathan_Liuti                        JonÃ¡Å¡_JanÄaÅÃ­                          Jordan_Cook                                JÃ¼rgen_Hermann
-                      ð¤                  ð» ð â ï¸                         ð ð¦ â ï¸                                                    ð                                ð                           ð» ð§ â¨ ð â ï¸ ð       ð ð¤
-                 [Kieran_W]                             [MHellmund]                                        [Manuel_Eggimann]                                                    [Marc_Abramowitz]                            [Marius_Gedminas]                                           [Martijn_Pieters]                 [Masahiro_Wada]
-                  Kieran_W                               MHellmund                                          Manuel_Eggimann                                                      Marc_Abramowitz                              Marius_Gedminas                                             Martijn_Pieters                   Masahiro_Wada
-                  ð ð                        ð                                            ð ð»                                                    ð» ð                            ð» ð                                              ð¤                       ð» â¨
-                [Massimo_Santini]                 [Michael_Herman]                                          [MichaÅ_GÃ³rny]                                                 [MichaÅ_Nowotka]                               [Mike]                                                       [Nate]                       [Nathan_Cahill]
-                 Massimo_Santini                   Michael_Herman                                            MichaÅ_GÃ³rny                                                   MichaÅ_Nowotka                                 Mike                                                         Nate                         Nathan_Cahill
-                      ð¤                        ð» ð                                           ð                                                              ð¤                                  ð» â¨                                                ð                          ð
-                       [Nick]                       [Olivier_Dalang]                                           [Oromion]                                              [Parker_Hancock]                                             [Paul_Moore]                                          [PaweÅ_Krefta]                      [Philipp_A.]
-                        Nick                         Olivier_Dalang                                             Oromion                                                Parker_Hancock                                               Paul_Moore                                            PaweÅ_Krefta                        Philipp_A.
-                        ð¤                          ð»                                             ð ð¦                           ð» â¨ ð â ï¸ ð ð¡ï¸               ð¤                                                ð                             ð
-               [Rasmus_Einarsson]                      [Roderic_Day]                             [Roman_Haritonov]                                                                 [Samuel_T.]                           [Sebastian_HÃ¶ffner]                                        [Serhii_Chvaliuk]                   [Simon_Biewald]
-                Rasmus_Einarsson                        Roderic_Day                               Roman_Haritonov                                                                   Samuel_T.                             Sebastian_HÃ¶ffner                                          Serhii_Chvaliuk                     Simon_Biewald
-                      ð                             ð                     ð» ð§ â¨ ð â ï¸ ð ð                              ð ð¤                    ð» â¨ â ï¸ ð¤                             ð ð»                 ð¡ï¸ ð¤
-                [Simon_Leiner]                      [Skipper_Seabold]                                             [Slin_Lee]                                               [Stavros_Korokithakis]                                [Taher_Chegini]                                         [TheTechromancer]                     [ValueRaider]
-                 Simon_Leiner                        Skipper_Seabold                                               Slin_Lee                                                 Stavros_Korokithakis                                  Taher_Chegini                                           TheTechromancer                       ValueRaider
-                   ð» â¨                        ð                                                   ð                                                  ð ð§ ð                             ð                                                  ð                            ð
-              [Vladimir_Panteleev]                [Willem_de_Groot]                                        [Wouter_Vanden_Hove]                                                [YetAnotherNerd]                                     [aaron-mf1]                                              [coryairbhb]                      [craig]
-               Vladimir_Panteleev                  Willem_de_Groot                                          Wouter_Vanden_Hove                                                  YetAnotherNerd                                       aaron-mf1                                                coryairbhb                        craig
-                      ð¤                        ð» ð                                            ð                                                     ð» â¨ ð                               ð¤                                                  ð                     ð» ð
-                     [denis-bz]                          [eserdk]                                                  [girst]                                                          [gorogoroumaru]                              [gsalvatella_]                                              [harvey251]                         [masavini]
-                      denis-bz                            eserdk                                                    girst                                                            gorogoroumaru                                 gsalvatella                                                harvey251                           masavini
-                        ð                           ð¤                                                  ð                                                             ð»                                    ð                                                   ð                           ð
-              [mbarkhau]                             [shiftinv]                                                [witionstheme]                                                          [yassine]                               [è°­ä¹é¼]
-               mbarkhau                               shiftinv                                                  witionstheme                                                            yassine                                 è°­ä¹é¼
-         ð» â ï¸ ð ð            ð» ð                                             ð                                                              ð                                ð
+       ) Steers"/>                           [Al_Johri]                  [Alex_Morega]                                           [Alex_Sinitsin]                                                       [Andrew_Kittredge]                                                 [Andrew_Stone]                     [Antonio_Lima]
+   Aaron ("AJ") Steers                        Al_Johri                    Alex_Morega                                             Alex_Sinitsin                                                         Andrew_Kittredge                                                   Andrew_Stone                       Antonio_Lima
+                                                ð¤                   ð ð                                        ð» ð                                                         ð                                                      ð ð»                ð» â¨ ð¤
+          ð¤
+  [Boris_Danilovich]                          [Charles]                  [Chris_Wesseling]                                       [Chris_de_Graaf]                                                    [Christoph_Reiter]                                                     [Daniel_Holth]                   [Daniel_Rech]
+   Boris_Danilovich                            Charles                    Chris_Wesseling                                         Chris_de_Graaf                                                      Christoph_Reiter                                                       Daniel_Holth                     Daniel_Rech
+       ð» ð                        ð                        ð¤                                             ð» â¨                                                     ð ð¤                                                       ð»                      ð» ð
+         [David_GIS]                   [David_Schmidt]                      [David_Stosik]                                      [Dragon_Dave_McKee]                                                    [Edward_Betts]                                             [Elan_RuusamÃ¤e]                         [Erik_KÃ¶rner]
+          David_GIS                     David_Schmidt                        David_Stosik                                        Dragon_Dave_McKee                                                      Edward_Betts                                               Elan_RuusamÃ¤e                           Erik_KÃ¶rner
+            ð                      ð ð»                      ð                                               ð»                                                         ð» ð                                      ð ð ð¤ ð»            ð ð¤
+          [Evan_D]                   [FemtoTrader]                      [Florian_Demmer]                                                 [GDR!]                                                        [Garrett_Reynolds]                                                    [Greg_Dingle]                  [Guangnan_Cheng]
+           Evan_D                     FemtoTrader                        Florian_Demmer                                                   GDR!                                                          Garrett_Reynolds                                                      Greg_Dingle                    Guangnan_Cheng
+            ð              ð» ð ð¤ â          ð» ð                                              ð                                                            ð»                                                            ð¤                      ð» â¨
+    [Honza_Javorek]                        [Iftah]                              [Ilya]                                             [J_Rob_Gant]                                                       [Jace_Browning]                                                    [Jakub_SemriÄ]                     [Jeff_O'Neill]
+     Honza_Javorek                          Iftah                                Ilya                                               J_Rob_Gant                                                         Jace_Browning                                                      Jakub_SemriÄ                       Jeff_O'Neill
+       ð ð¤                  ð ð»                      ð»                                           ð» ð                                                    ð» ð                                                  ð» ð¤                       ð
+    [Jeremy_Douglass]              [Jessy_Williams]                   [John_Vandenberg]                                            [Jonathan_Liuti]                                            [JonÃ¡Å¡_JanÄaÅÃ­k]                                  [Jordan_Cook]                              [JÃ¼rgen_Hermann]
+     Jeremy_Douglass                Jessy_Williams                     John_Vandenberg                                              Jonathan_Liuti                                              JonÃ¡Å¡_JanÄaÅÃ­k                                    Jordan_Cook                                JÃ¼rgen_Hermann
+          ð¤                 ð» ð â ï¸�       ð ð¦ â ï¸                                    ð                                                       ð                                     ð» ð§ â¨ ð â ï¸ ð       ð ð¤
+      [Kieran_W]                             [MHellmund]               [Manuel_Eggimann]                                        [Marc_Abramowitz]                                                    [Marius_Gedminas]                                                    [Martijn_Pieters]                 [Masahiro_Wada]
+       Kieran_W                               MHellmund                 Manuel_Eggimann                                          Marc_Abramowitz                                                      Marius_Gedminas                                                      Martijn_Pieters                   Masahiro_Wada
+       ð ð                        ð                   ð ð»                                        ð» ð                                                    ð» ð                                                       ð¤                       ð» â¨
+    [Massimo_Santini]                 [Michael_Herman]                  [Michal_PorteÅ¡]                                       [MichaÅ_GÃ³rny]                                                 [MichaÅ_Nowotka]                                                     [Mike]                                [Nate]
+     Massimo_Santini                   Michael_Herman                    Michal_PorteÅ¡                                         MichaÅ_GÃ³rny                                                   MichaÅ_Nowotka                                                       Mike                                  Nate
+          ð¤                        ð» ð                ð ð»                                           ð                                                              ð¤                                                        ð» â¨                         ð
+      [Nathan_Cahill]                          [Nick]                     [Olivier_Dalang]                                          [Oromion]                                              [Parker_Hancock]                                                                   [Paul_Moore]                   [PaweÅ_Krefta]
+       Nathan_Cahill                            Nick                       Olivier_Dalang                                            Oromion                                                Parker_Hancock                                                                     Paul_Moore                     PaweÅ_Krefta
+           ð                             ð¤                        ð»                                            ð ð¦                           ð» â¨ ð â ï¸ ð ð¡ï¸ ð¤                              ð¤                         ð
+        [Philipp_A.]                   [Rasmus_Einarsson]                   [Roderic_Day]                             [Roman_Haritonov]                                                                 [Samuel_T.]                                            [Sebastian_HÃ¶ffner]                      [Serhii_Chvaliuk]
+         Philipp_A.                     Rasmus_Einarsson                     Roderic_Day                               Roman_Haritonov                                                                   Samuel_T.                                              Sebastian_HÃ¶ffner                        Serhii_Chvaliuk
+            ð                          ð                           ð                    ð» ð§ â¨ ð â ï¸ ð ð                              ð ð¤                                     ð» â¨ â ï¸ ð¤           ð ð»
+    [Simon_Biewald]                     [Simon_Leiner]                   [Skipper_Seabold]                                             [Slin_Lee]                                               [Stavros_Korokithakis]                                                     [Taher_Chegini]                   [TheTechromancer]
+     Simon_Biewald                       Simon_Leiner                     Skipper_Seabold                                               Slin_Lee                                                 Stavros_Korokithakis                                                       Taher_Chegini                     TheTechromancer
+     ð¡ï¸ ð¤               ð» â¨                      ð                                                  ð                                                  ð ð§ ð                                                   ð                           ð
+       [ValueRaider]                  [Vladimir_Panteleev]             [Willem_de_Groot]                                        [Wouter_Vanden_Hove]                                                [YetAnotherNerd]                                                          [aaron-mf1]                        [coryairbhb]
+        ValueRaider                    Vladimir_Panteleev               Willem_de_Groot                                          Wouter_Vanden_Hove                                                  YetAnotherNerd                                                            aaron-mf1                          coryairbhb
+           ð                           ð¤                     ð» ð                                            ð                                                     ð» â¨ ð                                                     ð¤                           ð
+        [craig]                              [denis-bz]                        [eserdk]                                                 [girst]                                                          [gorogoroumaru]                                                    [gsalvatella_]                       [harvey251]
+         craig                                denis-bz                          eserdk                                                   girst                                                            gorogoroumaru                                                      gsalvatella                          harvey251
+       ð» ð                        ð                         ð¤                                                 ð                                                             ð»                                                          ð                            ð
+         [masavini]                   [mbarkhau]                           [shiftinv]                                               [witionstheme]                                                          [yassine]                                                     [è°­ä¹é¼]
+          masavini                     mbarkhau                             shiftinv                                                 witionstheme                                                            yassine                                                       è°­ä¹é¼
+            ð             ð» â ï¸ ð �          ð» ð                                             ð                                                              ð                                                       ð
    --- This page was made using [all-contributors](https://github.com/all-
 contributors/all-contributors). See [emoji key](https://allcontributors.org/
 docs/en/emoji-key) for details on contribution types. If you notice a missing
 contributor or contribution type, please update it!
```

### Comparing `requests_cache-1.0.1/HISTORY.md` & `requests_cache-1.1.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 # History
 
-## Unreleased
-* Add support for regular expressions when using `urls_expire_after`
+## 1.2.0 (TBD)
+* ⚠️ Remove `CachedSession` and `BaseCache` methods [deprecated in 1.0](#deprecations-1-0)
 
-## 1.0.1 (2023-03-24)
+## 1.1.0 (2023-06-30)
+
+⚙️ **Session settings:**
+* Add support for regular expressions with `urls_expire_after`
+
+💾 **SQLite Backend:**
+* Add `busy_timeout` argument (see [SQLite docs](https://www.sqlite.org/pragma.html#pragma_busy_timeout) for details)
+* In WAL journaling mode (`wal=True`), default to 'normal' synchronous mode instead of 'full'
+* Fix potential `OperationalError: database is locked` in multithreaded SQLite usage during bulk delete operations
+* Fix deadlock in multithreaded SQLite usage if a thread encounters an error during COMMIT
+
+🪲 **Bugfixes:**
+* Fix loading cached JSON content with `decode_content=True` when the root element is a list
+* Fix `BaseCache.recreate_keys()` to normalize response bodies with `b'None'`
+* Fix `BaseCache.contains()` for multipart POST requests
+* Fix `CachedResponse.history` not being fully deserialized on python<=3.8
+* Fix request matching with `Vary` and redirects
+* Skip normalizing `CachedResponse.url` so it always matches the original request URL
+* Avoid unnecessary cache writes for revalidation requests if headers and expiration are unchanged
+* Add compatibility with urllib3 2.0
+
+### 1.0.1 (2023-03-24)
 * Ignore `Cache-Control: must-revalidate` and `no-cache` response headers with `cache_control=False`
 
 ## 1.0.0 (2023-03-01)
 [See all unreleased issues and PRs](https://github.com/requests-cache/requests-cache/milestone/10?closed=1)
 
 🕗 **Expiration & headers:**
 * Add support for `Cache-Control: min-fresh`
@@ -125,17 +146,17 @@
 * Raise an error for invalid expiration string values (except for headers containing httpdates)
   * Previously, this would be quietly ignored, and the response would be cached indefinitely
 * Fix behavior for `stale_if_error` if an error response code is added to `allowable_codes`
 
 📦 **Dependencies:**
 * Replace `appdirs` with `platformdirs`
 
-⚠️ **Deprecations:**
+⚠️ <a id="deprecations-1-0">**Deprecations:**</a>
 
-The following methods are deprecated, and will be removed in a future release. The recommended
+The following methods are deprecated, and will be removed in **1.2**. The recommended
 replacements are listed below. If this causes problems for you, please open an issue to discuss.
 * `CachedSession.remove_expired_responses()`: `BaseCache.delete(expired=True)`
 * `BaseCache.remove_expired_responses()`: `BaseCache.delete(expired=True)`
 * `BaseCache.delete_url()`: `BaseCache.delete(urls=[...])`
 * `BaseCache.delete_urls()`: `BaseCache.delete(urls=[...])`
 * `BaseCache.has_key()`: `BaseCache.contains()`
 * `BaseCache.has_url()`: `BaseCache.contains(url=...)`
```

### Comparing `requests_cache-1.0.1/LICENSE` & `requests_cache-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/README.md` & `requests_cache-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docker-compose.yml` & `requests_cache-1.1.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/dynamodb.png` & `requests_cache-1.1.0/docs/_static/dynamodb.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/dynamodb_32px.png` & `requests_cache-1.1.0/docs/_static/dynamodb_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/dynamodb_create_table.png` & `requests_cache-1.1.0/docs/_static/dynamodb_create_table.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/dynamodb_items.png` & `requests_cache-1.1.0/docs/_static/dynamodb_items.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/dynamodb_response.png` & `requests_cache-1.1.0/docs/_static/dynamodb_response.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/favicon.ico` & `requests_cache-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-json.png` & `requests_cache-1.1.0/docs/_static/file-json.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-json_32px.png` & `requests_cache-1.1.0/docs/_static/file-json_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-pickle.png` & `requests_cache-1.1.0/docs/_static/file-pickle.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-pickle_32px.png` & `requests_cache-1.1.0/docs/_static/file-pickle_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-toml.png` & `requests_cache-1.1.0/docs/_static/file-toml.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-toml_32px.png` & `requests_cache-1.1.0/docs/_static/file-toml_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-yaml.png` & `requests_cache-1.1.0/docs/_static/file-yaml.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-yaml_32px.png` & `requests_cache-1.1.0/docs/_static/file-yaml_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/file-yaml_32px.png.png` & `requests_cache-1.1.0/docs/_static/file-yaml_32px.png.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/files-generic.png` & `requests_cache-1.1.0/docs/_static/files-generic.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/files-generic_32px.png` & `requests_cache-1.1.0/docs/_static/files-generic_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/files-json.png` & `requests_cache-1.1.0/docs/_static/files-json.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/files-json_32px.png` & `requests_cache-1.1.0/docs/_static/files-json_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/memcached.png` & `requests_cache-1.1.0/docs/_static/memcached.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/memcached_32px.png` & `requests_cache-1.1.0/docs/_static/memcached_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/memory_32px.png` & `requests_cache-1.1.0/docs/_static/memory_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/mongodb.png` & `requests_cache-1.1.0/docs/_static/mongodb.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/mongodb_32px.png` & `requests_cache-1.1.0/docs/_static/mongodb_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/mongodb_vscode.png` & `requests_cache-1.1.0/docs/_static/mongodb_vscode.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/redis.png` & `requests_cache-1.1.0/docs/_static/redis.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/redis_32px.png` & `requests_cache-1.1.0/docs/_static/redis_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/requests-cache-gh-preview.png` & `requests_cache-1.1.0/docs/_static/requests-cache-gh-preview.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/requests-cache-icon.png` & `requests_cache-1.1.0/docs/_static/requests-cache-icon.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/requests-cache-logo-dark.webp` & `requests_cache-1.1.0/docs/_static/requests-cache-logo-dark.webp`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/requests-cache-logo-header.png` & `requests_cache-1.1.0/docs/_static/requests-cache-logo-header.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/requests-cache-logo-light.webp` & `requests_cache-1.1.0/docs/_static/requests-cache-logo-light.webp`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/sqlite.png` & `requests_cache-1.1.0/docs/_static/sqlite.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/sqlite_32px.png` & `requests_cache-1.1.0/docs/_static/sqlite_32px.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/_static/toml.png` & `requests_cache-1.1.0/docs/_static/toml.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/conf.py` & `requests_cache-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/examples.md` & `requests_cache-1.1.0/docs/examples.md`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 ```
 
 :::{dropdown} Example
 :animate: fade-in-slide-down
 :color: primary
 :icon: file-code
 
-[benchmark.py](https://github.com/requests-cache/requests-cache/blob/main/examples/rps_graph.py)
+[rps_graph.py](https://github.com/requests-cache/requests-cache/blob/main/examples/rps_graph.py)
 ```{literalinclude} ../examples/rps_graph.py
 :lines: 9-
 ```
 :::
 
 :::{dropdown} Screenshot
 :animate: fade-in-slide-down
```

### Comparing `requests_cache-1.0.1/docs/index.md` & `requests_cache-1.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/project_info/code_of_conduct.md` & `requests_cache-1.1.0/docs/project_info/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/project_info/codeshelter.md` & `requests_cache-1.1.0/docs/project_info/codeshelter.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/reference.md` & `requests_cache-1.1.0/docs/reference.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/sample_data/sample_response_binary.json` & `requests_cache-1.1.0/docs/sample_data/sample_response_binary.json`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/sample_data/sample_response_binary.yaml` & `requests_cache-1.1.0/docs/sample_data/sample_response_binary.yaml`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/sample_data/sample_response_json.json` & `requests_cache-1.1.0/docs/sample_data/sample_response_json.json`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/sample_data/sample_response_json.yaml` & `requests_cache-1.1.0/docs/sample_data/sample_response_json.yaml`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/advanced_requests.md` & `requests_cache-1.1.0/docs/user_guide/advanced_requests.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/backends/dynamodb.md` & `requests_cache-1.1.0/docs/user_guide/backends/dynamodb.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/backends/filesystem.md` & `requests_cache-1.1.0/docs/user_guide/backends/filesystem.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/backends/gridfs.md` & `requests_cache-1.1.0/docs/user_guide/backends/gridfs.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/backends/mongodb.md` & `requests_cache-1.1.0/docs/user_guide/backends/mongodb.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/backends/redis.md` & `requests_cache-1.1.0/docs/user_guide/backends/redis.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/backends/sqlite.md` & `requests_cache-1.1.0/docs/user_guide/backends/sqlite.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,80 +5,103 @@
 [SQLite](https://www.sqlite.org/) is a fast and lightweight SQL database engine that stores data
 either in memory or in a single file on disk.
 
 ## Use Cases
 Despite its simplicity, SQLite is a powerful tool. For example, it's the primary storage system for
 a number of common applications including Firefox, Chrome, and many components of both Android and
 iOS. It's well suited for caching, and requires no extra configuration or dependencies, which is why
-it's 'used as the default backend for requests-cache.
+it's used as the default backend for requests-cache.
 
 ## Usage Example
-SQLite is the default backend, but if you want to pass extra connection options or just want to be
-explicit, initialize your session with a {py:class}`.SQLiteCache` instance:
+SQLite will be used as the default backend without providing any arguments. If you want to pass
+extra connection options or just want to be explicit, initialize your session with a
+{py:class}`.SQLiteCache` instance:
 ```python
 >>> from requests_cache import CachedSession, SQLiteCache
->>> session = CachedSession(backend=SQLiteCache())
+>>> backend = SQLiteCache()
+>>> session = CachedSession(backend=backend)
 ```
 
-Or by alias:
+Or initialize it by alias:
 ```python
 >>> session = CachedSession(backend='sqlite')
 ```
 
 ## Connection Options
 This backend accepts any keyword arguments for {py:func}`sqlite3.connect`:
 ```python
->>> backend = SQLiteCache('http_cache', timeout=30)
->>> session = CachedSession(backend=backend)
+>>> backend = SQLiteCache(timeout=30)
 ```
 
 ## Cache Files
-- See {ref}`files` for general info on specifying cache paths
+- By default, a file named `http_cache.sqlite` will be created in the current working directory
+- You can specify a different cache filename using the first positional argument to {py:class}`.SQLiteCache`
 - If you specify a name without an extension, the default extension `.sqlite` will be used
+- See {ref}`files` for general info on specifying cache paths
+
+Example
+```python
+>>> backend = SQLiteCache('cache/http_cache.sqlite')
+```
 
 ### In-Memory Caching
 SQLite also supports [in-memory databases](https://www.sqlite.org/inmemorydb.html).
 You can enable this (in "shared" memory mode) with the `use_memory` option:
 ```python
->>> session = CachedSession('http_cache', use_memory=True)
+>>> backend = SQLiteCache(use_memory=True)
 ```
 
 Or specify a memory URI with additional options:
 ```python
->>> session = CachedSession(':file:memdb1?mode=memory')
+>>> backend = SQLiteCache(':file:memdb1?mode=memory')
 ```
 
 Or just `:memory:`, if you are only using the cache from a single thread:
 ```python
->>> session = CachedSession(':memory:')
+>>> backend = SQLiteCache(':memory:')
 ```
 
 ## Performance
 When working with average-sized HTTP responses (\< 1MB) and using a modern SSD for file storage, you
 can expect speeds of around:
 - Write: 2-8ms
 - Read: 0.2-0.6ms
 
 Of course, this will vary based on hardware specs, response size, and other factors.
 
+The `fast_save` option can be used to increase cache write performance, but with the possibility of
+data loss. See `pragma: synchronous <https://www.sqlite.org/pragma.html#pragma_synchronous>`_
+for details.
+```python
+>>> backend = SQLiteCache(fast_save=True)
+```
+
 ## Concurrency
 SQLite supports concurrent access, so it is safe to use from a multi-threaded and/or multi-process
 application. It supports unlimited concurrent reads. Writes, however, are queued and run in serial,
 so if you need to make large volumes of concurrent requests, you may want to consider a different
 backend that's specifically made for that kind of workload, like {py:class}`.RedisCache`.
 
+One option to consider is `Write Ahead Logging <https://sqlite.org/wal.html>`_. This comes with a
+number of tradeoffs, but most notably it allows read operations to not block writes. This can be
+enabled with the `wal` option:
+```python
+>>> backend = SQLiteCache(wal=True)
+```
+
 ## Hosting Services and Filesystem Compatibility
 There are some caveats to using SQLite with some hosting services, based on what kind of storage is
 available:
 
 - NFS:
   - SQLite may be used on a NFS, but is usually only safe to use from a single process at a time.
     See the [SQLite FAQ](https://www.sqlite.org/faq.html#q5) for details.
   - PythonAnywhere is one example of a host that uses NFS-backed storage. Using SQLite from a
     multiprocess application will likely result in `sqlite3.OperationalError: database is locked`.
 - Ephemeral storage:
   - Heroku [explicitly disables SQLite](https://devcenter.heroku.com/articles/sqlite3) on its dynos.
   - AWS [EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html),
     [Lambda (depending on configuration)](https://aws.amazon.com/blogs/compute/choosing-between-aws-lambda-data-storage-options-in-web-apps/),
     and some other AWS services use ephemeral storage that only persists for the lifetime of the
-    instance. This is fine for short-term caching. For longer-term persistance, you can use an
+    instance. This is fine for short-term caching. For longer-term persistance, you can store the
+    cache on an
     [attached EBS volume](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-attaching-volume.html).
```

### Comparing `requests_cache-1.0.1/docs/user_guide/backends.md` & `requests_cache-1.1.0/docs/user_guide/backends.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/compatibility.md` & `requests_cache-1.1.0/docs/user_guide/compatibility.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/expiration.md` & `requests_cache-1.1.0/docs/user_guide/expiration.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/files.md` & `requests_cache-1.1.0/docs/user_guide/files.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/filtering.md` & `requests_cache-1.1.0/docs/user_guide/filtering.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/general.md` & `requests_cache-1.1.0/docs/user_guide/general.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/headers.md` & `requests_cache-1.1.0/docs/user_guide/headers.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/inspection.md` & `requests_cache-1.1.0/docs/user_guide/inspection.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/installation.md` & `requests_cache-1.1.0/docs/user_guide/installation.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/matching.md` & `requests_cache-1.1.0/docs/user_guide/matching.md`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 the `foo` request parameter from the cache key, meaning these three requests will all use the same
 cached response:
 ```python
 >>> session = CachedSession(ignored_parameters=['foo'])
 >>> response_1 = session.get('https://example.com')          # cache miss
 >>> response_2 = session.get('https://example.com?foo=bar')  # cache hit
 >>> response_3 = session.get('https://example.com?foo=qux')  # cache hit
->>> assert response_1.cache_key == response_2.cache_key == response_3.cache_key
+>>> assert response_2.cache_key == response_3.cache_key
 ```
 
 ### Recreating Cache Keys
 There are some situations where request matching behavior may change, which causes previously cached
 responses to become obsolete:
 * You start using a custom cache key, or change other settings that affect request matching
 * A new version of requests-cache is released that includes new or changed request matching behavior
```

### Comparing `requests_cache-1.0.1/docs/user_guide/security.md` & `requests_cache-1.1.0/docs/user_guide/security.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/serializers.md` & `requests_cache-1.1.0/docs/user_guide/serializers.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/user_guide/troubleshooting.md` & `requests_cache-1.1.0/docs/user_guide/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/vector/requests-cache-logo-header.svg` & `requests_cache-1.1.0/docs/vector/requests-cache-logo-header.svg`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/vector/requests-cache-logo.svg` & `requests_cache-1.1.0/docs/vector/requests-cache-logo.svg`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/docs/vector/requests_cache_icon.svg` & `requests_cache-1.1.0/docs/vector/requests_cache_icon.svg`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/basic_patching.py` & `requests_cache-1.1.0/examples/basic_patching.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/basic_sessions.py` & `requests_cache-1.1.0/examples/basic_sessions.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/benchmark.py` & `requests_cache-1.1.0/examples/benchmark.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/cloudformation.yml` & `requests_cache-1.1.0/examples/cloudformation.yml`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/convert_cache.py` & `requests_cache-1.1.0/examples/convert_cache.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/custom_request_matcher.py` & `requests_cache-1.1.0/examples/custom_request_matcher.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/expiration.py` & `requests_cache-1.1.0/examples/expiration.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/external_config.py` & `requests_cache-1.1.0/examples/external_config.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/generate_test_db.py` & `requests_cache-1.1.0/examples/generate_test_db.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/github_actions.yml` & `requests_cache-1.1.0/examples/github_actions.yml`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/log_requests.py` & `requests_cache-1.1.0/examples/log_requests.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/pygithub.py` & `requests_cache-1.1.0/examples/pygithub.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/rps_graph.png` & `requests_cache-1.1.0/examples/rps_graph.png`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/rps_graph.py` & `requests_cache-1.1.0/examples/rps_graph.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/threads.py` & `requests_cache-1.1.0/examples/threads.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/time_machine_backtesting.py` & `requests_cache-1.1.0/examples/time_machine_backtesting.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/url_patterns.py` & `requests_cache-1.1.0/examples/url_patterns.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/examples/vcr.py` & `requests_cache-1.1.0/examples/vcr.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/pyproject.toml` & `requests_cache-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requests-cache"
-version = "1.0.1"
+version = "1.1.0"
 description = "A persistent cache for python requests"
 authors = ["Roman Haritonov", "Jordan Cook"]
 license = "BSD-2-Clause"
 readme = "README.md"
 documentation = "https://requests-cache.readthedocs.io"
 homepage = "https://github.com/requests-cache/requests-cache"
 repository = "https://github.com/requests-cache/requests-cache"
@@ -49,15 +49,15 @@
 bson                       = {optional=true, version=">=0.5"}
 itsdangerous               = {optional=true, version=">=2.0"}
 pyyaml                     = {optional=true, version=">=5.4"}
 ujson                      = {optional=true, version=">=5.4"}
 
 # Dependencies for building documentation;
 # defined here because readthedocs doesn't (yet?) support poetry.dev-dependencies
-furo                       = {optional=true, version="^2022.12.7"}
+furo                       = {optional=true, version="^2023.3"}
 linkify-it-py              = {optional=true, version="^2.0"}
 myst-parser                = {optional=true, version="^1.0"}
 sphinx                     = {optional=true, version="^5.0.2"}
 sphinx-autodoc-typehints   = {optional=true, version=">=1.19"}
 sphinx-automodapi          = {optional=true, version=">=0.14"}
 sphinx-copybutton          = {optional=true, version=">=0.5"}
 sphinx-design              = {optional=true, version=">=0.2"}
@@ -85,29 +85,30 @@
             "sphinx-automodapi", "sphinx-copybutton", "sphinx-design", "sphinx-notfound-page",
             "sphinxcontrib-apidoc", "sphinxext-opengraph"]
 
 [tool.poetry.dev-dependencies]
 # For unit + integration tests
 coverage              = "^7.1"
 psutil                = "^5.0"
-pytest                = "^7.2"
+pytest                = "^7.3"
 pytest-clarity        = "^1.0.1"
 pytest-cov            = ">=3.0"
 pytest-rerunfailures  = "^10.1"
 pytest-xdist          = ">=2.2"
 requests-mock         = "^1.9"
 responses             = "0.19.0"
 tenacity              = "^8.0"
 timeout-decorator     = "^0.5"
+time-machine          = {version = "^2.9", markers = "implementation_name != 'pypy'"}
 
 # Tools for linting, type checking, etc. are managed with pre-commit
 pre-commit            = "^2.19"
 
 # For convenience in local development
-nox                   = "^2022.1.7"
+nox                   = "^2023.4"
 nox-poetry            = "^1.0.0"
 rich                  = ">=10.0"
 sphinx-autobuild      = "^2021.3.14"
 
 # Workaround for missing dependency on python 3.7
 zipp                  = {version = ">=3.8", python = "<3.8"}
 
@@ -151,7 +152,14 @@
     'examples/',
     'tests/compat/',
 ]
 known_first_party = ['tests']
 
 [tool.mypy]
 ignore_missing_imports = true
+
+
+[tool.ruff]
+format = 'grouped'
+line-length = 120
+select = ['B', 'C4','C90', 'E', 'F']
+ignore = ['B023']
```

### Comparing `requests_cache-1.0.1/requests_cache/_utils.py` & `requests_cache-1.1.0/requests_cache/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Minor internal utility functions that don't really belong anywhere else"""
+from contextlib import contextmanager
 from inspect import signature
 from logging import getLogger
 from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Tuple
 
+from urllib3 import filepost
+
 KwargDict = Dict[str, Any]
 logger = getLogger('requests_cache')
 
 
 def chunkify(iterable: Optional[Iterable], max_size: int) -> Iterator[List]:
     """Split an iterable into chunks of a max size"""
     iterable = list(iterable or [])
@@ -62,14 +65,26 @@
     func: Callable, kwargs: Dict, extras: Optional[Iterable[str]] = None
 ) -> KwargDict:
     """Get the subset of non-None ``kwargs`` that are valid arguments for ``func``"""
     kwargs, _ = split_kwargs(func, kwargs, extras)
     return {k: v for k, v in kwargs.items() if v is not None}
 
 
+@contextmanager
+def patch_form_boundary():
+    """If the ``files`` param is present, patch the form boundary used to separate multipart
+    uploads. ``requests`` does not provide a way to pass a custom boundary to urllib3, so this just
+    monkey-patches it instead.
+    """
+    original_boundary = filepost.choose_boundary
+    filepost.choose_boundary = lambda: '##requests-cache-form-boundary##'
+    yield
+    filepost.choose_boundary = original_boundary
+
+
 def split_kwargs(
     func: Callable, kwargs: Dict, extras: Optional[Iterable[str]] = None
 ) -> Tuple[KwargDict, KwargDict]:
     """Split ``kwargs`` into two dicts: those that are valid arguments for ``func``,  and those that
     are not
     """
     params = list(signature(func).parameters)
```

### Comparing `requests_cache-1.0.1/requests_cache/backends/__init__.py` & `requests_cache-1.1.0/requests_cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/backends/base.py` & `requests_cache-1.1.0/requests_cache/backends/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,16 +85,19 @@
             response: Response to save
             expires: Absolute expiration time for this response
         """
         cache_key = cache_key or self.create_key(response.request)
         cached_response = CachedResponse.from_response(response, expires=expires)
         cached_response = redact_response(cached_response, self._settings.ignored_parameters)
         self.responses[cache_key] = cached_response
-        for r in response.history:
-            self.redirects[self.create_key(r.request)] = cache_key
+
+        # Save redirect aliases, unless this is a revalidation (i.e., it was saved previously)
+        if response.history and not cached_response.revalidated:
+            for r in response.history:
+                self.redirects[self.create_key(r.request)] = cache_key
 
     def clear(self):
         """Delete all items from the cache"""
         logger.info('Clearing all items from the cache')
         self.responses.clear()
         self.redirects.clear()
 
@@ -224,14 +227,17 @@
     def recreate_keys(self):
         """Recreate cache keys for all previously cached responses"""
         logger.debug('Recreating all cache keys')
         old_keys = list(self.responses.keys())
 
         for old_cache_key in old_keys:
             response = self.responses[old_cache_key]
+            # Adjust empty request body for reponses cached before 1.0
+            if response.request.body == b'None':
+                response.request.body = b''
             new_cache_key = self.create_key(response.request)
             if new_cache_key != old_cache_key:
                 self.responses[new_cache_key] = response
                 del self.responses[old_cache_key]
 
     def reset_expiration(self, expire_after: ExpirationTime = None):
         """Set a new expiration value to set on existing cache items
@@ -271,74 +277,82 @@
     # (or could be kept indefinitely if someone really needs them)
     # --------------------
 
     def delete_url(self, url: str, method: str = 'GET', **kwargs):
         warn(
             'BaseCache.delete_url() is deprecated; please use .delete(urls=...) instead',
             DeprecationWarning,
+            stacklevel=2,
         )
         self.delete(requests=[Request(method, url, **kwargs)])
 
     def delete_urls(self, urls: Iterable[str], method: str = 'GET', **kwargs):
         warn(
             'BaseCache.delete_urls() is deprecated; please use .delete(urls=...) instead',
             DeprecationWarning,
+            stacklevel=2,
         )
         self.delete(requests=[Request(method, url, **kwargs) for url in urls])
 
     def has_key(self, key: str) -> bool:
         warn(
             'BaseCache.has_key() is deprecated; please use .contains() instead',
             DeprecationWarning,
+            stacklevel=2,
         )
         return self.contains(key)
 
     def has_url(self, url: str, method: str = 'GET', **kwargs) -> bool:
         warn(
             'BaseCache.has_url() is deprecated; please use .contains(url=...) instead',
             DeprecationWarning,
+            stacklevel=2,
         )
         return self.contains(request=Request(method, url, **kwargs))
 
     def keys(self, check_expiry: bool = False) -> Iterator[str]:
         warn(
             'BaseCache.keys() is deprecated; '
             'please use .filter() or BaseCache.responses.keys() instead',
             DeprecationWarning,
+            stacklevel=2,
         )
         yield from self.redirects.keys()
         if not check_expiry:
             yield from self.responses.keys()
         else:
             for response in self.filter(expired=False):
                 yield response.cache_key
 
     def response_count(self, check_expiry: bool = False) -> int:
         warn(
             'BaseCache.response_count() is deprecated; '
             'please use .filter() or len(BaseCache.responses) instead',
             DeprecationWarning,
+            stacklevel=2,
         )
         return len(list(self.filter(expired=not check_expiry)))
 
     def remove_expired_responses(self, expire_after: ExpirationTime = None):
         warn(
             'BaseCache.remove_expired_responses() is deprecated; '
             'please use .delete(expired=True) instead',
             DeprecationWarning,
+            stacklevel=2,
         )
         if expire_after:
             self.reset_expiration(expire_after)
         self.delete(expired=True, invalid=True)
 
     def values(self, check_expiry: bool = False) -> Iterator[CachedResponse]:
         warn(
             'BaseCache.values() is deprecated; '
             'please use .filter() or BaseCache.responses.values() instead',
             DeprecationWarning,
+            stacklevel=2,
         )
         yield from self.filter(expired=not check_expiry)
 
 
 KT = TypeVar('KT')
 VT = TypeVar('VT')
```

### Comparing `requests_cache-1.0.1/requests_cache/backends/dynamodb.py` & `requests_cache-1.1.0/requests_cache/backends/dynamodb.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/backends/filesystem.py` & `requests_cache-1.1.0/requests_cache/backends/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ):
         super().__init__(cache_name=str(cache_name), **kwargs)
         skwargs = {'serializer': serializer, **kwargs} if serializer else kwargs
         self.responses: FileDict = FileDict(
             cache_name, use_temp=use_temp, decode_content=decode_content, **skwargs
         )
         self.redirects: SQLiteDict = SQLiteDict(
-            self.cache_dir / 'redirects.sqlite', 'redirects', no_serializer=True, **kwargs
+            self.cache_dir / 'redirects.sqlite', 'redirects', serializer=None, **kwargs
         )
 
     @property
     def cache_dir(self) -> Path:
         """Base directory for cache files"""
         return Path(self.responses.cache_dir)
 
@@ -90,15 +90,15 @@
     def _try_io(self, ignore_errors: bool = False):
         """Attempt an I/O operation, and either ignore errors or re-raise them as KeyErrors"""
         try:
             with self._lock:
                 yield
         except (EOFError, IOError, OSError, PickleError) as e:
             if not ignore_errors:
-                raise KeyError(e)
+                raise KeyError from e
 
     def _path(self, key) -> Path:
         return self.cache_dir / f'{key}{self.extension}'
 
     def __getitem__(self, key):
         mode = 'rb' if self.is_binary else 'r'
         with self._try_io():
```

### Comparing `requests_cache-1.0.1/requests_cache/backends/gridfs.py` & `requests_cache-1.1.0/requests_cache/backends/gridfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             with self._lock:
                 result = self.fs.find_one({'_id': key})
                 if result is None:
                     raise KeyError
                 return self.deserialize(key, result.read())
         except CorruptGridFile as e:
             logger.warning(e, exc_info=True)
-            raise KeyError
+            raise KeyError from e
 
     def __setitem__(self, key, item):
         value = self.serialize(item)
         encoding = None if isinstance(value, bytes) else 'utf-8'
 
         with self._lock:
             try:
```

### Comparing `requests_cache-1.0.1/requests_cache/backends/mongodb.py` & `requests_cache-1.1.0/requests_cache/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/backends/redis.py` & `requests_cache-1.1.0/requests_cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/backends/sqlite.py` & `requests_cache-1.1.0/requests_cache/backends/sqlite.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,40 +8,45 @@
 import threading
 from contextlib import contextmanager
 from logging import getLogger
 from os import unlink
 from os.path import getsize, isfile
 from pathlib import Path
 from tempfile import gettempdir
-from time import time
+from time import sleep, time
 from typing import Collection, Iterator, List, Optional, Tuple, Type, Union
 
 from platformdirs import user_cache_dir
 
 from .._utils import chunkify, get_valid_kwargs
 from ..models.response import CachedResponse
 from ..policy import ExpirationTime
 from ..serializers import SerializerType, pickle_serializer
 from . import BaseCache, BaseStorage
 from .base import VT
 
 MEMORY_URI = 'file::memory:?cache=shared'
 SQLITE_MAX_VARIABLE_NUMBER = 999
+DEFAULT_WRITE_RETRIES = 3
+
 AnyPath = Union[Path, str]
 logger = getLogger(__name__)
 
 
 class SQLiteCache(BaseCache):
     """SQLite cache backend.
 
     Args:
         db_path: Database file path
         use_cache_dir: Store datebase in a user cache directory (e.g., `~/.cache/http_cache.sqlite`)
         use_temp: Store database in a temp directory (e.g., ``/tmp/http_cache.sqlite``)
         use_memory: Store database in memory instead of in a file
+        busy_timeout: Timeout in milliseconds for SQLite to wait if a table is locked.
+            See `pragma: busy_timeout <https://www.sqlite.org/pragma.html#pragma_busy_timeout>`_
+            for details.
         fast_save: Significantly increases cache write performance, but with the possibility of data
             loss. See `pragma: synchronous <https://www.sqlite.org/pragma.html#pragma_synchronous>`_
             for details.
         wal: Use `Write Ahead Logging <https://sqlite.org/wal.html>`_, so readers do not block writers.
         kwargs: Additional keyword arguments for :py:func:`sqlite3.connect`
     """
 
@@ -52,15 +57,19 @@
         **kwargs,
     ):
         super().__init__(cache_name=str(db_path), **kwargs)
         # Only override serializer if a non-None value is specified
         skwargs = {'serializer': serializer, **kwargs} if serializer else kwargs
         self.responses: SQLiteDict = SQLiteDict(db_path, table_name='responses', **skwargs)
         self.redirects: SQLiteDict = SQLiteDict(
-            db_path, table_name='redirects', serializer=None, **kwargs
+            db_path,
+            table_name='redirects',
+            lock=self.responses._lock,
+            serializer=None,
+            **kwargs,
         )
 
     @property
     def db_path(self) -> AnyPath:
         return self.responses.db_path
 
     def clear(self):
@@ -86,25 +95,25 @@
         if keys:
             self.responses.bulk_delete(keys)
         if expired:
             self._delete_expired()
 
         # For any remaining conditions, use base implementation
         if kwargs:
-            with self.responses._lock, self.redirects._lock:
+            with self.responses._lock:
                 return super().delete(**kwargs)
         else:
             self._prune_redirects()
 
         self.responses.vacuum()
         self.redirects.vacuum()
 
     def _delete_expired(self):
         """A more efficient implementation of deleting expired responses in SQL"""
-        with self.responses.connection(commit=True) as con:
+        with self.responses._lock, self.responses.connection(commit=True) as con:
             con.execute(
                 f'DELETE FROM {self.responses.table_name} WHERE expires <= ?', (round(time()),)
             )
 
     def _prune_redirects(self):
         """A more efficient implementation of removing invalid redirects in SQL"""
         with self.redirects.connection(commit=True) as conn:
@@ -165,34 +174,39 @@
 
 
 class SQLiteDict(BaseStorage):
     """A dictionary-like interface for SQLite"""
 
     def __init__(
         self,
-        db_path,
-        table_name='http_cache',
-        fast_save=False,
+        db_path: AnyPath,
+        table_name: str = 'http_cache',
+        busy_timeout: Optional[int] = None,
+        fast_save: bool = False,
+        retries: Optional[int] = DEFAULT_WRITE_RETRIES,
         serializer: Optional[SerializerType] = pickle_serializer,
         use_cache_dir: bool = False,
         use_memory: bool = False,
         use_temp: bool = False,
         wal: bool = False,
         **kwargs,
     ):
         super().__init__(serializer=serializer, **kwargs)
         self._can_commit = True
         self._connection: Optional[sqlite3.Connection] = None
-        self._lock = threading.RLock()
+        self._lock = kwargs.pop('lock', threading.RLock())
         self.connection_kwargs = get_valid_kwargs(sqlite_template, kwargs)
         self.connection_kwargs.setdefault('check_same_thread', False)
         if use_memory:
             self.connection_kwargs['uri'] = True
         self.db_path = _get_sqlite_cache_path(db_path, use_cache_dir, use_temp, use_memory)
+        self.busy_timeout = busy_timeout
         self.fast_save = fast_save
+        # Provisional option: number of times to retry writing if db is locked. Set to 0 to disable.
+        self.retries = retries
         self.table_name = table_name
         self.wal = wal
         self.init_db()
 
     def init_db(self):
         """Initialize the database, if it hasn't already been"""
         self.close()
@@ -211,35 +225,44 @@
                 ')'
             )
             con.execute(f'CREATE INDEX IF NOT EXISTS expires_idx ON {self.table_name}(expires)')
 
     @contextmanager
     def connection(self, commit=False) -> Iterator[sqlite3.Connection]:
         """Get a thread-local database connection"""
-        if not self._connection:
-            logger.debug(f'Opening connection to {self.db_path}:{self.table_name}')
-            self._connection = sqlite3.connect(self.db_path, **self.connection_kwargs)
-            if self.fast_save:
-                self._connection.execute('PRAGMA synchronous = 0;')
-            if self.wal:
-                self._connection.execute('PRAGMA journal_mode = wal')
+        with self._lock:
+            if not self._connection:
+                logger.debug(f'Opening connection to {self.db_path}:{self.table_name}')
+                self._connection = sqlite3.connect(self.db_path, **self.connection_kwargs)
+                # Note: DBAPI doesn't support integer placeholders
+                if self.busy_timeout is not None:
+                    self._connection.execute(f'PRAGMA busy_timeout={self.busy_timeout}')
+                if self.fast_save:
+                    self._connection.execute('PRAGMA synchronous=OFF')
+                if self.wal:
+                    self._connection.execute('PRAGMA journal_mode=WAL')
+                # In WAL mode, default to normal sync mode (best balance between safety/performance)
+                if self.wal and not self.fast_save:
+                    self._connection.execute('PRAGMA synchronous=NORMAL')
 
-        # Any write operations need to be run in serial
-        if commit and self._can_commit:
-            self._lock.acquire()
-        yield self._connection
+        # Multithreaded write operations must be run in serial
         if commit and self._can_commit:
-            self._connection.commit()
-            self._lock.release()
+            with self._lock:
+                yield self._connection
+                self._connection.commit()
+        # Read operations can be run in parallel (no lock or COMMIT)
+        else:
+            yield self._connection
 
     def close(self):
         """Close any active connections"""
-        if self._connection:
-            self._connection.close()
-            self._connection = None
+        with self._lock:
+            if self._connection:
+                self._connection.close()
+                self._connection = None
 
     @contextmanager
     def bulk_commit(self):
         """Insert a large number of records within a single transaction
 
         Example:
 
@@ -264,22 +287,47 @@
         with self.connection(commit=True) as con:
             cur = con.execute(f'DELETE FROM {self.table_name} WHERE key=?', (key,))
         if not cur.rowcount:
             raise KeyError
 
     def __getitem__(self, key):
         with self.connection() as con:
-            row = con.execute(f'SELECT value FROM {self.table_name} WHERE key=?', (key,)).fetchone()
-        # raise error after the with block, otherwise the connection will be locked
-        if not row:
-            raise KeyError
+            cur = con.execute(f'SELECT value FROM {self.table_name} WHERE key=?', (key,))
+            row = cur.fetchone()
+            cur.close()
+            if not row:
+                raise KeyError(key)
 
-        return self.deserialize(key, row[0])
+            return self.deserialize(key, row[0])
 
     def __setitem__(self, key, value):
+        if not self.retries:
+            self._write(key, value)
+            return
+
+        for i in range(self.retries):
+            try:
+                self._write(key, value)
+                return
+            # Even with WAL mode, rarely a write may fail with SQLITE_BUSY; if so, retry up to
+            # self._retries times. Any other errors will be re-raised.
+            except sqlite3.OperationalError as e:
+                if 'database is locked' not in str(e):
+                    raise
+                elif i < self.retries - 1:
+                    logger.warning(
+                        f'Database is locked in thread {threading.get_ident()}; '
+                        f'retrying ({i+1}/{self.retries})'
+                    )
+                    sleep(0.1)
+                # On last retry, log the error and abort the write
+                else:
+                    logger.error(e)
+
+    def _write(self, key, value):
         # If available, set expiration as a timestamp in unix format
         expires = getattr(value, 'expires_unix', None)
         value = self.serialize(value)
         with self.connection(commit=True) as con:
             con.execute(
                 f'INSERT OR REPLACE INTO {self.table_name} (key,value,expires) VALUES (?,?,?)',
                 (key, value, expires),
@@ -297,15 +345,15 @@
         """Delete multiple items from the cache, without raising errors for any missing items.
         Supports deleting by either key or by value.
         """
         if not keys and not values:
             return
 
         column = 'key' if keys else 'value'
-        with self.connection(commit=True) as con:
+        with self._lock, self.connection(commit=True) as con:
             # Split into small enough chunks for SQLite to handle
             for chunk in chunkify(keys or values, max_size=SQLITE_MAX_VARIABLE_NUMBER):
                 marks, args = _format_sequence(chunk)
                 statement = f'DELETE FROM {self.table_name} WHERE {column} IN ({marks})'
                 con.execute(statement, args)
 
     def clear(self):
@@ -422,15 +470,15 @@
     db_path = db_path.expanduser().absolute()
     try:
         db_path.parent.mkdir(parents=True, exist_ok=True)
     except FileExistsError:
         raise FileExistsError(
             f'Parent path exists and is not a directory: {db_path.parent}.'
             'Please either delete the file or choose a different path.'
-        )
+        ) from None
     return db_path
 
 
 def sqlite_template(
     timeout: float = 5.0,
     detect_types: int = 0,
     isolation_level: Optional[str] = None,
```

### Comparing `requests_cache-1.0.1/requests_cache/cache_keys.py` & `requests_cache-1.1.0/requests_cache/cache_keys.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .. automodsumm:: requests_cache.cache_keys
    :functions-only:
    :nosignatures:
 """
 from __future__ import annotations
 
 import json
+from contextlib import nullcontext
 from hashlib import blake2b
 from logging import getLogger
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
@@ -23,15 +24,15 @@
 )
 from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 
 from requests import Request, Session
 from requests.models import CaseInsensitiveDict
 from url_normalize import url_normalize
 
-from ._utils import decode, encode
+from ._utils import decode, encode, patch_form_boundary
 
 __all__ = [
     'create_key',
     'normalize_body',
     'normalize_headers',
     'normalize_request',
     'normalize_params',
@@ -110,15 +111,18 @@
     * Redacting potentially sensitive info from cached requests
 
     Args:
         request: Request object to normalize
         ignored_parameters: Request paramters, headers, and/or JSON body params to exclude
     """
     if isinstance(request, Request):
-        norm_request: AnyPreparedRequest = Session().prepare_request(request)
+        # For a multipart POST request that hasn't been prepared, we need to patch the form boundary
+        # so the request body will have a consistent hash
+        with patch_form_boundary() if request.files else nullcontext():
+            norm_request: AnyPreparedRequest = Session().prepare_request(request)
     else:
         norm_request = request.copy()
 
     norm_request.method = (norm_request.method or '').upper()
     norm_request.url = normalize_url(norm_request.url or '', ignored_parameters)
     norm_request.headers = normalize_headers(norm_request.headers, ignored_parameters)
     norm_request.body = normalize_body(norm_request, ignored_parameters)
@@ -138,27 +142,15 @@
     return CaseInsensitiveDict(headers)
 
 
 def normalize_url(url: str, ignored_parameters: ParamList) -> str:
     """Normalize and filter a URL. This includes request parameters, IDN domains, scheme, host,
     port, etc.
     """
-    # Strip query params from URL, sort and filter, and reassemble into a complete URL
-    url_tokens = urlparse(url)
-    url = urlunparse(
-        (
-            url_tokens.scheme,
-            url_tokens.netloc,
-            url_tokens.path,
-            url_tokens.params,
-            normalize_params(url_tokens.query, ignored_parameters),
-            url_tokens.fragment,
-        )
-    )
-
+    url = filter_url(url, ignored_parameters)
     return url_normalize(url)
 
 
 def normalize_body(request: AnyPreparedRequest, ignored_parameters: ParamList) -> bytes:
     """Normalize and filter a request body if possible, depending on Content-Type"""
     if not request.body:
         return b''
@@ -206,15 +198,15 @@
 
     return query_str
 
 
 def redact_response(response: CachedResponse, ignored_parameters: ParamList) -> CachedResponse:
     """Redact any ignored parameters (potentially containing sensitive info) from a cached request"""
     if ignored_parameters:
-        response.url = normalize_url(response.url, ignored_parameters)
+        response.url = filter_url(response.url, ignored_parameters)
         response.request = normalize_request(response.request, ignored_parameters)  # type: ignore
     return response
 
 
 def filter_sort_json(data: Union[List, Mapping], ignored_parameters: ParamList):
     if isinstance(data, Mapping):
         return filter_sort_dict(data, ignored_parameters)
@@ -236,7 +228,23 @@
     return [(k, 'REDACTED' if k in ignored_parameters else v) for k, v in sorted(data)]
 
 
 def filter_sort_list(data: List, ignored_parameters: ParamList = None) -> List:
     if not ignored_parameters:
         return sorted(data)
     return [k for k in sorted(data) if k not in set(ignored_parameters)]
+
+
+def filter_url(url: str, ignored_parameters: ParamList) -> str:
+    """Filter ignored parameters out of a URL"""
+    # Strip query params from URL, sort and filter, and reassemble into a complete URL
+    url_tokens = urlparse(url)
+    return urlunparse(
+        (
+            url_tokens.scheme,
+            url_tokens.netloc,
+            url_tokens.path,
+            url_tokens.params,
+            normalize_params(url_tokens.query, ignored_parameters),
+            url_tokens.fragment,
+        )
+    )
```

### Comparing `requests_cache-1.0.1/requests_cache/models/base.py` & `requests_cache-1.1.0/requests_cache/models/base.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/models/raw_response.py` & `requests_cache-1.1.0/requests_cache/models/raw_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     """
 
     decode_content: bool = field(default=None)
     headers: HTTPHeaderDict = field(factory=HTTPHeaderDict)
     reason: str = field(default=None)
     request_url: str = field(default=None)
     status: int = field(default=0)
-    strict: int = field(default=0)
     version: int = field(default=0)
 
     def __init__(self, body: Optional[bytes] = None, **kwargs):
         """First initialize via HTTPResponse, then via attrs"""
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         super().__init__(body=BytesIO(body or b''), preload_content=False, **kwargs)
         self._body = body
@@ -48,25 +47,35 @@
     def from_response(cls, response: Response) -> 'CachedHTTPResponse':
         """Create a CachedHTTPResponse based on an original response"""
         # Copy basic attributes
         raw = response.raw
         kwargs = {k: getattr(raw, k, None) for k in fields_dict(cls).keys()}
         kwargs['request_url'] = raw._request_url
 
-        # Copy response data and restore response object to its original state
+        # Read and copy raw response data, and then restore response object to its previous state
+        # This is necessary so streaming responses behave consistently with or without the cache
         if getattr(raw, '_fp', None) and not is_fp_closed(raw._fp):
-            body = raw.read(decode_content=False)
-            kwargs['body'] = body
-            raw._fp = BytesIO(body)
-            response.content  # This property reads, decodes, and stores response content
-
-            # After reading, reset file pointer on original raw response
-            raw._fp = BytesIO(body)
-            raw._fp_bytes_read = 0
-            raw.length_remaining = len(body)
+            # Body has already been read & decoded by requests
+            if getattr(raw, '_has_decoded_content', False):
+                body = response.content
+                kwargs['body'] = body
+                raw._fp = BytesIO(body)
+                raw._fp_bytes_read = 0
+                raw.length_remaining = len(body)
+            # Body has not yet been read
+            else:
+                body = raw.read(decode_content=False)
+                kwargs['body'] = body
+                raw._fp = BytesIO(body)
+                _ = response.content  # This property reads, decodes, and stores response content
+
+                # After reading, reset file pointer on original raw response
+                raw._fp = BytesIO(body)
+                raw._fp_bytes_read = 0
+                raw.length_remaining = len(body)
 
         return cls(**kwargs)  # type: ignore  # False positive in mypy 0.920+?
 
     @classmethod
     def from_cached_response(cls, response: 'CachedResponse'):
         """Create a CachedHTTPResponse based on a cached response"""
         obj = cls(
```

### Comparing `requests_cache-1.0.1/requests_cache/models/request.py` & `requests_cache-1.1.0/requests_cache/models/request.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/models/response.py` & `requests_cache-1.1.0/requests_cache/models/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ..policy import ExpirationTime, get_expiration_datetime
 from . import CachedHTTPResponse, CachedRequest, RichMixin
 
 if TYPE_CHECKING:
     from ..policy.actions import CacheActions
 
 DATETIME_FORMAT = '%Y-%m-%d %H:%M:%S %Z'  # Format used for __str__ only
-DecodedContent = Union[Dict, str, None]
+DecodedContent = Union[Dict, List, str, None]
 logger = getLogger(__name__)
 
 
 @define(auto_attribs=False, repr=False, slots=False)
 class BaseResponse(Response):
     """Wrapper class for responses returned by :py:class:`.CachedSession`. This mainly exists to
     provide type hints for extra cache-related attributes that are added to non-cached responses.
```

### Comparing `requests_cache-1.0.1/requests_cache/patcher.py` & `requests_cache-1.1.0/requests_cache/patcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 
 
 def remove_expired_responses():
     """Remove expired responses from the cache"""
     warn(
         'remove_expired_responses() is deprecated; please use delete() instead',
         DeprecationWarning,
+        stacklevel=2,
     )
     delete(expired=True)
 
 
 def _patch_session_factory(session_factory: Type[OriginalSession] = CachedSession):
     logger.debug(f'Patching requests.Session with class: {session_factory.__name__}')
     requests.Session = requests.sessions.Session = session_factory  # type: ignore
```

### Comparing `requests_cache-1.0.1/requests_cache/policy/__init__.py` & `requests_cache-1.1.0/requests_cache/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/policy/actions.py` & `requests_cache-1.1.0/requests_cache/policy/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,14 +239,22 @@
         return request
 
     def update_revalidated_response(
         self, response: Response, cached_response: 'CachedResponse'
     ) -> 'CachedResponse':
         """After revalidation, update the cached response's expiration and headers"""
         logger.debug(f'Response for URL {response.request.url} has not been modified')
+
+        # Skip updating the cached response if expiration and headers are unchanged
+        # Ignore validators missing from new response, since they may be omitted
+        headers_changed = any(
+            cached_response.headers.get(k) != v for k, v in response.headers.items()
+        )
+        self.skip_write = self.expires == cached_response.expires and not headers_changed
+
         cached_response.expires = self.expires
         cached_response.headers.update(response.headers)
         cached_response.revalidated = True
         return cached_response
 
     def _update_from_response_headers(self, directives: CacheDirectives):
         """Check response headers for expiration and other cache directives"""
@@ -292,17 +300,23 @@
         """If the cached response contains Vary, check that the specified request headers match"""
         vary = cached_response.headers.get('Vary')
         if not vary:
             return True
         elif vary == '*':
             return False
 
-        # Generate a secondary cache key based on Vary for both the cached request and new request
+        # Generate a secondary cache key based on Vary for both the cached request and new request.
+        # If there are redirects, compare the new request against the last request in the chain.
         key_kwargs['match_headers'] = [k.strip() for k in vary.split(',')]
-        vary_cache_key = create_key(cached_response.request, **key_kwargs)
+        vary_request = (
+            cached_response.history[-1].request
+            if cached_response.history
+            else cached_response.request
+        )
+        vary_cache_key = create_key(vary_request, **key_kwargs)
         headers_match = create_key(self._request, **key_kwargs) == vary_cache_key
         if not headers_match:
             _log_vary_diff(
                 self._request.headers, cached_response.request.headers, key_kwargs['match_headers']
             )
         return headers_match
```

### Comparing `requests_cache-1.0.1/requests_cache/policy/directives.py` & `requests_cache-1.1.0/requests_cache/policy/directives.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/policy/expiration.py` & `requests_cache-1.1.0/requests_cache/policy/expiration.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/policy/settings.py` & `requests_cache-1.1.0/requests_cache/policy/settings.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/serializers/__init__.py` & `requests_cache-1.1.0/requests_cache/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/serializers/cattrs.py` & `requests_cache-1.1.0/requests_cache/serializers/cattrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,27 +105,36 @@
     # Convert dict-like objects to and from plain dicts
     converter.register_unstructure_hook(RequestsCookieJar, lambda obj: dict(obj.items()))
     converter.register_structure_hook(RequestsCookieJar, lambda obj, cls: cookiejar_from_dict(obj))
     converter.register_unstructure_hook(CaseInsensitiveDict, dict)
     converter.register_structure_hook(
         CaseInsensitiveDict, lambda obj, cls: CaseInsensitiveDict(obj)
     )
-    # Convert decoded JSON body back to string
+
+    # Convert decoded JSON body back to a string. If the object is a valid JSON root (dict or list),
+    # that means it was previously saved in human-readable format due to `decode_content=True`.
+    # After this hook runs, the body will also be re-encoded with `_encode_content()`.
     converter.register_structure_hook(
-        DecodedContent, lambda obj, cls: json.dumps(obj) if isinstance(obj, dict) else obj
+        DecodedContent, lambda obj, cls: json.dumps(obj) if isinstance(obj, (dict, list)) else obj
     )
 
+    def structure_fwd_ref(obj, cls):
+        # python<=3.8: ForwardRef may not have been evaluated yet
+        if not cls.__forward_evaluated__:  # pragma: no cover
+            cls._evaluate(globals(), locals())
+        return converter.structure(obj, cls.__forward_value__)
+
     # Resolve forward references (required for CachedResponse.history)
     converter.register_unstructure_hook_func(
         lambda cls: cls.__class__ is ForwardRef,
         lambda obj, cls=None: converter.unstructure(obj, cls.__forward_value__ if cls else None),
     )
     converter.register_structure_hook_func(
         lambda cls: cls.__class__ is ForwardRef,
-        lambda obj, cls: converter.structure(obj, cls.__forward_value__),
+        structure_fwd_ref,
     )
 
     return converter
 
 
 def make_decimal_timedelta_converter(**kwargs) -> Converter:
     """Make a converter that uses Decimals instead of floats to represent timedelta objects"""
@@ -153,15 +162,17 @@
         response_dict.pop('_content', None)
 
     # Otherwise, it is most likely a binary body
     return response_dict
 
 
 def _encode_content(response: CachedResponse) -> CachedResponse:
-    """Re-encode response body if saved as JSON or text; has no effect for a binary response body"""
+    """Re-encode response body if saved as JSON or text (via ``decode_content=True``).
+    This has no effect for a binary response body.
+    """
     if isinstance(response._decoded_content, str):
         response._content = response._decoded_content.encode('utf-8')
         response._decoded_content = None
         response.encoding = 'utf-8'  # Set encoding explicitly so requests doesn't have to guess
         response.headers['Content-Length'] = str(len(response._content))  # Size may have changed
     return response
```

### Comparing `requests_cache-1.0.1/requests_cache/serializers/pipeline.py` & `requests_cache-1.1.0/requests_cache/serializers/pipeline.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/serializers/preconf.py` & `requests_cache-1.1.0/requests_cache/serializers/preconf.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/requests_cache/session.py` & `requests_cache-1.1.0/requests_cache/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from logging import getLogger
 from threading import RLock, Thread
 from typing import TYPE_CHECKING, Iterable, MutableMapping, Optional, Union
 
 from requests import PreparedRequest
 from requests import Session as OriginalSession
 from requests.hooks import dispatch_hook
-from urllib3 import filepost
 
-from ._utils import get_valid_kwargs
+from ._utils import get_valid_kwargs, patch_form_boundary
 from .backends import BackendSpecifier, init_backend
 from .models import AnyResponse, CachedResponse, OriginalResponse
 from .policy import (
     DEFAULT_CACHE_NAME,
     DEFAULT_IGNORED_PARAMS,
     DEFAULT_METHODS,
     DEFAULT_STATUS_CODES,
@@ -230,15 +229,16 @@
         response = super().send(request, **kwargs)
         actions.update_from_response(response)
 
         if not actions.skip_write:
             self.cache.save_response(response, actions.cache_key, actions.expires)
         elif cached_response is not None and response.status_code == 304:
             cached_response = actions.update_revalidated_response(response, cached_response)
-            self.cache.save_response(cached_response, actions.cache_key, actions.expires)
+            if not actions.skip_write:
+                self.cache.save_response(cached_response, actions.cache_key, actions.expires)
             return cached_response
         else:
             logger.debug(f'Skipping cache write for URL: {request.url}')
         return OriginalResponse.wrap_response(response, actions)
 
     def _resend(
         self,
@@ -363,19 +363,7 @@
     """Get a 504: Not Cached error response, for use with only-if-cached option"""
     return CachedResponse(
         url=request.url or '',
         status_code=504,
         reason='Not Cached',
         request=request,  # type: ignore
     )
-
-
-@contextmanager
-def patch_form_boundary():
-    """If the ``files`` param is present, patch the form boundary used to separate multipart
-    uploads. ``requests`` does not provide a way to pass a custom boundary to urllib3, so this just
-    monkey-patches it instead.
-    """
-    original_boundary = filepost.choose_boundary
-    filepost.choose_boundary = lambda: '##requests-cache-form-boundary##'
-    yield
-    filepost.choose_boundary = original_boundary
```

### Comparing `requests_cache-1.0.1/tests/benchmark_serializers.py` & `requests_cache-1.1.0/tests/benchmark_serializers.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/compat/httpbin_sample.test-db` & `requests_cache-1.1.0/tests/compat/httpbin_sample.test-db`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/compat/test_requests_mock_combine_cache.py` & `requests_cache-1.1.0/tests/compat/test_requests_mock_combine_cache.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/compat/test_requests_mock_disable_cache.py` & `requests_cache-1.1.0/tests/compat/test_requests_mock_disable_cache.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/compat/test_requests_mock_load_cache.py` & `requests_cache-1.1.0/tests/compat/test_requests_mock_load_cache.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/compat/test_responses_load_cache.py` & `requests_cache-1.1.0/tests/compat/test_responses_load_cache.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/conftest.py` & `requests_cache-1.1.0/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Note: The protocol ``http(s)+mock://`` helps :py:class:`requests_mock.Adapter` play nicely with
 :py:class:`requests.PreparedRequest`. More info here:
 https://requests-mock.readthedocs.io/en/latest/adapter.html
 """
 import os
 import platform
 import warnings
-from contextlib import contextmanager
+from contextlib import contextmanager, nullcontext
 from datetime import datetime, timedelta
 from functools import wraps
 from importlib import import_module
 from logging import basicConfig, getLogger
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 from uuid import uuid4
@@ -26,14 +26,21 @@
 from requests_mock import ANY as ANY_METHOD
 from requests_mock import Adapter
 from rich.logging import RichHandler
 from timeout_decorator import timeout
 
 from requests_cache import ALL_METHODS, CachedSession, install_cache, uninstall_cache
 
+# ignore missing time-travel library on PyPy
+try:
+    from time_machine import travel as time_travel
+except ImportError:
+    time_travel = nullcontext
+
+
 # Configure logging to show log output when tests fail (or with pytest -s)
 basicConfig(
     level='INFO',
     format='%(message)s',
     datefmt='[%m-%d %H:%M:%S]',
     handlers=[RichHandler(rich_tracebacks=True, markup=True)],
 )
@@ -64,22 +71,27 @@
     'xml',
 ]
 HTTPDATE_STR = 'Fri, 16 APR 2021 21:13:00 GMT'
 HTTPDATE_DATETIME = datetime(2021, 4, 16, 21, 13)
 EXPIRED_DT = datetime.utcnow() - timedelta(1)
 ETAG = '"644b5b0155e6404a9cc4bd9d8b1ae730"'
 LAST_MODIFIED = 'Thu, 05 Jul 2012 15:31:30 GMT'
+START_DT = datetime.utcnow()
+YESTERDAY = datetime.utcnow() - timedelta(days=1)
 
 MOCKED_URL = 'http+mock://requests-cache.com/text'
 MOCKED_URL_ETAG = 'http+mock://requests-cache.com/etag'
 MOCKED_URL_HTTPS = 'https+mock://requests-cache.com/text'
 MOCKED_URL_JSON = 'http+mock://requests-cache.com/json'
+MOCKED_URL_JSON_LIST = 'http+mock://requests-cache.com/json_list'
 MOCKED_URL_REDIRECT = 'http+mock://requests-cache.com/redirect'
 MOCKED_URL_REDIRECT_TARGET = 'http+mock://requests-cache.com/redirect_target'
 MOCKED_URL_VARY = 'http+mock://requests-cache.com/vary'
+MOCKED_URL_VARY_REDIRECT = 'http+mock://requests-cache.com/vary-redirect'
+MOCKED_URL_VARY_REDIRECT_TARGET = 'http+mock://requests-cache.com/vary-redirect-target'
 MOCKED_URL_404 = 'http+mock://requests-cache.com/nonexistent'
 MOCKED_URL_500 = 'http+mock://requests-cache.com/answer?q=this-statement-is-false'
 MOCKED_URL_200_404 = 'http+mock://requests-cache.com/200-404'
 MOCK_PROTOCOLS = ['mock://', 'http+mock://', 'https+mock://']
 
 CACHE_NAME = 'pytest_cache'
 PROJECT_DIR = Path(__file__).parent.parent.absolute()
@@ -195,53 +207,78 @@
         MOCKED_URL_JSON,
         headers={'Content-Type': 'application/json'},
         json={'message': 'mock json response'},
         status_code=200,
     )
     adapter.register_uri(
         ANY_METHOD,
+        MOCKED_URL_JSON_LIST,
+        headers={'Content-Type': 'application/json'},
+        json=['item_1', 'item_2', {'message': 'mock json response'}],
+        status_code=200,
+    )
+    adapter.register_uri(
+        ANY_METHOD,
         MOCKED_URL_REDIRECT,
         headers={'Content-Type': 'text/plain', 'Location': MOCKED_URL_REDIRECT_TARGET},
-        text='mock redirect response',
+        text='mock redirect response (1/2)',
         status_code=302,
     )
     adapter.register_uri(
         ANY_METHOD,
         MOCKED_URL_REDIRECT_TARGET,
         headers={'Content-Type': 'text/plain'},
-        text='mock redirected response',
+        text='mock redirect response (2/2)',
         status_code=200,
     )
     adapter.register_uri(
         ANY_METHOD,
         MOCKED_URL_VARY,
         headers={'Content-Type': 'text/plain', 'Vary': 'Accept'},
         text='mock response with Vary header',
         status_code=200,
     )
+    adapter.register_uri(
+        ANY_METHOD,
+        MOCKED_URL_VARY_REDIRECT,
+        headers={
+            'Content-Type': 'text/plain',
+            'Vary': 'Accept',
+            'Location': MOCKED_URL_VARY_REDIRECT_TARGET,
+        },
+        text='mock redirect response with Vary header (1/2)',
+        status_code=302,
+    )
+    adapter.register_uri(
+        ANY_METHOD,
+        MOCKED_URL_VARY_REDIRECT_TARGET,
+        headers={'Content-Type': 'text/plain', 'Vary': 'Accept-Language'},
+        text='mock redirect response with Vary header (2/2)',
+        status_code=200,
+    )
     adapter.register_uri(ANY_METHOD, MOCKED_URL_404, status_code=404)
     adapter.register_uri(ANY_METHOD, MOCKED_URL_500, status_code=500)
     adapter.register_uri(
         ANY_METHOD, MOCKED_URL_200_404, [{"status_code": 200}, {"status_code": 404}]
     )
     return adapter
 
 
 def get_mock_response(
     method='GET',
     url='https://img.site.com/base/img.jpg',
     status_code=200,
-    headers={},
-    request_headers={},
+    headers=None,
+    request_headers=None,
 ):
     return MagicMock(
         url=url,
         status_code=status_code,
-        headers=headers,
-        request=Request(method=method, url=url, headers=request_headers),
+        headers=headers or {},
+        request=Request(method=method, url=url, headers=request_headers or {}),
     )
 
 
 def assert_delta_approx_equal(dt1: datetime, dt2: datetime, target_delta, threshold_seconds=2):
     """Assert that the given datetimes are approximately ``target_delta`` seconds apart"""
     diff_in_seconds = (dt2 - dt1).total_seconds()
     assert abs(diff_in_seconds - target_delta) <= threshold_seconds
```

### Comparing `requests_cache-1.0.1/tests/generate_test_db.py` & `requests_cache-1.1.0/tests/generate_test_db.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/integration/base_cache_test.py` & `requests_cache-1.1.0/tests/integration/base_cache_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,23 @@
     CACHE_NAME,
     ETAG,
     EXPIRED_DT,
     HTTPBIN_FORMATS,
     HTTPBIN_METHODS,
     HTTPDATE_STR,
     LAST_MODIFIED,
+    MOCKED_URL_JSON,
+    MOCKED_URL_JSON_LIST,
     N_ITERATIONS,
     N_REQUESTS_PER_ITERATION,
     N_WORKERS,
     USE_PYTEST_HTTPBIN,
     assert_delta_approx_equal,
     httpbin,
+    mount_mock_adapter,
     skip_pypy,
 )
 
 logger = getLogger(__name__)
 
 
 VALIDATOR_HEADERS = [{'ETag': ETAG}, {'Last-Modified': LAST_MODIFIED}]
@@ -248,46 +251,47 @@
             'send',
             return_value=MagicMock(status_code=304, headers=updated_response_headers),
         ):
             response = session.get(url, params=first_response_headers)
         assert response.from_cache is True
         assert response.is_expired is False
 
-        # Make sure an immediate subsequent request will be served from the cache for another max-age==60 secondss
-        try:
-            with patch.object(Session, 'send', side_effect=AssertionError):
-                response = session.get(url, params=first_response_headers)
-        except AssertionError:
-            assert False, (
-                "Session tried to perform re-validation although cached response should have been "
-                "refreshened."
-            )
+        # Make sure an immediate subsequent request will be served from the cache for another 60 seconds
+        with patch.object(Session, 'send', side_effect=AssertionError):
+            response = session.get(url, params=first_response_headers)
         assert response.from_cache is True
         assert response.is_expired is False
 
-    @pytest.mark.parametrize('stream', [True, False])
-    def test_response_decode(self, stream):
-        """Test that gzip-compressed raw responses (including streamed responses) can be manually
-        decompressed with decode_content=True
-        """
+    def test_decode_gzip_response(self):
+        """Test that gzip-compressed responses read decompressed content with decode_content=True"""
         session = self.init_session()
-        response = session.get(httpbin('gzip'), stream=stream)
+        response = session.get(httpbin('gzip'))
         assert b'gzipped' in response.content
-        if stream is True:
-            assert b'gzipped' in response.raw.read(None, decode_content=True)
         response.raw._fp = BytesIO(response.content)
 
         cached_response = CachedResponse.from_response(response)
         assert b'gzipped' in cached_response.content
-        assert b'gzipped' in cached_response.raw.read(None, decode_content=True)
+        assert b'gzipped' in cached_response.raw.read(amt=None, decode_content=True)
+
+    @pytest.mark.parametrize('decode_content', [True, False])
+    @pytest.mark.parametrize('url', [MOCKED_URL_JSON, MOCKED_URL_JSON_LIST])
+    def test_decode_json_response(self, decode_content, url):
+        """Test that JSON responses (with both dict and list root) are correctly returned from the
+        cache, regardless of `decode_content` setting"""
+        session = self.init_session(decode_content=decode_content)
+        session = mount_mock_adapter(session)
+
+        r1 = session.get(url)
+        r2 = session.get(url)
+        assert r1.json() == r2.json()
 
     def test_multipart_upload(self):
         session = self.init_session()
         session.post(httpbin('post'), files={'file1': BytesIO(b'10' * 1024)})
-        for i in range(5):
+        for _ in range(5):
             assert session.post(httpbin('post'), files={'file1': BytesIO(b'10' * 1024)}).from_cache
 
     def test_delete__expired(self):
         session = self.init_session(expire_after=1)
 
         # Populate the cache with several responses that should expire immediately
         for response_format in HTTPBIN_FORMATS:
@@ -300,15 +304,15 @@
         session.get(httpbin('redirect/3'), expire_after=-1)
         assert len(session.cache.redirects.keys()) == 4
         session.cache.delete(expired=True)
 
         assert len(session.cache.responses.keys()) == 2
         assert len(session.cache.redirects.keys()) == 3
         assert not session.cache.contains(url=httpbin('redirect/1'))
-        assert not any([session.cache.contains(url=httpbin(f)) for f in HTTPBIN_FORMATS])
+        assert not any(session.cache.contains(url=httpbin(f)) for f in HTTPBIN_FORMATS)
 
     @pytest.mark.parametrize('method', HTTPBIN_METHODS)
     def test_filter_request_headers(self, method):
         url = httpbin(method.lower())
         session = self.init_session(ignored_parameters=['Authorization'])
         response = session.request(method, url, headers={"Authorization": "<Secret Key>"})
         assert response.from_cache is False
```

### Comparing `requests_cache-1.0.1/tests/integration/base_storage_test.py` & `requests_cache-1.1.0/tests/integration/base_storage_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         caches = [self.init_cache(index=i) for i in range(10)]
         for i in range(self.num_instances):
             caches[i][f'key_{i}'] = f'value_{i}'
             caches[i][f'key_{i+1}'] = f'value_{i+1}'
 
         for i in range(self.num_instances):
             cache = caches[i]
-            cache[f'key_{i}'] == f'value_{i}'
+            assert cache[f'key_{i}'] == f'value_{i}'
             assert len(cache) == 2
             assert f'key_{i}' in cache and f'key_{i+1}' in cache
 
             del cache[f'key_{i}']
             assert f'key_{i}' not in cache
 
     def test_iterable_methods(self):
```

### Comparing `requests_cache-1.0.1/tests/integration/test_dynamodb.py` & `requests_cache-1.1.0/tests/integration/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/integration/test_filesystem.py` & `requests_cache-1.1.0/tests/integration/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/integration/test_memory.py` & `requests_cache-1.1.0/tests/integration/test_memory.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/integration/test_mongodb.py` & `requests_cache-1.1.0/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/integration/test_redis.py` & `requests_cache-1.1.0/tests/integration/test_redis.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/integration/test_sqlite.py` & `requests_cache-1.1.0/tests/integration/test_sqlite.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import pickle
+import sqlite3
 from datetime import datetime, timedelta
 from os.path import join
 from tempfile import NamedTemporaryFile, gettempdir
 from threading import Thread
 from unittest.mock import patch
 
 import pytest
@@ -130,28 +131,94 @@
         cache['key_2'] = 'value_2'
 
         cache = self.init_cache(clear=False)
         assert 2 not in cache
         assert cache._can_commit is True
 
     @skip_pypy
-    @pytest.mark.parametrize('kwargs', [{'fast_save': True}, {'wal': True}])
+    @pytest.mark.parametrize('kwargs', [{'busy_timeout': 5}, {'fast_save': True}, {'wal': True}])
     def test_pragma(self, kwargs):
         """Test settings that make additional PRAGMA statements"""
         cache_1 = self.init_cache('cache_1', **kwargs)
         cache_2 = self.init_cache('cache_2', **kwargs)
 
         n = 500
         for i in range(n):
             cache_1[f'key_{i}'] = f'value_{i}'
             cache_2[f'key_{i*2}'] = f'value_{i}'
 
         assert set(cache_1.keys()) == {f'key_{i}' for i in range(n)}
         assert set(cache_2.values()) == {f'value_{i}' for i in range(n)}
 
+    def test_busy_timeout(self):
+        cache = self.init_cache(busy_timeout=5)
+        with cache.connection() as con:
+            r = con.execute('PRAGMA busy_timeout').fetchone()
+            assert r[0] == 5
+
+    def test_wal_sync_mode(self):
+        # Should default to 'NORMAL' (1)
+        cache = self.init_cache(wal=True)
+        with cache.connection() as con:
+            r = con.execute('PRAGMA synchronous').fetchone()
+            assert r[0] == 1
+
+        # Not recommended, but should still work
+        cache = self.init_cache(wal=True, fast_save=True)
+        with cache.connection() as con:
+            r = con.execute('PRAGMA synchronous').fetchone()
+            assert r[0] == 0
+
+    def test_write_retry(self):
+        cache = self.init_cache()
+        locked_error = sqlite3.OperationalError('database is locked')
+        with patch.object(cache, '_write', side_effect=[locked_error, 1]) as mock_write:
+            cache['key_1'] = 'value_1'
+            assert mock_write.call_count == 2
+
+    def test_write_retry__exceeded_retries(self):
+        cache = self.init_cache()
+        locked_error = sqlite3.OperationalError('database is locked')
+
+        with patch.object(cache, '_write', side_effect=locked_error) as mock_write:
+            cache['key_1'] = 'value_1'
+            assert mock_write.call_count == 3
+            assert 'key_1' not in cache
+
+        # Set a custom number of retries
+        cache = self.init_cache(retries=5)
+        with patch.object(cache, '_write', side_effect=locked_error) as mock_write:
+            cache['key_1'] = 'value_1'
+            assert mock_write.call_count == 5
+
+        # Set retries to 0 to disable retrying
+        cache = self.init_cache(retries=0)
+        with patch.object(cache, '_write', side_effect=locked_error) as mock_write:
+            with pytest.raises(sqlite3.OperationalError):
+                cache['key_1'] = 'value_1'
+            assert mock_write.call_count == 1
+
+        # Expect no change to behavior if retrying is disabled and there are no errors
+        cache['key_1'] = 'value_1'
+        assert 'key_1' in cache
+
+    def test_write_retry__other_errors(self):
+        """Errors other than 'OperationalError: database is locked' should not be retried"""
+        cache = self.init_cache()
+
+        error_1 = sqlite3.OperationalError('no more rows available')
+        with patch.object(cache, '_write', side_effect=error_1):
+            with pytest.raises(sqlite3.OperationalError):
+                cache['key_1'] = 'value_1'
+
+        error_2 = sqlite3.DatabaseError('hard drive is on fire')
+        with patch.object(cache, '_write', side_effect=error_2):
+            with pytest.raises(sqlite3.DatabaseError):
+                cache['key_1'] = 'value_1'
+
     @skip_pypy
     @pytest.mark.parametrize('limit', [None, 50])
     def test_sorted__by_size(self, limit):
         cache = self.init_cache()
 
         # Insert items with decreasing size
         for i in range(100):
@@ -159,15 +226,15 @@
             cache[f'key_{i}'] = f'value_{i}_{suffix}'
 
         # Sorted items should be in ascending order by size
         items = list(cache.sorted(key='size'))
         assert len(items) == limit or 100
 
         prev_item = None
-        for i, item in enumerate(items):
+        for item in items:
             assert prev_item is None or len(prev_item) > len(item)
 
     @skip_pypy
     def test_sorted__reversed(self):
         cache = self.init_cache()
 
         for i in range(100):
@@ -197,15 +264,15 @@
             cache[f'key_{i}'] = response
 
         # Sorted items should be in ascending order by expiration time
         items = list(cache.sorted(key='expires'))
         assert len(items) == limit or 100
 
         prev_item = None
-        for i, item in enumerate(items):
+        for item in items:
             assert prev_item is None or prev_item.expires < item.expires
 
     @skip_pypy
     def test_sorted__exclude_expired(self):
         cache = self.init_cache()
         now = datetime.utcnow()
 
@@ -219,15 +286,15 @@
             cache[f'key_{i}'] = response
 
         # Items should only include unexpired (even numbered) items, and still be in sorted order
         items = list(cache.sorted(key='expires', expired=False))
         assert len(items) == 50
         prev_item = None
 
-        for i, item in enumerate(items):
+        for item in items:
             assert prev_item is None or prev_item.expires < item.expires
             assert item.status_code % 2 == 0
 
     @skip_pypy
     def test_sorted__error(self):
         """sorted() should handle deserialization errors and not return invalid responses"""
 
@@ -341,11 +408,11 @@
             session.cache.responses[f'key_{i}'] = response
 
         # Sorted items should be in ascending order by expiration time
         items = list(session.cache.sorted(key='expires', expired=False, reversed=True, limit=100))
         assert len(items) == 100
 
         prev_item = None
-        for i, item in enumerate(items):
+        for item in items:
             assert prev_item is None or prev_item.expires < item.expires
             assert item.cache_key
             assert not item.is_expired
```

### Comparing `requests_cache-1.0.1/tests/integration/test_upgrade.py` & `requests_cache-1.1.0/tests/integration/test_upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
     The previously cached responses should be either replaced or retrieved without any errors.
     """
     copyfile(db_path, tempfile_path)
     session = CachedSession(tempfile_path)
 
     for response_format in HTTPBIN_FORMATS:
-        session.get(httpbin(response_format)).from_cache
+        session.get(httpbin(response_format))
         assert session.get(httpbin(response_format)).from_cache is True
```

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.3.0` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.3.0`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.4.0` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.4.0`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.4.13` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.4.13`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.5.0` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.5.0`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.5.1` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.5.1`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.5.2` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.5.2`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.6.0` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.6.0`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.6.1` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.6.1`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.6.2` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.6.2`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.6.3` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.6.3`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.6.4` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.6.4`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.7.0` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.7.0`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.7.1` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.7.1`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.7.2` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.7.2`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.7.3` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.7.3`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.7.4` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.7.4`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.7.5` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.7.5`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.8.0` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.8.0`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.8.1` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.8.1`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.0` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.0`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.1` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.1`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.2` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.2`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.3` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.3`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.4` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.4`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.5` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.5`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.6` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.6`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.7` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.7`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.0.9.8` & `requests_cache-1.1.0/tests/sample_data/sample.db.0.9.8`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/sample.db.1.0.0` & `requests_cache-1.1.0/tests/sample_data/sample.db.1.0.0`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/vcr_requests_cache.yaml` & `requests_cache-1.1.0/tests/sample_data/vcr_requests_cache.yaml`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/sample_data/vcr_vcrpy.yaml` & `requests_cache-1.1.0/tests/sample_data/vcr_vcrpy.yaml`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/unit/models/test_base.py` & `requests_cache-1.1.0/tests/unit/models/test_base.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/unit/models/test_raw_response.py` & `requests_cache-1.1.0/tests/unit/models/test_raw_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     assert dict(response.raw.headers) == dict(raw.headers) == {'Content-Type': 'text/plain'}
     assert raw.read(None) == b'mock response'
     assert response.raw.decode_content is raw.decode_content is False
     assert response.raw.reason is raw.reason is None
     if hasattr(response.raw, '_request_url'):
         assert response.raw._request_url is raw.request_url is None
     assert response.raw.status == raw.status == 200
-    assert response.raw.strict == raw.strict == 0
     assert response.raw.version == raw.version == 0
 
 
 def test_read():
     raw = CachedHTTPResponse(body=b'mock response')
     assert raw.read(10) == b'mock respo'
     assert raw.read(None) == b'nse'
```

### Comparing `requests_cache-1.0.1/tests/unit/models/test_request.py` & `requests_cache-1.1.0/tests/unit/models/test_request.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/unit/models/test_response.py` & `requests_cache-1.1.0/tests/unit/models/test_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 def test_history(mock_session):
     original_response = mock_session.get(MOCKED_URL)
     original_response.history = [mock_session.get(MOCKED_URL)] * 3
     response = CachedResponse.from_response(original_response)
     assert len(response.history) == 3
-    assert all([isinstance(r, CachedResponse) for r in response.history])
+    assert all(isinstance(r, CachedResponse) for r in response.history)
 
 
 @pytest.mark.parametrize(
     'expires, is_expired',
     [
         (datetime.utcnow() + timedelta(days=1), False),
         (datetime.utcnow() - timedelta(days=1), True),
@@ -114,24 +114,24 @@
 def test_str(mock_session):
     """Just ensure that a subset of relevant attrs get included in the response str; the format
     may change without breaking the test.
     """
     response = CachedResponse.from_response(mock_session.get(MOCKED_URL))
     response._content = b'1010'
     expected_values = ['GET', MOCKED_URL, 200, '4 bytes', 'created', 'expires', 'fresh']
-    assert all([str(v) in str(response) for v in expected_values])
+    assert all(str(v) in str(response) for v in expected_values)
 
 
 def test_repr(mock_session):
     """Just ensure that a subset of relevant attrs get included in the response repr"""
     response = CachedResponse.from_response(mock_session.get(MOCKED_URL))
     expected_values = ['GET', MOCKED_URL, 200, 'ISO-8859-1', response.headers]
     print(repr(response))
     assert repr(response).startswith('CachedResponse(') and repr(response).endswith(')')
-    assert all([str(v) in repr(response) for v in expected_values])
+    assert all(str(v) in repr(response) for v in expected_values)
 
 
 @pytest.mark.parametrize(
     'n_bytes, expected_size',
     [
         (None, '0 bytes'),
         (5, '5 bytes'),
```

### Comparing `requests_cache-1.0.1/tests/unit/policy/test_actions.py` & `requests_cache-1.1.0/tests/unit/policy/test_actions.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/unit/policy/test_expiration.py` & `requests_cache-1.1.0/tests/unit/policy/test_expiration.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/unit/test_base_cache.py` & `requests_cache-1.1.0/tests/unit/test_base_cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """BaseCache tests that use mocked responses only"""
 import pickle
 from datetime import datetime, timedelta
 from logging import getLogger
 from pickle import PickleError
-from time import sleep
 from unittest.mock import patch
 
 import pytest
 from requests import Request
 
 from requests_cache.backends import BaseCache, SQLiteCache, SQLiteDict
 from requests_cache.cache_keys import create_key
@@ -15,20 +14,23 @@
 from requests_cache.session import CachedSession
 from tests.conftest import (
     MOCKED_URL,
     MOCKED_URL_ETAG,
     MOCKED_URL_HTTPS,
     MOCKED_URL_JSON,
     MOCKED_URL_REDIRECT,
+    START_DT,
+    YESTERDAY,
     ignore_deprecation,
     mount_mock_adapter,
     patch_normalize_url,
+    skip_pypy,
+    time_travel,
 )
 
-YESTERDAY = datetime.utcnow() - timedelta(days=1)
 logger = getLogger(__name__)
 
 
 class InvalidResponse:
     """Class that will raise an error when unpickled"""
 
     def __init__(self):
@@ -49,71 +51,90 @@
     mock_session.get(MOCKED_URL, params={'foo': 'bar'})
     request = Request('GET', MOCKED_URL, params={'foo': 'bar'})
     assert mock_session.cache.contains(request=request)
     request.params = None
     assert not mock_session.cache.contains(request=request)
 
 
+def test_contains__multipart_request(mock_session):
+    files = [('file', ('test.txt', b'content'))]
+    mock_session.settings.allowable_methods = ('GET', 'POST')
+    mock_session.post(MOCKED_URL, files=files)
+    request = Request('POST', MOCKED_URL, files=files)
+    assert mock_session.cache.contains(request=request)
+    request.files = None
+    assert not mock_session.cache.contains(request=request)
+
+
 def test_contains__url(mock_session):
     mock_session.get(MOCKED_URL)
     assert mock_session.cache.contains(url=MOCKED_URL)
     assert not mock_session.cache.contains(url=f'{MOCKED_URL}?foo=bar')
 
 
+@skip_pypy  # time-machine doesn't work on PyPy
 @patch_normalize_url
 def test_delete__expired(mock_normalize_url, mock_session):
     unexpired_url = f'{MOCKED_URL}?x=1'
     mock_session.mock_adapter.register_uri(
         'GET', unexpired_url, status_code=200, text='mock response'
     )
     mock_session.settings.expire_after = 1
-    mock_session.get(MOCKED_URL)
-    mock_session.get(MOCKED_URL_JSON)
-    sleep(1.1)
+
+    with time_travel(START_DT):
+        mock_session.get(MOCKED_URL)
+        mock_session.get(MOCKED_URL_JSON)
+
     mock_session.settings.expire_after = 2
-    mock_session.get(unexpired_url)
+    with time_travel(START_DT + timedelta(seconds=1.1)):
+        mock_session.get(unexpired_url)
 
     # At this point we should have 1 unexpired response and 2 expired responses
     assert len(mock_session.cache.responses) == 3
 
     # Use the generic BaseCache implementation, not the SQLite-specific one
-    BaseCache.delete(mock_session.cache, expired=True)
+    with time_travel(START_DT + timedelta(seconds=2)):
+        BaseCache.delete(mock_session.cache, expired=True)
     assert len(mock_session.cache.responses) == 1
+
     cached_response = list(mock_session.cache.responses.values())[0]
     assert cached_response.url == unexpired_url
 
     # Now the last response should be expired as well
-    sleep(2)
-    BaseCache.delete(mock_session.cache, expired=True)
+    with time_travel(START_DT + timedelta(seconds=4)):
+        BaseCache.delete(mock_session.cache, expired=True)
     assert len(mock_session.cache.responses) == 0
 
 
+@skip_pypy
 def test_delete__expired__per_request(mock_session):
-    # Cache 3 responses with different expiration times
     second_url = f'{MOCKED_URL}/endpoint_2'
     third_url = f'{MOCKED_URL}/endpoint_3'
     mock_session.mock_adapter.register_uri('GET', second_url, status_code=200)
     mock_session.mock_adapter.register_uri('GET', third_url, status_code=200)
-    mock_session.get(MOCKED_URL)
-    mock_session.get(second_url, expire_after=2)
-    mock_session.get(third_url, expire_after=4)
-
-    # All 3 responses should still be cached
-    mock_session.cache.delete(expired=True)
-    for response in mock_session.cache.responses.values():
-        logger.info(f'Expires in {response.expires_delta} seconds')
-    assert len(mock_session.cache.responses) == 3
 
-    # One should be expired after 2s, and another should be expired after 4s
-    sleep(2)
-    mock_session.cache.delete(expired=True)
-    assert len(mock_session.cache.responses) == 2
-    sleep(2)
-    mock_session.cache.delete(expired=True)
-    assert len(mock_session.cache.responses) == 1
+    # Cache 3 responses with different expiration times
+    with time_travel(START_DT):
+        mock_session.get(MOCKED_URL)
+        mock_session.get(second_url, expire_after=5)
+        mock_session.get(third_url, expire_after=10)
+
+        # All 3 responses should still be cached
+        mock_session.cache.delete(expired=True)
+        for response in mock_session.cache.responses.values():
+            logger.info(f'Expires in {response.expires_delta} seconds')
+        assert len(mock_session.cache.responses) == 3
+
+    # One should be expired after 5s, and another should be expired after 10s
+    with time_travel(START_DT + timedelta(seconds=6)):
+        mock_session.cache.delete(expired=True)
+        assert len(mock_session.cache.responses) == 2
+    with time_travel(START_DT + timedelta(seconds=11)):
+        mock_session.cache.delete(expired=True)
+        assert len(mock_session.cache.responses) == 1
 
 
 def test_delete__invalid(tempfile_path):
     class BadSerialzier:
         def dumps(self, value):
             return pickle.dumps(value)
 
@@ -136,40 +157,43 @@
     BaseCache.delete(mock_session.cache, expired=True, invalid=True)
 
     assert len(mock_session.cache.responses) == 1
     assert mock_session.get(MOCKED_URL).from_cache is True
     assert mock_session.get(MOCKED_URL_JSON).from_cache is False
 
 
+@skip_pypy
 def test_delete__older_than(mock_session):
     # Cache 4 responses with different creation times
-    response_0 = CachedResponse(request=CachedRequest(method='GET', url='https://test.com/test_0'))
-    mock_session.cache.save_response(response_0)
-    response_1 = CachedResponse(request=CachedRequest(method='GET', url='https://test.com/test_1'))
-    response_1.created_at -= timedelta(seconds=1)
-    mock_session.cache.save_response(response_1)
-    response_2 = CachedResponse(request=CachedRequest(method='GET', url='https://test.com/test_2'))
-    response_2.created_at -= timedelta(seconds=2)
-    mock_session.cache.save_response(response_2)
-    response_3 = CachedResponse(request=CachedRequest(method='GET', url='https://test.com/test_3'))
-    response_3.created_at -= timedelta(seconds=3)
-    mock_session.cache.save_response(response_3)
+    with time_travel(START_DT):
+        request = CachedRequest(method='GET', url='https://test.com/test_0')
+        mock_session.cache.save_response(CachedResponse(request=request))
+    with time_travel(START_DT - timedelta(seconds=1.1)):
+        request = CachedRequest(method='GET', url='https://test.com/test_1')
+        mock_session.cache.save_response(CachedResponse(request=request))
+    with time_travel(START_DT - timedelta(seconds=2.1)):
+        request = CachedRequest(method='GET', url='https://test.com/test_2')
+        mock_session.cache.save_response(CachedResponse(request=request))
+    with time_travel(START_DT - timedelta(seconds=3.1)):
+        request = CachedRequest(method='GET', url='https://test.com/test_3')
+        mock_session.cache.save_response(CachedResponse(request=request))
 
     # Incrementally remove responses older than 3, 2, and 1 seconds
-    assert len(mock_session.cache.responses) == 4
-    mock_session.cache.delete(older_than=timedelta(seconds=3))
-    assert len(mock_session.cache.responses) == 3
-    mock_session.cache.delete(older_than=timedelta(seconds=2))
-    assert len(mock_session.cache.responses) == 2
-    mock_session.cache.delete(older_than=timedelta(seconds=1))
-    assert len(mock_session.cache.responses) == 1
+    with time_travel(START_DT):
+        assert len(mock_session.cache.responses) == 4
+        mock_session.cache.delete(older_than=timedelta(seconds=3))
+        assert len(mock_session.cache.responses) == 3
+        mock_session.cache.delete(older_than=timedelta(seconds=2))
+        assert len(mock_session.cache.responses) == 2
+        mock_session.cache.delete(older_than=timedelta(seconds=1))
+        assert len(mock_session.cache.responses) == 1
 
     # Remove the last response after it's 1 second old
-    sleep(1)
-    mock_session.cache.delete(older_than=timedelta(seconds=1))
+    with time_travel(START_DT + timedelta(seconds=1.1)):
+        mock_session.cache.delete(older_than=timedelta(seconds=1))
     assert len(mock_session.cache.responses) == 0
 
 
 def test_delete__urls(mock_session):
     urls = [MOCKED_URL, MOCKED_URL_JSON, MOCKED_URL_REDIRECT]
     for url in urls:
         mock_session.get(url)
@@ -226,14 +250,35 @@
     assert old_cache_keys == new_cache_keys
 
     # Check that responses are returned from the cache correctly using the new key function
     for url in urls:
         assert mock_session.get(url).from_cache is True
 
 
+def test_recreate_keys__empty_response_body(mock_session):
+    # Cache some initial responses with default key function, and modify request body (pre-1.0)
+    urls = [MOCKED_URL, MOCKED_URL_JSON, MOCKED_URL_ETAG]
+    for url in urls:
+        r = mock_session.get(url)
+        r = CachedResponse.from_response(r)
+        r.request.body = b'None'
+        mock_session.cache.responses[r.cache_key] = r
+
+    # Switch to a new key function and recreate keys
+    def new_key_fn(*args, **kwargs):
+        return create_key(*args, **kwargs) + '_suffix'
+
+    mock_session.settings.key_fn = new_key_fn
+    mock_session.cache.recreate_keys()
+
+    # Check that responses are returned from the cache correctly using the new key function
+    for url in urls:
+        assert mock_session.get(url).from_cache is True
+
+
 def test_reset_expiration__extend_expiration(mock_session):
     # Start with an expired response
     mock_session.settings.expire_after = datetime.utcnow() - timedelta(seconds=1)
     mock_session.get(MOCKED_URL)
 
     # Set expiration in the future
     mock_session.cache.reset_expiration(datetime.utcnow() + timedelta(seconds=1))
```

### Comparing `requests_cache-1.0.1/tests/unit/test_cache_keys.py` & `requests_cache-1.1.0/tests/unit/test_cache_keys.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """The cache_keys module is mostly covered indirectly via other tests.
 This just contains tests for some extra edge cases not covered elsewhere.
 """
 import json
 
 import pytest
-from requests import Request
+from requests import Request, Response
 
-from requests_cache.cache_keys import MAX_NORM_BODY_SIZE, create_key, normalize_request
+from requests_cache.cache_keys import (
+    MAX_NORM_BODY_SIZE,
+    create_key,
+    normalize_request,
+    redact_response,
+)
 
 CACHE_KEY = 'e25f7e6326966e82'
 
 
 @pytest.mark.parametrize(
     'url, params',
     [
@@ -57,14 +62,27 @@
     )
     request_2 = Request(
         method='GET', url='https://img.site.com/base/img.jpg?param_1=b&param_1=a', params={'k': 'v'}
     )
     assert create_key(request_1) == create_key(request_2)
 
 
+def test_redact_response__escaped_params():
+    """Test that redact_response() handles escaped request parameters"""
+    request = Request(
+        method='GET',
+        url='https://img.site.com/base/img.jpg?ignored_param=value_1&param_2=value_2',
+    )
+    response = Response()
+    response.url = 'https://img.site.com/base/img.jpg?where=code%3D123'
+    response.request = request
+    redacted_response = redact_response(response, [])
+    assert redacted_response.url == 'https://img.site.com/base/img.jpg?where=code%3D123'
+
+
 def test_normalize_request__json_body():
     request = Request(
         method='GET',
         url='https://img.site.com/base/img.jpg',
         data=b'{"param_1": "value_1", "param_2": "value_2"}',
         headers={'Content-Type': 'application/json'},
     )
```

### Comparing `requests_cache-1.0.1/tests/unit/test_patcher.py` & `requests_cache-1.1.0/tests/unit/test_patcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,25 +53,25 @@
     mock_clear.assert_not_called()
 
 
 @patch.object(OriginalSession, 'request')
 @patch.object(CachedSession, 'request')
 def test_disabled(cached_request, original_request, installed_session):
     with requests_cache.disabled():
-        for i in range(3):
+        for _ in range(3):
             requests.get('some_url')
     assert cached_request.call_count == 0
     assert original_request.call_count == 3
 
 
 @patch.object(OriginalSession, 'request')
 @patch.object(CachedSession, 'request')
 def test_enabled(cached_request, original_request, tempfile_path):
     with requests_cache.enabled(tempfile_path):
-        for i in range(3):
+        for _ in range(3):
             requests.get('some_url')
     assert cached_request.call_count == 3
     assert original_request.call_count == 0
 
 
 def test_is_installed():
     assert requests_cache.is_installed() is False
```

### Comparing `requests_cache-1.0.1/tests/unit/test_serializers.py` & `requests_cache-1.1.0/tests/unit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `requests_cache-1.0.1/tests/unit/test_session.py` & `requests_cache-1.1.0/tests/unit/test_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,34 @@
 from requests import HTTPError, Request, RequestException
 from requests.structures import CaseInsensitiveDict
 
 from requests_cache import ALL_METHODS, CachedSession
 from requests_cache._utils import get_placeholder_class
 from requests_cache.backends import BACKEND_CLASSES, BaseCache
 from requests_cache.backends.base import DESERIALIZE_ERRORS
+from requests_cache.models import CachedResponse
 from requests_cache.policy.expiration import DO_NOT_CACHE, EXPIRE_IMMEDIATELY, NEVER_EXPIRE
 from tests.conftest import (
     MOCKED_URL,
     MOCKED_URL_200_404,
     MOCKED_URL_404,
     MOCKED_URL_500,
     MOCKED_URL_ETAG,
     MOCKED_URL_HTTPS,
     MOCKED_URL_JSON,
     MOCKED_URL_REDIRECT,
     MOCKED_URL_REDIRECT_TARGET,
     MOCKED_URL_VARY,
+    MOCKED_URL_VARY_REDIRECT,
+    MOCKED_URL_VARY_REDIRECT_TARGET,
+    START_DT,
     ignore_deprecation,
     patch_normalize_url,
+    skip_pypy,
+    time_travel,
 )
 
 logger = getLogger(__name__)
 
 # Basic initialization
 # -----------------------------------------------------
 
@@ -191,20 +197,28 @@
     mock_session.get(MOCKED_URL)
     assert mock_session.get(MOCKED_URL).from_cache is True
     assert mock_session.get(MOCKED_URL, verify=False).from_cache is False
     assert mock_session.get(MOCKED_URL, verify='/path/to/cert').from_cache is False
 
 
 def test_response_history(mock_session):
+    """When a request results in redirects:
+    * An alias for the redirect should be added to 'redirects' table/collection
+    * Both the original and target URLs should be retrievable from the cache
+    * CachedResponse.history should be populated with CachedResponse objects
+    """
     mock_session.get(MOCKED_URL_REDIRECT)
     r = mock_session.get(MOCKED_URL_REDIRECT_TARGET)
 
     assert r.from_cache is True
     assert len(mock_session.cache.redirects) == 1
 
+    r2 = mock_session.get(MOCKED_URL_REDIRECT)
+    assert isinstance(r2.history[0], CachedResponse)
+
 
 # Request matching
 # -----------------------------------------------------
 
 
 @pytest.mark.parametrize('method', ['POST', 'PUT'])
 def test_raw_data(method, mock_session):
@@ -323,25 +337,49 @@
     assert mock_session.get(MOCKED_URL, headers=headers_3).from_cache is False
 
 
 def test_match_headers__vary(mock_session):
     """Vary should be used to validate headers, if available.
     It should also override `match_headers` for the secondary cache key, if both are provided.
     """
-    # mock_session.settings.match_headers = ['Accept-Encoding']
     headers_1 = {'Accept': 'application/json', 'User-Agent': 'qutebrowser'}
     headers_2 = {'Accept': 'application/json', 'User-Agent': 'Firefox'}
     headers_3 = {'Accept': 'text/plain', 'User-Agent': 'qutebrowser'}
+    mock_session.get(MOCKED_URL_VARY, headers=headers_1)
 
-    assert mock_session.get(MOCKED_URL_VARY, headers=headers_1).from_cache is False
     assert mock_session.get(MOCKED_URL_VARY, headers=headers_1).from_cache is True
     assert mock_session.get(MOCKED_URL_VARY, headers=headers_2).from_cache is True
     assert mock_session.get(MOCKED_URL_VARY, headers=headers_3).from_cache is False
 
 
+@pytest.mark.parametrize(
+    'headers, expected_from_cache',
+    [
+        ({'Accept': 'text/plain', 'Accept-Language': 'en-US'}, True),
+        ({'Accept-Language': 'en-US'}, True),
+        ({'Accept-Language': 'en-GB'}, False),
+        ({'Accept': 'application/json'}, False),
+        ({}, False),
+    ],
+)
+def test_match_headers__vary_with_redirects(headers, expected_from_cache, mock_session):
+    """With Vary + redirects, Vary should match against the last request in the redirect chain.
+    * 1st response has `Vary: Accept` (shouldn't be matched)
+    * 2nd response has `Vary: Accept-Language` (should be matched)
+    """
+    r = mock_session.get(
+        MOCKED_URL_VARY_REDIRECT,
+        headers={'Accept': 'text/plain', 'Accept-Language': 'en-US'},
+    )
+    assert r.url == MOCKED_URL_VARY_REDIRECT_TARGET
+
+    r2 = mock_session.get(MOCKED_URL_VARY_REDIRECT, headers=headers)
+    assert r2.from_cache is expected_from_cache
+
+
 def test_include_get_headers():
     """include_get_headers is aliased to match_headers for backwards-compatibility"""
     session = CachedSession(include_get_headers=True, backend='memory')
     assert session.settings.match_headers is True
 
 
 # Error handling
@@ -353,85 +391,94 @@
     """If there is an error while fetching a cached response, a new one should be fetched"""
     mock_session.get(MOCKED_URL)
 
     with patch.object(mock_session.cache.responses.serializer, 'loads', side_effect=exception_cls):
         assert mock_session.get(MOCKED_URL).from_cache is False
 
 
+@skip_pypy
 def test_expired_request_error(mock_session):
     """Without stale_if_error (default), if there is an error while re-fetching an expired
     response, the request should be re-raised
     """
     mock_session.settings.stale_if_error = False
     mock_session.settings.expire_after = 1
-    mock_session.get(MOCKED_URL)
-    sleep(1)
+
+    with time_travel(START_DT):
+        mock_session.get(MOCKED_URL)
 
     with patch.object(mock_session.cache, 'save_response', side_effect=ValueError):
-        with pytest.raises(ValueError):
-            mock_session.get(MOCKED_URL)
+        with time_travel(START_DT + timedelta(seconds=1.1)):
+            with pytest.raises(ValueError):
+                mock_session.get(MOCKED_URL)
 
 
+@skip_pypy
 def test_stale_if_error__exception(mock_session):
     """With stale_if_error, expect to get old cache data if there is an exception during a request"""
     mock_session.settings.stale_if_error = True
     mock_session.settings.expire_after = 1
+    with time_travel(START_DT):
+        assert mock_session.get(MOCKED_URL).from_cache is False
+        assert mock_session.get(MOCKED_URL).from_cache is True
 
-    assert mock_session.get(MOCKED_URL).from_cache is False
-    assert mock_session.get(MOCKED_URL).from_cache is True
-    sleep(1)
     with patch.object(mock_session.cache, 'save_response', side_effect=RequestException):
-        response = mock_session.get(MOCKED_URL)
-        assert response.from_cache is True and response.is_expired is True
+        with time_travel(START_DT + timedelta(seconds=1.1)):
+            response = mock_session.get(MOCKED_URL)
+            assert response.from_cache is True and response.is_expired is True
 
 
+@skip_pypy
 def test_stale_if_error__error_code(mock_session):
     """With stale_if_error, expect to get old cache data if a response has an error status code,
     that is not in allowable_codes.
     """
     mock_session.settings.stale_if_error = True
     mock_session.settings.expire_after = 1
     mock_session.settings.allowable_codes = (200,)
 
-    assert mock_session.get(MOCKED_URL_200_404).status_code == 200
+    with time_travel(START_DT):
+        assert mock_session.get(MOCKED_URL_200_404).status_code == 200
 
-    sleep(1)
+    with time_travel(START_DT + timedelta(seconds=1.1)):
+        response = mock_session.get(MOCKED_URL_200_404)
 
-    response = mock_session.get(MOCKED_URL_200_404)
     assert response.status_code == 200
     assert response.from_cache is True
     assert response.is_expired is True
 
 
+@skip_pypy
 def test_stale_if_error__error_code_in_allowable_codes(mock_session):
     """With stale_if_error, expect to get the failed response if a response has an error status code,
     that is in allowable_codes.
     """
     mock_session.settings.stale_if_error = True
     mock_session.settings.expire_after = 1
     mock_session.settings.allowable_codes = (200, 404)
 
-    assert mock_session.get(MOCKED_URL_200_404).status_code == 200
+    with time_travel(START_DT):
+        assert mock_session.get(MOCKED_URL_200_404).status_code == 200
 
-    sleep(1)
+    with time_travel(START_DT + timedelta(seconds=1.1)):
+        response = mock_session.get(MOCKED_URL_200_404)
 
-    response = mock_session.get(MOCKED_URL_200_404)
     assert response.status_code == 404
     assert response.from_cache is False
     assert response.is_expired is False
 
 
 def test_stale_if_error__max_stale(mock_session):
     """With stale_if_error as a time value, expect to get old cache data if a response has an error
     status code AND it is expired by less than the specified time
     """
     mock_session.settings.stale_if_error = timedelta(seconds=15)
     mock_session.settings.expire_after = datetime.utcnow() - timedelta(seconds=10)
     mock_session.settings.allowable_codes = (200,)
-    mock_session.get(MOCKED_URL_200_404).from_cache
+    mock_session.get(MOCKED_URL_200_404)
 
     response = mock_session.get(MOCKED_URL_200_404)
     assert response.from_cache is True
     assert response.is_expired is True
 
     mock_session.settings.stale_if_error = 5
     with pytest.raises(HTTPError):
@@ -443,25 +490,25 @@
     session = CachedSession(old_data_on_error=True, backend='memory')
     assert session.settings.stale_if_error is True
 
 
 def test_cache_disabled(mock_session):
     mock_session.get(MOCKED_URL)
     with mock_session.cache_disabled():
-        for i in range(2):
+        for _ in range(2):
             assert mock_session.get(MOCKED_URL).from_cache is False
     assert mock_session.get(MOCKED_URL).from_cache is True
 
 
 def test_cache_disabled__nested(mock_session):
     mock_session.get(MOCKED_URL)
     with mock_session.cache_disabled():
         mock_session.get(MOCKED_URL)
         with mock_session.cache_disabled():
-            for i in range(2):
+            for _ in range(2):
                 assert mock_session.get(MOCKED_URL).from_cache is False
     assert mock_session.get(MOCKED_URL).from_cache is True
 
 
 def test_unpickle_errors(mock_session):
     """If there is an error during deserialization, the request should be made again"""
     assert mock_session.get(MOCKED_URL_JSON).from_cache is False
@@ -600,15 +647,15 @@
     for hook in ('response',):
 
         def hook_func(r, *args, **kwargs):
             state[hook] += 1
             assert r.from_cache is True
             return r
 
-        for i in range(5):
+        for _ in range(5):
             mock_session.get(MOCKED_URL, hooks={hook: hook_func})
         assert state[hook] == 5
 
 
 def test_expire_after_alias(mock_session):
     """CachedSession has an `expire_after` property for backwards-compatibility"""
     mock_session.expire_after = 60
@@ -765,46 +812,50 @@
     assert response.from_cache is True and response.is_expired is False
 
 
 # Additional request() and send() options
 # -----------------------------------------------------
 
 
+@skip_pypy  # time-machine doesn't work on PyPy
 def test_request_expire_after__enable_expiration(mock_session):
     """No per-session expiration is set, but then overridden for a single request"""
     mock_session.settings.expire_after = None
-    response = mock_session.get(MOCKED_URL, expire_after=1)
-    assert response.from_cache is False
-    assert mock_session.get(MOCKED_URL).from_cache is True
+    with time_travel(START_DT):
+        response = mock_session.get(MOCKED_URL, expire_after=1)
+        assert response.from_cache is False
+        assert mock_session.get(MOCKED_URL).from_cache is True
 
-    sleep(1)
-    response = mock_session.get(MOCKED_URL)
-    assert response.from_cache is False
+    with time_travel(START_DT + timedelta(seconds=1.1)):
+        response = mock_session.get(MOCKED_URL)
+        assert response.from_cache is False
 
 
 def test_request_expire_after__disable_expiration(mock_session):
     """A per-session expiration is set, but then disabled for a single request"""
     mock_session.settings.expire_after = 60
     response = mock_session.get(MOCKED_URL, expire_after=NEVER_EXPIRE)
     response = mock_session.get(MOCKED_URL, expire_after=NEVER_EXPIRE)
     assert response.from_cache is True
     assert response.expires is None
 
 
+@skip_pypy
 def test_request_expire_after__prepared_request(mock_session):
     """Pre-request expiration should also work for PreparedRequests with CachedSession.send()"""
     mock_session.settings.expire_after = None
-    request = Request('GET', MOCKED_URL, headers={}, data=None).prepare()
-    response = mock_session.send(request, expire_after=1)
-    assert response.from_cache is False
-    assert mock_session.send(request).from_cache is True
+    with time_travel(START_DT):
+        request = Request('GET', MOCKED_URL, headers={}, data=None).prepare()
+        response = mock_session.send(request, expire_after=1)
+        assert response.from_cache is False
+        assert mock_session.send(request).from_cache is True
 
-    sleep(1)
-    response = mock_session.get(MOCKED_URL)
-    assert response.from_cache is False
+    with time_travel(START_DT + timedelta(seconds=1.1)):
+        response = mock_session.get(MOCKED_URL)
+        assert response.from_cache is False
 
 
 def test_request_only_if_cached__cached(mock_session):
     """only_if_cached has no effect if the response is already cached"""
     mock_session.get(MOCKED_URL)
     response = mock_session.get(MOCKED_URL, only_if_cached=True)
     assert response.from_cache is True
@@ -815,30 +866,34 @@
     """only_if_cached should return a 504 response if it is not already cached"""
     response = mock_session.get(MOCKED_URL, only_if_cached=True)
     assert response.status_code == 504
     with pytest.raises(HTTPError):
         response.raise_for_status()
 
 
+@skip_pypy
 def test_request_only_if_cached__expired(mock_session):
     """By default, only_if_cached will not return an expired response"""
-    mock_session.get(MOCKED_URL, expire_after=1)
-    sleep(1)
+    with time_travel(START_DT):
+        mock_session.get(MOCKED_URL, expire_after=1)
 
-    response = mock_session.get(MOCKED_URL, only_if_cached=True)
+    with time_travel(START_DT + timedelta(seconds=1.1)):
+        response = mock_session.get(MOCKED_URL, only_if_cached=True)
     assert response.status_code == 504
 
 
+@skip_pypy
 def test_request_only_if_cached__stale_if_error__expired(mock_session):
     """only_if_cached *will* return an expired response if stale_if_error is also set"""
-    mock_session.get(MOCKED_URL, expire_after=1)
-    sleep(1)
+    with time_travel(START_DT):
+        mock_session.get(MOCKED_URL, expire_after=1)
 
-    mock_session.settings.stale_if_error = True
-    response = mock_session.get(MOCKED_URL, only_if_cached=True)
+    with time_travel(START_DT + timedelta(seconds=1.1)):
+        mock_session.settings.stale_if_error = True
+        response = mock_session.get(MOCKED_URL, only_if_cached=True)
     assert response.status_code == 200
     assert response.from_cache is True
     assert response.is_expired is True
 
 
 def test_request_only_if_cached__skips_revalidate(mock_session):
     """only_if_cached should skip other revalidation conditions if the response isn't expired.
@@ -855,14 +910,56 @@
     request = Request('GET', MOCKED_URL, headers={}).prepare()
     response = mock_session.send(request, only_if_cached=True)
     assert response.status_code == 504
     with pytest.raises(HTTPError):
         response.raise_for_status()
 
 
+def test_revalidation__skip_update(mock_session):
+    """After a revalidation request, the response should not be updated in the cache if expiration
+    and headers are unchanged.
+    """
+    # With no expiration (NEVER_EXPIRE), the expiration value in the cache will not change.
+    mock_session.settings.expire_after = NEVER_EXPIRE
+    response_1 = mock_session.get(MOCKED_URL_ETAG)
+    mock_session.mock_adapter.register_uri('GET', MOCKED_URL_ETAG, status_code=304)
+
+    with patch.object(mock_session.cache, 'save_response') as mock_save:
+        response_2 = mock_session.get(MOCKED_URL_ETAG, refresh=True)
+        mock_save.assert_not_called()
+
+    assert response_2.from_cache is True and response_2.revalidated is True
+    assert response_1.expires == response_2.expires
+
+
+def test_revalidation__update_cache(mock_session):
+    """After a revalidation request, the response should be updated in the cache with new expiration
+    and/or headers (if either changed).
+    """
+    mock_session.settings.expire_after = -1
+    response_1 = mock_session.get(MOCKED_URL_ETAG)
+    assert response_1.expires is None
+    mock_session.mock_adapter.register_uri('GET', MOCKED_URL_ETAG, status_code=304)
+
+    # Expiration has changed
+    with patch.object(mock_session.cache, 'save_response') as mock_save:
+        response_2 = mock_session.get(MOCKED_URL_ETAG, refresh=True, expire_after=60)
+        mock_save.assert_called()
+    assert response_2.expires is not None
+
+    # Headers have changed
+    mock_session.mock_adapter.register_uri(
+        'GET', MOCKED_URL_ETAG, headers={'new_header': 'true'}, status_code=304
+    )
+    with patch.object(mock_session.cache, 'save_response') as mock_save:
+        response_3 = mock_session.get(MOCKED_URL_ETAG, refresh=True, expire_after=60)
+        mock_save.assert_called()
+    assert response_3.headers['new_header'] == 'true'
+
+
 def test_request_refresh(mock_session):
     """The refresh option should send a conditional request, if possible"""
     response_1 = mock_session.get(MOCKED_URL_ETAG, expire_after=60)
     response_2 = mock_session.get(MOCKED_URL_ETAG)
     mock_session.mock_adapter.register_uri('GET', MOCKED_URL_ETAG, status_code=304)
 
     response_3 = mock_session.get(MOCKED_URL_ETAG, refresh=True, expire_after=60)
```

### Comparing `requests_cache-1.0.1/PKG-INFO` & `requests_cache-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-cache
-Version: 1.0.1
+Version: 1.1.0
 Summary: A persistent cache for python requests
 Home-page: https://github.com/requests-cache/requests-cache
 License: BSD-2-Clause
 Keywords: requests,python-requests,cache,http,http-client,web,webscraping,performance,sqlite,redis,mongodb,gridfs,dynamodb
 Author: Roman Haritonov
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 Provides-Extra: security
 Provides-Extra: yaml
 Requires-Dist: attrs (>=21.2)
 Requires-Dist: boto3 (>=1.15) ; extra == "dynamodb" or extra == "all"
 Requires-Dist: botocore (>=1.18) ; extra == "dynamodb" or extra == "all"
 Requires-Dist: bson (>=0.5) ; extra == "bson"
 Requires-Dist: cattrs (>=22.2)
-Requires-Dist: furo (>=2022.12.7,<2023.0.0) ; extra == "docs"
+Requires-Dist: furo (>=2023.3,<2024.0) ; extra == "docs"
 Requires-Dist: itsdangerous (>=2.0) ; extra == "security" or extra == "all"
 Requires-Dist: linkify-it-py (>=2.0,<3.0) ; extra == "docs"
 Requires-Dist: myst-parser (>=1.0,<2.0) ; extra == "docs"
 Requires-Dist: platformdirs (>=2.5)
 Requires-Dist: pymongo (>=3) ; extra == "mongodb" or extra == "all"
 Requires-Dist: pyyaml (>=5.4) ; extra == "yaml" or extra == "all"
 Requires-Dist: redis (>=3) ; extra == "redis" or extra == "all"
```

