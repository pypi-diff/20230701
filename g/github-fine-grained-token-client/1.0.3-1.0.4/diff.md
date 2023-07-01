# Comparing `tmp/github_fine_grained_token_client-1.0.3.tar.gz` & `tmp/github_fine_grained_token_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_fine_grained_token_client-1.0.3.tar", max compression
+gzip compressed data, was "github_fine_grained_token_client-1.0.4.tar", max compression
```

## Comparing `github_fine_grained_token_client-1.0.3.tar` & `github_fine_grained_token_client-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1067 2023-06-29 19:03:44.061691 github_fine_grained_token_client-1.0.3/LICENSE
--rw-r--r--   0        0        0     2920 2023-06-29 19:03:44.061691 github_fine_grained_token_client-1.0.3/README.md
--rw-r--r--   0        0        0     2256 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/__init__.py
--rw-r--r--   0        0        0      529 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/abstract_http_session.py
--rw-r--r--   0        0        0    10737 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/app.py
--rw-r--r--   0        0        0    36910 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/asynchronous_client.py
--rw-r--r--   0        0        0     9393 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/cli.py
--rw-r--r--   0        0        0     2492 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/common.py
--rw-r--r--   0        0        0     2146 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/credentials.py
--rw-r--r--   0        0        0      441 2023-06-29 19:03:44.062691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/dev.py
--rw-r--r--   0        0        0     7054 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/permissions.py
--rw-r--r--   0        0        0     3927 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/persisting_http_session.py
--rw-r--r--   0        0        0     2817 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/two_factor_authentication.py
--rw-r--r--   0        0        0        0 2023-06-29 19:03:44.085691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/__init__.py
--rw-r--r--   0        0        0      458 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/asyncio.py
--rw-r--r--   0        0        0      677 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/bs4.py
--rw-r--r--   0        0        0      568 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/sequences.py
--rw-r--r--   0        0        0     1564 2023-06-29 19:03:44.063691 github_fine_grained_token_client-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 github_fine_grained_token_client-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-01 14:39:23.754248 github_fine_grained_token_client-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2920 2023-07-01 14:39:23.754248 github_fine_grained_token_client-1.0.4/README.md
+-rw-r--r--   0        0        0     2256 2023-07-01 14:39:23.754248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/__init__.py
+-rw-r--r--   0        0        0      529 2023-07-01 14:39:23.754248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/abstract_http_session.py
+-rw-r--r--   0        0        0    10737 2023-07-01 14:39:23.754248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/app.py
+-rw-r--r--   0        0        0    37822 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/asynchronous_client.py
+-rw-r--r--   0        0        0     9393 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/cli.py
+-rw-r--r--   0        0        0     2580 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/common.py
+-rw-r--r--   0        0        0     2146 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/credentials.py
+-rw-r--r--   0        0        0      441 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/dev.py
+-rw-r--r--   0        0        0     7054 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/permissions.py
+-rw-r--r--   0        0        0     3927 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/persisting_http_session.py
+-rw-r--r--   0        0        0     2817 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/two_factor_authentication.py
+-rw-r--r--   0        0        0        0 2023-07-01 14:39:23.780248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/utils/__init__.py
+-rw-r--r--   0        0        0      458 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/utils/asyncio.py
+-rw-r--r--   0        0        0      677 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/utils/bs4.py
+-rw-r--r--   0        0        0      568 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/utils/sequences.py
+-rw-r--r--   0        0        0     1564 2023-07-01 14:39:23.755248 github_fine_grained_token_client-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 github_fine_grained_token_client-1.0.4/PKG-INFO
```

### Comparing `github_fine_grained_token_client-1.0.3/LICENSE` & `github_fine_grained_token_client-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/README.md` & `github_fine_grained_token_client-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/__init__.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/__init__.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/abstract_http_session.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/abstract_http_session.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/app.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/app.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/asynchronous_client.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/asynchronous_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     AllRepositories,
     FineGrainedTokenBulkInfo,
     FineGrainedTokenCompletePersistentInfo,
     FineGrainedTokenIndividualInfo,
     FineGrainedTokenScope,
     FineGrainedTokenStandardInfo,
     LoginError,
+    NotImplementedTwoFactorAuthenticationMethodError,
     PublicRepositories,
     RepositoryNotFoundError,
     SelectRepositories,
     TokenCreationError,
     TokenNameAlreadyTakenError,
     TwoFactorAuthenticationError,
     UnexpectedContentError,
@@ -246,14 +247,28 @@
                         html.select("#js-flash-container")
                     )
                     if login_error is not None:
                         raise LoginError(login_error.get_text().strip())
                     raise UnexpectedContentError(
                         "ended up back on login page but not sure why"
                     )
+                if str(response.url).startswith(
+                    self._make_url("/sessions/two-factor/")
+                ) and str(response.url) != self._make_url(
+                    "/sessions/two-factor/app"
+                ):
+                    raise NotImplementedTwoFactorAuthenticationMethodError(
+                        f"ended up on page {response.url} which indicates "
+                        "that your default 2FA method is something other than "
+                        '"authenticator app", but currently, only 2FA via an '
+                        "authenticator app is supported and must be set as "
+                        "the default in your GitHub authentication settings; "
+                        "issue: https://gitlab.com/smheidrich/"
+                        "github-fine-grained-token-client/-/issues/14"
+                    )
                 if (
                     destination_url is not None
                     and str(response.url) != destination_url
                     and str(response.url)
                     != self._make_url("/sessions/two-factor/app")
                 ):
                     raise UnexpectedPageError(
```

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/cli.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/cli.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/common.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     pass
 
 
 class TwoFactorAuthenticationError(Exception):
     pass
 
 
+class NotImplementedTwoFactorAuthenticationMethodError(NotImplementedError):
+    pass
+
+
 class TokenCreationError(Exception):
     pass
 
 
 class TokenNameError(TokenCreationError):
     pass
```

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/credentials.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/credentials.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/permissions.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/permissions.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/persisting_http_session.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/persisting_http_session.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/two_factor_authentication.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/two_factor_authentication.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/bs4.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/utils/bs4.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/github_fine_grained_token_client/utils/sequences.py` & `github_fine_grained_token_client-1.0.4/github_fine_grained_token_client/utils/sequences.py`

 * *Files identical despite different names*

### Comparing `github_fine_grained_token_client-1.0.3/pyproject.toml` & `github_fine_grained_token_client-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "github-fine-grained-token-client"
-version = "1.0.3"
+version = "1.0.4"
 description = "Library and CLI tool for creating fine-grained GitHub tokens"
 authors = ["smheidrich <smheidrich@weltenfunktion.de>"]
 readme = "README.md"
 homepage = "https://smheidrich.gitlab.io/github-fine-grained-token-client/"
 repository = "https://gitlab.com/smheidrich/github-fine-grained-token-client"
 documentation = "https://smheidrich.gitlab.io/github-fine-grained-token-client/"
```

### Comparing `github_fine_grained_token_client-1.0.3/PKG-INFO` & `github_fine_grained_token_client-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-fine-grained-token-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library and CLI tool for creating fine-grained GitHub tokens
 Home-page: https://smheidrich.gitlab.io/github-fine-grained-token-client/
 Author: smheidrich
 Author-email: smheidrich@weltenfunktion.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

