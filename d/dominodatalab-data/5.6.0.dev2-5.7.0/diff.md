# Comparing `tmp/dominodatalab_data-5.6.0.dev2.tar.gz` & `tmp/dominodatalab_data-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dominodatalab_data-5.6.0.dev2.tar", max compression
+gzip compressed data, was "dominodatalab_data-5.7.0.tar", max compression
```

## Comparing `dominodatalab_data-5.6.0.dev2.tar` & `dominodatalab_data-5.7.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0    10891 2022-06-17 19:33:52.493061 dominodatalab_data-5.6.0.dev2/LICENSE
--rw-r--r--   0        0        0     5982 2022-06-17 19:33:52.493416 dominodatalab_data-5.6.0.dev2/README.md
--rw-r--r--   0        0        0      102 2022-06-17 19:33:52.493643 dominodatalab_data-5.6.0.dev2/datasource_api_client/__init__.py
--rw-r--r--   0        0        0       47 2022-06-17 19:33:52.493859 dominodatalab_data-5.6.0.dev2/datasource_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-06-17 19:33:52.494005 dominodatalab_data-5.6.0.dev2/datasource_api_client/api/datasource/__init__.py
--rw-r--r--   0        0        0     4143 2022-12-01 18:54:53.827728 dominodatalab_data-5.6.0.dev2/datasource_api_client/api/datasource/get_datasource_by_name.py
--rw-r--r--   0        0        0        0 2022-06-17 19:33:52.494364 dominodatalab_data-5.6.0.dev2/datasource_api_client/api/proxy/__init__.py
--rw-r--r--   0        0        0     3381 2022-12-01 18:54:53.828165 dominodatalab_data-5.6.0.dev2/datasource_api_client/api/proxy/get_key_url.py
--rw-r--r--   0        0        0     3434 2022-12-01 18:54:53.828604 dominodatalab_data-5.6.0.dev2/datasource_api_client/api/proxy/list_keys.py
--rw-r--r--   0        0        0     2204 2022-12-01 18:54:53.829023 dominodatalab_data-5.6.0.dev2/datasource_api_client/api/proxy/log_metric.py
--rw-r--r--   0        0        0     1661 2022-06-17 19:33:52.495000 dominodatalab_data-5.6.0.dev2/datasource_api_client/client.py
--rw-r--r--   0        0        0      695 2022-06-17 19:33:52.495223 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/__init__.py
--rw-r--r--   0        0        0     1173 2022-06-17 19:33:52.495394 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_config.py
--rw-r--r--   0        0        0     4708 2022-06-17 19:33:52.495556 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_dto.py
--rw-r--r--   0        0        0     1199 2022-06-17 19:33:52.495710 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_dto_added_by.py
--rw-r--r--   0        0        0      428 2023-01-23 19:53:50.934111 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_dto_auth_type.py
--rw-r--r--   0        0        0      712 2023-01-23 19:53:50.936744 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_dto_data_source_type.py
--rw-r--r--   0        0        0      170 2022-06-17 19:33:52.496194 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_dto_status.py
--rw-r--r--   0        0        0     1905 2022-06-17 19:33:52.496344 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_owner_info.py
--rw-r--r--   0        0        0     1498 2022-06-17 19:33:52.496503 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/error_response.py
--rw-r--r--   0        0        0     3569 2022-06-17 19:33:52.496662 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/key_request.py
--rw-r--r--   0        0        0     3880 2022-12-01 18:54:53.830852 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/list_request.py
--rw-r--r--   0        0        0      153 2022-06-17 19:33:52.496968 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/log_metric_m.py
--rw-r--r--   0        0        0      239 2022-06-17 19:33:52.497120 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/log_metric_t.py
--rw-r--r--   0        0        0     2084 2022-06-17 19:33:52.497270 dominodatalab_data-5.6.0.dev2/datasource_api_client/models/proxy_error_response.py
--rw-r--r--   0        0        0      939 2022-06-17 19:33:52.497422 dominodatalab_data-5.6.0.dev2/datasource_api_client/types.py
--rw-r--r--   0        0        0      369 2022-06-17 19:33:52.498752 dominodatalab_data-5.6.0.dev2/domino_data/__init__.py
--rw-r--r--   0        0        0        0 2022-12-01 18:54:53.831027 dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/__init__.py
--rw-r--r--   0        0        0     3801 2023-04-03 15:43:18.645563 dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/client.py
--rw-r--r--   0        0        0      684 2022-12-01 18:54:53.832478 dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/exceptions.py
--rw-r--r--   0        0        0     2966 2023-01-04 16:07:48.401852 dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/git.py
--rw-r--r--   0        0        0      683 2023-01-04 16:07:48.403057 dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/logging.py
--rw-r--r--   0        0        0     1223 2023-01-04 16:07:48.405079 dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/run.py
--rw-r--r--   0        0        0     8180 2023-04-03 15:43:18.647140 dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/sync.py
--rw-r--r--   0        0        0     4527 2022-11-01 18:48:22.635731 dominodatalab_data-5.6.0.dev2/domino_data/auth.py
--rw-r--r--   0        0        0    10464 2023-03-20 19:22:28.913599 dominodatalab_data-5.6.0.dev2/domino_data/configuration_gen.py
--rw-r--r--   0        0        0    25149 2023-04-04 19:08:31.379631 dominodatalab_data-5.6.0.dev2/domino_data/data_sources.py
--rw-r--r--   0        0        0      894 2023-01-04 16:07:48.407684 dominodatalab_data-5.6.0.dev2/domino_data/logging.py
--rw-r--r--   0        0        0        0 2022-06-17 19:33:52.499858 dominodatalab_data-5.6.0.dev2/domino_data/py.typed
--rw-r--r--   0        0        0        0 2022-06-17 19:33:52.500015 dominodatalab_data-5.6.0.dev2/domino_data/training_sets/__init__.py
--rw-r--r--   0        0        0    13955 2022-11-01 18:48:22.638301 dominodatalab_data-5.6.0.dev2/domino_data/training_sets/client.py
--rw-r--r--   0        0        0     3588 2022-06-17 19:33:52.500395 dominodatalab_data-5.6.0.dev2/domino_data/training_sets/model.py
--rw-r--r--   0        0        0      104 2023-03-22 20:55:07.504701 dominodatalab_data-5.6.0.dev2/feature_store_api_client/__init__.py
--rw-r--r--   0        0        0       47 2023-03-22 20:55:07.608604 dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 20:55:07.642166 dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     2657 2023-03-22 20:55:43.492057 dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/get.py
--rw-r--r--   0        0        0     2861 2023-03-22 20:55:43.484056 dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/get_feature_view_name_store.py
--rw-r--r--   0        0        0     3383 2023-03-22 20:55:43.517321 dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/post.py
--rw-r--r--   0        0        0     1870 2023-03-22 20:55:43.459031 dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/post_featureview.py
--rw-r--r--   0        0        0     3215 2023-03-22 20:55:43.522840 dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/post_lock.py
--rw-r--r--   0        0        0     3144 2023-03-22 20:55:43.523213 dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/post_unlock.py
--rw-r--r--   0        0        0     1822 2023-03-22 20:55:43.469889 dominodatalab_data-5.6.0.dev2/feature_store_api_client/client.py
--rw-r--r--   0        0        0     1443 2023-03-22 20:55:42.273428 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/__init__.py
--rw-r--r--   0        0        0     2002 2023-03-22 20:55:43.488903 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/auth_config.py
--rw-r--r--   0        0        0     1513 2023-03-22 20:55:43.471506 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/auth_config_fields.py
--rw-r--r--   0        0        0     1166 2023-03-22 20:55:43.485806 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/auth_config_meta.py
--rw-r--r--   0        0        0      170 2023-03-22 20:55:42.266939 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/auth_field_name.py
--rw-r--r--   0        0        0      197 2023-03-22 20:55:42.238844 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/auth_type.py
--rw-r--r--   0        0        0      668 2023-03-22 20:55:42.288884 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/config_field_name.py
--rw-r--r--   0        0        0     2987 2023-03-22 20:55:43.591807 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/create_feature_store_request.py
--rw-r--r--   0        0        0     1323 2023-03-22 20:55:43.538533 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/create_feature_store_request_offline_store_config.py
--rw-r--r--   0        0        0     1832 2023-03-22 20:55:43.581484 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/entity.py
--rw-r--r--   0        0        0     1721 2023-03-22 20:55:43.578194 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature.py
--rw-r--r--   0        0        0     3878 2023-03-22 20:55:43.649694 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_store.py
--rw-r--r--   0        0        0     1252 2023-03-22 20:55:43.558771 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_store_offline_store_config.py
--rw-r--r--   0        0        0      175 2023-03-22 20:55:42.320963 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_store_sync_result.py
--rw-r--r--   0        0        0     1148 2023-03-22 20:55:43.562270 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_tags.py
--rw-r--r--   0        0        0     3863 2023-03-22 20:55:43.690892 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_view.py
--rw-r--r--   0        0        0     3261 2023-03-22 20:55:43.682470 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_view_request.py
--rw-r--r--   0        0        0     1209 2023-03-22 20:55:43.591240 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_view_request_tags.py
--rw-r--r--   0        0        0     1171 2023-03-22 20:55:43.590373 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_view_tags.py
--rw-r--r--   0        0        0     2968 2023-03-22 20:55:43.689231 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/field.py
--rw-r--r--   0        0        0      340 2023-03-22 20:55:42.291611 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/git_provider_name.py
--rw-r--r--   0        0        0     2405 2023-03-22 20:55:43.681639 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/lock_feature_store_request.py
--rw-r--r--   0        0        0     1750 2023-03-22 20:55:43.658307 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/metadata.py
--rw-r--r--   0        0        0     2552 2023-03-22 20:55:43.688892 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/offline_store_config.py
--rw-r--r--   0        0        0     1556 2023-03-22 20:55:43.672272 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/offline_store_config_fields.py
--rw-r--r--   0        0        0      219 2023-03-22 20:55:42.310466 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/offline_store_type.py
--rw-r--r--   0        0        0     1895 2023-03-22 20:55:43.683506 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/unlock_feature_store_request.py
--rw-r--r--   0        0        0     2459 2023-04-03 15:43:18.647763 dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/upsert_feature_views_request.py
--rw-r--r--   0        0        0      939 2023-03-22 20:55:43.653052 dominodatalab_data-5.6.0.dev2/feature_store_api_client/types.py
--rw-r--r--   0        0        0     3770 2023-04-03 19:06:42.714768 dominodatalab_data-5.6.0.dev2/pyproject.toml
--rw-r--r--   0        0        0      103 2022-06-17 19:33:52.511546 dominodatalab_data-5.6.0.dev2/training_set_api_client/__init__.py
--rw-r--r--   0        0        0       47 2022-06-17 19:33:52.511807 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-06-17 19:33:52.511995 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     1441 2022-06-17 19:33:52.512214 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/delete_training_set_name.py
--rw-r--r--   0        0        0     1576 2022-06-17 19:33:52.512390 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/delete_training_set_name_number.py
--rw-r--r--   0        0        0     2242 2022-06-17 19:33:52.512565 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/get_training_set_name.py
--rw-r--r--   0        0        0     2525 2022-06-17 19:33:52.512716 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/get_training_set_name_number.py
--rw-r--r--   0        0        0     3679 2022-06-17 19:33:52.512881 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/post_find.py
--rw-r--r--   0        0        0     2832 2022-06-17 19:33:52.513035 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/post_training_set_name.py
--rw-r--r--   0        0        0     3801 2022-06-17 19:33:52.513198 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/post_version_find.py
--rw-r--r--   0        0        0     2716 2022-06-17 19:33:52.513339 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/put_training_set_name.py
--rw-r--r--   0        0        0     3049 2022-06-17 19:33:52.513478 dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/put_training_set_name_number.py
--rw-r--r--   0        0        0     1661 2022-06-17 19:33:52.513626 dominodatalab_data-5.6.0.dev2/training_set_api_client/client.py
--rw-r--r--   0        0        0     1139 2022-06-17 19:33:52.513861 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/__init__.py
--rw-r--r--   0        0        0     3301 2022-06-17 19:33:52.514040 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/create_training_set_version_request.py
--rw-r--r--   0        0        0     1280 2022-06-17 19:33:52.514213 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/create_training_set_version_request_meta.py
--rw-r--r--   0        0        0     1995 2022-06-17 19:33:52.514387 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/monitoring_meta.py
--rw-r--r--   0        0        0     2411 2022-06-17 19:33:52.514750 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set.py
--rw-r--r--   0        0        0     2010 2022-06-17 19:33:52.515025 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_filter.py
--rw-r--r--   0        0        0     1204 2022-06-17 19:33:52.515206 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_filter_meta.py
--rw-r--r--   0        0        0     1171 2022-06-17 19:33:52.515360 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_meta.py
--rw-r--r--   0        0        0     4472 2022-06-17 19:33:52.515516 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version.py
--rw-r--r--   0        0        0     2545 2022-06-17 19:33:52.515673 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version_filter.py
--rw-r--r--   0        0        0     1242 2022-06-17 19:33:52.515825 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version_filter_meta.py
--rw-r--r--   0        0        0     1303 2022-06-17 19:33:52.515970 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version_filter_training_set_meta.py
--rw-r--r--   0        0        0     1209 2022-06-17 19:33:52.516132 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version_meta.py
--rw-r--r--   0        0        0     1844 2022-06-17 19:33:52.516276 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/update_training_set_request.py
--rw-r--r--   0        0        0     1242 2022-06-17 19:33:52.516430 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/update_training_set_request_meta.py
--rw-r--r--   0        0        0     3070 2022-06-17 19:33:52.516575 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/update_training_set_version_request.py
--rw-r--r--   0        0        0     1280 2022-06-17 19:33:52.516715 dominodatalab_data-5.6.0.dev2/training_set_api_client/models/update_training_set_version_request_meta.py
--rw-r--r--   0        0        0      984 2022-06-17 19:33:52.516851 dominodatalab_data-5.6.0.dev2/training_set_api_client/types.py
--rw-r--r--   0        0        0     7627 1970-01-01 00:00:00.000000 dominodatalab_data-5.6.0.dev2/setup.py
--rw-r--r--   0        0        0     7450 1970-01-01 00:00:00.000000 dominodatalab_data-5.6.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0    10891 2022-12-13 21:08:46.883572 dominodatalab_data-5.7.0/LICENSE
+-rw-r--r--   0        0        0     5982 2023-06-30 18:10:37.170554 dominodatalab_data-5.7.0/README.md
+-rw-r--r--   0        0        0      102 2022-12-13 21:08:46.888200 dominodatalab_data-5.7.0/datasource_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-12-13 21:08:46.888449 dominodatalab_data-5.7.0/datasource_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.888635 dominodatalab_data-5.7.0/datasource_api_client/api/datasource/__init__.py
+-rw-r--r--   0        0        0     4143 2023-06-21 23:24:10.676184 dominodatalab_data-5.7.0/datasource_api_client/api/datasource/get_datasource_by_name.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.889007 dominodatalab_data-5.7.0/datasource_api_client/api/proxy/__init__.py
+-rw-r--r--   0        0        0     3381 2022-12-13 21:08:46.889155 dominodatalab_data-5.7.0/datasource_api_client/api/proxy/get_key_url.py
+-rw-r--r--   0        0        0     3434 2022-12-13 21:08:46.889278 dominodatalab_data-5.7.0/datasource_api_client/api/proxy/list_keys.py
+-rw-r--r--   0        0        0     2204 2022-12-13 21:08:46.889429 dominodatalab_data-5.7.0/datasource_api_client/api/proxy/log_metric.py
+-rw-r--r--   0        0        0     1661 2022-12-13 21:08:46.889565 dominodatalab_data-5.7.0/datasource_api_client/client.py
+-rw-r--r--   0        0        0      695 2022-12-13 21:08:46.889828 dominodatalab_data-5.7.0/datasource_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1173 2022-12-13 21:08:46.890343 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_config.py
+-rw-r--r--   0        0        0     4708 2022-12-13 21:08:46.890492 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto.py
+-rw-r--r--   0        0        0     1199 2022-12-13 21:08:46.890641 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_added_by.py
+-rw-r--r--   0        0        0      428 2023-01-20 00:18:54.638950 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_auth_type.py
+-rw-r--r--   0        0        0      712 2023-01-20 00:18:54.639696 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_data_source_type.py
+-rw-r--r--   0        0        0      170 2022-12-13 21:08:46.891095 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_status.py
+-rw-r--r--   0        0        0     1905 2022-12-13 21:08:46.891294 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_owner_info.py
+-rw-r--r--   0        0        0     1498 2022-12-13 21:08:46.891428 dominodatalab_data-5.7.0/datasource_api_client/models/error_response.py
+-rw-r--r--   0        0        0     3569 2022-12-13 21:08:46.891567 dominodatalab_data-5.7.0/datasource_api_client/models/key_request.py
+-rw-r--r--   0        0        0     3880 2022-12-13 21:08:46.891715 dominodatalab_data-5.7.0/datasource_api_client/models/list_request.py
+-rw-r--r--   0        0        0      153 2022-12-13 21:08:46.891858 dominodatalab_data-5.7.0/datasource_api_client/models/log_metric_m.py
+-rw-r--r--   0        0        0      239 2022-12-13 21:08:46.891994 dominodatalab_data-5.7.0/datasource_api_client/models/log_metric_t.py
+-rw-r--r--   0        0        0     2084 2022-12-13 21:08:46.892129 dominodatalab_data-5.7.0/datasource_api_client/models/proxy_error_response.py
+-rw-r--r--   0        0        0      939 2022-12-13 21:08:46.892280 dominodatalab_data-5.7.0/datasource_api_client/types.py
+-rw-r--r--   0        0        0      369 2022-12-13 21:08:46.893659 dominodatalab_data-5.7.0/domino_data/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.893983 dominodatalab_data-5.7.0/domino_data/_feature_store/__init__.py
+-rw-r--r--   0        0        0     3801 2023-02-06 21:42:31.303590 dominodatalab_data-5.7.0/domino_data/_feature_store/client.py
+-rw-r--r--   0        0        0      684 2022-12-13 21:08:46.894282 dominodatalab_data-5.7.0/domino_data/_feature_store/exceptions.py
+-rw-r--r--   0        0        0     2966 2023-01-04 19:29:57.407758 dominodatalab_data-5.7.0/domino_data/_feature_store/git.py
+-rw-r--r--   0        0        0      683 2023-01-04 19:29:57.408054 dominodatalab_data-5.7.0/domino_data/_feature_store/logging.py
+-rw-r--r--   0        0        0     1223 2023-01-04 19:29:57.408553 dominodatalab_data-5.7.0/domino_data/_feature_store/run.py
+-rw-r--r--   0        0        0     8180 2023-02-06 21:42:31.304886 dominodatalab_data-5.7.0/domino_data/_feature_store/sync.py
+-rw-r--r--   0        0        0     4527 2022-12-13 21:08:46.894894 dominodatalab_data-5.7.0/domino_data/auth.py
+-rw-r--r--   0        0        0    10464 2023-02-06 21:42:28.586341 dominodatalab_data-5.7.0/domino_data/configuration_gen.py
+-rw-r--r--   0        0        0    27063 2023-06-30 22:30:47.388304 dominodatalab_data-5.7.0/domino_data/data_sources.py
+-rw-r--r--   0        0        0      894 2023-01-04 19:29:57.409242 dominodatalab_data-5.7.0/domino_data/logging.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895616 dominodatalab_data-5.7.0/domino_data/py.typed
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895810 dominodatalab_data-5.7.0/domino_data/training_sets/__init__.py
+-rw-r--r--   0        0        0    13955 2022-12-13 21:08:46.895997 dominodatalab_data-5.7.0/domino_data/training_sets/client.py
+-rw-r--r--   0        0        0     3588 2022-12-13 21:08:46.896143 dominodatalab_data-5.7.0/domino_data/training_sets/model.py
+-rw-r--r--   0        0        0     2550 2023-06-30 22:30:47.388714 dominodatalab_data-5.7.0/domino_data/transfer.py
+-rw-r--r--   0        0        0      104 2022-12-13 21:08:46.896371 dominodatalab_data-5.7.0/feature_store_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-12-13 21:08:46.896618 dominodatalab_data-5.7.0/feature_store_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.896866 dominodatalab_data-5.7.0/feature_store_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     2657 2022-12-13 21:08:46.897016 dominodatalab_data-5.7.0/feature_store_api_client/api/default/get.py
+-rw-r--r--   0        0        0     2861 2022-12-13 21:08:46.897152 dominodatalab_data-5.7.0/feature_store_api_client/api/default/get_feature_view_name_store.py
+-rw-r--r--   0        0        0     3383 2022-12-13 21:08:46.897295 dominodatalab_data-5.7.0/feature_store_api_client/api/default/post.py
+-rw-r--r--   0        0        0     1870 2022-12-13 21:08:46.897427 dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_featureview.py
+-rw-r--r--   0        0        0     3215 2022-12-13 21:08:46.897553 dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_lock.py
+-rw-r--r--   0        0        0     3144 2022-12-13 21:08:46.897705 dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_unlock.py
+-rw-r--r--   0        0        0     1822 2022-12-13 21:08:46.897860 dominodatalab_data-5.7.0/feature_store_api_client/client.py
+-rw-r--r--   0        0        0     1443 2023-02-06 21:42:31.307225 dominodatalab_data-5.7.0/feature_store_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2002 2022-12-13 21:08:46.898606 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config.py
+-rw-r--r--   0        0        0     1513 2022-12-13 21:08:46.898839 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config_fields.py
+-rw-r--r--   0        0        0     1166 2022-12-13 21:08:46.898998 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config_meta.py
+-rw-r--r--   0        0        0      170 2022-12-13 21:08:46.899130 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_field_name.py
+-rw-r--r--   0        0        0      197 2022-12-13 21:08:46.899246 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_type.py
+-rw-r--r--   0        0        0      668 2022-12-13 21:08:46.899363 dominodatalab_data-5.7.0/feature_store_api_client/models/config_field_name.py
+-rw-r--r--   0        0        0     2987 2022-12-13 21:08:46.899487 dominodatalab_data-5.7.0/feature_store_api_client/models/create_feature_store_request.py
+-rw-r--r--   0        0        0     1323 2022-12-13 21:08:46.899636 dominodatalab_data-5.7.0/feature_store_api_client/models/create_feature_store_request_offline_store_config.py
+-rw-r--r--   0        0        0     1832 2022-12-13 21:08:46.899849 dominodatalab_data-5.7.0/feature_store_api_client/models/entity.py
+-rw-r--r--   0        0        0     1721 2023-02-06 21:42:31.308456 dominodatalab_data-5.7.0/feature_store_api_client/models/feature.py
+-rw-r--r--   0        0        0     3878 2022-12-13 21:08:46.900117 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store.py
+-rw-r--r--   0        0        0     1252 2022-12-13 21:08:46.900229 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store_offline_store_config.py
+-rw-r--r--   0        0        0      175 2022-12-13 21:08:46.900333 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store_sync_result.py
+-rw-r--r--   0        0        0     1148 2023-02-06 21:42:31.309808 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_tags.py
+-rw-r--r--   0        0        0     3863 2022-12-13 21:08:46.900460 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view.py
+-rw-r--r--   0        0        0     3261 2023-02-06 21:42:31.311302 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_request.py
+-rw-r--r--   0        0        0     1209 2022-12-13 21:08:46.900686 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_request_tags.py
+-rw-r--r--   0        0        0     1171 2022-12-13 21:08:46.901421 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_tags.py
+-rw-r--r--   0        0        0     2968 2022-12-13 21:08:46.901544 dominodatalab_data-5.7.0/feature_store_api_client/models/field.py
+-rw-r--r--   0        0        0      340 2022-12-13 21:08:46.901657 dominodatalab_data-5.7.0/feature_store_api_client/models/git_provider_name.py
+-rw-r--r--   0        0        0     2405 2022-12-13 21:08:46.901774 dominodatalab_data-5.7.0/feature_store_api_client/models/lock_feature_store_request.py
+-rw-r--r--   0        0        0     1750 2022-12-13 21:08:46.901882 dominodatalab_data-5.7.0/feature_store_api_client/models/metadata.py
+-rw-r--r--   0        0        0     2552 2022-12-13 21:08:46.901982 dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_config.py
+-rw-r--r--   0        0        0     1556 2022-12-13 21:08:46.902065 dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_config_fields.py
+-rw-r--r--   0        0        0      219 2022-12-13 21:08:46.902164 dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_type.py
+-rw-r--r--   0        0        0     1895 2022-12-13 21:08:46.902282 dominodatalab_data-5.7.0/feature_store_api_client/models/unlock_feature_store_request.py
+-rw-r--r--   0        0        0     2459 2023-02-06 21:42:31.312038 dominodatalab_data-5.7.0/feature_store_api_client/models/upsert_feature_views_request.py
+-rw-r--r--   0        0        0      939 2022-12-13 21:08:46.902477 dominodatalab_data-5.7.0/feature_store_api_client/types.py
+-rw-r--r--   0        0        0     3831 2023-06-30 22:49:15.478754 dominodatalab_data-5.7.0/pyproject.toml
+-rw-r--r--   0        0        0      103 2022-12-13 21:08:46.910476 dominodatalab_data-5.7.0/training_set_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-12-13 21:08:46.910619 dominodatalab_data-5.7.0/training_set_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.910785 dominodatalab_data-5.7.0/training_set_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     1441 2022-12-13 21:08:46.910908 dominodatalab_data-5.7.0/training_set_api_client/api/default/delete_training_set_name.py
+-rw-r--r--   0        0        0     1576 2022-12-13 21:08:46.911013 dominodatalab_data-5.7.0/training_set_api_client/api/default/delete_training_set_name_number.py
+-rw-r--r--   0        0        0     2242 2022-12-13 21:08:46.911099 dominodatalab_data-5.7.0/training_set_api_client/api/default/get_training_set_name.py
+-rw-r--r--   0        0        0     2525 2022-12-13 21:08:46.911182 dominodatalab_data-5.7.0/training_set_api_client/api/default/get_training_set_name_number.py
+-rw-r--r--   0        0        0     3679 2022-12-13 21:08:46.911276 dominodatalab_data-5.7.0/training_set_api_client/api/default/post_find.py
+-rw-r--r--   0        0        0     2832 2022-12-13 21:08:46.911364 dominodatalab_data-5.7.0/training_set_api_client/api/default/post_training_set_name.py
+-rw-r--r--   0        0        0     3801 2022-12-13 21:08:46.911452 dominodatalab_data-5.7.0/training_set_api_client/api/default/post_version_find.py
+-rw-r--r--   0        0        0     2716 2022-12-13 21:08:46.911584 dominodatalab_data-5.7.0/training_set_api_client/api/default/put_training_set_name.py
+-rw-r--r--   0        0        0     3049 2022-12-13 21:08:46.911684 dominodatalab_data-5.7.0/training_set_api_client/api/default/put_training_set_name_number.py
+-rw-r--r--   0        0        0     1661 2022-12-13 21:08:46.911774 dominodatalab_data-5.7.0/training_set_api_client/client.py
+-rw-r--r--   0        0        0     1139 2022-12-13 21:08:46.911917 dominodatalab_data-5.7.0/training_set_api_client/models/__init__.py
+-rw-r--r--   0        0        0     3301 2022-12-13 21:08:46.912007 dominodatalab_data-5.7.0/training_set_api_client/models/create_training_set_version_request.py
+-rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.912105 dominodatalab_data-5.7.0/training_set_api_client/models/create_training_set_version_request_meta.py
+-rw-r--r--   0        0        0     1995 2022-12-13 21:08:46.912303 dominodatalab_data-5.7.0/training_set_api_client/models/monitoring_meta.py
+-rw-r--r--   0        0        0     2411 2022-12-13 21:08:46.912407 dominodatalab_data-5.7.0/training_set_api_client/models/training_set.py
+-rw-r--r--   0        0        0     2010 2022-12-13 21:08:46.912513 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_filter.py
+-rw-r--r--   0        0        0     1204 2022-12-13 21:08:46.912628 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_filter_meta.py
+-rw-r--r--   0        0        0     1171 2022-12-13 21:08:46.912764 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_meta.py
+-rw-r--r--   0        0        0     4472 2022-12-13 21:08:46.912863 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version.py
+-rw-r--r--   0        0        0     2545 2022-12-13 21:08:46.912963 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter.py
+-rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913081 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter_meta.py
+-rw-r--r--   0        0        0     1303 2022-12-13 21:08:46.913192 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter_training_set_meta.py
+-rw-r--r--   0        0        0     1209 2022-12-13 21:08:46.913297 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_meta.py
+-rw-r--r--   0        0        0     1844 2022-12-13 21:08:46.913396 dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_request.py
+-rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913504 dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_request_meta.py
+-rw-r--r--   0        0        0     3070 2022-12-13 21:08:46.913600 dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_version_request.py
+-rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.913689 dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_version_request_meta.py
+-rw-r--r--   0        0        0      984 2022-12-13 21:08:46.913773 dominodatalab_data-5.7.0/training_set_api_client/types.py
+-rw-r--r--   0        0        0     7310 1970-01-01 00:00:00.000000 dominodatalab_data-5.7.0/PKG-INFO
```

### Comparing `dominodatalab_data-5.6.0.dev2/LICENSE` & `dominodatalab_data-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/README.md` & `dominodatalab_data-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/api/datasource/get_datasource_by_name.py` & `dominodatalab_data-5.7.0/datasource_api_client/api/datasource/get_datasource_by_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/api/proxy/get_key_url.py` & `dominodatalab_data-5.7.0/datasource_api_client/api/proxy/get_key_url.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/api/proxy/list_keys.py` & `dominodatalab_data-5.7.0/datasource_api_client/api/proxy/list_keys.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/api/proxy/log_metric.py` & `dominodatalab_data-5.7.0/datasource_api_client/api/proxy/log_metric.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/client.py` & `dominodatalab_data-5.7.0/datasource_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/__init__.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_config.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_dto.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_dto_added_by.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_added_by.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_dto_data_source_type.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_data_source_type.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/datasource_owner_info.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_owner_info.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/error_response.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/key_request.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/key_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/list_request.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/list_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/models/proxy_error_response.py` & `dominodatalab_data-5.7.0/datasource_api_client/models/proxy_error_response.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/datasource_api_client/types.py` & `dominodatalab_data-5.7.0/datasource_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/client.py` & `dominodatalab_data-5.7.0/domino_data/_feature_store/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/exceptions.py` & `dominodatalab_data-5.7.0/domino_data/_feature_store/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/git.py` & `dominodatalab_data-5.7.0/domino_data/_feature_store/git.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/logging.py` & `dominodatalab_data-5.7.0/domino_data/_feature_store/logging.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/run.py` & `dominodatalab_data-5.7.0/domino_data/_feature_store/run.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/_feature_store/sync.py` & `dominodatalab_data-5.7.0/domino_data/_feature_store/sync.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/auth.py` & `dominodatalab_data-5.7.0/domino_data/auth.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/configuration_gen.py` & `dominodatalab_data-5.7.0/domino_data/configuration_gen.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/data_sources.py` & `dominodatalab_data-5.7.0/domino_data/data_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import os
 
 import attr
 import backoff
 import httpx
 import pandas
