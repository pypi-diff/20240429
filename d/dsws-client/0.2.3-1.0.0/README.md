# Comparing `tmp/dsws_client-0.2.3.tar.gz` & `tmp/dsws_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsws_client-0.2.3.tar", max compression
+gzip compressed data, was "dsws_client-1.0.0.tar", last modified: Sun Apr 28 23:15:27 2024, max compression
```

## Comparing `dsws_client-0.2.3.tar` & `dsws_client-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0      753 2024-01-30 19:30:59.760152 dsws_client-0.2.3/README.md
--rw-r--r--   0        0        0      319 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/__init__.py
--rw-r--r--   0        0        0    10015 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/client.py
--rw-r--r--   0        0        0     1139 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/config.py
--rw-r--r--   0        0        0     2542 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/converters.py
--rw-r--r--   0        0        0    11641 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/ds_request.py
--rw-r--r--   0        0        0     3233 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/ds_response.py
--rw-r--r--   0        0        0      510 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/exceptions.py
--rw-r--r--   0        0        0     8195 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/parse.py
--rw-r--r--   0        0        0        0 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/py.typed
--rw-r--r--   0        0        0      436 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/utils.py
--rw-r--r--   0        0        0      488 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/value_objects/__init__.py
--rw-r--r--   0        0        0     1603 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/value_objects/enums.py
--rw-r--r--   0        0        0      266 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/value_objects/types.py
--rw-r--r--   0        0        0       77 2024-01-30 19:30:59.760152 dsws_client-0.2.3/dsws_client/version.py
--rw-r--r--   0        0        0     3645 2024-01-30 19:30:59.760152 dsws_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 dsws_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      753 2024-04-28 23:15:09.255058 dsws_client-1.0.0/README.md
+-rw-r--r--   0        0        0      319 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/__init__.py
+-rw-r--r--   0        0        0    11479 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/client.py
+-rw-r--r--   0        0        0     1589 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/config.py
+-rw-r--r--   0        0        0      757 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/converters.py
+-rw-r--r--   0        0        0     9523 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/ds_request.py
+-rw-r--r--   0        0        0     5417 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/ds_response.py
+-rw-r--r--   0        0        0      510 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/exceptions.py
+-rw-r--r--   0        0        0     5698 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/parse.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/py.typed
+-rw-r--r--   0        0        0      508 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/value_objects/__init__.py
+-rw-r--r--   0        0        0     1603 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/value_objects/enums.py
+-rw-r--r--   0        0        0      563 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/value_objects/types.py
+-rw-r--r--   0        0        0       77 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/version.py
+-rw-r--r--   0        0        0     3206 2024-04-28 23:15:27.647108 dsws_client-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     2567 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/test_client.py
+-rw-r--r--   0        0        0     1248 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/test_parsing.py
+-rw-r--r--   0        0        0     4935 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/test_requests.py
+-rw-r--r--   0        0        0     1784 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/test_responses.py
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 dsws_client-1.0.0/PKG-INFO
```

### Comparing `dsws_client-0.2.3/README.md` & `dsws_client-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dsws_client-0.2.3/dsws_client/client.py` & `dsws_client-1.0.0/dsws_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,268 +1,255 @@
-import json
+"""The DSWS client."""
+
+import concurrent.futures
+import itertools
 import logging
 import sys
-import urllib.parse
-from typing import Any, Dict, List, Optional, Type, TypeVar, Union
+from typing import Any, Dict, Iterator, List, Optional, Type, TypeVar, Union
 
-import requests
+import httpx
+import msgspec
 
 from dsws_client.config import DSWSConfig
 from dsws_client.ds_request import (
     DSDataRequest,
     DSDataType,
     DSDate,
     DSGetDataBundleRequest,
     DSGetDataRequest,
     DSGetTokenRequest,
     DSInstrument,
     DSRequest,
     bundle_identifiers,
-    to_ds_dict,
 )
 from dsws_client.ds_response import (
     DSGetDataBundleResponse,
     DSGetDataResponse,
     DSGetTokenResponse,
 )
 from dsws_client.exceptions import (
     InvalidResponseError,
     RequestFailedError,
 )
 from dsws_client.parse import ParsedResponse, responses_to_records
-from dsws_client.value_objects import DateType, DSStringKVPair
+from dsws_client.value_objects import DateType, DSStringKVPair, Token
 
 logger = logging.getLogger(__name__)
 
 ResponseCls = TypeVar("ResponseCls")
 
 
 class DSWSClient:
