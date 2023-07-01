# Comparing `tmp/newrelic_sb_sdk-0.7.0.tar.gz` & `tmp/newrelic_sb_sdk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic_sb_sdk-0.7.0.tar", max compression
+gzip compressed data, was "newrelic_sb_sdk-0.8.0.tar", max compression
```

## Comparing `newrelic_sb_sdk-0.7.0.tar` & `newrelic_sb_sdk-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1379 2023-06-12 17:54:32.162562 newrelic_sb_sdk-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2761 2023-06-12 17:52:06.862280 newrelic_sb_sdk-0.7.0/README.md
--rw-r--r--   0        0        0     2788 2023-06-12 17:54:32.154562 newrelic_sb_sdk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-12 17:54:40.318579 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/__init__.py
--rw-r--r--   0        0        0   385992 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/_modidx.py
--rw-r--r--   0        0        0     4902 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/enums.py
--rw-r--r--   0        0        0      769 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/utils.py
--rw-r--r--   0        0        0     2024 2023-06-12 17:51:48.142247 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/__init__.py
--rw-r--r--   0        0        0      372 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/base.py
--rw-r--r--   0        0        0      747 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/encoders.py
--rw-r--r--   0        0        0     2235 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/mixins.py
--rw-r--r--   0        0        0     1175 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/__init__.py
--rw-r--r--   0        0        0     1095 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/enums.py
--rw-r--r--   0        0        0     1006 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/pages.py
--rw-r--r--   0        0        0      593 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/utils.py
--rw-r--r--   0        0        0     3583 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/widgets.py
--rw-r--r--   0        0        0      200 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/__init__.py
--rw-r--r--   0        0        0    58585 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/enums.py
--rw-r--r--   0        0        0   358452 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/input_objects.py
--rw-r--r--   0        0        0   751350 2023-06-12 17:47:57.225961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/objects.py
--rw-r--r--   0        0        0     3054 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/scalars.py
--rw-r--r--   0        0        0        0 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/__init__.py
--rw-r--r--   0        0        0      329 2023-06-12 17:51:48.142247 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/query.py
--rw-r--r--   0        0        0      787 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/response.py
--rw-r--r--   0        0        0     1901 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/text.py
--rw-r--r--   0        0        0     4600 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1529 2023-07-01 07:27:04.765278 newrelic_sb_sdk-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-03-04 20:34:24.170848 newrelic_sb_sdk-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3001 2023-07-01 07:20:37.782587 newrelic_sb_sdk-0.8.0/README.md
+-rw-r--r--   0        0        0     2923 2023-07-01 07:27:04.765278 newrelic_sb_sdk-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-01 07:27:04.769277 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/__init__.py
+-rw-r--r--   0        0        0   389324 2023-07-01 07:06:47.079444 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/_modidx.py
+-rw-r--r--   0        0        0     4902 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/__init__.py
+-rw-r--r--   0        0        0     1541 2023-03-12 12:22:19.009570 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/enums.py
+-rw-r--r--   0        0        0      769 2023-06-05 12:25:15.706671 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/utils.py
+-rw-r--r--   0        0        0     2024 2023-06-12 17:56:42.971757 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/base.py
+-rw-r--r--   0        0        0      747 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/encoders.py
+-rw-r--r--   0        0        0     2235 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/mixins.py
+-rw-r--r--   0        0        0     1175 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/__init__.py
+-rw-r--r--   0        0        0     1095 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/enums.py
+-rw-r--r--   0        0        0     1006 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/pages.py
+-rw-r--r--   0        0        0      593 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/utils.py
+-rw-r--r--   0        0        0     3583 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/widgets.py
+-rw-r--r--   0        0        0      200 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/__init__.py
+-rw-r--r--   0        0        0    58745 2023-07-01 07:06:47.079444 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/enums.py
+-rw-r--r--   0        0        0   362780 2023-07-01 07:06:47.079444 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/input_objects.py
+-rw-r--r--   0        0        0   753602 2023-07-01 07:06:47.083444 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/objects.py
+-rw-r--r--   0        0        0     3054 2023-06-10 11:02:34.187465 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/scalars.py
+-rw-r--r--   0        0        0        0 2023-03-10 03:57:33.232743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      329 2023-06-12 17:56:42.971757 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/query.py
+-rw-r--r--   0        0        0      787 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/response.py
+-rw-r--r--   0        0        0     1901 2023-03-10 03:57:33.232743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/text.py
+-rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.8.0/PKG-INFO
```

### Comparing `newrelic_sb_sdk-0.7.0/CHANGELOG.md` & `newrelic_sb_sdk-0.8.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.8.0] - 2023-07-01
+
+* Update GraphQL submodule with a fresh schema version.
+* Update dependencies
+* Add tests
+* Add autoplush with GitLab CI/CD
+
 ## [0.7.0] - 2023-06-12
 
 * Rename arguments in NewRelicGqlClient.build_query method and build_query function from `query_params` to `params` and  `query_string` to `template`.
 * Update graphql module.
 * Add metadata about language info in GraphQL notebook.
 * Add new clasifiers for PyPi.
 * Add build status badge.
