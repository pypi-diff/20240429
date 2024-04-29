# Comparing `tmp/py_ucan-0.4.0.tar.gz` & `tmp/py_ucan-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ucan-0.4.0.tar", max compression
+gzip compressed data, was "py_ucan-0.5.0.tar", max compression
```

## Comparing `py_ucan-0.4.0.tar` & `py_ucan-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-04-28 03:25:15.512725 py_ucan-0.4.0/LICENSE
--rw-r--r--   0        0        0     3707 2024-04-28 03:25:15.512725 py_ucan-0.4.0/README.md
--rw-r--r--   0        0        0    10266 2024-04-28 03:25:16.516728 py_ucan-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2277 2024-04-28 03:25:16.524728 py_ucan-0.4.0/src/ucan/__init__.py
--rw-r--r--   0        0        0      744 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/constants.py
--rw-r--r--   0        0        0       30 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/__init__.py
--rw-r--r--   0        0        0     6739 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/attenuation.py
--rw-r--r--   0        0        0     3059 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/plugins.py
--rw-r--r--   0        0        0     1484 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/semver.py
--rw-r--r--   0        0        0     6731 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/token.py
--rw-r--r--   0        0        0     4121 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/types.py
--rw-r--r--   0        0        0     5965 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/core/verify.py
--rw-r--r--   0        0        0      181 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/default_plugins/__init__.py
--rw-r--r--   0        0        0     2853 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/default_plugins/ed25519.py
--rw-r--r--   0        0        0        0 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/py.typed
--rw-r--r--   0        0        0      849 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/schemas.py
--rw-r--r--   0        0        0      205 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/typing.py
--rw-r--r--   0        0        0     2192 2024-04-28 03:25:15.512725 py_ucan-0.4.0/src/ucan/utils.py
--rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 py_ucan-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 14:45:14.398558 py_ucan-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3702 2024-04-28 14:45:14.398558 py_ucan-0.5.0/README.md
+-rw-r--r--   0        0        0    10266 2024-04-28 14:45:15.430575 py_ucan-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2366 2024-04-28 14:45:15.434575 py_ucan-0.5.0/src/ucan/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/constants.py
+-rw-r--r--   0        0        0       30 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/__init__.py
+-rw-r--r--   0        0        0     6751 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/attenuation.py
+-rw-r--r--   0        0        0     5191 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/capability.py
+-rw-r--r--   0        0        0     3059 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/plugins.py
+-rw-r--r--   0        0        0     1479 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/semver.py
+-rw-r--r--   0        0        0     5538 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/token.py
+-rw-r--r--   0        0        0     3346 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/types.py
+-rw-r--r--   0        0        0     5997 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/verify.py
+-rw-r--r--   0        0        0      181 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/default_plugins/__init__.py
+-rw-r--r--   0        0        0     2853 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/default_plugins/ed25519.py
+-rw-r--r--   0        0        0     1524 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/encoding.py
+-rw-r--r--   0        0        0        0 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/py.typed
+-rw-r--r--   0        0        0     1284 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/schemas.py
+-rw-r--r--   0        0        0      205 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/typing.py
+-rw-r--r--   0        0        0     2192 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/utils.py
+-rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 py_ucan-0.5.0/PKG-INFO
```

### Comparing `py_ucan-0.4.0/LICENSE` & `py_ucan-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ucan-0.4.0/README.md` & `py_ucan-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # py-ucan
 
 This is a Python library to help the web applications make use
 of UCANs in their authorization flows. To learn more about UCANs and how you
