# Comparing `tmp/py_ucan-0.5.0.tar.gz` & `tmp/py_ucan-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ucan-0.5.0.tar", max compression
+gzip compressed data, was "py_ucan-0.5.1.tar", max compression
```

## Comparing `py_ucan-0.5.0.tar` & `py_ucan-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-04-28 14:45:14.398558 py_ucan-0.5.0/LICENSE
--rw-r--r--   0        0        0     3702 2024-04-28 14:45:14.398558 py_ucan-0.5.0/README.md
--rw-r--r--   0        0        0    10266 2024-04-28 14:45:15.430575 py_ucan-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2366 2024-04-28 14:45:15.434575 py_ucan-0.5.0/src/ucan/__init__.py
--rw-r--r--   0        0        0      744 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/constants.py
--rw-r--r--   0        0        0       30 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/__init__.py
--rw-r--r--   0        0        0     6751 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/attenuation.py
--rw-r--r--   0        0        0     5191 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/capability.py
--rw-r--r--   0        0        0     3059 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/plugins.py
--rw-r--r--   0        0        0     1479 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/semver.py
--rw-r--r--   0        0        0     5538 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/token.py
--rw-r--r--   0        0        0     3346 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/types.py
--rw-r--r--   0        0        0     5997 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/core/verify.py
--rw-r--r--   0        0        0      181 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/default_plugins/__init__.py
--rw-r--r--   0        0        0     2853 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/default_plugins/ed25519.py
--rw-r--r--   0        0        0     1524 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/encoding.py
--rw-r--r--   0        0        0        0 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/py.typed
--rw-r--r--   0        0        0     1284 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/schemas.py
--rw-r--r--   0        0        0      205 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/typing.py
--rw-r--r--   0        0        0     2192 2024-04-28 14:45:14.398558 py_ucan-0.5.0/src/ucan/utils.py
--rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 py_ucan-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-29 04:19:43.475551 py_ucan-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4655 2024-04-29 04:19:43.475551 py_ucan-0.5.1/README.md
+-rw-r--r--   0        0        0    10266 2024-04-29 04:19:44.567542 py_ucan-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2366 2024-04-29 04:19:44.575542 py_ucan-0.5.1/src/ucan/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-29 04:19:43.475551 py_ucan-0.5.1/src/ucan/constants.py
+-rw-r--r--   0        0        0       30 2024-04-29 04:19:43.475551 py_ucan-0.5.1/src/ucan/core/__init__.py
+-rw-r--r--   0        0        0     6751 2024-04-29 04:19:43.475551 py_ucan-0.5.1/src/ucan/core/attenuation.py
+-rw-r--r--   0        0        0     5191 2024-04-29 04:19:43.475551 py_ucan-0.5.1/src/ucan/core/capability.py
+-rw-r--r--   0        0        0     3059 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/core/plugins.py
+-rw-r--r--   0        0        0     1479 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/core/semver.py
+-rw-r--r--   0        0        0     5538 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/core/token.py
+-rw-r--r--   0        0        0     3334 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/core/types.py
+-rw-r--r--   0        0        0     5997 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/core/verify.py
+-rw-r--r--   0        0        0      181 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/default_plugins/__init__.py
+-rw-r--r--   0        0        0     2853 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/default_plugins/ed25519.py
+-rw-r--r--   0        0        0     1555 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/encoding.py
+-rw-r--r--   0        0        0        0 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/py.typed
+-rw-r--r--   0        0        0     1305 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/schemas.py
+-rw-r--r--   0        0        0      205 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/typing.py
+-rw-r--r--   0        0        0     2192 2024-04-29 04:19:43.479551 py_ucan-0.5.1/src/ucan/utils.py
+-rw-r--r--   0        0        0     5539 1970-01-01 00:00:00.000000 py_ucan-0.5.1/PKG-INFO
```

### Comparing `py_ucan-0.5.0/LICENSE` & `py_ucan-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/pyproject.toml` & `py_ucan-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # ----------------------------------------------------------------------------------------------------------------------
 # poetry
 [tool.poetry]
 package-mode = true
 name = "py-ucan"
-version = "0.5.0"
+version = "0.5.1"
 description = "Python Ucan"
 readme = "README.md"
 authors = [
     "Subham Agarwal <subhamagr@users.noreply.github.com>",
 ]
 maintainers = []
 # links