-    """Client for the DSWS web service."""
+    """
+    Client for the DSWS web service.
 
-    def __init__(self, username: str, password: str, **kwargs: Any) -> None:
-        """
-        Initialize the client.
+    It can be shared between threads.
 
-        Args:
-            username: DSWS username.
-            password: DSWS password.
-            **kwargs: Additional keyword arguments passed to the config object.
-        """
+    Args:
+        username: The DSWS username.
+        password: The DSWS password.
+        host (default: "https://product.datastream.com"): The DSWS host URL.
+        timeout (default: 180): The timeout configuration to use when sending
+            requests.
+        proxy (optional): A proxy URL where all the traffic should be routed.
+        ssl_cert (optional): SSL certificates (a.k.a CA bundle) used to
+            verify the identity of requested hosts.
+        app_id (default: dsws-client-VERSION): The app ID to use in the
+            request.
+        data_source (optional): The data source to use in the request.
+        max_concurrency (default: 1): The maximum number of concurrent
+            requests to make.
+        debug (default: False): If True, print the request and response
+            data to stdout.
+    """
+
+    def __init__(self, username: str, password: str, **kwargs: Any) -> None:
         config = DSWSConfig(**kwargs)
         self._username = username
         self._password = password
-        self._url = urllib.parse.urljoin(config.base_url, config.path)
-        self._session = requests.Session()
-        self._proxies = (
-            None
-            if config.proxy is None
-            else {"http": config.proxy, "https": config.proxy}
-        )
-        self._timeout = config.timeout
-        self._ssl_cert = config.ssl_cert
-        self._token_response: Optional[DSGetTokenResponse] = None
+        self._session = httpx.Client(
+            base_url=config.base_url,
+            timeout=config.timeout,
+            proxies=config.proxies,  # type: ignore[arg-type]
+            verify=config.ssl_cert or True,
+            headers={"Content-Type": "application/json"},
+        )
+        self._max_concurrency = config.max_concurrency
         self._app_id = config.app_id
         self._data_source = config.data_source
         self._debug = config.debug
+        self._token: Optional[Token] = None
 
     @property
     def token(self) -> str:
         """Get a token."""
-        if self._token_response is None or self._token_response.is_expired:
-            self._token_response = self.get_token()
-        return self._token_response.token_value
+        if self._token is None or self._token.is_expired:
+            self._token = self.fetch_token()
+        return self._token.token_value
 
     def fetch_snapshot_data(
         self,
         identifiers: List[str],
         fields: List[str],
-        start: DateType = "",
+        start: Optional[DateType] = None,
         tag: Optional[str] = None,
     ) -> ParsedResponse:
         """Fetch snapshot data."""
