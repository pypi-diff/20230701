# Comparing `tmp/guniflask-0.9.1.tar.gz` & `tmp/guniflask-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/guniflask-0.9.1.tar", last modified: Wed Sep 16 07:51:56 2020, max compression
+gzip compressed data, was "dist/guniflask-0.9.2.tar", last modified: Thu Sep 17 13:06:18 2020, max compression
```

## Comparing `guniflask-0.9.1.tar` & `guniflask-0.9.2.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/
--rw-r--r--   0 jadbin     (501) staff       (20)     1063 2020-08-06 02:10:04.000000 guniflask-0.9.1/LICENSE
--rw-r--r--   0 jadbin     (501) staff       (20)      153 2020-08-06 02:10:04.000000 guniflask-0.9.1/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)     2370 2020-09-16 07:51:56.000000 guniflask-0.9.1/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)     1310 2020-09-15 06:36:11.000000 guniflask-0.9.1/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/docs/
--rw-r--r--   0 jadbin     (501) staff       (20)      606 2020-08-06 02:10:04.000000 guniflask-0.9.1/docs/Makefile
--rw-r--r--   0 jadbin     (501) staff       (20)      723 2020-09-15 17:24:04.000000 guniflask-0.9.1/docs/app.rst
--rw-r--r--   0 jadbin     (501) staff       (20)     1006 2020-09-15 17:24:04.000000 guniflask-0.9.1/docs/blueprints.rst
--rw-r--r--   0 jadbin     (501) staff       (20)    10066 2020-09-16 07:46:40.000000 guniflask-0.9.1/docs/changelog.rst
--rw-r--r--   0 jadbin     (501) staff       (20)     5382 2020-08-06 02:10:04.000000 guniflask-0.9.1/docs/conf.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2000 2020-08-06 02:10:04.000000 guniflask-0.9.1/docs/config.rst
--rw-r--r--   0 jadbin     (501) staff       (20)     1250 2020-08-06 02:10:04.000000 guniflask-0.9.1/docs/debug.rst
--rw-r--r--   0 jadbin     (501) staff       (20)      726 2020-08-06 02:10:04.000000 guniflask-0.9.1/docs/deploy.rst
--rw-r--r--   0 jadbin     (501) staff       (20)      613 2020-09-15 06:35:42.000000 guniflask-0.9.1/docs/index.rst
--rw-r--r--   0 jadbin     (501) staff       (20)      831 2020-08-06 02:10:04.000000 guniflask-0.9.1/docs/log.rst
--rw-r--r--   0 jadbin     (501) staff       (20)      813 2020-08-06 02:10:04.000000 guniflask-0.9.1/docs/make.bat
--rw-r--r--   0 jadbin     (501) staff       (20)     1162 2020-09-15 17:24:04.000000 guniflask-0.9.1/docs/orm.rst
--rw-r--r--   0 jadbin     (501) staff       (20)     1197 2020-08-06 02:10:04.000000 guniflask-0.9.1/docs/run.rst
--rw-r--r--   0 jadbin     (501) staff       (20)     2262 2020-09-15 17:24:04.000000 guniflask-0.9.1/docs/settings.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2020-09-16 07:46:40.000000 guniflask-0.9.1/guniflask/__init__.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/annotation/
--rw-r--r--   0 jadbin     (501) staff       (20)     2648 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/annotation/__init__.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/app/
--rw-r--r--   0 jadbin     (501) staff       (20)       48 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/app/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      484 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/app/factory.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2213 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/app/initializer.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/beans/
--rw-r--r--   0 jadbin     (501) staff       (20)      538 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2021 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/constructor_resolver.py
--rw-r--r--   0 jadbin     (501) staff       (20)    11769 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/default_factory.py
--rw-r--r--   0 jadbin     (501) staff       (20)      489 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/definition.py
--rw-r--r--   0 jadbin     (501) staff       (20)      686 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/definition_registry.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1823 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/errors.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1276 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/factory.py
--rw-r--r--   0 jadbin     (501) staff       (20)      445 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/factory_post_processor.py
--rw-r--r--   0 jadbin     (501) staff       (20)      402 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/lifecycle.py
--rw-r--r--   0 jadbin     (501) staff       (20)      814 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/name_generator.py
--rw-r--r--   0 jadbin     (501) staff       (20)      377 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/post_processor.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3127 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/beans/singleton_registry.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/config/
--rw-r--r--   0 jadbin     (501) staff       (20)       49 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/config/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3736 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/config/app_config.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/context/
--rw-r--r--   0 jadbin     (501) staff       (20)     1047 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3895 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/annotation.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3806 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/annotation_config_registry.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1112 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/annotation_config_utils.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1570 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/autowired_post_processor.py
--rw-r--r--   0 jadbin     (501) staff       (20)      836 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/bean_context.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1296 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/bean_name_generator.py
--rw-r--r--   0 jadbin     (501) staff       (20)      642 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/condition.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1016 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/condition_evaluator.py
--rw-r--r--   0 jadbin     (501) staff       (20)      296 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/config_constants.py
--rw-r--r--   0 jadbin     (501) staff       (20)     5509 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/config_post_processor.py
--rw-r--r--   0 jadbin     (501) staff       (20)      471 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/context_aware_processor.py
--rw-r--r--   0 jadbin     (501) staff       (20)     5840 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/default_bean_context.py
--rw-r--r--   0 jadbin     (501) staff       (20)      215 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/event.py
--rw-r--r--   0 jadbin     (501) staff       (20)      270 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/event_listener.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1757 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/context/event_publisher.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/distributed/
--rw-r--r--   0 jadbin     (501) staff       (20)       52 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/distributed/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1228 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/distributed/local_lock.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/oauth2/
--rw-r--r--   0 jadbin     (501) staff       (20)     1938 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      959 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/abstract_endpoint.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1145 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/authentication.py
--rw-r--r--   0 jadbin     (501) staff       (20)      393 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/authentication_details.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1201 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/authentication_filter.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2347 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/authentication_manager.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1712 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/client_details.py
--rw-r--r--   0 jadbin     (501) staff       (20)      933 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/client_details_service.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1289 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/client_details_user_details_service.py
--rw-r--r--   0 jadbin     (501) staff       (20)      949 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/client_grant.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1156 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/errors.py
--rw-r--r--   0 jadbin     (501) staff       (20)      757 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/oauth2_utils.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2122 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/password_grant.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1116 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/refresh_grant.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4022 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/request.py
--rw-r--r--   0 jadbin     (501) staff       (20)     6519 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/request_factory.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2530 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/token.py
--rw-r--r--   0 jadbin     (501) staff       (20)     9610 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/token_converter.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4791 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/token_endpoint.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1387 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/token_extractor.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2961 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/token_granter.py
--rw-r--r--   0 jadbin     (501) staff       (20)    10340 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/token_service.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4275 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2/token_store.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/oauth2_config/
--rw-r--r--   0 jadbin     (501) staff       (20)      490 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2_config/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      736 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2_config/annotation.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3839 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2_config/authorization_server_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)    10912 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2_config/authorization_server_configurer.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1245 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2_config/client_details_service_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)      585 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2_config/client_details_service_configurer.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1838 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2_config/resource_server_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4069 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/oauth2_config/resource_server_configurer.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/orm/
--rw-r--r--   0 jadbin     (501) staff       (20)      273 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/orm/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1351 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/orm/base_model.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3120 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/orm/model_utils.py
--rw-r--r--   0 jadbin     (501) staff       (20)      792 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/orm/sqlalchemy_wrapper.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/scheduling/
--rw-r--r--   0 jadbin     (501) staff       (20)      360 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1237 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/annotation.py
--rw-r--r--   0 jadbin     (501) staff       (20)      979 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/async_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)      907 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/async_executor.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2489 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/async_post_processor.py
--rw-r--r--   0 jadbin     (501) staff       (20)      144 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/config_constants.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1031 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/scheduling_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2364 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/scheduling_post_processor.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2241 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/scheduling/task_scheduler.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/security/
--rw-r--r--   0 jadbin     (501) staff       (20)     1446 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1247 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/access_annotation.py
--rw-r--r--   0 jadbin     (501) staff       (20)      818 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/authentication.py
--rw-r--r--   0 jadbin     (501) staff       (20)      279 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/authentication_manager.py
--rw-r--r--   0 jadbin     (501) staff       (20)      432 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/authentication_provider.py
--rw-r--r--   0 jadbin     (501) staff       (20)      907 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/authentication_token.py
--rw-r--r--   0 jadbin     (501) staff       (20)      339 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/authentication_user_details_service.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1898 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/basic_authentication_filter.py
--rw-r--r--   0 jadbin     (501) staff       (20)      695 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/context.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1504 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/dao_authentication_provider.py
--rw-r--r--   0 jadbin     (501) staff       (20)      517 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/errors.py
--rw-r--r--   0 jadbin     (501) staff       (20)      831 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/jwt.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2946 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/jwt_provider.py
--rw-r--r--   0 jadbin     (501) staff       (20)      759 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/password_encoder.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1299 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/preauth_provider.py
--rw-r--r--   0 jadbin     (501) staff       (20)      555 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/preauth_token.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2125 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/provider_manager.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1421 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/user.py
--rw-r--r--   0 jadbin     (501) staff       (20)      315 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/user_details.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1279 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/user_details_authentication_provider.py
--rw-r--r--   0 jadbin     (501) staff       (20)      644 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/user_details_by_name_service.py
--rw-r--r--   0 jadbin     (501) staff       (20)      261 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/user_details_service.py
--rw-r--r--   0 jadbin     (501) staff       (20)      150 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security/web_authentication_details.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/security_config/
--rw-r--r--   0 jadbin     (501) staff       (20)      494 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      627 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/annotation.py
--rw-r--r--   0 jadbin     (501) staff       (20)      977 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/authentication_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2026 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/authentication_manager_builder.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2542 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/configured_security_builder.py
--rw-r--r--   0 jadbin     (501) staff       (20)      569 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/cors_configurer.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1174 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/dao_authentication_configurer.py
--rw-r--r--   0 jadbin     (501) staff       (20)      644 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/http_basic_configurer.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4357 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/http_security.py
--rw-r--r--   0 jadbin     (501) staff       (20)      378 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/http_security_builder.py
--rw-r--r--   0 jadbin     (501) staff       (20)      413 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/provider_manager_builder.py
--rw-r--r--   0 jadbin     (501) staff       (20)      538 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/security_builder.py
--rw-r--r--   0 jadbin     (501) staff       (20)      502 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/security_configurer.py
--rw-r--r--   0 jadbin     (501) staff       (20)      385 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/user_details_aware_configurer.py
--rw-r--r--   0 jadbin     (501) staff       (20)      599 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/web_security.py
--rw-r--r--   0 jadbin     (501) staff       (20)      681 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/web_security_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     5111 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/security_config/web_security_configurer.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/service_discovery/
--rw-r--r--   0 jadbin     (501) staff       (20)      262 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/service_discovery/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     5715 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/service_discovery/config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4690 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/service_discovery/consul.py
--rw-r--r--   0 jadbin     (501) staff       (20)      313 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/service_discovery/discovery_client.py
--rw-r--r--   0 jadbin     (501) staff       (20)       65 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/service_discovery/errors.py
--rw-r--r--   0 jadbin     (501) staff       (20)      926 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/service_discovery/heath_endpoint.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1182 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/service_discovery/load_balancer_client.py
--rw-r--r--   0 jadbin     (501) staff       (20)      210 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/service_discovery/service_instance.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/utils/
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:04.000000 guniflask-0.9.1/guniflask/utils/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      437 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/utils/context.py
--rw-r--r--   0 jadbin     (501) staff       (20)      353 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/utils/datatime.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2717 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/utils/inspect.py
--rw-r--r--   0 jadbin     (501) staff       (20)      291 2020-08-06 02:10:04.000000 guniflask-0.9.1/guniflask/utils/network.py
--rw-r--r--   0 jadbin     (501) staff       (20)      798 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/utils/path.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2202 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/utils/request.py
--rw-r--r--   0 jadbin     (501) staff       (20)      835 2020-08-06 02:10:04.000000 guniflask-0.9.1/guniflask/utils/string.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask/web/
--rw-r--r--   0 jadbin     (501) staff       (20)     1107 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2132 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/bind_annotation.py
--rw-r--r--   0 jadbin     (501) staff       (20)    11309 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/blueprint_post_processor.py
--rw-r--r--   0 jadbin     (501) staff       (20)       72 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/config_constants.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1329 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/context.py
--rw-r--r--   0 jadbin     (501) staff       (20)      864 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/cors.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1489 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/filter_annotation.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4223 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/param_annotation.py
--rw-r--r--   0 jadbin     (501) staff       (20)      700 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/request_filter.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1428 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/scheduling_config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1297 2020-09-15 17:24:04.000000 guniflask-0.9.1/guniflask/web/user_context.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/guniflask.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)     2370 2020-09-16 07:51:55.000000 guniflask-0.9.1/guniflask.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)     6370 2020-09-16 07:51:55.000000 guniflask-0.9.1/guniflask.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2020-09-16 07:51:55.000000 guniflask-0.9.1/guniflask.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2020-09-16 07:51:55.000000 guniflask-0.9.1/guniflask.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)      134 2020-09-16 07:51:55.000000 guniflask-0.9.1/guniflask.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       16 2020-09-16 07:51:55.000000 guniflask-0.9.1/guniflask.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       17 2020-08-06 02:10:04.000000 guniflask-0.9.1/requirements/docs.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:04.000000 guniflask-0.9.1/requirements/test.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2020-09-16 07:51:56.000000 guniflask-0.9.1/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     2177 2020-09-15 17:24:04.000000 guniflask-0.9.1/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:04.000000 guniflask-0.9.1/tests/__init__.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/tests/test_config/
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:04.000000 guniflask-0.9.1/tests/test_config/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4180 2020-09-15 17:24:04.000000 guniflask-0.9.1/tests/test_config/test_settings.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-16 07:51:56.000000 guniflask-0.9.1/tests/test_utils/
--rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:04.000000 guniflask-0.9.1/tests/test_utils/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1927 2020-09-15 17:24:04.000000 guniflask-0.9.1/tests/test_utils/test_request_utils.py
--rw-r--r--   0 jadbin     (501) staff       (20)      912 2020-08-06 02:10:04.000000 guniflask-0.9.1/tests/test_utils/test_string_utils.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1063 2020-08-06 02:10:04.000000 guniflask-0.9.2/LICENSE
+-rw-r--r--   0 jadbin     (501) staff       (20)      153 2020-08-06 02:10:04.000000 guniflask-0.9.2/MANIFEST.in
+-rw-r--r--   0 jadbin     (501) staff       (20)     2370 2020-09-17 13:06:18.000000 guniflask-0.9.2/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)     1310 2020-09-15 06:36:11.000000 guniflask-0.9.2/README.rst
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/docs/
+-rw-r--r--   0 jadbin     (501) staff       (20)      606 2020-08-06 02:10:04.000000 guniflask-0.9.2/docs/Makefile
+-rw-r--r--   0 jadbin     (501) staff       (20)      723 2020-09-15 17:24:04.000000 guniflask-0.9.2/docs/app.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)     1006 2020-09-15 17:24:04.000000 guniflask-0.9.2/docs/blueprints.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)    10256 2020-09-17 13:03:52.000000 guniflask-0.9.2/docs/changelog.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)     5382 2020-08-06 02:10:04.000000 guniflask-0.9.2/docs/conf.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2000 2020-08-06 02:10:04.000000 guniflask-0.9.2/docs/config.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)     1250 2020-08-06 02:10:04.000000 guniflask-0.9.2/docs/debug.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)      726 2020-08-06 02:10:04.000000 guniflask-0.9.2/docs/deploy.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)      613 2020-09-15 06:35:42.000000 guniflask-0.9.2/docs/index.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)      831 2020-08-06 02:10:04.000000 guniflask-0.9.2/docs/log.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)      813 2020-08-06 02:10:04.000000 guniflask-0.9.2/docs/make.bat
+-rw-r--r--   0 jadbin     (501) staff       (20)     1162 2020-09-15 17:24:04.000000 guniflask-0.9.2/docs/orm.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)     1197 2020-08-06 02:10:04.000000 guniflask-0.9.2/docs/run.rst
+-rw-r--r--   0 jadbin     (501) staff       (20)     2262 2020-09-15 17:24:04.000000 guniflask-0.9.2/docs/settings.rst
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/
+-rw-r--r--   0 jadbin     (501) staff       (20)       38 2020-09-17 13:04:37.000000 guniflask-0.9.2/guniflask/__init__.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/annotation/
+-rw-r--r--   0 jadbin     (501) staff       (20)     2648 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/annotation/__init__.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/app/
+-rw-r--r--   0 jadbin     (501) staff       (20)       48 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/app/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      484 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/app/factory.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2213 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/app/initializer.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/beans/
+-rw-r--r--   0 jadbin     (501) staff       (20)      538 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2021 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/constructor_resolver.py
+-rw-r--r--   0 jadbin     (501) staff       (20)    11769 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/default_factory.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      489 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/definition.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      686 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/definition_registry.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1823 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/errors.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1276 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/factory.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      445 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/factory_post_processor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      402 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/lifecycle.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      814 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/name_generator.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      377 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/post_processor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3127 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/beans/singleton_registry.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/config/
+-rw-r--r--   0 jadbin     (501) staff       (20)       49 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/config/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3736 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/config/app_config.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/context/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1047 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3895 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/annotation.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3806 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/annotation_config_registry.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1112 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/annotation_config_utils.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1570 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/autowired_post_processor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      836 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/bean_context.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1296 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/bean_name_generator.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      642 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/condition.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1016 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/condition_evaluator.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      296 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/config_constants.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     5509 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/config_post_processor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      471 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/context_aware_processor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     5840 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/default_bean_context.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      215 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/event.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      270 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/event_listener.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1757 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/context/event_publisher.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/distributed/
+-rw-r--r--   0 jadbin     (501) staff       (20)       52 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/distributed/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1228 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/distributed/local_lock.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/oauth2/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1938 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      959 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/abstract_endpoint.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1145 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/authentication.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      393 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/authentication_details.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1201 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/authentication_filter.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2347 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/authentication_manager.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1712 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/client_details.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      933 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/client_details_service.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1289 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/client_details_user_details_service.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      949 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/client_grant.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1156 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/errors.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      757 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/oauth2_utils.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2122 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/password_grant.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1116 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/refresh_grant.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4022 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/request.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     6519 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/request_factory.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2530 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/token.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     9610 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/token_converter.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4791 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/token_endpoint.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1387 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/token_extractor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2961 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/token_granter.py
+-rw-r--r--   0 jadbin     (501) staff       (20)    10340 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/token_service.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4275 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2/token_store.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask/oauth2_config/
+-rw-r--r--   0 jadbin     (501) staff       (20)      490 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2_config/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      736 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2_config/annotation.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3839 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2_config/authorization_server_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)    10912 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2_config/authorization_server_configurer.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1245 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2_config/client_details_service_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      585 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2_config/client_details_service_configurer.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1838 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2_config/resource_server_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4069 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/oauth2_config/resource_server_configurer.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/guniflask/orm/
+-rw-r--r--   0 jadbin     (501) staff       (20)      273 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/orm/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1351 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/orm/base_model.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3120 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/orm/model_utils.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      792 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/orm/sqlalchemy_wrapper.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/guniflask/scheduling/
+-rw-r--r--   0 jadbin     (501) staff       (20)      360 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1237 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/annotation.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      979 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/async_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      907 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/async_executor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2489 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/async_post_processor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      144 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/config_constants.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1031 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/scheduling_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2364 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/scheduling_post_processor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2241 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/scheduling/task_scheduler.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/guniflask/security/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1446 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1247 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/access_annotation.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      818 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/authentication.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      279 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/authentication_manager.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      432 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/authentication_provider.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      907 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/authentication_token.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      339 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/authentication_user_details_service.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1898 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/basic_authentication_filter.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      695 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/context.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1504 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/dao_authentication_provider.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      517 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/errors.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      831 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/jwt.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2946 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/jwt_provider.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      759 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/password_encoder.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1299 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/preauth_provider.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      555 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/preauth_token.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2125 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/provider_manager.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1421 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/user.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      315 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/user_details.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1279 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/user_details_authentication_provider.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      644 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/user_details_by_name_service.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      261 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/user_details_service.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      150 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security/web_authentication_details.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/guniflask/security_config/
+-rw-r--r--   0 jadbin     (501) staff       (20)      494 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      627 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/annotation.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      977 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/authentication_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2026 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/authentication_manager_builder.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2542 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/configured_security_builder.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      569 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/cors_configurer.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1174 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/dao_authentication_configurer.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      644 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/http_basic_configurer.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4357 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/http_security.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      378 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/http_security_builder.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      413 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/provider_manager_builder.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      538 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/security_builder.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      502 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/security_configurer.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      385 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/user_details_aware_configurer.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      599 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/web_security.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      681 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/web_security_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     5111 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/security_config/web_security_configurer.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/guniflask/service_discovery/
+-rw-r--r--   0 jadbin     (501) staff       (20)      262 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/service_discovery/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     5715 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/service_discovery/config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4690 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/service_discovery/consul.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      313 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/service_discovery/discovery_client.py
+-rw-r--r--   0 jadbin     (501) staff       (20)       65 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/service_discovery/errors.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      926 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/service_discovery/heath_endpoint.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1182 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/service_discovery/load_balancer_client.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      210 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/service_discovery/service_instance.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/guniflask/utils/
+-rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:04.000000 guniflask-0.9.2/guniflask/utils/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      437 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/utils/context.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      353 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/utils/datatime.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2717 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/utils/inspect.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      291 2020-08-06 02:10:04.000000 guniflask-0.9.2/guniflask/utils/network.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      798 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/utils/path.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2202 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/utils/request.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      835 2020-08-06 02:10:04.000000 guniflask-0.9.2/guniflask/utils/string.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/guniflask/web/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1107 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2132 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/bind_annotation.py
+-rw-r--r--   0 jadbin     (501) staff       (20)    11309 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/blueprint_post_processor.py
+-rw-r--r--   0 jadbin     (501) staff       (20)       72 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/config_constants.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1329 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/context.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      864 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/cors.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1489 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/filter_annotation.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4223 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/param_annotation.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      700 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/request_filter.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1428 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/scheduling_config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1297 2020-09-15 17:24:04.000000 guniflask-0.9.2/guniflask/web/user_context.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask.egg-info/
+-rw-r--r--   0 jadbin     (501) staff       (20)     2370 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask.egg-info/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)     6370 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask.egg-info/SOURCES.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask.egg-info/dependency_links.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask.egg-info/not-zip-safe
+-rw-r--r--   0 jadbin     (501) staff       (20)      134 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask.egg-info/requires.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       16 2020-09-17 13:06:17.000000 guniflask-0.9.2/guniflask.egg-info/top_level.txt
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/requirements/
+-rw-r--r--   0 jadbin     (501) staff       (20)       17 2020-08-06 02:10:04.000000 guniflask-0.9.2/requirements/docs.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       18 2020-08-06 02:10:04.000000 guniflask-0.9.2/requirements/test.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       38 2020-09-17 13:06:18.000000 guniflask-0.9.2/setup.cfg
+-rw-r--r--   0 jadbin     (501) staff       (20)     2177 2020-09-15 17:24:04.000000 guniflask-0.9.2/setup.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/tests/
+-rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:04.000000 guniflask-0.9.2/tests/__init__.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/tests/test_config/
+-rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:04.000000 guniflask-0.9.2/tests/test_config/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4180 2020-09-15 17:24:04.000000 guniflask-0.9.2/tests/test_config/test_settings.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2020-09-17 13:06:18.000000 guniflask-0.9.2/tests/test_utils/
+-rw-r--r--   0 jadbin     (501) staff       (20)       15 2020-08-06 02:10:04.000000 guniflask-0.9.2/tests/test_utils/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1927 2020-09-15 17:24:04.000000 guniflask-0.9.2/tests/test_utils/test_request_utils.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      912 2020-08-06 02:10:04.000000 guniflask-0.9.2/tests/test_utils/test_string_utils.py
```

### Comparing `guniflask-0.9.1/LICENSE` & `guniflask-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/PKG-INFO` & `guniflask-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: guniflask
-Version: 0.9.1
+Version: 0.9.2
 Summary: Better coding experience for Flask
 Home-page: https://github.com/jadbin/guniflask
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: MIT
 Description: =========
         guniflask