+import urllib3
 from pyarrow import ArrowException, flight, parquet
 
 import domino_data.configuration_gen
 from datasource_api_client.api.datasource import get_datasource_by_name
 from datasource_api_client.api.proxy import get_key_url, list_keys, log_metric
 from datasource_api_client.models import DatasourceConfig as APIConfig
 from datasource_api_client.models import (
@@ -26,14 +27,15 @@
     LogMetricT,
     ProxyErrorResponse,
 )
 
 from .auth import AuthenticatedClient, AuthMiddlewareFactory, ProxyClient, get_jwt_token
 from .configuration_gen import Config, CredElem, DatasourceConfig, find_datasource_klass
 from .logging import logger
+from .transfer import MAX_WORKERS, BlobTransfer
 
 ACCEPT_HEADERS = {"Accept": "application/json"}
 ADLS_HEADERS = {"X-Ms-Blob-Type": "BlockBlob"}
 
 CREDENTIAL_TYPE = "credential"
 CONFIGURATION_TYPE = "configuration"
 
@@ -105,14 +107,18 @@
     datasource: "ObjectStoreDatasource" = attr.ib(repr=False)
     key: str = attr.ib()
 
     def http(self) -> httpx.Client:
         """Get datasource http client."""
         return self.datasource.http()
 
