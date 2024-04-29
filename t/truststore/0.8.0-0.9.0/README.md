# Comparing `tmp/truststore-0.8.0.tar.gz` & `tmp/truststore-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truststore-0.8.0.tar", last modified: Fri Sep  8 04:11:42 2023, max compression
+gzip compressed data, was "truststore-0.9.0.tar", last modified: Mon Apr 29 17:14:14 2024, max compression
```

## Comparing `truststore-0.8.0.tar` & `truststore-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,22 @@
--rw-r--r--   0        0        0     1086 2023-09-08 04:11:42.000000 truststore-0.8.0/LICENSE
--rw-r--r--   0        0        0     2986 2023-09-08 04:11:42.000000 truststore-0.8.0/README.md
--rw-r--r--   0        0        0     1240 2023-09-08 04:11:42.000000 truststore-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      403 2023-09-08 04:11:42.000000 truststore-0.8.0/src/truststore/__init__.py
--rw-r--r--   0        0        0     9857 2023-09-08 04:11:42.000000 truststore-0.8.0/src/truststore/_api.py
--rw-r--r--   0        0        0    17694 2023-09-08 04:11:42.000000 truststore-0.8.0/src/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2023-09-08 04:11:42.000000 truststore-0.8.0/src/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2023-09-08 04:11:42.000000 truststore-0.8.0/src/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17468 2023-09-08 04:11:42.000000 truststore-0.8.0/src/truststore/_windows.py
--rw-r--r--   0        0        0        0 2023-09-08 04:11:42.000000 truststore-0.8.0/src/truststore/py.typed
--rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 truststore-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-29 17:14:14.000000 truststore-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3399 2024-04-29 17:14:14.000000 truststore-0.9.0/README.md
+-rw-r--r--   0        0        0      639 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0      805 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0       31 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/requirements.txt
+-rw-r--r--   0        0        0      620 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0     6386 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/source/index.md
+-rw-r--r--   0        0        0     1389 2024-04-29 17:14:14.000000 truststore-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      403 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/__init__.py
+-rw-r--r--   0        0        0    10325 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_api.py
+-rw-r--r--   0        0        0    17608 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_macos.py
+-rw-r--r--   0        0        0     2324 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_openssl.py
+-rw-r--r--   0        0        0     1130 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_ssl_constants.py
+-rw-r--r--   0        0        0    17891 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_windows.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/py.typed
+-rw-r--r--   0        0        0      561 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     5293 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0    13592 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/test_api.py
+-rw-r--r--   0        0        0     1288 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/test_custom_ca.py
+-rw-r--r--   0        0        0     3814 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/test_inject.py
+-rw-r--r--   0        0        0     1663 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/test_sslcontext.py
+-rw-r--r--   0        0        0     4490 1970-01-01 00:00:00.000000 truststore-0.9.0/PKG-INFO
```

### Comparing `truststore-0.8.0/LICENSE` & `truststore-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `truststore-0.8.0/README.md` & `truststore-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 Truststore **requires Python 3.10 or later** and supports the following platforms:
 - macOS 10.8+ via [Security framework](https://developer.apple.com/documentation/security)
 - Windows via [CryptoAPI](https://docs.microsoft.com/en-us/windows/win32/seccrypto/cryptography-functions#certificate-verification-functions)
 - Linux via OpenSSL
 
 ## User Guide
 
+> **Warning**
+> **PLEASE READ:** `inject_into_ssl()` **must not be used by libraries or packages** as it will cause issues on import time when integrated with other libraries.
+> Libraries and packages should instead use `truststore.SSLContext` directly which is detailed below.
+> 
+> The `inject_into_ssl()` function is intended only for use in applications and scripts.
+
 You can inject `truststore` into the standard library `ssl` module so the functionality is used
 by every library by default. To do so use the `truststore.inject_into_ssl()` function:
 
 ```python
 import truststore
 truststore.inject_into_ssl()
 
@@ -53,15 +59,15 @@
 http = aiohttp.ClientSession()
 resp = await http.request("GET", "https://example.com")
 
 import requests
 resp = requests.get("https://example.com")
 ```
 
-If you'd like finer-grained control you can create your own `truststore.SSLContext` instance
+If you'd like finer-grained control or you're developing a library or package you can create your own `truststore.SSLContext` instance
 and use it anywhere you'd use an `ssl.SSLContext`:
 
 ```python
 import ssl
 import truststore
 
 ctx = truststore.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
