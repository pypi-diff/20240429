# Comparing `tmp/siwe-2.4.1.tar.gz` & `tmp/siwe-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siwe-2.4.1.tar", max compression
+gzip compressed data, was "siwe-3.0.0.tar", max compression
```

## Comparing `siwe-2.4.1.tar` & `siwe-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11355 2022-04-22 10:09:49.867220 siwe-2.4.1/LICENSE-APACHE
--rw-r--r--   0        0        0     1064 2022-04-22 10:09:49.867290 siwe-2.4.1/LICENSE-MIT
--rw-r--r--   0        0        0     2864 2023-08-23 08:06:58.067383 siwe-2.4.1/README.md
--rw-r--r--   0        0        0     1363 2024-01-04 08:59:41.697861 siwe-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      281 2023-08-23 08:06:58.068654 siwe-2.4.1/siwe/__init__.py
--rw-r--r--   0        0        0     1140 2023-08-23 08:06:58.068871 siwe-2.4.1/siwe/defs.py
--rw-r--r--   0        0        0       24 2023-08-23 08:06:58.069054 siwe-2.4.1/siwe/grammars/__init__.py
--rw-r--r--   0        0        0     1794 2023-08-23 08:06:58.069359 siwe-2.4.1/siwe/grammars/eip4361.py
--rw-r--r--   0        0        0      949 2023-08-23 08:06:58.069570 siwe-2.4.1/siwe/grammars/rfc3339.py
--rw-r--r--   0        0        0      510 2023-08-23 08:06:58.069813 siwe-2.4.1/siwe/grammars/rfc5234.py
--rw-r--r--   0        0        0     2466 2023-08-23 08:06:58.070036 siwe-2.4.1/siwe/parsed.py
--rw-r--r--   0        0        0    10408 2023-08-23 08:06:58.070216 siwe-2.4.1/siwe/siwe.py
--rw-r--r--   0        0        0     4046 1970-01-01 00:00:00.000000 siwe-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2022-04-22 10:09:49.867220 siwe-3.0.0/LICENSE-APACHE
+-rw-r--r--   0        0        0     1064 2022-04-22 10:09:49.867290 siwe-3.0.0/LICENSE-MIT
+-rw-r--r--   0        0        0     2864 2023-08-23 08:06:58.067383 siwe-3.0.0/README.md
+-rw-r--r--   0        0        0     1495 2024-04-29 13:41:47.633060 siwe-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      281 2023-08-23 08:06:58.068654 siwe-3.0.0/siwe/__init__.py
+-rw-r--r--   0        0        0     1209 2024-04-29 13:40:43.815310 siwe-3.0.0/siwe/defs.py
+-rw-r--r--   0        0        0       24 2023-08-23 08:06:58.069054 siwe-3.0.0/siwe/grammars/__init__.py
+-rw-r--r--   0        0        0     1855 2024-04-29 13:40:43.815690 siwe-3.0.0/siwe/grammars/eip4361.py
+-rw-r--r--   0        0        0      949 2023-08-23 08:06:58.069570 siwe-3.0.0/siwe/grammars/rfc3339.py
+-rw-r--r--   0        0        0      510 2023-08-23 08:06:58.069813 siwe-3.0.0/siwe/grammars/rfc5234.py
+-rw-r--r--   0        0        0     2553 2024-04-29 13:40:43.815979 siwe-3.0.0/siwe/parsed.py
+-rw-r--r--   0        0        0    12325 2024-04-29 13:40:43.816341 siwe-3.0.0/siwe/siwe.py
+-rw-r--r--   0        0        0     4058 1970-01-01 00:00:00.000000 siwe-3.0.0/PKG-INFO
```

### Comparing `siwe-2.4.1/LICENSE-APACHE` & `siwe-3.0.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `siwe-2.4.1/LICENSE-MIT` & `siwe-3.0.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `siwe-2.4.1/README.md` & `siwe-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `siwe-2.4.1/siwe/defs.py` & `siwe-3.0.0/siwe/defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Regexes for the various fields."""
 
+SCHEME = "((?P<scheme>([a-zA-Z][a-zA-Z0-9\\+\\-\\.]*))://)?"
 DOMAIN = "(?P<domain>([^/?#]+)) wants you to sign in with your Ethereum account:\\n"
 ADDRESS = "(?P<address>0x[a-zA-Z0-9]{40})\\n\\n"
 STATEMENT = "((?P<statement>[^\\n]+)\\n)?\\n"
 URI = "(([^ :/?#]+):)?(//([^ /?#]*))?([^ ?#]*)(\\?([^ #]*))?(#(.*))?"
 URI_LINE = f"URI: (?P<uri>{URI}?)\\n"
 VERSION = "Version: (?P<version>1)\\n"
 CHAIN_ID = "Chain ID: (?P<chainId>[0-9]+)\\n"
@@ -15,10 +16,10 @@
 )
 ISSUED_AT = f"Issued At: (?P<issuedAt>{DATETIME})"
 EXPIRATION_TIME = f"(\\nExpiration Time: (?P<expirationTime>{DATETIME}))?"
 NOT_BEFORE = f"(\\nNot Before: (?P<notBefore>{DATETIME}))?"
 REQUEST_ID = "(\\nRequest ID: (?P<requestId>[-._~!$&'()*+,;=:@%a-zA-Z0-9]*))?"
 RESOURCES = f"(\\nResources:(?P<resources>(\\n- {URI})+))?"
 REGEX_MESSAGE = (
-    f"^{DOMAIN}{ADDRESS}{STATEMENT}{URI_LINE}{VERSION}{CHAIN_ID}{NONCE}"
+    f"^{SCHEME}{DOMAIN}{ADDRESS}{STATEMENT}{URI_LINE}{VERSION}{CHAIN_ID}{NONCE}"
     f"{ISSUED_AT}{EXPIRATION_TIME}{NOT_BEFORE}{REQUEST_ID}{RESOURCES}$"
 )
```

