# Comparing `tmp/tenduke_core-1.1.0.tar.gz` & `tmp/tenduke_core-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenduke_core-1.1.0.tar", max compression
+gzip compressed data, was "tenduke_core-2.0.0.tar", max compression
```

## Comparing `tenduke_core-1.1.0.tar` & `tenduke_core-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1108 2024-04-10 03:35:47.803895 tenduke_core-1.1.0/LICENSE
--rw-r--r--   0        0        0     2843 2024-04-10 03:35:47.804812 tenduke_core-1.1.0/README.md
--rw-r--r--   0        0        0     3624 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      191 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/__init__.py
--rw-r--r--   0        0        0      659 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/__init__.py
--rw-r--r--   0        0        0     1665 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/auth_provider.py
--rw-r--r--   0        0        0     1022 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/device_auth_response.py
--rw-r--r--   0        0        0     7252 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/device_flow_client.py
--rw-r--r--   0        0        0     6413 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/oauth_client.py
--rw-r--r--   0        0        0     7029 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/pkce_flow_client.py
--rw-r--r--   0        0        0     1540 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/token_response.py
--rw-r--r--   0        0        0     1789 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/user_info.py
--rw-r--r--   0        0        0     4121 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/base_model.py
--rw-r--r--   0        0        0      135 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/config/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/config/tenduke_config.py
--rw-r--r--   0        0        0      319 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/exceptions/__init__.py
--rw-r--r--   0        0        0     2494 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/exceptions/api.py
--rw-r--r--   0        0        0     5939 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/exceptions/oauth.py
--rw-r--r--   0        0        0     1858 2024-04-10 03:35:47.806645 tenduke_core-1.1.0/tenduke_core/exceptions/validation.py
--rw-r--r--   0        0        0        0 2024-04-10 03:35:47.828645 tenduke_core-1.1.0/tenduke_core/py.typed
--rw-r--r--   0        0        0      865 2024-04-10 03:35:47.806645 tenduke_core-1.1.0/tenduke_core/session_factory.py
--rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 tenduke_core-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-04-29 01:50:39.175564 tenduke_core-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2843 2024-04-29 01:50:39.175564 tenduke_core-2.0.0/README.md
+-rw-r--r--   0        0        0     3624 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      191 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/__init__.py
+-rw-r--r--   0        0        0      661 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/__init__.py
+-rw-r--r--   0        0        0     1665 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/auth_provider.py
+-rw-r--r--   0        0        0     1022 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/device_auth_response.py
+-rw-r--r--   0        0        0     7364 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/device_flow_client.py
+-rw-r--r--   0        0        0     6516 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/oauth_client.py
+-rw-r--r--   0        0        0     1115 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/oidc_discovery.py
+-rw-r--r--   0        0        0     7029 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/pkce_flow_client.py
+-rw-r--r--   0        0        0     1540 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/token_response.py
+-rw-r--r--   0        0        0     1789 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/auth/user_info.py
+-rw-r--r--   0        0        0     4121 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/base_model.py
+-rw-r--r--   0        0        0      135 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/config/__init__.py
+-rw-r--r--   0        0        0     4484 2024-04-29 01:50:39.176564 tenduke_core-2.0.0/tenduke_core/config/tenduke_config.py
+-rw-r--r--   0        0        0      319 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/exceptions/__init__.py
+-rw-r--r--   0        0        0     2494 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/exceptions/api.py
+-rw-r--r--   0        0        0     5939 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/exceptions/oauth.py
+-rw-r--r--   0        0        0     1858 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/exceptions/validation.py
+-rw-r--r--   0        0        0      100 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/http/__init__.py
+-rw-r--r--   0        0        0     1590 2024-04-29 01:50:39.177564 tenduke_core-2.0.0/tenduke_core/http/session_factory.py
+-rw-r--r--   0        0        0        0 2024-04-29 01:50:39.204564 tenduke_core-2.0.0/tenduke_core/py.typed
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 tenduke_core-2.0.0/PKG-INFO
```

### Comparing `tenduke_core-1.1.0/LICENSE` & `tenduke_core-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/README.md` & `tenduke_core-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/pyproject.toml` & `tenduke_core-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenduke_core"
-version = "1.1.0"
+version = "2.0.0"
 description = "Shared code supporting 10Duke SDKs"
 authors = []
 repository = "https://gitlab.com/10Duke/core/python-core"
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "tenduke_core"},
```

### Comparing `tenduke_core-1.1.0/tenduke_core/auth/__init__.py` & `tenduke_core-2.0.0/tenduke_core/auth/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Authentication and Authorization.
 
 Includes helpers for authenticating with Open ID Connect and OAuth and
 authorization providers for 10Duke API calls.
 """
+
 from .auth_provider import IdTokenAuth
 from .device_auth_response import DeviceAuthorizationResponse
 from .device_flow_client import DeviceFlowClient
 from .oauth_client import OAuthClient
 from .pkce_flow_client import PkceFlowClient
 from .token_response import TokenResponse
 from .user_info import UserInfo
```

### Comparing `tenduke_core-1.1.0/tenduke_core/auth/auth_provider.py` & `tenduke_core-2.0.0/tenduke_core/auth/auth_provider.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/tenduke_core/auth/device_auth_response.py` & `tenduke_core-2.0.0/tenduke_core/auth/device_auth_response.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/tenduke_core/auth/device_flow_client.py` & `tenduke_core-2.0.0/tenduke_core/auth/device_flow_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Helper to perform OAuth device flow."""
 import asyncio
 from datetime import datetime, timedelta, timezone
 from typing import Dict, Optional
 