```

### Comparing `truststore-0.8.0/pyproject.toml` & `truststore-0.9.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -17,14 +17,15 @@
   "Operating System :: MacOS",
   "Operating System :: Microsoft",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.13",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version", "description"]
 requires-python = ">= 3.10"
 
 [project.urls]
@@ -34,7 +35,13 @@
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 filterwarnings = [
   "error",
   # See: aio-libs/aiohttp#7545
   "ignore:.*datetime.utcfromtimestamp().*:DeprecationWarning",
 ]
+markers = [
+  "internet: test requires Internet access"
+]
+
+[tool.flit.sdist]
+include = ["docs", "tests"]
```

### Comparing `truststore-0.8.0/src/truststore/_api.py` & `truststore-0.9.0/src/truststore/_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import platform
 import socket
 import ssl
+import sys
 import typing
 
-import _ssl  # type: ignore[import]
-
 from ._ssl_constants import (
     _original_SSLContext,
     _original_super_SSLContext,
     _truststore_SSLContext_dunder_class,
     _truststore_SSLContext_super_class,
 )
 
@@ -45,15 +44,15 @@
 
 def extract_from_ssl() -> None:
     """Restores the :class:`ssl.SSLContext` class to its original state"""
     setattr(ssl, "SSLContext", _original_SSLContext)
     try:
         import urllib3.util.ssl_ as urllib3_ssl
 
-        urllib3_ssl.SSLContext = _original_SSLContext
+        urllib3_ssl.SSLContext = _original_SSLContext  # type: ignore[assignment]
     except ImportError:
         pass
 
 
 class SSLContext(_truststore_SSLContext_super_class):  # type: ignore[misc]
     """SSLContext API that uses system certificates on all platforms"""
 
@@ -167,24 +166,21 @@
 
     def cert_store_stats(self) -> dict[str, int]:
         raise NotImplementedError()
 
     @typing.overload
     def get_ca_certs(
         self, binary_form: typing.Literal[False] = ...
-    ) -> list[typing.Any]:
-        ...
+    ) -> list[typing.Any]: ...
 
     @typing.overload
-    def get_ca_certs(self, binary_form: typing.Literal[True] = ...) -> list[bytes]:
-        ...
+    def get_ca_certs(self, binary_form: typing.Literal[True] = ...) -> list[bytes]: ...
 
     @typing.overload
-    def get_ca_certs(self, binary_form: bool = ...) -> typing.Any:
-        ...
+    def get_ca_certs(self, binary_form: bool = ...) -> typing.Any: ...
 
     def get_ca_certs(self, binary_form: bool = False) -> list[typing.Any] | list[bytes]:
         raise NotImplementedError()
 
     @property
     def check_hostname(self) -> bool:
         return self._ctx.check_hostname
@@ -272,31 +268,42 @@
     @verify_mode.setter
     def verify_mode(self, value: ssl.VerifyMode) -> None:
         _original_super_SSLContext.verify_mode.__set__(  # type: ignore[attr-defined]
             self._ctx, value
         )
 
 
+# Python 3.13+ makes get_unverified_chain() a public API that only returns DER
+# encoded certificates. We detect whether we need to call public_bytes() for 3.10->3.12
+# Pre-3.13 returned None instead of an empty list from get_unverified_chain()
+if sys.version_info >= (3, 13):
+
+    def _get_unverified_chain_bytes(sslobj: ssl.SSLObject) -> list[bytes]:
+        unverified_chain = sslobj.get_unverified_chain() or ()  # type: ignore[attr-defined]
+        return [cert for cert in unverified_chain]
+
+else:
+    import _ssl  # type: ignore[import-not-found]
+
+    def _get_unverified_chain_bytes(sslobj: ssl.SSLObject) -> list[bytes]:
+        unverified_chain = sslobj.get_unverified_chain() or ()  # type: ignore[attr-defined]
+        return [cert.public_bytes(_ssl.ENCODING_DER) for cert in unverified_chain]
+
+
 def _verify_peercerts(
     sock_or_sslobj: ssl.SSLSocket | ssl.SSLObject, server_hostname: str | None
 ) -> None:
     """
     Verifies the peer certificates from an SSLSocket or SSLObject
     against the certificates in the OS trust store.
     """
     sslobj: ssl.SSLObject = sock_or_sslobj  # type: ignore[assignment]
     try:
         while not hasattr(sslobj, "get_unverified_chain"):
             sslobj = sslobj._sslobj  # type: ignore[attr-defined]
     except AttributeError:
         pass
 