```

### Comparing `py_ucan-0.5.0/src/ucan/__init__.py` & `py_ucan-0.5.1/src/ucan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     VerifyResult,
     VerifyResultError,
     VerifyResultOk,
 )
 from ucan.default_plugins import ed25519_plugin, EdKeypair
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 __all__ = (
     # attrs of this module
     "Plugins",
     "PluginInjectedAPI",
     "default_plugins",
```

### Comparing `py_ucan-0.5.0/src/ucan/constants.py` & `py_ucan-0.5.1/src/ucan/constants.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/src/ucan/core/attenuation.py` & `py_ucan-0.5.1/src/ucan/core/attenuation.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/src/ucan/core/capability.py` & `py_ucan-0.5.1/src/ucan/core/capability.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/src/ucan/core/plugins.py` & `py_ucan-0.5.1/src/ucan/core/plugins.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/src/ucan/core/semver.py` & `py_ucan-0.5.1/src/ucan/core/semver.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/src/ucan/core/token.py` & `py_ucan-0.5.1/src/ucan/core/token.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/src/ucan/core/types.py` & `py_ucan-0.5.1/src/ucan/core/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typing as t
 import typing_extensions as te
 
 import pydantic as pyd
 
 from ucan.core.capability import Capability
 from ucan.core.semver import SemVer
-from ucan.encoding import JWTBase64UrlEncoder
+from ucan.encoding import Base64UrlEncoder
 from ucan.schemas import BaseModel, JWTBase64Str
 
 
 # Function types
 
 
 @te.runtime_checkable
@@ -59,15 +59,15 @@
 
     @property
     def signed_data_bytes(self) -> bytes:
         return self.signed_data.encode("utf8")
 
     @property
     def signature_bytes(self) -> bytes:
-        return JWTBase64UrlEncoder.decode(self.signature)
+        return Base64UrlEncoder.decode(self.signature)
 
     @pyd.model_serializer
     def ser_model(self) -> dict[str, t.Any]:
         """Custom model serializer to serialize fields with their alias names.
 
         Returns:
             dict[str, t.Any]: model serialzied as dict.
@@ -80,15 +80,15 @@
             "signedData": self.signed_data,
             "signature": self.signature,
         }
 
     @classmethod
     def decode(cls, encoded_ucan: str) -> te.Self:
         try:
-            decoded_token = JWTBase64UrlEncoder.unverified_decode_complete(encoded_ucan)
+            decoded_token = Base64UrlEncoder.unverified_decode_complete(encoded_ucan)
 
             raw_header = decoded_token["header"]
             token_header = UcanHeader.model_validate(raw_header, strict=False)
 
             raw_payload = decoded_token["payload"]
             token_payload = UcanPayload.model_validate(raw_payload, strict=False)
 
@@ -96,15 +96,15 @@
             encoded_header, encoded_payload, encoded_signature = encoded_ucan.split(".")
             signed_data = f"{encoded_header}.{encoded_payload}"
 
             return cls(
                 header=token_header,
                 payload=token_payload,
                 signed_data=signed_data,
-                signature=JWTBase64UrlEncoder.encode(signature_bytes),
+                signature=Base64UrlEncoder.encode(signature_bytes),
             )
 
         except ValueError as err:
             msg = (
                 f"Can't parse UCAN: {encoded_ucan}: Expected JWT format: "
                 "3 dot-separated base64url-encoded values."
             )
```

### Comparing `py_ucan-0.5.0/src/ucan/core/verify.py` & `py_ucan-0.5.1/src/ucan/core/verify.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/src/ucan/default_plugins/ed25519.py` & `py_ucan-0.5.1/src/ucan/default_plugins/ed25519.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/src/ucan/encoding.py` & `py_ucan-0.5.1/src/ucan/encoding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 import typing as t
 
 import jwt
 
 
-class JWTBase64UrlEncoder:
+__all__ = ("Base64UrlEncoder",)
+
+
+class Base64UrlEncoder:
     """URL-safe Base64 encoder."""
 
     @classmethod
     def decode(cls, data: t.AnyStr) -> bytes:
         """Decode the data from base64 encoded bytes to original bytes data.
 
         Args:
```

### Comparing `py_ucan-0.5.0/src/ucan/schemas.py` & `py_ucan-0.5.1/src/ucan/schemas.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Pydantic models, fields and utils used accross the `ucan` package."""
 
+from __future__ import annotations
+
 import typing as t
 import typing_extensions as te
 
 import pydantic as pyd
 
-from ucan.encoding import JWTBase64UrlEncoder
+from ucan.encoding import Base64UrlEncoder
 from ucan.utils import validate_is_did
 
 
 # typing
 T_BaseModel = t.TypeVar("T_BaseModel", bound=pyd.BaseModel)
 
 
@@ -41,11 +43,9 @@
 
 # Custom Pydantic Fields
 
 StringNonEmpty = te.Annotated[
     str, pyd.StringConstraints(strip_whitespace=True, min_length=1)
 ]
 DidString = te.Annotated[str, pyd.AfterValidator(validate_is_did)]
-JWTBase64Bytes = te.Annotated[bytes, pyd.AfterValidator(JWTBase64UrlEncoder.decode)]
-JWTBase64Str = te.Annotated[
-    str, pyd.AfterValidator(JWTBase64UrlEncoder.validate_encoded)
-]
+JWTBase64Bytes = te.Annotated[bytes, pyd.AfterValidator(Base64UrlEncoder.decode)]
+JWTBase64Str = te.Annotated[str, pyd.AfterValidator(Base64UrlEncoder.validate_encoded)]
```

### Comparing `py_ucan-0.5.0/src/ucan/utils.py` & `py_ucan-0.5.1/src/ucan/utils.py`

 * *Files identical despite different names*

### Comparing `py_ucan-0.5.0/PKG-INFO` & `py_ucan-0.5.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-Metadata-Version: 2.1
-Name: py-ucan
-Version: 0.5.0
-Summary: Python Ucan
-Home-page: https://github.com/fileverse/py-ucan
-Author: Subham Agarwal
-Author-email: subhamagr@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: base58 (==2.1.1)
-Requires-Dist: cryptography (==42.0.5)
-Requires-Dist: pydantic (==2.7.1)
-Requires-Dist: pyjwt (==2.8.0)
-Requires-Dist: typing_extensions (==4.11.0)
-Project-URL: Bug Tracker, https://github.com/fileverse/py-ucan/issues
-Project-URL: Documentation, https://github.com/fileverse/py-ucan
-Project-URL: Repository, https://github.com/fileverse/py-ucan
-Description-Content-Type: text/markdown
-
 # py-ucan
 
+[![pypi](https://img.shields.io/pypi/v/py-ucan.svg?color=4B8BBE)](https://pypi.org/project/py-ucan/)
+
 This is a Python library to help the web applications make use
 of UCANs in their authorization flows. To learn more about UCANs and how you
 might use them in your application, visit [ucan website](https://ucan.xyz) or
 read the [spec](https://github.com/ucan-wg/spec).
 
 
-## Installation
+<a id="contents"></a>
+
+# **Contents**
+
+- [Installation](#installation)
+- [Usage](#usage)
+    - [Ucan Objects](#ucan-objects)
+        - [ucan.ResourcePointer](#ucan-objects-resource-pointer)
+    - [Validating UCAN Tokens](#validating-ucan-tokens)
+    - [Verifying UCAN Invocations](#verifying-ucan-invocations)
+
+<a id="installation"></a>
+
+## Installation [`⇧`](#contents)
 
 ```
 pip install -U py-ucan
 ```
 
-## Usage
+<a id="usage"></a>
+
+## Usage [`⇧`](#contents)
+
+<a id="ucan-objects"></a>
 
 ### Ucan objects
 
+All the objects are based on [Pydantic V2](https://docs.pydantic.dev/latest/) models. Ideally you would only need to use [`model_validate`](https://docs.pydantic.dev/latest/api/base_model/#pydantic.BaseModel.model_validate) and [`model_dump`](https://docs.pydantic.dev/latest/api/base_model/#pydantic.BaseModel.model_dump) of pydantic model functions, but please go through the docs for advanced usage.
+
 NOTE: Ojects can be instantiated with field names in camel case, but to access those fields, you need to use their snake case names.
 
+<a id="ucan-objects-resource-pointer"></a>
+
 #### ucan.ResourcePointer
 
 ```py
 
+from ucan import ResourcePointer
+
 # -- from string
 resource = ResourcePointer.decode("fileverse://solo.fileverse.io")
 print(resource.scheme, resource.hier_part)
 # output: fileverse //solo.fileverse.io
 
 # -- from json: snake case
 resource = ResourcePointer.model_validate({"scheme": "fileverse", "hier_part": "//solo.fileverse.io"})
@@ -66,17 +68,17 @@
 # output: fileverse //solo.fileverse.io
 
 # -- from kwargs: camel case
 resource = ResourcePointer(scheme="fileverse", hierPart="//solo.fileverse.io")
 print(resource.scheme, resource.hier_part)
 # output: fileverse //solo.fileverse.io
 
-# dump to json
-# all the objects above will dump to json with camel case fields
-resource = ResourcePointer(scheme="fileverse", hier_part="//solo.fileverse.io").model_dump()
+# dump to python dict
+# all the objects above will dump to a dict with camel case fields
+print(resource.model_dump()) 
 # output: {"scheme": "fileverse", "hierPart": "//solo.fileverse.io"}
 
 ```
 
 
 ### Validating UCAN Tokens
 
@@ -148,8 +150,7 @@
     # The UCAN authorized the user
     pass
 
 else:
     # Unauthorized
     pass
 ```
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