+from tenduke_core.http.session_factory import SessionFactory
+
 from ..config import TendukeConfig
 from ..exceptions.oauth import raise_error_from_error_response
 from ..exceptions.validation import (
     DeviceCodeAuthorizationUrlMissingError,
     TokenUrlMissingError,
 )
 from .device_auth_response import DeviceAuthorizationResponse
@@ -81,28 +83,28 @@
             return (
                 self._verification_uri_complete
                 or self._verification_url_complete
                 or self._verification_uri
                 or self._verification_url
             )
 
-    def __init__(self, config: TendukeConfig):
+    def __init__(self, config: TendukeConfig, session_factory: SessionFactory):
         """Construct an instance of the DeviceFlowClient.
 
         Args:
             config:
                 Configuration parameters for interacting with the OAuth / Open ID Authorization
                 Server.
         """
         self._device_code = None
         self._expires_at = None
         self._user_code: str = ""
         self._interval = 5
         self._verification_uri = self.VerificationUri()
-        super().__init__(config)
+        super().__init__(config, session_factory)
 
     def authorize(self) -> DeviceAuthorizationResponse:
         """Make the authorization request and return the details to display to the user.
 
         Returns:
             A DeviceAuthorizationResponse object containing the code and uri needed to fetch a
             token.
```

### Comparing `tenduke_core-1.1.0/tenduke_core/auth/oauth_client.py` & `tenduke_core-2.0.0/tenduke_core/auth/oauth_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """OAuth / Open ID Connect client."""
 from dataclasses import dataclass
 
+from tenduke_core.http.session_factory import SessionFactory
+
 # conditional import for Python versions <= 3.10
 try:
     from datetime import UTC
 except ImportError:
     from datetime import timezone
     UTC = timezone.utc
 
@@ -75,15 +77,15 @@
             return cls(token.id_token, expiry)
         return None
 
 
 class OAuthClient:
     """OAuth / Open ID Connect client."""
 
-    def __init__(self, config: TendukeConfig):
+    def __init__(self, config: TendukeConfig, session_factory: SessionFactory):
         """
         Construct an instance of the OAuth Client.
 
         Args:
             config:
                 Configuration parameters for interacting with the OAuth / Open ID Authorization
                 Server.