-        responses = self.fetch_all(
+        request_bundles = self.construct_request_bundles(
             identifiers=identifiers,
             fields=fields,
             start=start,
-            end="",
+            end=None,
             frequency=None,
             kind=0,
             tag=tag,
             return_symbol_names=True,
             return_field_names=True,
         )
-        data_responses = []
-        for response in responses:
-            data_responses.extend(response.data_responses)
+        responses = self.fetch_all(request_bundles)
+        data_responses = itertools.chain.from_iterable(
+            response.data_responses for response in responses
+        )
         return responses_to_records(data_responses)
 
     def fetch_timeseries_data(  # noqa: PLR0913
         self,
         identifiers: List[str],
         fields: List[str],
-        start: DateType = "",
-        end: DateType = "",
+        start: Optional[DateType] = None,
+        end: Optional[DateType] = None,
         frequency: str = "D",
         tag: Optional[str] = None,
     ) -> ParsedResponse:
         """Fetch timeseries data."""
-        responses = self.fetch_all(
+        request_bundles = self.construct_request_bundles(
             identifiers=identifiers,
             fields=fields,
             start=start,
             end=end,
             frequency=frequency,
             kind=1,
             tag=tag,
             return_symbol_names=True,
             return_field_names=True,
         )
-        data_responses = []
-        for response in responses:
-            data_responses.extend(response.data_responses)
+        responses = self.fetch_all(request_bundles)
+        data_responses = itertools.chain.from_iterable(
+            response.data_responses for response in responses
+        )
         return responses_to_records(data_responses)
 
-    def fetch_one(  # noqa: PLR0913
+    def fetch_one(
         self,
-        identifiers: Union[str, List[str]],
-        fields: List[str],
-        start: DateType,
-        end: DateType = "",
-        frequency: str = "D",
-        kind: int = 1,
-        tag: Optional[str] = None,
-        *,
-        return_symbol_names: bool = False,
-        return_field_names: bool = False,
-        instrument_props: Optional[Dict[str, str]] = None,
-        field_props: Optional[Dict[str, str]] = None,
+        data_request: DSDataRequest,
+        **kwargs: object,
     ) -> DSGetDataResponse:
-        """Fetch data from the DSWS web service."""
-        request = self.construct_request(
-            identifiers=identifiers,
-            fields=fields,
-            start=start,
-            end=end,
-            frequency=frequency,
-            kind=kind,
-            tag=tag,
-            return_symbol_names=return_symbol_names,
-            return_field_names=return_field_names,
-            instrument_props=instrument_props,
-            field_props=field_props,
-        )
-        return self.get_data(request)
-
-    def fetch_all(  # noqa: PLR0913
-        self,
-        identifiers: List[str],
-        fields: List[str],
-        start: DateType,
-        end: DateType = "",
-        frequency: Optional[str] = "D",
-        kind: int = 1,
-        tag: Optional[str] = None,
-        *,
-        return_symbol_names: bool = False,
-        return_field_names: bool = False,
-        instrument_props: Optional[Dict[str, str]] = None,
-        field_props: Optional[Dict[str, str]] = None,
-    ) -> List[DSGetDataBundleResponse]:
-        """Fetch as many bundles as needed to get all items."""
-        instrument = DSInstrument.construct(
-            identifiers,
-            return_names=return_symbol_names,
-            properties=instrument_props,
-        )
-        data_types = [
-            DSDataType.construct(
-                field,
-                return_names=return_field_names,
-                properties=field_props,
-            )
-            for field in fields
-        ]
-        date = DSDate(start, end, frequency, kind)
-        identifier_bundles = bundle_identifiers(instrument, len(data_types))
-        responses = []
-        for identifier_bundle in identifier_bundles:
-            data_requests = []
-            for instrument in identifier_bundle:
-                data_requests.append(
-                    DSDataRequest(instrument, data_types, date, tag=tag)
-                )
-            responses.append(self.get_data_bundle(data_requests))
-        return responses
-
-    def get_token(self, **kwargs: Any) -> DSGetTokenResponse:
-        """
-        Fetch a new token.
-
-        Args:
-            **kwargs: Additional properties to set on the request.
-
-        Returns:
-            A token response.
-        """
-        return self._execute_request(
-            DSGetTokenRequest(self._username, self._password, properties=kwargs),
-            DSGetTokenResponse,
-        )
-
-    def get_data(self, data_request: DSDataRequest, **kwargs: Any) -> DSGetDataResponse:
         """
         Post a data request.
 
         Args:
             data_request: A data request.
             **kwargs: Additional properties to set on the request.
 
         Returns:
             A data response.
         """
+        logger.debug("fetching one")
         return self._execute_request(
             DSGetDataRequest(
                 token_value=self.token,
                 data_request=data_request,
-                properties=kwargs,
+                properties=[
+                    DSStringKVPair(key, value) for key, value in kwargs.items()
+                ],
             ),
             DSGetDataResponse,
         )
 
-    def get_data_bundle(
+    def fetch_bundle(
         self,
         data_requests: List[DSDataRequest],
-        **kwargs: Any,
+        **kwargs: object,
     ) -> DSGetDataBundleResponse:
         """
         Post multiple data requests.
 
         Args:
             data_requests: A list of data requests.
             **kwargs: Additional properties to set on the request.
 
         Returns:
             A data bundle response.
         """
+        logger.debug("fetching bundle")
         return self._execute_request(
             DSGetDataBundleRequest(
                 token_value=self.token,
                 data_requests=data_requests,
-                properties=kwargs,
+                properties=[
+                    DSStringKVPair(key, value) for key, value in kwargs.items()
+                ],
             ),
             DSGetDataBundleResponse,
         )
 
+    def fetch_all(
+        self,
+        request_bundles: List[List[DSDataRequest]],
+    ) -> Iterator[DSGetDataBundleResponse]:
+        """Fetch as many bundles as needed to get all items."""
+        if self._max_concurrency > 1:
+            yield from self._fetch_all_threaded(request_bundles)
+        else:
+            for bundle in request_bundles:
+                yield self.fetch_bundle(bundle)
+
+    def _fetch_all_threaded(
+        self,
+        request_bundles: List[List[DSDataRequest]],
+    ) -> Iterator[DSGetDataBundleResponse]:
+        """Fetch as many bundles as needed to get all items (concurrently)."""
+        with concurrent.futures.ThreadPoolExecutor(
+            max_workers=self._max_concurrency
+        ) as executor:
+            logger.debug("fetching bundles in parallel")
+            futures = [
+                executor.submit(self.fetch_bundle, bundle) for bundle in request_bundles
+            ]
+            for future in concurrent.futures.as_completed(futures):
+                yield future.result()
+
+    def fetch_token(self, **kwargs: object) -> Token:
+        """
+        Fetch a new token.
+
+        Args:
+            **kwargs: Additional properties to set on the request.
+
+        Returns:
+            A token.
+        """
+        token_response = self._execute_request(
+            DSGetTokenRequest(
+                self._username,
+                self._password,
+                properties=[
+                    DSStringKVPair(key, value) for key, value in kwargs.items()
+                ],
+            ),
+            DSGetTokenResponse,
+        )
+        return token_response.to_token()
+
     def construct_request(  # noqa: PLR0913
         self,
         identifiers: Union[str, List[str]],
         fields: List[str],
-        start: DateType,
-        end: DateType,
+        start: Optional[DateType],
+        end: Optional[DateType],
         frequency: Optional[str],
         kind: int,
         tag: Optional[str] = None,
         *,
         return_symbol_names: bool = False,
         return_field_names: bool = False,
         instrument_props: Optional[Dict[str, str]] = None,
@@ -273,47 +260,89 @@
             identifiers,
             return_names=return_symbol_names,
             properties=instrument_props,
         )
         data_types = [
             DSDataType.construct(
                 field,
-                return_names=return_field_names,
+                return_name=return_field_names,
                 properties=field_props,
             )
             for field in fields
         ]
-        date = DSDate(start, end, frequency, kind)
+        date = DSDate.construct(start, end, frequency, kind)
         return DSDataRequest(instrument, data_types, date, tag)
 
+    def construct_request_bundles(  # noqa: PLR0913
+        self,
+        identifiers: List[str],
+        fields: List[str],
+        start: Optional[DateType],
+        end: Optional[DateType],
+        frequency: Optional[str],
+        kind: int,
+        tag: Optional[str] = None,
+        *,
+        return_symbol_names: bool = False,
+        return_field_names: bool = False,
+        instrument_props: Optional[Dict[str, str]] = None,
+        field_props: Optional[Dict[str, str]] = None,
+    ) -> List[List[DSDataRequest]]:
+        """Construct a list of data request bundles."""
+        instrument = DSInstrument.construct(
+            identifiers,
+            return_names=return_symbol_names,
+            properties=instrument_props,
+        )
+        data_types = [
+            DSDataType.construct(
+                field,
+                return_name=return_field_names,
+                properties=field_props,
+            )
+            for field in fields
+        ]
+        date = DSDate.construct(start, end, frequency, kind)
+        identifier_bundles = bundle_identifiers(instrument, len(data_types))
+        request_bundles = []
+        for identifier_bundle in identifier_bundles:
+            data_requests = []
+            for instrument in identifier_bundle:
+                data_requests.append(
+                    DSDataRequest(instrument, data_types, date, tag=tag)
+                )
+            request_bundles.append(data_requests)
+        return request_bundles
+
     def _execute_request(
         self,
         request: DSRequest,
         response_cls: Type[ResponseCls],
     ) -> ResponseCls:
         """Execute a request."""
-        if self._app_id is not None:
-            request.properties.append(DSStringKVPair("__AppId", self._app_id))
-        if self._data_source is not None:
-            request.properties.append(DSStringKVPair("Source", self._data_source))
-        request_url = urllib.parse.urljoin(self._url, request.path)
-        request_dict = to_ds_dict(request)
+        logger.debug("executing request")
+        self._prep_request(request)
+        request_data = msgspec.json.encode(request)
         if self._debug:
-            sys.stdout.write(f"sending request: {request_dict!s}")
+            sys.stdout.write(f"sending request: {request_data!s}")
         response = self._session.post(
-            request_url,
-            json=request_dict,
-            proxies=self._proxies,
-            verify=self._ssl_cert,
-            timeout=self._timeout,
+            request.path,
+            content=request_data,
         )
-        if not response.ok:
+        if not response.is_success:
             msg = f"request failed: {response.text}"
             raise RequestFailedError(msg, response.status_code)
         try:
-            json_response = response.json()
-        except json.JSONDecodeError as exc:
+            response_decoded = msgspec.json.decode(response.content, type=response_cls)
+        except (msgspec.ValidationError, ValueError, TypeError) as exc:
             msg = f"invalid response: {response.text}"
             raise InvalidResponseError(msg) from exc
         if self._debug:
-            sys.stdout.write(f"received response: {json_response!s}")
-        return response_cls(**json_response)
+            sys.stdout.write(f"received response: {response_decoded!s}")
+        return response_decoded
+
+    def _prep_request(self, request: DSRequest) -> None:
+        """Prepare a request."""
+        if self._app_id is not None:
+            request.properties.append(DSStringKVPair("__AppId", self._app_id))
+        if self._data_source is not None:
+            request.properties.append(DSStringKVPair("Source", self._data_source))
```

### Comparing `dsws_client-0.2.3/dsws_client/config.py` & `dsws_client-1.0.0/dsws_client/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 import os
-from typing import Any, ClassVar, Optional
+import urllib.parse
+from typing import Any, ClassVar, Dict, Optional
 
 import attrs
+import httpx
 from dotenv import load_dotenv
 
 from dsws_client.version import __version__
 
 
 @attrs.define()
 class DSWSConfig:
     """Configuration for the DSWS client."""
 
     path: ClassVar[str] = "/DSWSClient/V1/DSService.svc/rest/"
-    base_url: str = "https://product.datastream.com"
+    host: str = "https://product.datastream.com"
     timeout: int = attrs.field(default=180, converter=int)
     proxy: Optional[str] = None
     ssl_cert: Optional[str] = None
     app_id: str = f"dsws-client-{__version__}"
     data_source: Optional[str] = None
+    max_concurrency: int = 1
     debug: bool = attrs.field(default=False, converter=attrs.converters.to_bool)
 
     def __init__(self, **kwargs: Any) -> None:
         """Load configuration from environment variables."""
         load_dotenv()
         init_dict = {}
         for field in attrs.fields(DSWSConfig):
             # try to get the value from kwargs, then from environment variables
             value = kwargs.get(field.name, os.getenv(field.name.upper()))
             if value is not None:
                 init_dict[field.name] = value
         self.__attrs_init__(**init_dict)  # type: ignore[attr-defined]
+
+    @property
+    def base_url(self) -> str:
+        """Return the base URL."""
+        return urllib.parse.urljoin(self.host, self.path)
+
+    @property
+    def proxies(self) -> Optional[Dict[str, httpx.HTTPTransport]]:
+        """Return the proxies."""
+        proxy = httpx.HTTPTransport(proxy=self.proxy)
+        return {"https://": proxy, "http://": proxy} if self.proxy else None
```

### Comparing `dsws_client-0.2.3/dsws_client/value_objects/enums.py` & `dsws_client-1.0.0/dsws_client/value_objects/enums.py`

 * *Files identical despite different names*

### Comparing `dsws_client-0.2.3/PKG-INFO` & `dsws_client-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 Metadata-Version: 2.1
 Name: dsws-client
-Version: 0.2.3
+Version: 1.0.0
 Summary: Python client for the Datastream Web Service API (DSWS)
+Author-Email: ljnsn <info@ljnsn.com>
 License: MIT
-Author: ljnsn
-Author-email: info@ljnsn.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: commitizen (>=2.42.0,<3.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.29.0,<3.0.0)
-Requires-Dist: setuptools ; python_version >= "3.12"
+Requires-Python: <4.0,>=3.8
+Requires-Dist: attrs>=23.1.0
+Requires-Dist: httpx>=0.27.0
+Requires-Dist: msgspec>=0.18.6
+Requires-Dist: python-dotenv>=1.0.0
+Requires-Dist: setuptools; python_version >= "3.12"
+Requires-Dist: typing-extensions>=4.11.0; python_version < "3.10"
 Description-Content-Type: text/markdown
 
 # dsws-client
 
 Python wrapper for the Datastream Web Services API (DSWS)
 
 To Connect to the Refinitiv Datastream database via Datastream Web Services, you need to have a Datastream subscription and a username/password to use this package.
@@ -32,8 +25,7 @@
 
 ## Why?
 
 There are two client libraries for DSWS that I am aware of, the official [DatastreamDSWS][1] and [pydatastream][2]. Both of them return data only as pandas dataframes. I needed something that doesn't depend on pandas, so I decided to make this client.
 
 [1]: https://github.com/DatastreamDSWS/Datastream
 [2]: https://github.com/vfilimonov/pydatastream
-
```