-might use them in your application, visit [https://ucan.xyz][ucan website] or
-read the [https://github.com/ucan-wg/spec][spec].
+might use them in your application, visit [ucan website](https://ucan.xyz) or
+read the [spec](https://github.com/ucan-wg/spec).
 
 
 ## Installation
 
 ```
 pip install -U py-ucan
 ```
@@ -19,15 +19,15 @@
 NOTE: Ojects can be instantiated with field names in camel case, but to access those fields, you need to use their snake case names.
 
 #### ucan.ResourcePointer
 
 ```py
 
 # -- from string
-resource = ResourcePointer.from_string("fileverse://solo.fileverse.io")
+resource = ResourcePointer.decode("fileverse://solo.fileverse.io")
 print(resource.scheme, resource.hier_part)
 # output: fileverse //solo.fileverse.io
 
 # -- from json: snake case
 resource = ResourcePointer.model_validate({"scheme": "fileverse", "hier_part": "//solo.fileverse.io"})
 print(resource.scheme, resource.hier_part)
 # output: fileverse //solo.fileverse.io
```

### Comparing `py_ucan-0.4.0/pyproject.toml` & `py_ucan-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # ----------------------------------------------------------------------------------------------------------------------
 # poetry
 [tool.poetry]
 package-mode = true
 name = "py-ucan"
-version = "0.4.0"
+version = "0.5.0"
 description = "Python Ucan"
 readme = "README.md"
 authors = [
     "Subham Agarwal <subhamagr@users.noreply.github.com>",
 ]
 maintainers = []
 # links
```

### Comparing `py_ucan-0.4.0/src/ucan/__init__.py` & `py_ucan-0.5.0/src/ucan/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,57 +6,50 @@
 
 import pydantic as pyd
 import pydantic.dataclasses
 
 from ucan.core import attenuation as attenuationlib
 from ucan.core import token as tokenlib
 from ucan.core import verify as verifylib
+from ucan.core.capability import Ability, Capability, ResourcePointer
 from ucan.core.plugins import Plugins
-from ucan.core.types import (
-    Ability,
-    Capability,
-    ResourcePointer,
-    Ucan,
-    UcanHeader,
-    UcanParts,
-    UcanPayload,
-)
+from ucan.core.types import Ucan, UcanHeader, UcanPayload
 from ucan.core.verify import (
     RequiredCapability,
     Verification,
     VerifyResult,
     VerifyResultError,
     VerifyResultOk,
 )
 from ucan.default_plugins import ed25519_plugin, EdKeypair
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 
 __all__ = (
     # attrs of this module
     "Plugins",
     "PluginInjectedAPI",
     "default_plugins",
     "injected_api",
     "delegation_chains",
+    "parse",
     "validate",
     "validate_proofs",
     "verify",
     # plugins
     "EdKeypair",
     "ed25519_plugin",
     # types
     "Ability",
     "Capability",
     "ResourcePointer",
     "Ucan",
     "UcanHeader",
-    "UcanParts",
     "UcanPayload",
     # verify types
     "RequiredCapability",
     "Verification",
     "VerifyResult",
     "VerifyResultError",
     "VerifyResultOk",
@@ -68,29 +61,32 @@
     kw_only=True,
     config=pyd.ConfigDict(extra="forbid", frozen=True, arbitrary_types_allowed=True),
 )
 class PluginInjectedAPI:
     """Ucan API with plugins injected."""
 
     delegation_chains: attenuationlib.DelegationChainsFunc
+    parse: tokenlib.TokenParseFunc
     validate: tokenlib.TokenValidateFunc
     validate_proofs: tokenlib.ValidateProofFunc
     verify: verifylib.VerifyTokenFunc
 
     @classmethod
     def from_plugins(cls, plugins: Plugins) -> te.Self:
         """Build `PluginInjectedAPI` from a `Plugins` object."""
         return cls(
+            parse=tokenlib.parse(plugins),
             validate=tokenlib.validate(plugins),
             verify=verifylib.verify(plugins),
             validate_proofs=tokenlib.validate_proofs(plugins),
             delegation_chains=attenuationlib.delegation_chains(plugins),
         )
 
 
 default_plugins = Plugins([ed25519_plugin])
 injected_api = PluginInjectedAPI.from_plugins(default_plugins)
 
 delegation_chains = injected_api.delegation_chains
+parse = injected_api.parse
 validate = injected_api.validate
 validate_proofs = injected_api.validate_proofs
 verify = injected_api.verify
```

### Comparing `py_ucan-0.4.0/src/ucan/constants.py` & `py_ucan-0.5.0/src/ucan/constants.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.4.0/src/ucan/core/attenuation.py` & `py_ucan-0.5.0/src/ucan/core/attenuation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import typing as t
 import typing_extensions as te
 
+from ucan.core.capability import Ability, Capability, ResourcePointer
 from ucan.core.plugins import Plugins
 from ucan.core.token import validate_proofs
-from ucan.core.types import Ability, Capability, IsRevokedFunc, ResourcePointer, Ucan
+from ucan.core.types import IsRevokedFunc, Ucan
 from ucan.schemas import BaseModel, validate_call
 
 
 @te.runtime_checkable
 class _CanDelegateResourceFunc(te.Protocol):
     async def __call__(
         self, parent_resource: ResourcePointer, child_resource: ResourcePointer
@@ -36,26 +37,26 @@
 class DelegationSemantics(te.NamedTuple):
     can_delegate_resource: _CanDelegateResourceFunc
     """
     * Whether a parent resource can delegate a child resource.
     *
     * An implementation may for example decide to return true for
     * `can_delegate_resource(
-        ResourcePointer.from_string("path:/parent/"),
-        ResourcePointer.from_string("path:/parent/child/"),
+        ResourcePointer.decode("path:/parent/"),
+        ResourcePointer.decode("path:/parent/child/"),
         )`
     """
     can_delegate_ability: _CanDelegateAbilityFunc
     """
     * Whether a parent ability can delegate a child ability.
     *
     * An implementation may for example decide to return true for
     * `can_delegate_ability(
-        Ability.from_string("crud/UPDATE"),
-        Ability.from_string("crud/CREATE"),
+        Ability.decode("crud/UPDATE"),
+        Ability.decode("crud/CREATE"),
         )`
     """
 
 
 class DelegatedCapability(BaseModel):
     capability: Capability
     ucan: Ucan
```

### Comparing `py_ucan-0.4.0/src/ucan/core/plugins.py` & `py_ucan-0.5.0/src/ucan/core/plugins.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.4.0/src/ucan/core/semver.py` & `py_ucan-0.5.0/src/ucan/core/semver.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from ucan.schemas import BaseModel
 
 
 __all__ = ("SemVer",)
 
 
 class SemVer(BaseModel):
-    """Ucan version."""
+    """UCAN version."""
 
     major: int
     minor: int
     patch: int
 
     @classmethod
-    def from_string(cls, value: str) -> te.Self:
+    def decode(cls, value: str) -> te.Self:
         """Load `SemVer` from a string value.
 
         Args:
             value (str): String in the format major.minor.patch
 
         Returns:
             te.Self: `SemVer` object.
```

### Comparing `py_ucan-0.4.0/src/ucan/core/token.py` & `py_ucan-0.5.0/src/ucan/core/token.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,30 +2,26 @@
 
 from __future__ import annotations
 
 import math
 import typing as t
 import typing_extensions as te
 
-import jwt
-from jwt.api_jwt import decode_complete
-
 from ucan.core.plugins import Plugins
-from ucan.core.types import Ucan, UcanHeader, UcanParts, UcanPayload
+from ucan.core.types import Ucan
 from ucan.schemas import validate_call
 from ucan.utils import aware_utcfromtimestamp, aware_utcnow
 
 
-class ProofError(Exception):
-    pass
+# typing
 
 
 @te.runtime_checkable
 class TokenParseFunc(te.Protocol):
-    async def __call__(self, encoded_ucan: str) -> UcanParts: ...
+    def __call__(self, encoded_ucan: str) -> Ucan: ...
 
 
 @te.runtime_checkable
 class TokenValidateFunc(te.Protocol):
     async def __call__(
         self,
         encoded_ucan: str,
@@ -49,14 +45,24 @@
         check_issuer: bool = True,
         check_signature: bool = True,
         check_is_expired: bool = True,
         check_is_too_early: bool = True,
     ) -> t.AsyncIterator[Ucan | Exception]: ...
 
 
+# exceptions
+
+
+class ProofError(Exception):
+    pass
+
+
+# utils
+
+
 def is_expired(ucan: Ucan) -> bool:
     """Check if a UCAN is expired."""
     return aware_utcfromtimestamp(ucan.payload.exp) <= aware_utcnow()
 
 
 def is_too_early(ucan: Ucan) -> bool:
     """Check if a UCAN is not active yet."""
@@ -64,34 +70,16 @@
         return False
     return ucan.payload.nbf > math.floor(aware_utcnow().timestamp())
 
 
 @validate_call
 def parse(plugins: Plugins) -> TokenParseFunc:
     @validate_call
-    async def _parse_inner(encoded_ucan: str) -> UcanParts:
-        try:
-            decoded_token = decode_complete(
-                encoded_ucan, options={"verify_signature": False}
-            )
-
-            raw_header = decoded_token["header"]
-            token_header = UcanHeader.model_validate(raw_header, strict=False)
-
-            raw_payload = decoded_token["payload"]
-            token_payload = UcanPayload.model_validate(raw_payload, strict=False)
-
-            return UcanParts(header=token_header, payload=token_payload)
-
-        except ValueError as err:
-            msg = (
-                f"Can't parse UCAN: {encoded_ucan}: Expected JWT format: "
-                "3 dot-separated base64url-encoded values."
-            )
-            raise ValueError(msg) from err
+    def _parse_inner(encoded_ucan: str) -> Ucan:
+        return Ucan.decode(encoded_ucan)
 
     return _parse_inner
 
 
 @validate_call
 def validate(plugins: Plugins) -> TokenValidateFunc:
     @validate_call
@@ -100,50 +88,39 @@
         *,
         check_issuer: bool = True,
         check_signature: bool = True,
         check_is_expired: bool = True,
         check_is_too_early: bool = True,
     ) -> Ucan:
         """Parse & Validate **one layer** of a UCAN."""
-        parsed = await parse(plugins)(encoded_ucan)
-        encoded_header, encoded_payload, encoded_signature = encoded_ucan.split(".")
-        signed_data = f"{encoded_header}.{encoded_payload}"
-        signed_data_bytes = signed_data.encode("utf8")
-        signature_bytes = jwt.utils.base64url_decode(encoded_signature)
+        parsed = parse(plugins)(encoded_ucan)
 
         if check_issuer and not await plugins.verify_issuer_alg(
             parsed.payload.iss, parsed.header.alg
         ):
             msg = (
                 f"Invalid UCAN: {encoded_ucan}: Issuer key type does not "
                 "match UCAN's `alg` property."
             )
             raise ValueError(msg)
 
         if check_signature:
             await plugins.verify_signature(
-                parsed.payload.iss, signed_data_bytes, signature_bytes
+                parsed.payload.iss, parsed.signed_data_bytes, parsed.signature_bytes
             )
 
-        ucan = Ucan(
-            header=parsed.header,
-            payload=parsed.payload,
-            signed_data=signed_data,
-            signature=encoded_signature,
-        )
-
-        if check_is_expired and is_expired(ucan):
+        if check_is_expired and is_expired(parsed):
             msg = f"Invalid UCAN: {encoded_ucan}: Expired."
             raise ValueError(msg)
 
-        if check_is_too_early and is_too_early(ucan):
+        if check_is_too_early and is_too_early(parsed):
             msg = f"Invalid UCAN: {encoded_ucan}: Not active yet (too early)."
             raise ValueError(msg)
 
-        return ucan
+        return parsed
 
     return _validate_inner
 
 
 @validate_call
 def validate_proofs(plugins: Plugins) -> ValidateProofFunc:
     @validate_call
```

### Comparing `py_ucan-0.4.0/src/ucan/core/verify.py` & `py_ucan-0.5.0/src/ucan/core/verify.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     capability_can_be_delegated,
     delegation_chains,
     DelegationChain,
     DelegationSemantics,
     equal_can_delegate,
     get_root_issuer,
 )
+from ucan.core.capability import Capability
 from ucan.core.plugins import Plugins
-from ucan.core.types import Capability, IsRevokedFunc, Ucan
+from ucan.core.types import IsRevokedFunc, Ucan
 from ucan.schemas import BaseModel, DidString, validate_call
 
 
 __all__ = (
     # models
     "RequiredCapability",
     "Verification",
```

### Comparing `py_ucan-0.4.0/src/ucan/default_plugins/ed25519.py` & `py_ucan-0.5.0/src/ucan/default_plugins/ed25519.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.4.0/src/ucan/utils.py` & `py_ucan-0.5.0/src/ucan/utils.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.4.0/PKG-INFO` & `py_ucan-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ucan
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python Ucan
 Home-page: https://github.com/fileverse/py-ucan
 Author: Subham Agarwal
 Author-email: subhamagr@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,16 +21,16 @@
 Project-URL: Repository, https://github.com/fileverse/py-ucan
 Description-Content-Type: text/markdown
 
 # py-ucan
 
 This is a Python library to help the web applications make use
 of UCANs in their authorization flows. To learn more about UCANs and how you
-might use them in your application, visit [https://ucan.xyz][ucan website] or
-read the [https://github.com/ucan-wg/spec][spec].
+might use them in your application, visit [ucan website](https://ucan.xyz) or
+read the [spec](https://github.com/ucan-wg/spec).
 
 
 ## Installation
 
 ```
 pip install -U py-ucan
 ```
@@ -42,15 +42,15 @@
 NOTE: Ojects can be instantiated with field names in camel case, but to access those fields, you need to use their snake case names.
 
 #### ucan.ResourcePointer
 
 ```py
 
 # -- from string
-resource = ResourcePointer.from_string("fileverse://solo.fileverse.io")
+resource = ResourcePointer.decode("fileverse://solo.fileverse.io")
 print(resource.scheme, resource.hier_part)
 # output: fileverse //solo.fileverse.io
 
 # -- from json: snake case
 resource = ResourcePointer.model_validate({"scheme": "fileverse", "hier_part": "//solo.fileverse.io"})
 print(resource.scheme, resource.hier_part)
 # output: fileverse //solo.fileverse.io
```

