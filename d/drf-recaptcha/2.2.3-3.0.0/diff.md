# Comparing `tmp/drf-recaptcha-2.2.3.tar.gz` & `tmp/drf-recaptcha-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-recaptcha-2.2.3.tar", last modified: Sun Apr 23 05:39:50 2023, max compression
+gzip compressed data, was "drf-recaptcha-3.0.0.tar", last modified: Sat Jul  1 15:24:36 2023, max compression
```

## Comparing `drf-recaptcha-2.2.3.tar` & `drf-recaptcha-3.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:50.904832 drf-recaptcha-2.2.3/drf_recaptcha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/drf_recaptcha/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 05:39:50.000000 drf-recaptcha-2.2.3/drf_recaptcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 05:39:50.908832 drf-recaptcha-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-23 05:39:39.000000 drf-recaptcha-2.2.3/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:36.166619 drf-recaptcha-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-01 15:24:36.166619 drf-recaptcha-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:36.162618 drf-recaptcha-3.0.0/drf_recaptcha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/drf_recaptcha/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:36.162618 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 15:24:36.000000 drf-recaptcha-3.0.0/drf_recaptcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-01 15:24:36.166619 drf-recaptcha-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:24:36.166619 drf-recaptcha-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_secret_key_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-01 15:24:23.000000 drf-recaptcha-3.0.0/tests/test_validator.py
```

### Comparing `drf-recaptcha-2.2.3/LICENSE.md` & `drf-recaptcha-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.3/PKG-INFO` & `drf-recaptcha-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-recaptcha
-Version: 2.2.3
+Version: 3.0.0
 Summary: Django rest framework recaptcha field serializer.
 Home-page: https://github.com/llybin/drf-recaptcha
 Author: Lev Lybin
 Author-email: lev.lybin@gmail.com
 License: MIT
 Keywords: django,drf,rest,django-rest-framework,reCAPTCHA,reCAPTCHA v2,reCAPTCHA v3
 Classifier: Development Status :: 5 - Production/Stable
@@ -114,14 +114,49 @@
         model = Feedback
         fields = ("phone", "full_name", "email", "comment", "recaptcha")
 
     def validate(self, attrs):
         attrs.pop("recaptcha")
         ...
         return attrs
+
+    
+class DynamicContextSecretKey(APIView):
+    def post(self, request):
+        if request.platform == "android":
+            recaptcha_secret_key = "SPECIAL_FOR_ANDROID"
+        else:
+            recaptcha_secret_key = "SPECIAL_FOR_IOS"
+        serializer = WithReCaptchaSerializer(
+            data=request.data,
+            context={
+                "request": request,
+                "recaptcha_secret_key": recaptcha_secret_key,
+            },
+        )
+        serializer.is_valid(raise_exception=True)
+        ...
+    
+
+class DynamicContextSecretKey(GenericAPIView):
+    serializer_class = WithReCaptchaSerializer
+    
+    def get_serializer_context(self):
+        if self.request.platform == "android":
+            recaptcha_secret_key = "SPECIAL_FOR_ANDROID"
+        else:
+            recaptcha_secret_key = "SPECIAL_FOR_IOS"
+        context = super().get_serializer_context()
+        context.update({"recaptcha_secret_key": recaptcha_secret_key})
+        return context
+    
+
+class MobileSerializer(Serializer):
+    recaptcha = ReCaptchaV3Field(secret_key="")
+    ...
 ```
 
 ## Settings
 
 `DRF_RECAPTCHA_SECRET_KEY` - set your Google reCAPTCHA secret key. Type: str.
 
 `DRF_RECAPTCHA_DEFAULT_V3_SCORE` - by default: `0.5`. Type: float.
@@ -130,14 +165,20 @@
 
 `DRF_RECAPTCHA_DOMAIN` - by default: `www.google.com`. Type: str.
 
 `DRF_RECAPTCHA_PROXY` - by default: `{}`. Type: dict. e.g. `{'http': 'http://127.0.0.1:8000', 'https': 'https://127.0.0.1:8000'}`
 
 `DRF_RECAPTCHA_VERIFY_REQUEST_TIMEOUT` - by default: `10`. Type: int.
 
+### Priority of secret_key value
+
+1.  settings `DRF_RECAPTCHA_SECRET_KEY`
+2.  the argument `secret_key` of field
+3.  request.context["recaptcha_secret_key"]
+
 ## reCAPTCHA v3
 
 Validation is passed if the score value returned by Google is greater than or equal to required score.
 
 Required score value: `0.0 - 1.0`
 
 ### Priority of score value
```