+    def pool_manager(self) -> urllib3.PoolManager:
+        """Get datasource http pool manager."""
+        return self.datasource.pool_manager()
+
     def get(self) -> bytes:
         """Get object content as bytes."""
         url = self.datasource.get_key_url(self.key, False)
         res = self.http().get(url)
         res.raise_for_status()
 
         self.datasource.client._log_metric(  # pylint: disable=protected-access
@@ -140,14 +146,33 @@
 
         self.datasource.client._log_metric(  # pylint: disable=protected-access
             self.datasource.datasource_type,
             content_size,
             False,
         )
 
+    def download(self, filename: str, max_workers: int = MAX_WORKERS) -> None:
+        """Download object content to file with multithreaded support.
+
+        The file will be created if it does not exists. File will be overwritten if it exists.
+
+        Args:
+            filename: path of file to write content to
+            max_workers: max parallelism for high speed download
+        """
+        url = self.datasource.get_key_url(self.key, False)
+        with open(filename, "wb") as file:
+            blob = BlobTransfer(url, file, max_workers=max_workers, http=self.pool_manager())
+
+        self.datasource.client._log_metric(  # pylint: disable=protected-access
+            self.datasource.datasource_type,
+            blob.content_size,
+            False,
+        )
+
     def download_fileobj(self, fileobj: Any) -> None:
         """Download object content to file like object.
 
         Args:
             fileobj: A file-like object to download into.
                 At a minimum, it must implement the write method and must accept bytes.
         """
@@ -312,14 +337,23 @@
             self._httpx = httpx.Client(headers=ADLS_HEADERS, verify=context)
         elif self.datasource_type == DatasourceDtoDataSourceType.GENERICS3CONFIG.value:
             self._httpx = httpx.Client(verify=False)  # nosec
         else:
             self._httpx = httpx.Client(verify=context)
         return self._httpx
 
+    def pool_manager(self) -> urllib3.PoolManager:
+        """Urllib3 pool manager for range downloads."""
+        if self.datasource_type == DatasourceDtoDataSourceType.ADLSCONFIG.value:
+            return urllib3.PoolManager(headers=ADLS_HEADERS)
+        elif self.datasource_type == DatasourceDtoDataSourceType.GENERICS3CONFIG.value:
+            return urllib3.PoolManager(assert_hostname=False)
+        else:
+            return urllib3.PoolManager()
+
     def _get_credential_override(self) -> Dict[str, str]:
         """Gets credentials override by merging service overrides and user overrides"""
         credentials = {}
 
         if self.auth_type == DatasourceDtoAuthType.OAUTH.value:
             credentials = load_oauth_credentials()
 
@@ -442,14 +476,26 @@
 
         Args:
             object_key: unique key of object
             filename: path of file to write content to.
         """
         self.Object(object_key).download_file(filename)
 
+    def download(self, object_key: str, filename: str, max_workers: int = MAX_WORKERS) -> None:
+        """Download object content to file located at filename.
+
+        The file will be created if it does not exists.
+
+        Args:
+            object_key: unique key of object
+            filename: path of file to write content to
+            max_workers: max parallelism for high speed download
+        """
+        self.Object(object_key).download(filename, max_workers)
+
     def download_fileobj(self, object_key: str, fileobj: Any) -> None:
         """Download object content to file like object.
 
         Args:
             object_key: unique key of object
             fileobj: A file-like object to download into.
                 At a minimum, it must implement the write method and must accept bytes.
```

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/logging.py` & `dominodatalab_data-5.7.0/domino_data/logging.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/training_sets/client.py` & `dominodatalab_data-5.7.0/domino_data/training_sets/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/domino_data/training_sets/model.py` & `dominodatalab_data-5.7.0/domino_data/training_sets/model.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/get.py` & `dominodatalab_data-5.7.0/feature_store_api_client/api/default/get.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/get_feature_view_name_store.py` & `dominodatalab_data-5.7.0/feature_store_api_client/api/default/get_feature_view_name_store.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/post.py` & `dominodatalab_data-5.7.0/feature_store_api_client/api/default/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/post_featureview.py` & `dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_featureview.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/post_lock.py` & `dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_lock.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/api/default/post_unlock.py` & `dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_unlock.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/client.py` & `dominodatalab_data-5.7.0/feature_store_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/__init__.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/auth_config.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/auth_config_fields.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config_fields.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/auth_config_meta.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/config_field_name.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/config_field_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/create_feature_store_request.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/create_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/create_feature_store_request_offline_store_config.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/create_feature_store_request_offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/entity.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/entity.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/feature.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_store.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_store_offline_store_config.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store_offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_tags.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_view.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_view_request.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_view_request_tags.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_request_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/feature_view_tags.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/field.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/field.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/lock_feature_store_request.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/lock_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/metadata.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/offline_store_config.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/offline_store_config_fields.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_config_fields.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/unlock_feature_store_request.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/unlock_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/models/upsert_feature_views_request.py` & `dominodatalab_data-5.7.0/feature_store_api_client/models/upsert_feature_views_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/feature_store_api_client/types.py` & `dominodatalab_data-5.7.0/feature_store_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/pyproject.toml` & `dominodatalab_data-5.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dominodatalab-data"
-version = "5.6.0dev2"
+version = "5.7.0"
 description = "Domino Data API for interacting with Domino Data features"
 readme = "README.md"
 authors = [
     "Gabriel Haim <gabriel.haim@dominodatalab.com>",
     "Aaron Read <aaron.read@dominodatalab.com>",
 ]
 license = "Apache Software License 2.0"
@@ -25,22 +25,23 @@
 ]
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []  #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [  #! Update me
-  "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.group.main.dependencies]
 python = "^3.8"
 pandas = ">=1.3.0"
 httpx = "^0.23.0"
 attrs = ">=20.1.0,<22.0.0"
@@ -48,40 +49,40 @@
 pyarrow = "^8.0.0"
 loguru = "^0.5.3"
 backoff = "^1.11.1"
 bson = "^0.5.10"
 
 [tool.poetry.group.dev.dependencies]
 Sphinx = "^5.3.0"
-bandit = "^1.7.0"
-black = {version = "^22.3.0", allow-prereleases = true}
-darglint = "^1.8.0"
+bandit = "^1.7.5"
+black = {version = "^22.12.0", allow-prereleases = true}
+darglint = "^1.8.1"
 flake8 = "^4.0.1"
-grpcio = "^1.41.0"
-isort = {extras = ["colors"], version = "^5.9.3"}
-mypy = "^0.910"
-mypy-extensions = "^0.4.3"
-openapi-python-client = "^0.11.1"
+grpcio = "^1.56.0"
+isort = {extras = ["colors"], version = "^5.12.0"}
+mypy = "^1.4.1"
+mypy-extensions = "^1.0.0"
+openapi-python-client = "^0.11.6"
 pdbpp = "^0.10.3"
-pre-commit = "^2.13.0"
-pydocstyle = "^6.1.1"
-pylint = "^2.9.6"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-pytest-recording = "^0.12.0"
-pyupgrade = "^2.23.1"
+pre-commit = "^2.21.0"
+pydocstyle = "^6.3.0"
+pylint = "^2.17.4"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+pytest-recording = "^0.12.2"
+pyupgrade = "^2.38.4"
 respx = "^0.20.1"
-safety = "^2.3.1"
-sphinx-rtd-theme = "^1.1.1"
-types-PyYAML = "^6.0.4"
-types-python-dateutil = "^2.8.19.4"
+safety = "^2.3.5"
+sphinx-rtd-theme = "^1.2.2"
+types-PyYAML = "^6.0.12.10"
+types-python-dateutil = "^2.8.19.13"
 
 [tool.poetry.group.featurestore.dependencies]
 feast = "^0.29.0"
-GitPython = "^3.1.30"
+GitPython = "^3.1.31"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 100
 color = true
```

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/delete_training_set_name.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/delete_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/delete_training_set_name_number.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/delete_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/get_training_set_name.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/get_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/get_training_set_name_number.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/get_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/post_find.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/post_find.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/post_training_set_name.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/post_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/post_version_find.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/post_version_find.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/put_training_set_name.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/put_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/api/default/put_training_set_name_number.py` & `dominodatalab_data-5.7.0/training_set_api_client/api/default/put_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/client.py` & `dominodatalab_data-5.7.0/training_set_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/__init__.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/create_training_set_version_request.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/create_training_set_version_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/create_training_set_version_request_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/create_training_set_version_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/monitoring_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/monitoring_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_filter.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_filter.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_filter_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_filter_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version_filter.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version_filter_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version_filter_training_set_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter_training_set_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/training_set_version_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/update_training_set_request.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/update_training_set_request_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/update_training_set_version_request.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_version_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/models/update_training_set_version_request_meta.py` & `dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_version_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/training_set_api_client/types.py` & `dominodatalab_data-5.7.0/training_set_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.6.0.dev2/setup.py` & `dominodatalab_data-5.7.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,279 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dominodatalab-data
+Version: 5.7.0
+Summary: Domino Data API for interacting with Domino Data features
+Home-page: https://github.com/dominodatalab/domino-data
+License: Apache Software License 2.0
+Author: Gabriel Haim
+Author-email: gabriel.haim@dominodatalab.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: attrs (>=20.1.0,<22.0.0)
+Requires-Dist: backoff (>=1.11.1,<2.0.0)
+Requires-Dist: bson (>=0.5.10,<0.6.0)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: loguru (>=0.5.3,<0.6.0)
+Requires-Dist: pandas (>=1.3.0)
+Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
+Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
+Project-URL: Repository, https://github.com/dominodatalab/domino-data
+Description-Content-Type: text/markdown
 
-packages = \
-['datasource_api_client',
- 'datasource_api_client.api',
- 'datasource_api_client.api.datasource',
- 'datasource_api_client.api.proxy',
- 'datasource_api_client.models',
- 'domino_data',
- 'domino_data._feature_store',
- 'domino_data.training_sets',
- 'feature_store_api_client',
- 'feature_store_api_client.api',
- 'feature_store_api_client.api.default',
- 'feature_store_api_client.models',
- 'training_set_api_client',
- 'training_set_api_client.api',
- 'training_set_api_client.api.default',
- 'training_set_api_client.models']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=20.1.0,<22.0.0',
- 'backoff>=1.11.1,<2.0.0',
- 'bson>=0.5.10,<0.6.0',
- 'httpx>=0.23.0,<0.24.0',
- 'loguru>=0.5.3,<0.6.0',
- 'pandas>=1.3.0',
- 'pyarrow>=8.0.0,<9.0.0',
- 'python-dateutil>=2.8.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'dominodatalab-data',
-    'version': '5.6.0.dev2',
-    'description': 'Domino Data API for interacting with Domino Data features',
-    'long_description': '# Domino Data API\n\n<div align="center">\n\n[![Build status](https://github.com/dominodatalab/domino-data/workflows/build/badge.svg?branch=main&event=push)](https://github.com/dominodatalab/domino-data/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/dominodatalab-data.svg)](https://pypi.org/project/dominodatalab-data/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/dominodatalab/domino-data/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/dominodatalab/domino-data/blob/main/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/dominodatalab/domino-data/releases)\n[![License](https://img.shields.io/github/license/dominodatalab/domino-data)](https://github.com/dominodatalab/domino-data/blob/main/LICENSE)\n\nDomino Data API for interacting with Access Data features\n\n</div>\n\n## Installation\n\n```bash\npip install -U dominodatalab-data\n```\n\nor install with `Poetry`\n\n```bash\npoetry add dominodatalab-data\n```\n\n### Makefile usage\n\n[`Makefile`](https://github.com/dominodatalab/domino-data/blob/main/Makefile) contains a lot of functions for faster development.\n\n<details>\n<summary>1. Download and remove Poetry</summary>\n<p>\n\nTo download and install Poetry run:\n\n```bash\nmake poetry-download\n```\n\nTo uninstall\n\n```bash\nmake poetry-remove\n```\n\n</p>\n</details>\n\n<details>\n<summary>2. Install all dependencies and pre-commit hooks</summary>\n<p>\n\nInstall requirements:\n\n```bash\nmake install\n```\n\nPre-commit hooks coulb be installed after `git init` via\n\n```bash\nmake pre-commit-install\n```\n\n</p>\n</details>\n\n<details>\n<summary>3. Codestyle</summary>\n<p>\n\nAutomatic formatting uses `pyupgrade`, `isort` and `black`.\n\n```bash\nmake codestyle\n\n# or use synonym\nmake formatting\n```\n\nCodestyle checks only, without rewriting files:\n\n```bash\nmake check-codestyle\n```\n\n> Note: `check-codestyle` uses `isort`, `black` and `darglint` library\n\n<details>\n<summary>4. Code security</summary>\n<p>\n\n```bash\nmake check-safety\n```\n\nThis command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.\n\n```bash\nmake check-safety\n```\n\n</p>\n</details>\n\n</p>\n</details>\n\n<details>\n<summary>5. Type checks</summary>\n<p>\n\nRun `mypy` static type checker\n\n```bash\nmake mypy\n```\n\n</p>\n</details>\n\n<details>\n<summary>6. Tests</summary>\n<p>\n\nRun `pytest`\n\n```bash\nmake test\n```\n\n</p>\n</details>\n\n<details>\n<summary>7. All linters</summary>\n<p>\n\nOf course there is a command to ~~rule~~ run all linters in one:\n\n```bash\nmake lint\n```\n\nthe same as:\n\n```bash\nmake test && make check-codestyle && make mypy && make check-safety\n```\n\n</p>\n</details>\n\n<details>\n<summary>8. Cleanup</summary>\n<p>\n\nDelete pycache files\n\n```bash\nmake pycache-remove\n```\n\nRemove package build\n\n```bash\nmake build-remove\n```\n\nOr to remove pycache and build:\n\n```bash\nmake clean-all\n```\n\n</p>\n</details>\n\n<details>\n<summary>9. Docs</summary>\n<p>\n\nBuild the documentation\n\n```bash\nmake docs\n```\n\nOpen the docs index page\n\n```bash\nmake open-docs\n```\n\n</p>\n</details>\n\n## 📈 Releases\n\nYou can see the list of available releases on the [GitHub Releases](https://github.com/dominodatalab/domino-data/releases) page.\n\nWe follow [Semantic Versions](https://semver.org/) specification.\n\nWe use [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). As pull requests are merged, a draft release is kept up-to-date listing the changes, ready to publish when you’re ready. With the categories option, you can categorize pull requests in release notes using labels.\n\n### List of labels and corresponding titles\n\n|               **Label**               |  **Title in Releases**  |\n| :-----------------------------------: | :---------------------: |\n|       `enhancement`, `feature`        |       🚀 Features       |\n| `bug`, `refactoring`, `bugfix`, `fix` | 🔧 Fixes & Refactoring  |\n|       `build`, `ci`, `testing`        | 📦 Build System & CI/CD |\n|              `breaking`               |   💥 Breaking Changes   |\n|            `documentation`            |    📝 Documentation     |\n|            `dependencies`             | ⬆️ Dependencies updates |\n\nYou can update it in [`release-drafter.yml`](https://github.com/dominodatalab/domino-data/blob/main/.github/release-drafter.yml).\n\nGitHub creates the `bug`, `enhancement`, and `documentation` labels for you. Dependabot creates the `dependencies` label. Create the remaining labels on the Issues tab of your GitHub repository, when you need them.\n\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/dominodatalab/domino-data)](https://github.com/dominodatalab/domino-data/blob/main/LICENSE)\n\nThis project is licensed under the terms of the `Apache Software License 2.0` license. See [LICENSE](https://github.com/dominodatalab/domino-data/blob/main/LICENSE) for more details.\n\n## 📃 Citation\n\n```bibtex\n@misc{dominodatalab-data,\n  author = {dominodatalab},\n  title = {Domino Data API for interacting with Access Data features},\n  year = {2021},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/dominodatalab/domino-data}}\n}\n```\n\n## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)\n\nThis project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)\n',
-    'author': 'Gabriel Haim',
-    'author_email': 'gabriel.haim@dominodatalab.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dominodatalab/domino-data',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+# Domino Data API
+
+<div align="center">
+
+[![Build status](https://github.com/dominodatalab/domino-data/workflows/build/badge.svg?branch=main&event=push)](https://github.com/dominodatalab/domino-data/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/dominodatalab-data.svg)](https://pypi.org/project/dominodatalab-data/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/dominodatalab/domino-data/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/dominodatalab/domino-data/blob/main/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/dominodatalab/domino-data/releases)
+[![License](https://img.shields.io/github/license/dominodatalab/domino-data)](https://github.com/dominodatalab/domino-data/blob/main/LICENSE)
+
+Domino Data API for interacting with Access Data features
+
+</div>
+
+## Installation
+
+```bash
+pip install -U dominodatalab-data
+```
+
+or install with `Poetry`
+
+```bash
+poetry add dominodatalab-data
+```
+
+### Makefile usage
+
+[`Makefile`](https://github.com/dominodatalab/domino-data/blob/main/Makefile) contains a lot of functions for faster development.
+
+<details>
+<summary>1. Download and remove Poetry</summary>
+<p>
+
+To download and install Poetry run:
+
+```bash
+make poetry-download
+```
+
+To uninstall
+
+```bash
+make poetry-remove
+```
+
+</p>
+</details>
+
+<details>
+<summary>2. Install all dependencies and pre-commit hooks</summary>
+<p>
+
+Install requirements:
+
+```bash
+make install
+```
+
+Pre-commit hooks coulb be installed after `git init` via
+
+```bash
+make pre-commit-install
+```
+
+</p>
+</details>
+
+<details>
+<summary>3. Codestyle</summary>
+<p>
+
+Automatic formatting uses `pyupgrade`, `isort` and `black`.
+
+```bash
+make codestyle
+
+# or use synonym
+make formatting
+```
+
+Codestyle checks only, without rewriting files:
+
+```bash
+make check-codestyle
+```
+
+> Note: `check-codestyle` uses `isort`, `black` and `darglint` library
+
+<details>
+<summary>4. Code security</summary>
+<p>
+
+```bash
+make check-safety
+```
+
+This command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.
+
+```bash
+make check-safety
+```
+
+</p>
+</details>
+
+</p>
+</details>
+
+<details>
+<summary>5. Type checks</summary>
+<p>
+
+Run `mypy` static type checker
+
+```bash
+make mypy
+```
+
+</p>
+</details>
+
+<details>
+<summary>6. Tests</summary>
+<p>
+
+Run `pytest`
+
+```bash
+make test
+```
+
+</p>
+</details>
+
+<details>
+<summary>7. All linters</summary>
+<p>
+
+Of course there is a command to ~~rule~~ run all linters in one:
+
+```bash
+make lint
+```
+
+the same as:
+
+```bash
+make test && make check-codestyle && make mypy && make check-safety
+```
+
+</p>
+</details>
+
+<details>
+<summary>8. Cleanup</summary>
+<p>
+
+Delete pycache files
+
+```bash
+make pycache-remove
+```
+
+Remove package build
+
+```bash
+make build-remove
+```
+
+Or to remove pycache and build:
+
+```bash
+make clean-all
+```
+
+</p>
+</details>
+
+<details>
+<summary>9. Docs</summary>
+<p>
+
+Build the documentation
+
+```bash
+make docs
+```
+
+Open the docs index page
+
+```bash
+make open-docs
+```
+
+</p>
+</details>
+
+## 📈 Releases
+
+You can see the list of available releases on the [GitHub Releases](https://github.com/dominodatalab/domino-data/releases) page.
+
+We follow [Semantic Versions](https://semver.org/) specification.
+
+We use [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). As pull requests are merged, a draft release is kept up-to-date listing the changes, ready to publish when you’re ready. With the categories option, you can categorize pull requests in release notes using labels.
+
+### List of labels and corresponding titles
+
+|               **Label**               |  **Title in Releases**  |
+| :-----------------------------------: | :---------------------: |
+|       `enhancement`, `feature`        |       🚀 Features       |
+| `bug`, `refactoring`, `bugfix`, `fix` | 🔧 Fixes & Refactoring  |
+|       `build`, `ci`, `testing`        | 📦 Build System & CI/CD |
+|              `breaking`               |   💥 Breaking Changes   |
+|            `documentation`            |    📝 Documentation     |
+|            `dependencies`             | ⬆️ Dependencies updates |
+
+You can update it in [`release-drafter.yml`](https://github.com/dominodatalab/domino-data/blob/main/.github/release-drafter.yml).
+
+GitHub creates the `bug`, `enhancement`, and `documentation` labels for you. Dependabot creates the `dependencies` label. Create the remaining labels on the Issues tab of your GitHub repository, when you need them.
+
+## 🛡 License
+
+[![License](https://img.shields.io/github/license/dominodatalab/domino-data)](https://github.com/dominodatalab/domino-data/blob/main/LICENSE)
+
+This project is licensed under the terms of the `Apache Software License 2.0` license. See [LICENSE](https://github.com/dominodatalab/domino-data/blob/main/LICENSE) for more details.
+
+## 📃 Citation
+
+```bibtex
+@misc{dominodatalab-data,
+  author = {dominodatalab},
+  title = {Domino Data API for interacting with Access Data features},
+  year = {2021},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/dominodatalab/domino-data}}
 }
+```
+
+## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
 
+This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)
 
-setup(**setup_kwargs)
```