@@ -93,15 +95,15 @@
         if config.idp_jwks_uri:
             self._idp_jwks_client = PyJWKClient(
                 config.idp_jwks_uri, cache_keys=True, lifespan=345000
             )
         self._try_to_refresh = True
         self._token: Optional[TokenResponse] = None
         self._id_token: Optional[IdToken] = None
-        self.session = config.session()
+        self.session = session_factory.create()
 
     @property
     def token(self) -> Optional[TokenResponse]:
         """The current token response."""
         return self._token
 
     @token.setter
```

### Comparing `tenduke_core-1.1.0/tenduke_core/auth/pkce_flow_client.py` & `tenduke_core-2.0.0/tenduke_core/auth/pkce_flow_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/tenduke_core/auth/token_response.py` & `tenduke_core-2.0.0/tenduke_core/auth/token_response.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/tenduke_core/auth/user_info.py` & `tenduke_core-2.0.0/tenduke_core/auth/user_info.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/tenduke_core/base_model.py` & `tenduke_core-2.0.0/tenduke_core/base_model.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/tenduke_core/config/tenduke_config.py` & `tenduke_core-2.0.0/tenduke_core/config/tenduke_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,16 @@
 """Dataclass for storing application configuration."""
 from dataclasses import dataclass
 from typing import Optional, Type, TypeVar
 
 import dataconf
-from requests import Session
-from requests.auth import AuthBase
-
-from ..session_factory import session_factory
 
 T = TypeVar("T", bound="TendukeConfig")
 
 
-def _load_openid_config(config):
-    """Load the Open ID details from a discovery URL."""
-    if not config.idp_oidc_discovery_url:
-        return
-    session = config.session()
-    response = session.get(config.idp_oidc_discovery_url)
-    response_json = response.json()
-    config.idp_oauth_device_code_url = response_json.get(
-        "device_authorization_endpoint", config.idp_oauth_device_code_url
-    )
-    config.idp_oauth_authorization_url = response_json.get(
-        "authorization_endpoint", config.idp_oauth_authorization_url
-    )
-    config.idp_oauth_token_url = response_json.get(
-        "token_endpoint", config.idp_oauth_token_url
-    )
-    config.idp_userinfo_url = response_json.get(
-        "userinfo_endpoint", config.idp_userinfo_url
-    )
-    config.idp_jwks_uri = response_json.get("jwks_uri", config.idp_jwks_uri)
-
-
 # These are the options for the program.
 # The number of attributes here breaks a pylint rule.
 # Breaking this up into idp/licensingapi/local or whatever sub-configs is likely
 # to cause more complexity for applications using the SDK.
 #
 # pylint: disable=too-many-instance-attributes
 @dataclass
@@ -122,27 +96,8 @@
         if file_name:
             config_builder = config_builder.file(file_name)
 
         if prefix:
             config_builder = config_builder.env(prefix)
 
         config = config_builder.on(TendukeConfig)
-        _load_openid_config(config)
         return config
-
-    def session(self, auth: Optional[AuthBase] = None) -> Session:
-        """Configure a requests Session with the configuration settings.
-
-        Args:
-            auth: Authorization provider hook to use for new session.
-
-        Returns:
-            Session object configured to match SDK configuration settings.
-        """
-        proxies = {}
-        if self.https_proxy:
-            proxies["https"] = self.https_proxy
-        return session_factory(
-            auth=auth,
-            timeout=(self.http_timeout_seconds, self.http_timeout_seconds),
-            proxies=proxies,
-        )
```

### Comparing `tenduke_core-1.1.0/tenduke_core/exceptions/api.py` & `tenduke_core-2.0.0/tenduke_core/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/tenduke_core/exceptions/oauth.py` & `tenduke_core-2.0.0/tenduke_core/exceptions/oauth.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/tenduke_core/exceptions/validation.py` & `tenduke_core-2.0.0/tenduke_core/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.1.0/PKG-INFO` & `tenduke_core-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenduke_core
-Version: 1.1.0
+Version: 2.0.0
 Summary: Shared code supporting 10Duke SDKs
 Home-page: https://gitlab.com/10Duke/core/python-core
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