### Comparing `drf-recaptcha-2.2.3/README.md` & `drf-recaptcha-3.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -78,14 +78,49 @@
         model = Feedback
         fields = ("phone", "full_name", "email", "comment", "recaptcha")
 
     def validate(self, attrs):
         attrs.pop("recaptcha")
         ...
         return attrs
+
+    
+class DynamicContextSecretKey(APIView):
+    def post(self, request):
+        if request.platform == "android":
+            recaptcha_secret_key = "SPECIAL_FOR_ANDROID"
+        else:
+            recaptcha_secret_key = "SPECIAL_FOR_IOS"
+        serializer = WithReCaptchaSerializer(
+            data=request.data,
+            context={
+                "request": request,
+                "recaptcha_secret_key": recaptcha_secret_key,
+            },
+        )
+        serializer.is_valid(raise_exception=True)
+        ...
+    
+
+class DynamicContextSecretKey(GenericAPIView):
+    serializer_class = WithReCaptchaSerializer
+    
+    def get_serializer_context(self):
+        if self.request.platform == "android":
+            recaptcha_secret_key = "SPECIAL_FOR_ANDROID"
+        else:
+            recaptcha_secret_key = "SPECIAL_FOR_IOS"
+        context = super().get_serializer_context()
+        context.update({"recaptcha_secret_key": recaptcha_secret_key})
+        return context
+    
+
+class MobileSerializer(Serializer):
+    recaptcha = ReCaptchaV3Field(secret_key="")
+    ...
 ```
 
 ## Settings
 
 `DRF_RECAPTCHA_SECRET_KEY` - set your Google reCAPTCHA secret key. Type: str.
 
 `DRF_RECAPTCHA_DEFAULT_V3_SCORE` - by default: `0.5`. Type: float.
@@ -94,14 +129,20 @@
 
 `DRF_RECAPTCHA_DOMAIN` - by default: `www.google.com`. Type: str.
 
 `DRF_RECAPTCHA_PROXY` - by default: `{}`. Type: dict. e.g. `{'http': 'http://127.0.0.1:8000', 'https': 'https://127.0.0.1:8000'}`
 
 `DRF_RECAPTCHA_VERIFY_REQUEST_TIMEOUT` - by default: `10`. Type: int.
 
+### Priority of secret_key value
+
+1.  settings `DRF_RECAPTCHA_SECRET_KEY`
+2.  the argument `secret_key` of field
+3.  request.context["recaptcha_secret_key"]
+
 ## reCAPTCHA v3
 
 Validation is passed if the score value returned by Google is greater than or equal to required score.
 
 Required score value: `0.0 - 1.0`
 
 ### Priority of score value
```

### Comparing `drf-recaptcha-2.2.3/drf_recaptcha/checks.py` & `drf-recaptcha-3.0.0/drf_recaptcha/checks.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.3/drf_recaptcha/client.py` & `drf-recaptcha-3.0.0/drf_recaptcha/client.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.3/drf_recaptcha/constants.py` & `drf-recaptcha-3.0.0/drf_recaptcha/constants.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.3/drf_recaptcha/fields.py` & `drf-recaptcha-3.0.0/drf_recaptcha/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from rest_framework.serializers import CharField
 
 from drf_recaptcha.constants import DEFAULT_V3_SCORE
 from drf_recaptcha.validators import ReCaptchaV2Validator, ReCaptchaV3Validator
 
 
 class ReCaptchaV2Field(CharField):
-    def __init__(self, **kwargs):
+    def __init__(self, secret_key: str = None, **kwargs):
         super().__init__(**kwargs)
 
         self.write_only = True
 