```

### Comparing `guniflask-0.9.1/README.rst` & `guniflask-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/Makefile` & `guniflask-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/app.rst` & `guniflask-0.9.2/docs/app.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/blueprints.rst` & `guniflask-0.9.2/docs/blueprints.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/changelog.rst` & `guniflask-0.9.2/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. _changelog:
 
 Changelog
 =========
 
+0.9.2 (2020-09-17)
+------------------
+
+- 新增UvicornWorker解决uvicorn提供的worker中存在的问题：(1) debug模式下worker无法reload；(2) 父进程退出后worker没有退出
+
 0.9.1 (2020-09-16)
 ------------------
 
 - 修复未加载gunicorn配置的错误
 
 0.9.0 (2020-09-16)
 ------------------
```

### Comparing `guniflask-0.9.1/docs/conf.py` & `guniflask-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/config.rst` & `guniflask-0.9.2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/debug.rst` & `guniflask-0.9.2/docs/debug.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/deploy.rst` & `guniflask-0.9.2/docs/deploy.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/index.rst` & `guniflask-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/log.rst` & `guniflask-0.9.2/docs/log.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/make.bat` & `guniflask-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/orm.rst` & `guniflask-0.9.2/docs/orm.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/run.rst` & `guniflask-0.9.2/docs/run.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/docs/settings.rst` & `guniflask-0.9.2/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/annotation/__init__.py` & `guniflask-0.9.2/guniflask/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/app/initializer.py` & `guniflask-0.9.2/guniflask/app/initializer.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/beans/__init__.py` & `guniflask-0.9.2/guniflask/beans/__init__.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/beans/constructor_resolver.py` & `guniflask-0.9.2/guniflask/beans/constructor_resolver.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/beans/default_factory.py` & `guniflask-0.9.2/guniflask/beans/default_factory.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/beans/definition_registry.py` & `guniflask-0.9.2/guniflask/beans/definition_registry.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/beans/errors.py` & `guniflask-0.9.2/guniflask/beans/errors.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/beans/factory.py` & `guniflask-0.9.2/guniflask/beans/factory.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/beans/name_generator.py` & `guniflask-0.9.2/guniflask/beans/name_generator.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/beans/singleton_registry.py` & `guniflask-0.9.2/guniflask/beans/singleton_registry.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/config/app_config.py` & `guniflask-0.9.2/guniflask/config/app_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/__init__.py` & `guniflask-0.9.2/guniflask/context/__init__.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/annotation.py` & `guniflask-0.9.2/guniflask/context/annotation.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/annotation_config_registry.py` & `guniflask-0.9.2/guniflask/context/annotation_config_registry.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/annotation_config_utils.py` & `guniflask-0.9.2/guniflask/context/annotation_config_utils.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/autowired_post_processor.py` & `guniflask-0.9.2/guniflask/context/autowired_post_processor.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/bean_context.py` & `guniflask-0.9.2/guniflask/context/bean_context.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/bean_name_generator.py` & `guniflask-0.9.2/guniflask/context/bean_name_generator.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/condition.py` & `guniflask-0.9.2/guniflask/context/condition.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/condition_evaluator.py` & `guniflask-0.9.2/guniflask/context/condition_evaluator.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/config_post_processor.py` & `guniflask-0.9.2/guniflask/context/config_post_processor.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/default_bean_context.py` & `guniflask-0.9.2/guniflask/context/default_bean_context.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/context/event_publisher.py` & `guniflask-0.9.2/guniflask/context/event_publisher.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/distributed/local_lock.py` & `guniflask-0.9.2/guniflask/distributed/local_lock.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/__init__.py` & `guniflask-0.9.2/guniflask/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/abstract_endpoint.py` & `guniflask-0.9.2/guniflask/oauth2/abstract_endpoint.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/authentication.py` & `guniflask-0.9.2/guniflask/oauth2/authentication.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/authentication_filter.py` & `guniflask-0.9.2/guniflask/oauth2/authentication_filter.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/authentication_manager.py` & `guniflask-0.9.2/guniflask/oauth2/authentication_manager.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/client_details.py` & `guniflask-0.9.2/guniflask/oauth2/client_details.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/client_details_service.py` & `guniflask-0.9.2/guniflask/oauth2/client_details_service.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/client_details_user_details_service.py` & `guniflask-0.9.2/guniflask/oauth2/client_details_user_details_service.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/client_grant.py` & `guniflask-0.9.2/guniflask/oauth2/client_grant.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/errors.py` & `guniflask-0.9.2/guniflask/oauth2/errors.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/oauth2_utils.py` & `guniflask-0.9.2/guniflask/oauth2/oauth2_utils.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/password_grant.py` & `guniflask-0.9.2/guniflask/oauth2/password_grant.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/refresh_grant.py` & `guniflask-0.9.2/guniflask/oauth2/refresh_grant.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/request.py` & `guniflask-0.9.2/guniflask/oauth2/request.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/request_factory.py` & `guniflask-0.9.2/guniflask/oauth2/request_factory.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/token.py` & `guniflask-0.9.2/guniflask/oauth2/token.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/token_converter.py` & `guniflask-0.9.2/guniflask/oauth2/token_converter.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/token_endpoint.py` & `guniflask-0.9.2/guniflask/oauth2/token_endpoint.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/token_extractor.py` & `guniflask-0.9.2/guniflask/oauth2/token_extractor.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/token_granter.py` & `guniflask-0.9.2/guniflask/oauth2/token_granter.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/token_service.py` & `guniflask-0.9.2/guniflask/oauth2/token_service.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2/token_store.py` & `guniflask-0.9.2/guniflask/oauth2/token_store.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2_config/annotation.py` & `guniflask-0.9.2/guniflask/oauth2_config/annotation.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2_config/authorization_server_config.py` & `guniflask-0.9.2/guniflask/oauth2_config/authorization_server_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2_config/authorization_server_configurer.py` & `guniflask-0.9.2/guniflask/oauth2_config/authorization_server_configurer.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2_config/client_details_service_config.py` & `guniflask-0.9.2/guniflask/oauth2_config/client_details_service_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2_config/client_details_service_configurer.py` & `guniflask-0.9.2/guniflask/oauth2_config/client_details_service_configurer.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2_config/resource_server_config.py` & `guniflask-0.9.2/guniflask/oauth2_config/resource_server_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/oauth2_config/resource_server_configurer.py` & `guniflask-0.9.2/guniflask/oauth2_config/resource_server_configurer.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/orm/base_model.py` & `guniflask-0.9.2/guniflask/orm/base_model.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/orm/model_utils.py` & `guniflask-0.9.2/guniflask/orm/model_utils.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/orm/sqlalchemy_wrapper.py` & `guniflask-0.9.2/guniflask/orm/sqlalchemy_wrapper.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/scheduling/annotation.py` & `guniflask-0.9.2/guniflask/scheduling/annotation.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/scheduling/async_config.py` & `guniflask-0.9.2/guniflask/scheduling/async_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/scheduling/async_executor.py` & `guniflask-0.9.2/guniflask/scheduling/async_executor.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/scheduling/async_post_processor.py` & `guniflask-0.9.2/guniflask/scheduling/async_post_processor.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/scheduling/scheduling_config.py` & `guniflask-0.9.2/guniflask/scheduling/scheduling_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/scheduling/scheduling_post_processor.py` & `guniflask-0.9.2/guniflask/scheduling/scheduling_post_processor.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/scheduling/task_scheduler.py` & `guniflask-0.9.2/guniflask/scheduling/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/__init__.py` & `guniflask-0.9.2/guniflask/security/__init__.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/access_annotation.py` & `guniflask-0.9.2/guniflask/security/access_annotation.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/authentication.py` & `guniflask-0.9.2/guniflask/security/authentication.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/authentication_token.py` & `guniflask-0.9.2/guniflask/security/authentication_token.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/basic_authentication_filter.py` & `guniflask-0.9.2/guniflask/security/basic_authentication_filter.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/context.py` & `guniflask-0.9.2/guniflask/security/context.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/dao_authentication_provider.py` & `guniflask-0.9.2/guniflask/security/dao_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/errors.py` & `guniflask-0.9.2/guniflask/security/errors.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/jwt.py` & `guniflask-0.9.2/guniflask/security/jwt.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/jwt_provider.py` & `guniflask-0.9.2/guniflask/security/jwt_provider.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/password_encoder.py` & `guniflask-0.9.2/guniflask/security/password_encoder.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/preauth_provider.py` & `guniflask-0.9.2/guniflask/security/preauth_provider.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/preauth_token.py` & `guniflask-0.9.2/guniflask/security/preauth_token.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/provider_manager.py` & `guniflask-0.9.2/guniflask/security/provider_manager.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/user.py` & `guniflask-0.9.2/guniflask/security/user.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/user_details_authentication_provider.py` & `guniflask-0.9.2/guniflask/security/user_details_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security/user_details_by_name_service.py` & `guniflask-0.9.2/guniflask/security/user_details_by_name_service.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/annotation.py` & `guniflask-0.9.2/guniflask/security_config/annotation.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/authentication_config.py` & `guniflask-0.9.2/guniflask/security_config/authentication_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/authentication_manager_builder.py` & `guniflask-0.9.2/guniflask/security_config/authentication_manager_builder.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/configured_security_builder.py` & `guniflask-0.9.2/guniflask/security_config/configured_security_builder.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/cors_configurer.py` & `guniflask-0.9.2/guniflask/security_config/cors_configurer.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/dao_authentication_configurer.py` & `guniflask-0.9.2/guniflask/security_config/dao_authentication_configurer.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/http_basic_configurer.py` & `guniflask-0.9.2/guniflask/security_config/http_basic_configurer.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/http_security.py` & `guniflask-0.9.2/guniflask/security_config/http_security.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/security_builder.py` & `guniflask-0.9.2/guniflask/security_config/security_builder.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/web_security.py` & `guniflask-0.9.2/guniflask/security_config/web_security.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/web_security_config.py` & `guniflask-0.9.2/guniflask/security_config/web_security_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/security_config/web_security_configurer.py` & `guniflask-0.9.2/guniflask/security_config/web_security_configurer.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/service_discovery/config.py` & `guniflask-0.9.2/guniflask/service_discovery/config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/service_discovery/consul.py` & `guniflask-0.9.2/guniflask/service_discovery/consul.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/service_discovery/heath_endpoint.py` & `guniflask-0.9.2/guniflask/service_discovery/heath_endpoint.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/service_discovery/load_balancer_client.py` & `guniflask-0.9.2/guniflask/service_discovery/load_balancer_client.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/utils/inspect.py` & `guniflask-0.9.2/guniflask/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/utils/path.py` & `guniflask-0.9.2/guniflask/utils/path.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/utils/request.py` & `guniflask-0.9.2/guniflask/utils/request.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/utils/string.py` & `guniflask-0.9.2/guniflask/utils/string.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/__init__.py` & `guniflask-0.9.2/guniflask/web/__init__.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/bind_annotation.py` & `guniflask-0.9.2/guniflask/web/bind_annotation.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/blueprint_post_processor.py` & `guniflask-0.9.2/guniflask/web/blueprint_post_processor.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/context.py` & `guniflask-0.9.2/guniflask/web/context.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/cors.py` & `guniflask-0.9.2/guniflask/web/cors.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/filter_annotation.py` & `guniflask-0.9.2/guniflask/web/filter_annotation.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/param_annotation.py` & `guniflask-0.9.2/guniflask/web/param_annotation.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/request_filter.py` & `guniflask-0.9.2/guniflask/web/request_filter.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/scheduling_config.py` & `guniflask-0.9.2/guniflask/web/scheduling_config.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask/web/user_context.py` & `guniflask-0.9.2/guniflask/web/user_context.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/guniflask.egg-info/PKG-INFO` & `guniflask-0.9.2/guniflask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: guniflask
-Version: 0.9.1
+Version: 0.9.2
 Summary: Better coding experience for Flask
 Home-page: https://github.com/jadbin/guniflask
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: MIT
 Description: =========
         guniflask
```

### Comparing `guniflask-0.9.1/guniflask.egg-info/SOURCES.txt` & `guniflask-0.9.2/guniflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/setup.py` & `guniflask-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/tests/test_config/test_settings.py` & `guniflask-0.9.2/tests/test_config/test_settings.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/tests/test_utils/test_request_utils.py` & `guniflask-0.9.2/tests/test_utils/test_request_utils.py`

 * *Files identical despite different names*

### Comparing `guniflask-0.9.1/tests/test_utils/test_string_utils.py` & `guniflask-0.9.2/tests/test_utils/test_string_utils.py`

 * *Files identical despite different names*