```

### Comparing `newrelic_sb_sdk-0.7.0/LICENSE.txt` & `newrelic_sb_sdk-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/README.md` & `newrelic_sb_sdk-0.8.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/newrelic-sb-sdk)
 ![PyPI - Package version](https://img.shields.io/pypi/v/newrelic-sb-sdk)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/newrelic-sb-sdk)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/newrelic-sb-sdk)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/1c25dec51e1c4a719be4c2d4ebe7eef6)](https://app.codacy.com/gl/softbutterfly/newrelic-sb-sdk/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/1c25dec51e1c4a719be4c2d4ebe7eef6)](https://app.codacy.com/gl/softbutterfly/newrelic-sb-sdk/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![pipeline status](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/badges/master/pipeline.svg)](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/commits/master)
 
 
 # New Relic SB SDK
 
 New Relic SDK built by SoftButterfly to automate common New Relic One observability platform tasks
```

#### html2text {}

```diff
@@ -4,14 +4,18 @@
 pyversions/newrelic-sb-sdk) ![PyPI - Package version](https://img.shields.io/
 pypi/v/newrelic-sb-sdk) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
 newrelic-sb-sdk) ![PyPI - MIT License](https://img.shields.io/pypi/l/newrelic-
 sb-sdk) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/
 1c25dec51e1c4a719be4c2d4ebe7eef6)](https://app.codacy.com/gl/softbutterfly/
 newrelic-sb-sdk/
 dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/
+1c25dec51e1c4a719be4c2d4ebe7eef6)](https://app.codacy.com/gl/softbutterfly/
+newrelic-sb-sdk/
+dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![pipeline status](https://gitlab.com/softbutterfly/open-source/newrelic-sb-
 sdk/badges/master/pipeline.svg)](https://gitlab.com/softbutterfly/open-source/
 newrelic-sb-sdk/-/commits/master) # New Relic SB SDK New Relic SDK built by
 SoftButterfly to automate common New Relic One observability platform tasks ##
 Requirements * Python 3.8.1 or higher * `enforce-typing` * `python-dotenv` *
 `requests` * `semver` * `sgqlc` ## Install Install from PyPI ```bash pip
 install newrelic-sb-sdk ``` ## Usage There is an example on how to use this
```

### Comparing `newrelic_sb_sdk-0.7.0/pyproject.toml` & `newrelic_sb_sdk-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "newrelic-sb-sdk"
-version = "0.7.0"
+version = "0.8.0"
 description = "New Relic SDK to interact with Nerdgraph API."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -39,24 +39,22 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.7.0/newrelic-sb-sdk-v0.7.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.8.0/newrelic-sb-sdk-v0.8.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
-enforce-typing = "^1.0.0.post1"
 python-dotenv = "^1.0.0"
 requests = "^2.31.0"
-semver = "^3.0.0"
 sgqlc = "^16.1"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.7"
@@ -76,16 +74,14 @@
 pandas = "^2.0.2"
 pre-commit = "^3.3.2"
 pycodestyle = "^2.10.0"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.4"
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
-pytest-vcr = "^1.0.2"
-pytest-xdist = "^3.3.1"
 tbump = "^6.10.0"
 tox = "^4.5.2"
 types-requests = "^2.31.0.1"
 
 [tool.black]
 target_version = ['py311']
 include = '\.pyi?$'