-        validator = ReCaptchaV2Validator(secret_key=settings.DRF_RECAPTCHA_SECRET_KEY)
+        secret_key = secret_key or settings.DRF_RECAPTCHA_SECRET_KEY
+
+        validator = ReCaptchaV2Validator(secret_key=secret_key)
         self.validators.append(validator)
 
 
 def validate_v3_settings_score_value(value: int or float or None, action: str = None):
     if value is None:
         return
 
@@ -56,15 +58,21 @@
         settings, "DRF_RECAPTCHA_DEFAULT_V3_SCORE", None
     )
     validate_v3_settings_score_value(default_score_from_settings)
     return default_score_from_settings
 
 
 class ReCaptchaV3Field(CharField):
-    def __init__(self, action: str, required_score: float = None, **kwargs):
+    def __init__(
+        self,
+        action: str,
+        required_score: float = None,
+        secret_key: str = None,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
 
         self.write_only = True
 
         action_score_from_settings = get_v3_action_score_from_settings(action)
         default_score_from_settings = get_v3_default_score_from_settings()
         validate_v3_settings_score_value(required_score, action)
@@ -72,18 +80,20 @@
         self.required_score = (
             action_score_from_settings
             or required_score
             or default_score_from_settings
             or DEFAULT_V3_SCORE
         )
 
+        secret_key = secret_key or settings.DRF_RECAPTCHA_SECRET_KEY
+
         self.__validator = ReCaptchaV3Validator(
             action=action,
             required_score=self.required_score,
-            secret_key=settings.DRF_RECAPTCHA_SECRET_KEY,
+            secret_key=secret_key,
         )
         self.validators.append(self.__validator)
 
     @property
     def score(self):
         score = self.__validator.score
         if score is None:
```

### Comparing `drf-recaptcha-2.2.3/drf_recaptcha/validators.py` & `drf-recaptcha-3.0.0/drf_recaptcha/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,139 @@
 import logging
+from typing import TYPE_CHECKING
 from urllib.error import HTTPError
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from ipware import get_client_ip
 from rest_framework.serializers import ValidationError
 
 from drf_recaptcha import client
 
+if TYPE_CHECKING:
+    from drf_recaptcha.client import RecaptchaResponse
+
 logger = logging.getLogger(__name__)
 
 
 class ReCaptchaValidator:
     requires_context = True
 
     messages = {
         "captcha_invalid": "Error verifying reCAPTCHA, please try again.",
         "captcha_error": "Error verifying reCAPTCHA, please try again.",
     }
-    recaptcha_client_ip = ""
-    recaptcha_secret_key = ""
+    default_recaptcha_secret_key = ""
+
+    def __call__(self, value, serializer_field):
+        if self._is_testing():
+            self._run_validation_as_testing()
+            return
+
+        client_ip = self._get_client_ip_from_context(serializer_field)
+        recaptcha_secret_key = self._get_secret_key_from_context_or_default(
+            serializer_field
+        )
+
+        check_captcha = self._get_captcha_response_with_payload(
+            value=value,
+            secret_key=recaptcha_secret_key,
+            client_ip=client_ip,
+        )
+
+        self._pre_validate_response(check_captcha)
+        self._process_response(check_captcha)
 
     @staticmethod
-    def is_testing() -> bool:
+    def _is_testing() -> bool:
         return getattr(settings, "DRF_RECAPTCHA_TESTING", False)
 
-    def testing_validation(self):
+    def _run_validation_as_testing(self):
         testing_result = getattr(settings, "DRF_RECAPTCHA_TESTING_PASS", True)
         if not testing_result:
             raise ValidationError(
                 self.messages["captcha_invalid"], code="captcha_invalid"
             )
 
-    def set_client_ip(self, serializer_field):
+    def _get_secret_key_from_context_or_default(self, serializer_field) -> str:
+        return serializer_field.context.get(
+            "recaptcha_secret_key", self.default_recaptcha_secret_key
+        )
+
+    @staticmethod
+    def _get_client_ip_from_context(serializer_field):
         request = serializer_field.context.get("request")
         if not request:
             raise ImproperlyConfigured(
                 "Couldn't get client ip address. Check your serializer gets context with request."
             )
 
-        self.recaptcha_client_ip, _ = get_client_ip(request)
+        recaptcha_client_ip, _ = get_client_ip(request)
+        return recaptcha_client_ip
 
-    def get_response(self, value: str) -> client.RecaptchaResponse:
+    def _get_captcha_response_with_payload(
+        self, value: str, secret_key: str, client_ip: str
+    ) -> "RecaptchaResponse":
         try:
             check_captcha = client.submit(
                 recaptcha_response=value,
-                secret_key=self.recaptcha_secret_key,
-                remoteip=self.recaptcha_client_ip,
+                secret_key=secret_key,
+                remoteip=client_ip,
             )
         except HTTPError:  # Catch timeouts, etc
             logger.exception("Couldn't get response, HTTPError")
             raise ValidationError(self.messages["captcha_error"], code="captcha_error")
 
         return check_captcha
 
-    def pre_validate_response(self, check_captcha: client.RecaptchaResponse):
-        if not check_captcha.is_valid:
-            logger.error(
-                "ReCAPTCHA validation failed due to: %s", check_captcha.error_codes
-            )
-            raise ValidationError(
-                self.messages["captcha_invalid"], code="captcha_invalid"
-            )
-
+    def _pre_validate_response(self, check_captcha: "RecaptchaResponse") -> None:
+        if check_captcha.is_valid:
+            return
 
-class ReCaptchaV2Validator(ReCaptchaValidator):
-    def __init__(self, secret_key):
-        self.recaptcha_secret_key = secret_key
+        logger.error(
+            "ReCAPTCHA validation failed due to: %s", check_captcha.error_codes
+        )
+        raise ValidationError(self.messages["captcha_invalid"], code="captcha_invalid")
 
-    def __call__(self, value, serializer_field=None):
-        if serializer_field and not self.recaptcha_client_ip:
-            self.set_client_ip(serializer_field)
+    def _process_response(self, check_captcha_response):
+        ...
 
-        if self.is_testing():
-            self.testing_validation()
-            return
 
-        check_captcha = self.get_response(value)
+class ReCaptchaV2Validator(ReCaptchaValidator):
+    def __init__(self, secret_key):
+        self.default_recaptcha_secret_key = secret_key
 
-        self.pre_validate_response(check_captcha)
+    def _process_response(self, check_captcha_response):
+        score = check_captcha_response.extra_data.get("score", None)
 
-        score = check_captcha.extra_data.get("score", None)
         if score is not None:
             logger.error(
                 "The response contains score, reCAPTCHA v2 response doesn't"
                 " contains score, probably secret key for reCAPTCHA v3"
             )
             raise ValidationError(self.messages["captcha_error"], code="captcha_error")
 
 
 class ReCaptchaV3Validator(ReCaptchaValidator):
     def __init__(self, action, required_score, secret_key):
         self.recaptcha_action = action
         self.recaptcha_required_score = required_score
-        self.recaptcha_secret_key = secret_key
         self.score = None
+        self.default_recaptcha_secret_key = secret_key
 
-    def __call__(self, value, serializer_field=None):
-        if serializer_field and not self.recaptcha_client_ip:
-            self.set_client_ip(serializer_field)
-
-        if self.is_testing():
-            self.testing_validation()
-            return
-
-        check_captcha = self.get_response(value)
-
-        self.pre_validate_response(check_captcha)
-
-        self.score = check_captcha.extra_data.get("score", None)
+    def _process_response(self, check_captcha_response):
+        self.score = check_captcha_response.extra_data.get("score", None)
         if self.score is None:
             logger.error(
                 "The response not contains score, reCAPTCHA v3 response must"
                 " contains score, probably secret key for reCAPTCHA v2"
             )
             raise ValidationError(self.messages["captcha_error"], code="captcha_error")
 
-        action = check_captcha.extra_data.get("action", "")
+        action = check_captcha_response.extra_data.get("action", "")
 
         if self.recaptcha_required_score >= float(self.score):
             logger.error(
                 "ReCAPTCHA validation failed due to score of %s"
                 " being lower than the required amount for action '%s'.",
                 self.score,
                 action,
```

### Comparing `drf-recaptcha-2.2.3/drf_recaptcha.egg-info/PKG-INFO` & `drf-recaptcha-3.0.0/drf_recaptcha.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-recaptcha
-Version: 2.2.3
+Version: 3.0.0
 Summary: Django rest framework recaptcha field serializer.
 Home-page: https://github.com/llybin/drf-recaptcha
 Author: Lev Lybin
 Author-email: lev.lybin@gmail.com
 License: MIT
 Keywords: django,drf,rest,django-rest-framework,reCAPTCHA,reCAPTCHA v2,reCAPTCHA v3
 Classifier: Development Status :: 5 - Production/Stable
@@ -114,14 +114,49 @@
         model = Feedback
         fields = ("phone", "full_name", "email", "comment", "recaptcha")
 
     def validate(self, attrs):
         attrs.pop("recaptcha")
         ...
         return attrs
+
+    
+class DynamicContextSecretKey(APIView):
+    def post(self, request):
+        if request.platform == "android":
+            recaptcha_secret_key = "SPECIAL_FOR_ANDROID"
+        else:
+            recaptcha_secret_key = "SPECIAL_FOR_IOS"
+        serializer = WithReCaptchaSerializer(
+            data=request.data,
+            context={
+                "request": request,
+                "recaptcha_secret_key": recaptcha_secret_key,
+            },
+        )
+        serializer.is_valid(raise_exception=True)
+        ...
+    
+
+class DynamicContextSecretKey(GenericAPIView):
+    serializer_class = WithReCaptchaSerializer
+    
+    def get_serializer_context(self):
+        if self.request.platform == "android":
+            recaptcha_secret_key = "SPECIAL_FOR_ANDROID"
+        else:
+            recaptcha_secret_key = "SPECIAL_FOR_IOS"
+        context = super().get_serializer_context()
+        context.update({"recaptcha_secret_key": recaptcha_secret_key})
+        return context
+    
+
+class MobileSerializer(Serializer):
+    recaptcha = ReCaptchaV3Field(secret_key="")
+    ...
 ```
 
 ## Settings
 
 `DRF_RECAPTCHA_SECRET_KEY` - set your Google reCAPTCHA secret key. Type: str.
 
 `DRF_RECAPTCHA_DEFAULT_V3_SCORE` - by default: `0.5`. Type: float.
@@ -130,14 +165,20 @@
 
 `DRF_RECAPTCHA_DOMAIN` - by default: `www.google.com`. Type: str.
 
 `DRF_RECAPTCHA_PROXY` - by default: `{}`. Type: dict. e.g. `{'http': 'http://127.0.0.1:8000', 'https': 'https://127.0.0.1:8000'}`
 
 `DRF_RECAPTCHA_VERIFY_REQUEST_TIMEOUT` - by default: `10`. Type: int.
 
+### Priority of secret_key value
+
+1.  settings `DRF_RECAPTCHA_SECRET_KEY`
+2.  the argument `secret_key` of field
+3.  request.context["recaptcha_secret_key"]
+
 ## reCAPTCHA v3
 
 Validation is passed if the score value returned by Google is greater than or equal to required score.
 
 Required score value: `0.0 - 1.0`
 
 ### Priority of score value
```

### Comparing `drf-recaptcha-2.2.3/drf_recaptcha.egg-info/SOURCES.txt` & `drf-recaptcha-3.0.0/drf_recaptcha.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -25,11 +25,14 @@
 00000180: 6368 612e 6567 672d 696e 666f 2f72 6571  cha.egg-info/req
 00000190: 7569 7265 732e 7478 740a 6472 665f 7265  uires.txt.drf_re
 000001a0: 6361 7074 6368 612e 6567 672d 696e 666f  captcha.egg-info
 000001b0: 2f74 6f70 5f6c 6576 656c 2e74 7874 0a74  /top_level.txt.t
 000001c0: 6573 7473 2f74 6573 745f 6368 6563 6b73  ests/test_checks
 000001d0: 2e70 790a 7465 7374 732f 7465 7374 5f66  .py.tests/test_f
 000001e0: 6965 6c64 732e 7079 0a74 6573 7473 2f74  ields.py.tests/t
-000001f0: 6573 745f 7365 7269 616c 697a 6572 732e  est_serializers.
-00000200: 7079 0a74 6573 7473 2f74 6573 745f 7465  py.tests/test_te
-00000210: 7374 696e 672e 7079 0a74 6573 7473 2f74  sting.py.tests/t
-00000220: 6573 745f 7661 6c69 6461 746f 722e 7079  est_validator.py
+000001f0: 6573 745f 7365 6372 6574 5f6b 6579 5f70  est_secret_key_p
+00000200: 7269 6f72 6974 792e 7079 0a74 6573 7473  riority.py.tests
+00000210: 2f74 6573 745f 7365 7269 616c 697a 6572  /test_serializer
+00000220: 732e 7079 0a74 6573 7473 2f74 6573 745f  s.py.tests/test_
+00000230: 7465 7374 696e 672e 7079 0a74 6573 7473  testing.py.tests
+00000240: 2f74 6573 745f 7661 6c69 6461 746f 722e  /test_validator.
+00000250: 7079                                     py
```

### Comparing `drf-recaptcha-2.2.3/setup.cfg` & `drf-recaptcha-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.3/setup.py` & `drf-recaptcha-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 def read(f):
     return open(f, encoding="utf-8").read()
 
 
 setup(
     name="drf-recaptcha",
-    version="2.2.3",
+    version="3.0.0",
     description="Django rest framework recaptcha field serializer.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Lev Lybin",
     author_email="lev.lybin@gmail.com",
     license="MIT",
     url="https://github.com/llybin/drf-recaptcha",
     packages=find_packages(exclude=["tests*"]),
     install_requires=[
         "django>=3.2",
         "djangorestframework>=3.11",
         "django-ipware>=2.1",
     ],
     setup_requires=["pytest-runner"],
-    tests_require=["pytest", "pytest-django", "pytest-cov"],
+    tests_require=["pytest", "pytest-django", "pytest-cov", "pytest-mock"],
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False,
     keywords=[
         "django",
         "drf",
         "rest",
```

### Comparing `drf-recaptcha-2.2.3/tests/test_checks.py` & `drf-recaptcha-3.0.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.3/tests/test_fields.py` & `drf-recaptcha-3.0.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.3/tests/test_serializers.py` & `drf-recaptcha-3.0.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `drf-recaptcha-2.2.3/tests/test_testing.py` & `drf-recaptcha-3.0.0/tests/test_testing.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,37 +7,41 @@
 @pytest.mark.parametrize(
     ("validator_class", "params"),
     [
         (ReCaptchaV2Validator, {}),
         (ReCaptchaV3Validator, {"action": "test_action", "required_score": 0.4}),
     ],
 )
-def test_recaptcha_validator_testing_success(validator_class, params, settings):
+def test_recaptcha_validator_testing_success(
+    validator_class, params, settings, mocked_serializer_field
+):
     settings.DRF_RECAPTCHA_TESTING = True
 
     validator = validator_class(secret_key="TEST_SECRET_KEY", **params)
     try:
-        validator("test_token")
+        validator("test_token", mocked_serializer_field)
     except ValidationError:
         pytest.fail("Validation is not passed")
 
 
 @pytest.mark.parametrize(
     ("validator_class", "params"),
     [
         (ReCaptchaV2Validator, {}),
         (ReCaptchaV3Validator, {"action": "test_action", "required_score": 0.4}),
     ],
 )
-def test_recaptcha_validator_testing_fail(validator_class, params, settings):
+def test_recaptcha_validator_testing_fail(
+    validator_class, params, settings, mocked_serializer_field
+):
     settings.DRF_RECAPTCHA_TESTING = True
     settings.DRF_RECAPTCHA_TESTING_PASS = False
 
     validator = validator_class(secret_key="TEST_SECRET_KEY", **params)
 
     with pytest.raises(ValidationError) as exc_info:
-        validator("test_token")
+        validator("test_token", mocked_serializer_field)
 
     assert (
         str(exc_info.value)
         == "[ErrorDetail(string='Error verifying reCAPTCHA, please try again.', code='captcha_invalid')]"
     )
```