### Comparing `siwe-2.4.1/siwe/grammars/eip4361.py` & `siwe-3.0.0/siwe/grammars/eip4361.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 @load_grammar_rules(
     [
         # RFC 3986
         ("URI", rfc3986.Rule("URI")),
         ("authority", rfc3986.Rule("authority")),
+        ("scheme", rfc3986.Rule("scheme")),
         ("reserved", rfc3986.Rule("reserved")),
         ("unreserved", rfc3986.Rule("unreserved")),
         ("reserved", rfc3986.Rule("reserved")),
         ("pchar", rfc3986.Rule("pchar")),
         # RFC 5234
         ("LF", rfc5234.Rule("LF")),
         ("HEXDIG", rfc5234.Rule("HEXDIG")),
@@ -27,20 +28,20 @@
         ("date-time", rfc3339.Rule("date-time")),
     ]
 )
 class Rule(_Rule):
     """Rules from EIP-4361."""
 
     grammar: ClassVar[List] = [
-        'sign-in-with-ethereum = domain %s" wants you to sign in with your Ethereum '
-        'account:" LF address LF LF [ statement LF ] LF %s"URI: " uri LF %s"Version: "'
-        ' version LF %s"Chain ID: " chain-id LF %s"Nonce: " nonce LF %s"Issued At: " '
-        'issued-at [ LF %s"Expiration Time: " expiration-time ] [ LF %s"Not Before: " '
-        'not-before ] [ LF %s"Request ID: " request-id ] [ LF %s"Resources:" resources '
-        "]",
+        'sign-in-with-ethereum = [ scheme "://" ] domain %s" wants you to sign in with '
+        'your Ethereum account:" LF address LF LF [ statement LF ] LF %s"URI: " uri LF '
+        '%s"Version: " version LF %s"Chain ID: " chain-id LF %s"Nonce: " nonce LF %s"'
+        'Issued At: " issued-at [ LF %s"Expiration Time: " expiration-time ] [ LF %s"'
+        'Not Before: " not-before ] [ LF %s"Request ID: " request-id ] [ LF %s"'
+        'Resources:" resources ]',
         "domain = authority",
         'address = "0x" 40HEXDIG',
         'statement = 1*( reserved / unreserved / " " )',
         "uri = URI",
         'version = "1"',
         "nonce = 8*( ALPHA / DIGIT )",
         "issued-at = date-time",
```

### Comparing `siwe-2.4.1/siwe/grammars/rfc3339.py` & `siwe-3.0.0/siwe/grammars/rfc3339.py`

 * *Files identical despite different names*

### Comparing `siwe-2.4.1/siwe/parsed.py` & `siwe-3.0.0/siwe/parsed.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         expr = re.compile(REGEX_MESSAGE)
         match = re.match(REGEX_MESSAGE, message)
 
         if not match:
             raise ValueError("Message did not match the regular expression.")
 
         self.match = match
+        self.scheme = match.group(expr.groupindex["scheme"])
         self.domain = match.group(expr.groupindex["domain"])
         self.address = match.group(expr.groupindex["address"])
         self.statement = match.group(expr.groupindex["statement"])
         self.uri = match.group(expr.groupindex["uri"])
         self.version = match.group(expr.groupindex["version"])
         self.nonce = match.group(expr.groupindex["nonce"])
         self.chain_id = match.group(expr.groupindex["chainId"])
@@ -45,14 +46,15 @@
         try:
             node = parser.parse_all(message)
         except abnf.ParseError as e:
             raise ValueError from e
 
         for child in node.children:
             if child.name in [
+                "scheme",
                 "domain",
                 "address",
                 "statement",
                 "uri",
                 "version",
                 "nonce",
                 "chain-id",
```

### Comparing `siwe-2.4.1/siwe/siwe.py` & `siwe-3.0.0/siwe/siwe.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 """Main module for SIWE messages construction and validation."""
 
 import secrets
 import string
-from datetime import datetime
+from datetime import datetime, timezone
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import eth_utils
-from dateutil.parser import isoparse
-from dateutil.tz import UTC
 from eth_account.messages import SignableMessage, _hash_eip191_message, encode_defunct
 from eth_typing import ChecksumAddress
-from pydantic.v1 import AnyUrl, BaseModel, Field, ValidationError, validator
+from pydantic import (
+    AnyUrl,
+    BaseModel,
+    BeforeValidator,
+    Field,
+    NonNegativeInt,
+    TypeAdapter,
+    field_validator,
+)
+from pydantic_core import core_schema
+from typing_extensions import Annotated
 from web3 import HTTPProvider, Web3
 from web3.exceptions import BadFunctionCallOutput
 
 from .parsed import ABNFParsedMessage, RegExpParsedMessage
 
 EIP1271_CONTRACT_ABI = [
     {
@@ -60,14 +68,20 @@
 
 class NotYetValidMessage(VerificationError):
     """The message is not yet valid."""
 
     pass
 
 
+class SchemeMismatch(VerificationError):
+    """The message does not contain the expected scheme."""
+
+    pass
+
+
 class DomainMismatch(VerificationError):
     """The message does not contain the expected domain."""
 
     pass
 
 
 class NonceMismatch(VerificationError):
@@ -90,79 +104,115 @@
     one = "1"
 
     def __str__(self):
         """EIP-4361 representation of the enum field."""
         return self.value
 
 
-class CustomDateTime(str):
-    """ISO-8601 datetime string.
+# NOTE: Do not override the original uri string, just do validation
+# https://github.com/pydantic/pydantic/issues/7186#issuecomment-1874338146
+AnyUrlTypeAdapter = TypeAdapter(AnyUrl)
+AnyUrlStr = Annotated[
+    str,
+    BeforeValidator(lambda value: AnyUrlTypeAdapter.validate_python(value) and value),
+]
+
+
+def datetime_from_iso8601_string(val: str) -> datetime:
+    """Convert an ISO-8601 Datetime string into a valid datetime object."""
+    return datetime.fromisoformat(val.replace(".000Z", "Z").replace("Z", "+00:00"))
 
-    Meant to enable transitivity of deserialisation and serialisation.
-    """
+
+# NOTE: Do not override the original string, but ensure we do timestamp validation
+class ISO8601Datetime(str):
+    """A special field class used to denote ISO-8601 Datetime strings."""
+
+    def __init__(self, val: str):
+        """Validate ISO-8601 string."""
+        # NOTE: `self` is already this class, we are just running our validation here
+        datetime_from_iso8601_string(val)
 
     @classmethod
-    def __get_validators__(cls):
-        """Retrieve the validate method."""
-        yield cls.validate
+    def __get_pydantic_core_schema__(cls, source, handler):
+        """Create valid pydantic schema object for this type."""
+        return core_schema.no_info_after_validator_function(
+            cls, core_schema.str_schema()
+        )
 
     @classmethod
-    def validate(cls, v: str):
-        """Validate the format."""
-        cls.date = isoparse(v)
-        return cls(v)
+    def from_datetime(
+        cls, dt: datetime, timespec: str = "milliseconds"
+    ) -> "ISO8601Datetime":
+        """Create an ISO-8601 formatted string from a datetime object."""
+        # NOTE: Only a useful classmethod for creating these objects
+        return ISO8601Datetime(
+            dt.astimezone(tz=timezone.utc)
+            .isoformat(timespec=timespec)
+            .replace("+00:00", "Z")
+        )
+
+    @property
+    def _datetime(self) -> datetime:
+        return datetime_from_iso8601_string(self)
+
+
+def utc_now() -> datetime:
+    """Get the current datetime as UTC timezone."""
+    return datetime.now(tz=timezone.utc)
 
 
 class SiweMessage(BaseModel):
     """A Sign-in with Ethereum (EIP-4361) message."""
 
-    domain: str = Field(regex="^[^/?#]+$")
+    scheme: Optional[str] = None
+    """RFC 3986 URI scheme for the authority that is requesting the signing."""
+    domain: str = Field(pattern="^[^/?#]+$")
     """RFC 4501 dns authority that is requesting the signing."""
     address: ChecksumAddress
     """Ethereum address performing the signing conformant to capitalization encoded
     checksum specified in EIP-55 where applicable.
     """
-    uri: AnyUrl
+    uri: AnyUrlStr
     """RFC 3986 URI referring to the resource that is the subject of the signing."""
     version: VersionEnum
     """Current version of the message."""
-    chain_id: int = Field(gt=0)
+    chain_id: NonNegativeInt
     """EIP-155 Chain ID to which the session is bound, and the network where Contract
     Accounts must be resolved.
     """
-    issued_at: CustomDateTime
+    issued_at: ISO8601Datetime
     """ISO 8601 datetime string of the current time."""
     nonce: str = Field(min_length=8)
     """Randomized token used to prevent replay attacks, at least 8 alphanumeric
     characters. Use generate_nonce() to generate a secure nonce and store it for
     verification later.
     """
-    statement: Optional[str] = Field(None, regex="^[^\n]+$")
+    statement: Optional[str] = Field(None, pattern="^[^\n]+$")
     """Human-readable ASCII assertion that the user will sign, and it must not contain
     `\n`.
     """
-    expiration_time: Optional[CustomDateTime] = Field(None)
+    expiration_time: Optional[ISO8601Datetime] = None
     """ISO 8601 datetime string that, if present, indicates when the signed
     authentication message is no longer valid.
     """
-    not_before: Optional[CustomDateTime] = Field(None)
+    not_before: Optional[ISO8601Datetime] = None
     """ISO 8601 datetime string that, if present, indicates when the signed
     authentication message will become valid.
     """
-    request_id: Optional[str] = Field(None)
+    request_id: Optional[str] = None
     """System-specific identifier that may be used to uniquely refer to the sign-in
     request.
     """
-    resources: Optional[List[AnyUrl]] = Field(None, min_items=1)
+    resources: Optional[List[AnyUrlStr]] = None
     """List of information or references to information the user wishes to have resolved
     as part of authentication by the relying party. They are expressed as RFC 3986 URIs
     separated by `\n- `.
     """
 
-    @validator("address")
+    @field_validator("address")
     @classmethod
     def address_is_checksum_address(cls, v: str) -> str:
         """Validate the address follows EIP-55 formatting."""
         if not Web3.is_checksum_address(v):
             raise ValueError("Message `address` must be in EIP-55 format")
         return v
 
@@ -170,32 +220,34 @@
         """Construct or parse a message."""
         if isinstance(message, str):
             if abnf:
                 parsed_message = ABNFParsedMessage(message=message)
             else:
                 parsed_message = RegExpParsedMessage(message=message)
             message_dict = parsed_message.__dict__
+
         elif isinstance(message, dict):
             message_dict = message
+
         else:
-            raise TypeError
+            raise TypeError(f"Unhandable message type: '{type(message)}'.")
+
         # TODO There is some redundancy in the checks when deserialising a message.
-        try:
-            super().__init__(**message_dict)
-        except ValidationError as e:
-            raise ValueError from e
+        super().__init__(**message_dict)
 
     def prepare_message(self) -> str:
         """Serialize to the EIP-4361 format for signing.
 
         It can then be passed to an EIP-191 signing function.
 
         :return: EIP-4361 formatted message, ready for EIP-191 signing.
         """
         header = f"{self.domain} wants you to sign in with your Ethereum account:"
+        if self.scheme:
+            header = f"{self.scheme}://{header}"
 
         uri_field = f"URI: {self.uri}"
 
         prefix = "\n".join([header, self.address])
 
         version_field = f"Version: {self.version}"
 
@@ -235,14 +287,15 @@
 
         return "\n\n".join([prefix, suffix])
 
     def verify(
         self,
         signature: str,
         *,
+        scheme: Optional[str] = None,
         domain: Optional[str] = None,
         nonce: Optional[str] = None,
         timestamp: Optional[datetime] = None,
         provider: Optional[HTTPProvider] = None,
     ) -> None:
         """Verify the validity of the message and its signature.
 
@@ -256,26 +309,31 @@
         needed. It is also configurable with the environment variable
         `WEB3_HTTP_PROVIDER_URI`
         :return: None if the message is valid and raises an exception otherwise
         """
         message = encode_defunct(text=self.prepare_message())
         w3 = Web3(provider=provider)
 
+        if scheme is not None and self.scheme != scheme:
+            raise SchemeMismatch()
         if domain is not None and self.domain != domain:
             raise DomainMismatch()
         if nonce is not None and self.nonce != nonce:
             raise NonceMismatch()
 
-        verification_time = datetime.now(UTC) if timestamp is None else timestamp
+        verification_time = utc_now() if timestamp is None else timestamp
         if (
             self.expiration_time is not None
-            and verification_time >= self.expiration_time.date
+            and verification_time >= self.expiration_time._datetime
         ):
             raise ExpiredMessage()
-        if self.not_before is not None and verification_time <= self.not_before.date:
+        if (
+            self.not_before is not None
+            and verification_time <= self.not_before._datetime
+        ):
             raise NotYetValidMessage()
 
         try:
             address = w3.eth.account.recover_message(message, signature=signature)
         except ValueError:
             address = None
         except eth_utils.exceptions.ValidationError:
```

### Comparing `siwe-2.4.1/PKG-INFO` & `siwe-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: siwe
-Version: 2.4.1
+Version: 3.0.0
 Summary: A Python implementation of Sign-In with Ethereum (EIP-4361).
 Home-page: https://login.xyz
 License: MIT OR Apache-2.0
 Keywords: SIWE,EIP-4361,Sign-In with Ethereum,Spruce ID
 Author: Spruce Systems, Inc.
 Author-email: hello@spruceid.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: abnf (==1.1.1)
-Requires-Dist: eth-account (>=0.8.0,<0.11)
-Requires-Dist: eth-typing (>=3.4.0,<4.0.0)
-Requires-Dist: eth-utils (>=2.2.0,<3.0.0)
-Requires-Dist: pydantic (>=2.1.1,<3.0.0)
-Requires-Dist: python-dateutil (==2.8.2)
-Requires-Dist: web3 (>=6.0.0,<7.0.0)
+Requires-Dist: abnf (>=2.2,<3)
+Requires-Dist: eth-account (>=0.11,<0.12)
+Requires-Dist: eth-typing (>=4,<5)
+Requires-Dist: eth-utils (>=4,<5)
+Requires-Dist: pydantic (>=2.7,<3)
+Requires-Dist: pydantic-core (>=2,<3)
+Requires-Dist: typing-extensions (>=4,<5)
+Requires-Dist: web3 (>=6.17,<7)
 Project-URL: Discord, https://discord.gg/Sf9tSFzrnt
 Project-URL: EIP, https://github.com/ethereum/EIPs/blob/master/EIPS/eip-4361.md
 Project-URL: Repository, https://github.com/spruceid/siwe-py
 Description-Content-Type: text/markdown
 
 # Sign-In with Ethereum
```