-    # SSLObject.get_unverified_chain() returns 'None'
-    # if the peer sends no certificates. This is common
-    # for the server-side scenario.
-    unverified_chain: typing.Sequence[_ssl.Certificate] = (
-        sslobj.get_unverified_chain() or ()  # type: ignore[attr-defined]
-    )
-    cert_bytes = [cert.public_bytes(_ssl.ENCODING_DER) for cert in unverified_chain]
+    cert_bytes = _get_unverified_chain_bytes(sslobj)
     _verify_peercerts_impl(
         sock_or_sslobj.context, cert_bytes, server_hostname=server_hostname
     )
```

### Comparing `truststore-0.8.0/src/truststore/_macos.py` & `truststore-0.9.0/src/truststore/_macos.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,14 @@
 
     Security.SecTrustSetAnchorCertificates.argtypes = [SecTrustRef, CFArrayRef]
     Security.SecTrustSetAnchorCertificates.restype = OSStatus
 
     Security.SecTrustSetAnchorCertificatesOnly.argtypes = [SecTrustRef, Boolean]
     Security.SecTrustSetAnchorCertificatesOnly.restype = OSStatus
 
-    Security.SecTrustEvaluate.argtypes = [SecTrustRef, POINTER(SecTrustResultType)]
-    Security.SecTrustEvaluate.restype = OSStatus
-
     Security.SecPolicyCreateRevocation.argtypes = [CFOptionFlags]
     Security.SecPolicyCreateRevocation.restype = SecPolicyRef
 
     Security.SecPolicyCreateSSL.argtypes = [Boolean, CFStringRef]
     Security.SecPolicyCreateSSL.restype = SecPolicyRef
 
     Security.SecTrustCreateWithCertificates.argtypes = [
@@ -255,14 +252,15 @@
         message = f"SecureTransport operation returned a non-zero OSStatus: {result}"
 
     raise ssl.SSLError(message)
 
 
 Security.SecTrustCreateWithCertificates.errcheck = _handle_osstatus  # type: ignore[assignment]
 Security.SecTrustSetAnchorCertificates.errcheck = _handle_osstatus  # type: ignore[assignment]
+Security.SecTrustSetAnchorCertificatesOnly.errcheck = _handle_osstatus  # type: ignore[assignment]
 Security.SecTrustGetTrustResult.errcheck = _handle_osstatus  # type: ignore[assignment]
 
 
 class CFConst:
     """CoreFoundation constants"""
 
     kCFStringEncodingUTF8 = CFStringEncoding(0x08000100)
@@ -413,29 +411,29 @@
         finally:
             # The certs are now being held by SecTrust so we can
             # release our handles for the array.
             if certs:
                 CoreFoundation.CFRelease(certs)
 
         # If there are additional trust anchors to load we need to transform
-        # the list of DER-encoded certificates into a CFArray. Otherwise
-        # pass 'None' to signal that we only want system / fetched certificates.
+        # the list of DER-encoded certificates into a CFArray.
         ctx_ca_certs_der: list[bytes] | None = ssl_context.get_ca_certs(
             binary_form=True
         )
         if ctx_ca_certs_der:
             ctx_ca_certs = None
             try:
-                ctx_ca_certs = _der_certs_to_cf_cert_array(cert_chain)
+                ctx_ca_certs = _der_certs_to_cf_cert_array(ctx_ca_certs_der)
                 Security.SecTrustSetAnchorCertificates(trust, ctx_ca_certs)
             finally:
                 if ctx_ca_certs:
                     CoreFoundation.CFRelease(ctx_ca_certs)
-        else:
-            Security.SecTrustSetAnchorCertificates(trust, None)
+
+        # We always want system certificates.
+        Security.SecTrustSetAnchorCertificatesOnly(trust, False)
 
         cf_error = CoreFoundation.CFErrorRef()
         sec_trust_eval_result = Security.SecTrustEvaluateWithError(
             trust, ctypes.byref(cf_error)
         )
         # sec_trust_eval_result is a bool (0 or 1)
         # where 1 means that the certs are trusted.
```

### Comparing `truststore-0.8.0/src/truststore/_openssl.py` & `truststore-0.9.0/src/truststore/_openssl.py`

 * *Files identical despite different names*

### Comparing `truststore-0.8.0/src/truststore/_ssl_constants.py` & `truststore-0.9.0/src/truststore/_ssl_constants.py`

 * *Files identical despite different names*

### Comparing `truststore-0.8.0/src/truststore/_windows.py` & `truststore-0.9.0/src/truststore/_windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,14 +321,20 @@
 
 def _verify_peercerts_impl(
     ssl_context: ssl.SSLContext,
     cert_chain: list[bytes],
     server_hostname: str | None = None,
 ) -> None:
     """Verify the cert_chain from the server using Windows APIs."""
+
+    # If the peer didn't send any certificates then
+    # we can't do verification. Raise an error.
+    if not cert_chain:
+        raise ssl.SSLCertVerificationError("Peer sent no certificates to verify")
+
     pCertContext = None
     hIntermediateCertStore = CertOpenStore(CERT_STORE_PROV_MEMORY, 0, None, 0, None)
     try:
         # Add intermediate certs to an in-memory cert store
         for cert_bytes in cert_chain[1:]:
             CertAddEncodedCertificateToStore(
                 hIntermediateCertStore,
@@ -371,32 +377,36 @@
                 None,
                 hIntermediateCertStore,
                 pCertContext,
                 pChainPara,
                 server_hostname,
                 chain_flags=chain_flags,
             )
-        except ssl.SSLCertVerificationError:
+        except ssl.SSLCertVerificationError as e:
             # If that fails but custom CA certs have been added
             # to the SSLContext using load_verify_locations,
             # try verifying using a custom chain engine
             # that trusts the custom CA certs.
             custom_ca_certs: list[bytes] | None = ssl_context.get_ca_certs(
                 binary_form=True
             )
             if custom_ca_certs:
-                _verify_using_custom_ca_certs(
-                    ssl_context,
-                    custom_ca_certs,
-                    hIntermediateCertStore,
-                    pCertContext,
-                    pChainPara,
-                    server_hostname,
-                    chain_flags=chain_flags,
-                )
+                try:
+                    _verify_using_custom_ca_certs(
+                        ssl_context,
+                        custom_ca_certs,
+                        hIntermediateCertStore,
+                        pCertContext,
+                        pChainPara,
+                        server_hostname,
+                        chain_flags=chain_flags,
+                    )
+                # Raise the original error, not the new error.
+                except ssl.SSLCertVerificationError:
+                    raise e from None
             else:
                 raise
     finally:
         CertCloseStore(hIntermediateCertStore, 0)
         if pCertContext:
             CertFreeCertificateContext(pCertContext)
```

### Comparing `truststore-0.8.0/PKG-INFO` & `truststore-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: truststore
-Version: 0.8.0
+Version: 0.9.0
 Summary: Verify certificates using native system trust stores
 Author-email: Seth Michael Larson <sethmichaellarson@gmail.com>, David Glick <david@glicksoftware.com>
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Project-URL: Documentation, https://truststore.readthedocs.io
 Project-URL: Source, https://github.com/sethmlarson/truststore
 
 # Truststore
 
@@ -55,14 +56,20 @@
 Truststore **requires Python 3.10 or later** and supports the following platforms:
 - macOS 10.8+ via [Security framework](https://developer.apple.com/documentation/security)
 - Windows via [CryptoAPI](https://docs.microsoft.com/en-us/windows/win32/seccrypto/cryptography-functions#certificate-verification-functions)
 - Linux via OpenSSL
 
 ## User Guide
 
+> **Warning**
+> **PLEASE READ:** `inject_into_ssl()` **must not be used by libraries or packages** as it will cause issues on import time when integrated with other libraries.
+> Libraries and packages should instead use `truststore.SSLContext` directly which is detailed below.
+> 
+> The `inject_into_ssl()` function is intended only for use in applications and scripts.
+
 You can inject `truststore` into the standard library `ssl` module so the functionality is used
 by every library by default. To do so use the `truststore.inject_into_ssl()` function:
 
 ```python
 import truststore
 truststore.inject_into_ssl()
 
@@ -75,15 +82,15 @@
 http = aiohttp.ClientSession()
 resp = await http.request("GET", "https://example.com")
 
 import requests
 resp = requests.get("https://example.com")
 ```
 
-If you'd like finer-grained control you can create your own `truststore.SSLContext` instance
+If you'd like finer-grained control or you're developing a library or package you can create your own `truststore.SSLContext` instance
 and use it anywhere you'd use an `ssl.SSLContext`:
 
 ```python
 import ssl
 import truststore
 
 ctx = truststore.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
```