@@ -104,10 +100,24 @@
   |buck-out
   |build
   |dist
   |legacy
 )/
 '''
 
+[tool.pytest.ini_options]
+testpaths = "tests"
+python_files = [
+  "**/test_*.py",
+]
+filterwarnings =[
+  "ignore::DeprecationWarning",
+  "ignore::PendingDeprecationWarning"
+]
+addopts = [
+  "--import-mode=importlib",
+  "--nbmake",
+]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/_modidx.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1108,14 +1108,18 @@
                 "GraphQL/enums.html#taggingmutationerrortype",
                 "newrelic_sb_sdk/graphql/enums.py",
             ),
             "newrelic_sb_sdk.graphql.enums.UserManagementRequestedTierName": (
                 "GraphQL/enums.html#usermanagementrequestedtiername",
                 "newrelic_sb_sdk/graphql/enums.py",
             ),
+            "newrelic_sb_sdk.graphql.enums.UserManagementTypeEnum": (
+                "GraphQL/enums.html#usermanagementtypeenum",
+                "newrelic_sb_sdk/graphql/enums.py",
+            ),
             "newrelic_sb_sdk.graphql.enums.WhatsNewContentType": (
                 "GraphQL/enums.html#whatsnewcontenttype",
                 "newrelic_sb_sdk/graphql/enums.py",
             ),
             "newrelic_sb_sdk.graphql.enums.WorkloadGroupRemainingEntitiesRuleBy": (
                 "GraphQL/enums.html#workloadgroupremainingentitiesruleby",
                 "newrelic_sb_sdk/graphql/enums.py",
@@ -1895,14 +1899,18 @@
                 "objects.html#authorizationmanagementaccountaccessgrant",
                 "newrelic_sb_sdk/graphql/input_objects.py",
             ),
             "newrelic_sb_sdk.graphql.input_objects.AuthorizationManagementGrantAccess": (
                 "GraphQL/input objects.html#authorizationmanagementgrantaccess",
                 "newrelic_sb_sdk/graphql/input_objects.py",
             ),
+            "newrelic_sb_sdk.graphql.input_objects.AuthorizationManagementGroupAccessGrant": (
+                "GraphQL/input objects.html#authorizationmanagementgroupaccessgrant",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
             "newrelic_sb_sdk.graphql.input_objects.AuthorizationManagementOrganizationAccessGrant": (
                 "GraphQL/input "
                 "objects.html#authorizationmanagementorganizationaccessgrant",
                 "newrelic_sb_sdk/graphql/input_objects.py",
             ),
             "newrelic_sb_sdk.graphql.input_objects.AuthorizationManagementRevokeAccess": (
                 "GraphQL/input objects.html#authorizationmanagementrevokeaccess",
@@ -3147,22 +3155,64 @@
                 "GraphQL/input objects.html#usermanagementdeletegroup",
                 "newrelic_sb_sdk/graphql/input_objects.py",
             ),
             "newrelic_sb_sdk.graphql.input_objects.UserManagementDeleteUser": (
                 "GraphQL/input objects.html#usermanagementdeleteuser",
                 "newrelic_sb_sdk/graphql/input_objects.py",
             ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementDisplayNameInput": (
+                "GraphQL/input objects.html#usermanagementdisplaynameinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementEmailInput": (
+                "GraphQL/input objects.html#usermanagementemailinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementEmailVerificationStateInput": (
+                "GraphQL/input "
+                "objects.html#usermanagementemailverificationstateinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementGroupFilterInput": (
+                "GraphQL/input objects.html#usermanagementgroupfilterinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementGroupIdInput": (
+                "GraphQL/input objects.html#usermanagementgroupidinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementNameInput": (
+                "GraphQL/input objects.html#usermanagementnameinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementPendingUpgradeRequestInput": (
+                "GraphQL/input "
+                "objects.html#usermanagementpendingupgraderequestinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementTypeInput": (
+                "GraphQL/input objects.html#usermanagementtypeinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
             "newrelic_sb_sdk.graphql.input_objects.UserManagementUpdateGroup": (
                 "GraphQL/input objects.html#usermanagementupdategroup",
                 "newrelic_sb_sdk/graphql/input_objects.py",
             ),
             "newrelic_sb_sdk.graphql.input_objects.UserManagementUpdateUser": (
                 "GraphQL/input objects.html#usermanagementupdateuser",
                 "newrelic_sb_sdk/graphql/input_objects.py",
             ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementUserFilterInput": (
+                "GraphQL/input objects.html#usermanagementuserfilterinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.input_objects.UserManagementUserIdInput": (
+                "GraphQL/input objects.html#usermanagementuseridinput",
+                "newrelic_sb_sdk/graphql/input_objects.py",
+            ),
             "newrelic_sb_sdk.graphql.input_objects.UserManagementUsersGroupsInput": (
                 "GraphQL/input objects.html#usermanagementusersgroupsinput",
                 "newrelic_sb_sdk/graphql/input_objects.py",
             ),
             "newrelic_sb_sdk.graphql.input_objects.UsersUserSearchQuery": (
                 "GraphQL/input objects.html#usersusersearchquery",
                 "newrelic_sb_sdk/graphql/input_objects.py",
@@ -5195,14 +5245,22 @@
                 "GraphQL/objects.html#entitygoldenmetricsdomaintypescoped",
                 "newrelic_sb_sdk/graphql/objects.py",
             ),
             "newrelic_sb_sdk.graphql.objects.EntityGoldenMetricsDomainTypeScopedResponse": (
                 "GraphQL/objects.html#entitygoldenmetricsdomaintypescopedresponse",
                 "newrelic_sb_sdk/graphql/objects.py",
             ),
+            "newrelic_sb_sdk.graphql.objects.EntityGoldenOriginalDefinitionWithSelector": (
+                "GraphQL/objects.html#entitygoldenoriginaldefinitionwithselector",
+                "newrelic_sb_sdk/graphql/objects.py",
+            ),
+            "newrelic_sb_sdk.graphql.objects.EntityGoldenOriginalQueryWithSelector": (
+                "GraphQL/objects.html#entitygoldenoriginalquerywithselector",
+                "newrelic_sb_sdk/graphql/objects.py",
+            ),
             "newrelic_sb_sdk.graphql.objects.EntityGoldenTag": (
                 "GraphQL/objects.html#entitygoldentag",
                 "newrelic_sb_sdk/graphql/objects.py",
             ),
             "newrelic_sb_sdk.graphql.objects.EntityGoldenTagsDomainTypeScoped": (
                 "GraphQL/objects.html#entitygoldentagsdomaintypescoped",
                 "newrelic_sb_sdk/graphql/objects.py",
```

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/__init__.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/enums.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/utils.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/client/__init__.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/client/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/encoders.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/encoders.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/mixins.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/mixins.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/__init__.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/enums.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/pages.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/pages.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/utils.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/widgets.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/widgets.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/enums.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,15 @@
     "SyntheticsMonitorPeriod",
     "SyntheticsMonitorStatus",
     "SyntheticsMonitorUpdateErrorType",
     "SyntheticsPrivateLocationMutationErrorType",
     "SyntheticsStepType",
     "TaggingMutationErrorType",
     "UserManagementRequestedTierName",
+    "UserManagementTypeEnum",
     "WhatsNewContentType",
     "WorkloadGroupRemainingEntitiesRuleBy",
     "WorkloadResultingGroupType",
     "WorkloadRollupStrategy",
     "WorkloadRuleThresholdType",
     "WorkloadStatusSource",
     "WorkloadStatusValue",
@@ -2175,14 +2176,19 @@
 
 
 class UserManagementRequestedTierName(sgqlc.types.Enum):
     __schema__ = nerdgraph
     __choices__ = ("BASIC_USER_TIER", "CORE_USER_TIER", "FULL_USER_TIER")
 
 
+class UserManagementTypeEnum(sgqlc.types.Enum):
+    __schema__ = nerdgraph
+    __choices__ = ("BASIC", "CORE", "FULL_PLATFORM")
+
+
 class WhatsNewContentType(sgqlc.types.Enum):
     __schema__ = nerdgraph
     __choices__ = ("ANNOUNCEMENT",)
 
 
 class WorkloadGroupRemainingEntitiesRuleBy(sgqlc.types.Enum):
     __schema__ = nerdgraph
```

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/input_objects.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/input_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,15 @@
     "ApiAccessKeySearchScope",
     "ApiAccessUpdateIngestKeyInput",
     "ApiAccessUpdateInput",
     "ApiAccessUpdateUserKeyInput",
     "ApmApplicationEntitySettings",
     "AuthorizationManagementAccountAccessGrant",
     "AuthorizationManagementGrantAccess",
+    "AuthorizationManagementGroupAccessGrant",
     "AuthorizationManagementOrganizationAccessGrant",
     "AuthorizationManagementRevokeAccess",
     "ChangeTrackingDataHandlingRules",
     "ChangeTrackingDeploymentInput",
     "ChangeTrackingSearchFilter",
     "ChangeTrackingTimeWindowInputWithDefaults",
     "CloudAlbIntegrationInput",
@@ -474,16 +475,26 @@
     "TaggingTagInput",
     "TaggingTagValueInput",
     "TimeWindowInput",
     "UserManagementCreateGroup",
     "UserManagementCreateUser",
     "UserManagementDeleteGroup",
     "UserManagementDeleteUser",
+    "UserManagementDisplayNameInput",
+    "UserManagementEmailInput",
+    "UserManagementEmailVerificationStateInput",
+    "UserManagementGroupFilterInput",
+    "UserManagementGroupIdInput",
+    "UserManagementNameInput",
+    "UserManagementPendingUpgradeRequestInput",
+    "UserManagementTypeInput",
     "UserManagementUpdateGroup",
     "UserManagementUpdateUser",
+    "UserManagementUserFilterInput",
+    "UserManagementUserIdInput",
     "UserManagementUsersGroupsInput",
     "UsersUserSearchQuery",
     "UsersUserSearchScope",
     "WhatsNewContentSearchQuery",
     "WorkloadAutomaticStatusInput",
     "WorkloadCreateInput",
     "WorkloadDuplicateInput",
@@ -605,14 +616,15 @@
     SortBy,
     SyntheticsDeviceOrientation,
     SyntheticsDeviceType,
     SyntheticsMonitorPeriod,
     SyntheticsMonitorStatus,
     SyntheticsStepType,
     UserManagementRequestedTierName,
+    UserManagementTypeEnum,
     WhatsNewContentType,
     WorkloadGroupRemainingEntitiesRuleBy,
     WorkloadRollupStrategy,
     WorkloadRuleThresholdType,
     WorkloadStatusValueInput,
 )
 from newrelic_sb_sdk.graphql.scalars import (
@@ -4000,54 +4012,78 @@
     role_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="roleId")
 
 
 class AuthorizationManagementGrantAccess(sgqlc.types.Input):
     __schema__ = nerdgraph
     __field_names__ = (
         "account_access_grants",
+        "group_access_grants",
         "group_id",
         "organization_access_grants",
     )
     account_access_grants = sgqlc.types.Field(
         sgqlc.types.list_of(
             sgqlc.types.non_null(AuthorizationManagementAccountAccessGrant)
         ),
         graphql_name="accountAccessGrants",
     )
 
+    group_access_grants = sgqlc.types.Field(
+        sgqlc.types.list_of(
+            sgqlc.types.non_null("AuthorizationManagementGroupAccessGrant")
+        ),
+        graphql_name="groupAccessGrants",
+    )
+
     group_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="groupId")
 
     organization_access_grants = sgqlc.types.Field(
         sgqlc.types.list_of(
             sgqlc.types.non_null("AuthorizationManagementOrganizationAccessGrant")
         ),
         graphql_name="organizationAccessGrants",
     )
 
 
+class AuthorizationManagementGroupAccessGrant(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("group_id", "role_id")
+    group_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="groupId")
+
+    role_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="roleId")
+
+
 class AuthorizationManagementOrganizationAccessGrant(sgqlc.types.Input):
     __schema__ = nerdgraph
     __field_names__ = ("role_id",)
     role_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="roleId")
 
 
 class AuthorizationManagementRevokeAccess(sgqlc.types.Input):
     __schema__ = nerdgraph
     __field_names__ = (
         "account_access_grants",
+        "group_access_grants",
         "group_id",
         "organization_access_grants",
     )
     account_access_grants = sgqlc.types.Field(
         sgqlc.types.list_of(
             sgqlc.types.non_null(AuthorizationManagementAccountAccessGrant)
         ),
         graphql_name="accountAccessGrants",
     )
 
+    group_access_grants = sgqlc.types.Field(
+        sgqlc.types.list_of(
+            sgqlc.types.non_null(AuthorizationManagementGroupAccessGrant)
+        ),
+        graphql_name="groupAccessGrants",
+    )
+
     group_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="groupId")
 
     organization_access_grants = sgqlc.types.Field(
         sgqlc.types.list_of(
             sgqlc.types.non_null(AuthorizationManagementOrganizationAccessGrant)
         ),
         graphql_name="organizationAccessGrants",
@@ -11346,14 +11382,78 @@
 
 class UserManagementDeleteUser(sgqlc.types.Input):
     __schema__ = nerdgraph
     __field_names__ = ("id",)
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="id")
 
 
+class UserManagementDisplayNameInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("contains", "eq")
+    contains = sgqlc.types.Field(String, graphql_name="contains")
+
+    eq = sgqlc.types.Field(String, graphql_name="eq")
+
+
+class UserManagementEmailInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("contains", "eq")
+    contains = sgqlc.types.Field(String, graphql_name="contains")
+
+    eq = sgqlc.types.Field(String, graphql_name="eq")
+
+
+class UserManagementEmailVerificationStateInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("pending",)
+    pending = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name="pending")
+
+
+class UserManagementGroupFilterInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("display_name", "id")
+    display_name = sgqlc.types.Field(
+        UserManagementDisplayNameInput, graphql_name="displayName"
+    )
+
+    id = sgqlc.types.Field("UserManagementGroupIdInput", graphql_name="id")
+
+
+class UserManagementGroupIdInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("eq", "in_")
+    eq = sgqlc.types.Field(ID, graphql_name="eq")
+
+    in_ = sgqlc.types.Field(
+        sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name="in"
+    )
+
+
+class UserManagementNameInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("contains", "eq")
+    contains = sgqlc.types.Field(String, graphql_name="contains")
+
+    eq = sgqlc.types.Field(String, graphql_name="eq")
+
+
+class UserManagementPendingUpgradeRequestInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("exists",)
+    exists = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name="exists")
+
+
+class UserManagementTypeInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("eq",)
+    eq = sgqlc.types.Field(
+        sgqlc.types.non_null(UserManagementTypeEnum), graphql_name="eq"
+    )
+
+
 class UserManagementUpdateGroup(sgqlc.types.Input):
     __schema__ = nerdgraph
     __field_names__ = ("display_name", "id")
     display_name = sgqlc.types.Field(
         sgqlc.types.non_null(String), graphql_name="displayName"
     )
 
@@ -11372,14 +11472,51 @@
     time_zone = sgqlc.types.Field(String, graphql_name="timeZone")
 
     user_type = sgqlc.types.Field(
         UserManagementRequestedTierName, graphql_name="userType"
     )
 
 
+class UserManagementUserFilterInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = (
+        "email",
+        "email_verification_state",
+        "id",
+        "name",
+        "pending_upgrade_request",
+        "type",
+    )
+    email = sgqlc.types.Field(UserManagementEmailInput, graphql_name="email")
+
+    email_verification_state = sgqlc.types.Field(
+        UserManagementEmailVerificationStateInput, graphql_name="emailVerificationState"
+    )
+
+    id = sgqlc.types.Field("UserManagementUserIdInput", graphql_name="id")
+
+    name = sgqlc.types.Field(UserManagementNameInput, graphql_name="name")
+
+    pending_upgrade_request = sgqlc.types.Field(
+        UserManagementPendingUpgradeRequestInput, graphql_name="pendingUpgradeRequest"
+    )
+
+    type = sgqlc.types.Field(UserManagementTypeInput, graphql_name="type")
+
+
+class UserManagementUserIdInput(sgqlc.types.Input):
+    __schema__ = nerdgraph
+    __field_names__ = ("eq", "in_")
+    eq = sgqlc.types.Field(ID, graphql_name="eq")
+
+    in_ = sgqlc.types.Field(
+        sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name="in"
+    )
+
+
 class UserManagementUsersGroupsInput(sgqlc.types.Input):
     __schema__ = nerdgraph
     __field_names__ = ("group_ids", "user_ids")
     group_ids = sgqlc.types.Field(
         sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))),
         graphql_name="groupIds",
     )
```

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/objects.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,14 +343,16 @@
     "EntityGoldenContextScopedGoldenMetrics",
     "EntityGoldenContextScopedGoldenTags",
     "EntityGoldenGoldenMetricsError",
     "EntityGoldenMetric",
     "EntityGoldenMetricDefinition",
     "EntityGoldenMetricsDomainTypeScoped",
     "EntityGoldenMetricsDomainTypeScopedResponse",
+    "EntityGoldenOriginalDefinitionWithSelector",
+    "EntityGoldenOriginalQueryWithSelector",
     "EntityGoldenTag",
     "EntityGoldenTagsDomainTypeScoped",
     "EntityGoldenTagsDomainTypeScopedResponse",
     "EntityRelationship",
     "EntityRelationshipNode",
     "EntityRelationshipRelatedEntitiesResult",
     "EntityRelationshipUserDefinedCreateOrReplaceResult",
@@ -1268,16 +1270,18 @@
     TaggingTagInput,
     TaggingTagValueInput,
     TimeWindowInput,
     UserManagementCreateGroup,
     UserManagementCreateUser,
     UserManagementDeleteGroup,
     UserManagementDeleteUser,
+    UserManagementGroupFilterInput,
     UserManagementUpdateGroup,
     UserManagementUpdateUser,
+    UserManagementUserFilterInput,
     UserManagementUsersGroupsInput,
     UsersUserSearchQuery,
     WhatsNewContentSearchQuery,
     WorkloadCreateInput,
     WorkloadDuplicateInput,
     WorkloadUpdateInput,
 )
@@ -6727,24 +6731,27 @@
 
 
 class AuthorizationManagementGrantedRole(sgqlc.types.Type):
     __schema__ = nerdgraph
     __field_names__ = (
         "account_id",
         "display_name",
+        "group_id",
         "id",
         "name",
         "organization_id",
         "role_id",
         "type",
     )
     account_id = sgqlc.types.Field(Int, graphql_name="accountId")
 
     display_name = sgqlc.types.Field(String, graphql_name="displayName")
 
+    group_id = sgqlc.types.Field(ID, graphql_name="groupId")
+
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="id")
 
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name="name")
 
     organization_id = sgqlc.types.Field(ID, graphql_name="organizationId")
 
     role_id = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name="roleId")
@@ -8973,25 +8980,52 @@
     type = sgqlc.types.Field(
         sgqlc.types.non_null(EntityGoldenGoldenMetricsErrorType), graphql_name="type"
     )
 
 
 class EntityGoldenMetric(sgqlc.types.Type):
     __schema__ = nerdgraph
-    __field_names__ = ("definition", "metric_name", "name", "query", "title", "unit")
+    __field_names__ = (
+        "definition",
+        "metric_name",
+        "name",
+        "original_definitions",
+        "original_queries",
+        "query",
+        "title",
+        "unit",
+    )
     definition = sgqlc.types.Field(
         sgqlc.types.non_null("EntityGoldenMetricDefinition"), graphql_name="definition"
     )
 
     metric_name = sgqlc.types.Field(
         sgqlc.types.non_null(String), graphql_name="metricName"
     )
 
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name="name")
 
+    original_definitions = sgqlc.types.Field(
+        sgqlc.types.non_null(
+            sgqlc.types.list_of(
+                sgqlc.types.non_null("EntityGoldenOriginalDefinitionWithSelector")
+            )
+        ),
+        graphql_name="originalDefinitions",
+    )
+
+    original_queries = sgqlc.types.Field(
+        sgqlc.types.non_null(
+            sgqlc.types.list_of(
+                sgqlc.types.non_null("EntityGoldenOriginalQueryWithSelector")
+            )
+        ),
+        graphql_name="originalQueries",
+    )
+
     query = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name="query")
 
     title = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name="title")
 
     unit = sgqlc.types.Field(
         sgqlc.types.non_null(EntityGoldenMetricUnit), graphql_name="unit"
     )
@@ -9050,14 +9084,36 @@
     )
 
     metrics = sgqlc.types.Field(
         EntityGoldenMetricsDomainTypeScoped, graphql_name="metrics"
     )
 
 
+class EntityGoldenOriginalDefinitionWithSelector(sgqlc.types.Type):
+    __schema__ = nerdgraph
+    __field_names__ = ("definition", "selector_value")
+    definition = sgqlc.types.Field(
+        sgqlc.types.non_null(EntityGoldenMetricDefinition), graphql_name="definition"
+    )
+
+    selector_value = sgqlc.types.Field(
+        sgqlc.types.non_null(String), graphql_name="selectorValue"
+    )
+
+
+class EntityGoldenOriginalQueryWithSelector(sgqlc.types.Type):
+    __schema__ = nerdgraph
+    __field_names__ = ("query", "selector_value")
+    query = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name="query")
+
+    selector_value = sgqlc.types.Field(
+        sgqlc.types.non_null(String), graphql_name="selectorValue"
+    )
+
+
 class EntityGoldenTag(sgqlc.types.Type):
     __schema__ = nerdgraph
     __field_names__ = ("key",)
     key = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name="key")
 
 
 class EntityGoldenTagsDomainTypeScoped(sgqlc.types.Type):
@@ -20161,27 +20217,36 @@
         args=sgqlc.types.ArgDict(
             (
                 (
                     "cursor",
                     sgqlc.types.Arg(String, graphql_name="cursor", default=None),
                 ),
                 (
+                    "filter",
+                    sgqlc.types.Arg(
+                        UserManagementGroupFilterInput,
+                        graphql_name="filter",
+                        default=None,
+                    ),
+                ),
+                (
                     "id",
                     sgqlc.types.Arg(
                         sgqlc.types.list_of(sgqlc.types.non_null(ID)),
                         graphql_name="id",
                         default=None,
                     ),
                 ),
             )
         ),
     )
     """Arguments:
 
     * `cursor` (`String`)
+    * `filter` (`UserManagementGroupFilterInput`)
     * `id` (`[ID!]`)
     """
 
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name="id")
 
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name="name")
 
@@ -20195,27 +20260,36 @@
         args=sgqlc.types.ArgDict(
             (
                 (
                     "cursor",
                     sgqlc.types.Arg(String, graphql_name="cursor", default=None),
                 ),
                 (
+                    "filter",
+                    sgqlc.types.Arg(
+                        UserManagementUserFilterInput,
+                        graphql_name="filter",
+                        default=None,
+                    ),
+                ),
+                (
                     "id",
                     sgqlc.types.Arg(
                         sgqlc.types.list_of(sgqlc.types.non_null(ID)),
                         graphql_name="id",
                         default=None,
                     ),
                 ),
             )
         ),
     )
     """Arguments:
 
     * `cursor` (`String`)
+    * `filter` (`UserManagementUserFilterInput`)
     * `id` (`[ID!]`)
     """
 
 
 class UserManagementAuthenticationDomains(sgqlc.types.Type):
     __schema__ = nerdgraph
     __field_names__ = ("authentication_domains", "next_cursor", "total_count")
```

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/scalars.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/scalars.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/response.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/response.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/text.py` & `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/text.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.7.0/PKG-INFO` & `newrelic_sb_sdk-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-sb-sdk
-Version: 0.7.0
+Version: 0.8.0
 Summary: New Relic SDK to interact with Nerdgraph API.
 Home-page: https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk
 License: MIT
 Keywords: Softbutterfly,New Relic,SDK
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -21,33 +21,32 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
-Requires-Dist: enforce-typing (>=1.0.0.post1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues
 Project-URL: Documentation, https://softbutterfly.gitlab.io/open-source/newrelic-sb-sdk/
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.7.0/newrelic-sb-sdk-v0.7.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.8.0/newrelic-sb-sdk-v0.8.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/newrelic-sb-sdk)
 ![PyPI - Package version](https://img.shields.io/pypi/v/newrelic-sb-sdk)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/newrelic-sb-sdk)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/newrelic-sb-sdk)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/1c25dec51e1c4a719be4c2d4ebe7eef6)](https://app.codacy.com/gl/softbutterfly/newrelic-sb-sdk/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/1c25dec51e1c4a719be4c2d4ebe7eef6)](https://app.codacy.com/gl/softbutterfly/newrelic-sb-sdk/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![pipeline status](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/badges/master/pipeline.svg)](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/commits/master)
 
 
 # New Relic SB SDK
 
 New Relic SDK built by SoftButterfly to automate common New Relic One observability platform tasks
```

