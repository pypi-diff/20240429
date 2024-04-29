# Comparing `tmp/resty_client-0.0.5.tar.gz` & `tmp/resty_client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resty_client-0.0.5.tar", max compression
+gzip compressed data, was "resty_client-0.0.6.tar", max compression
```

## Comparing `resty_client-0.0.5.tar` & `resty_client-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rw-r--r--   0        0        0     1090 2024-01-23 13:22:57.074926 resty_client-0.0.5/LICENSE
--rw-r--r--   0        0        0     1119 2024-04-26 19:35:16.403290 resty_client-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3906 2024-04-26 19:31:39.072847 resty_client-0.0.5/README.md
--rw-r--r--   0        0        0      172 2024-04-26 09:56:00.652385 resty_client-0.0.5/resty/__init__.py
--rw-r--r--   0        0        0      230 2024-04-26 09:22:05.024491 resty_client-0.0.5/resty/__version__.py
--rw-r--r--   0        0        0       89 2024-04-25 16:40:33.939395 resty_client-0.0.5/resty/clients/__init__.py
--rw-r--r--   0        0        0       89 2024-04-25 15:52:51.149933 resty_client-0.0.5/resty/clients/httpx/__init__.py
--rw-r--r--   0        0        0     2912 2024-04-26 08:35:43.160377 resty_client-0.0.5/resty/clients/httpx/clients.py
--rw-r--r--   0        0        0      294 2024-04-25 15:59:43.497633 resty_client-0.0.5/resty/clients/types.py
--rw-r--r--   0        0        0      371 2024-04-25 16:23:57.349870 resty_client-0.0.5/resty/constants.py
--rw-r--r--   0        0        0      370 2024-04-22 14:23:32.559298 resty_client-0.0.5/resty/enums.py
--rw-r--r--   0        0        0     1027 2024-04-26 12:14:34.090077 resty_client-0.0.5/resty/exceptions.py
--rw-r--r--   0        0        0      251 2024-04-26 12:21:28.058775 resty_client-0.0.5/resty/managers/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-26 12:52:01.561816 resty_client-0.0.5/resty/managers/builders.py
--rw-r--r--   0        0        0     7181 2024-04-26 15:18:16.950582 resty_client-0.0.5/resty/managers/managers.py
--rw-r--r--   0        0        0     2837 2024-04-26 14:45:33.821123 resty_client-0.0.5/resty/managers/types.py
--rw-r--r--   0        0        0      460 2024-04-26 09:56:25.334802 resty_client-0.0.5/resty/middlewares/__init__.py
--rw-r--r--   0        0        0     1657 2024-04-25 18:35:38.358135 resty_client-0.0.5/resty/middlewares/managers.py
--rw-r--r--   0        0        0     1374 2024-04-26 19:15:16.618265 resty_client-0.0.5/resty/middlewares/status.py
--rw-r--r--   0        0        0     1250 2024-04-25 16:00:21.928605 resty_client-0.0.5/resty/middlewares/types.py
--rw-r--r--   0        0        0      166 2024-04-26 10:30:15.667616 resty_client-0.0.5/resty/serializers/__init__.py
--rw-r--r--   0        0        0      850 2024-04-26 10:37:30.410789 resty_client-0.0.5/resty/serializers/serializers.py
--rw-r--r--   0        0        0      854 2024-04-26 10:24:34.542849 resty_client-0.0.5/resty/serializers/types.py
--rw-r--r--   0        0        0      829 2024-04-26 14:16:08.475872 resty_client-0.0.5/resty/types.py
--rw-r--r--   0        0        0     4302 1970-01-01 00:00:00.000000 resty_client-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-01-23 13:22:57.074926 resty_client-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1119 2024-04-29 09:02:17.215111 resty_client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3848 2024-04-29 09:02:17.192109 resty_client-0.0.6/README.md
+-rw-r--r--   0        0        0      172 2024-04-26 09:56:00.652385 resty_client-0.0.6/resty/__init__.py
+-rw-r--r--   0        0        0      230 2024-04-29 09:02:17.203113 resty_client-0.0.6/resty/__version__.py
+-rw-r--r--   0        0        0       89 2024-04-25 16:40:33.939395 resty_client-0.0.6/resty/clients/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-25 15:52:51.149933 resty_client-0.0.6/resty/clients/httpx/__init__.py
+-rw-r--r--   0        0        0     3004 2024-04-29 12:23:12.636204 resty_client-0.0.6/resty/clients/httpx/clients.py
+-rw-r--r--   0        0        0      294 2024-04-25 15:59:43.497633 resty_client-0.0.6/resty/clients/types.py
+-rw-r--r--   0        0        0      371 2024-04-25 16:23:57.349870 resty_client-0.0.6/resty/constants.py
+-rw-r--r--   0        0        0      370 2024-04-22 14:23:32.559298 resty_client-0.0.6/resty/enums.py
+-rw-r--r--   0        0        0     1027 2024-04-26 12:14:34.090077 resty_client-0.0.6/resty/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:18:36.519083 resty_client-0.0.6/resty/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:18:40.851573 resty_client-0.0.6/resty/ext/django/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:18:46.962686 resty_client-0.0.6/resty/ext/django/middlewares/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-29 10:04:19.894590 resty_client-0.0.6/resty/ext/django/middlewares/pagination/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-29 10:00:34.116831 resty_client-0.0.6/resty/ext/django/middlewares/pagination/constants.py
+-rw-r--r--   0        0        0     2050 2024-04-29 10:51:23.583862 resty_client-0.0.6/resty/ext/django/middlewares/pagination/middlewares.py
+-rw-r--r--   0        0        0      251 2024-04-26 12:21:28.058775 resty_client-0.0.6/resty/managers/__init__.py
+-rw-r--r--   0        0        0     1342 2024-04-29 08:47:22.452360 resty_client-0.0.6/resty/managers/builders.py
+-rw-r--r--   0        0        0     7551 2024-04-29 10:04:20.033608 resty_client-0.0.6/resty/managers/managers.py
+-rw-r--r--   0        0        0     2499 2024-04-29 08:58:44.810177 resty_client-0.0.6/resty/managers/types.py
+-rw-r--r--   0        0        0      460 2024-04-26 09:56:25.334802 resty_client-0.0.6/resty/middlewares/__init__.py
+-rw-r--r--   0        0        0     1657 2024-04-25 18:35:38.358135 resty_client-0.0.6/resty/middlewares/managers.py
+-rw-r--r--   0        0        0     1362 2024-04-29 08:47:22.476363 resty_client-0.0.6/resty/middlewares/status.py
+-rw-r--r--   0        0        0     1250 2024-04-25 16:00:21.928605 resty_client-0.0.6/resty/middlewares/types.py
+-rw-r--r--   0        0        0      166 2024-04-26 10:30:15.667616 resty_client-0.0.6/resty/serializers/__init__.py
+-rw-r--r--   0        0        0      850 2024-04-26 10:37:30.410789 resty_client-0.0.6/resty/serializers/serializers.py
+-rw-r--r--   0        0        0      854 2024-04-26 10:24:34.542849 resty_client-0.0.6/resty/serializers/types.py
+-rw-r--r--   0        0        0      829 2024-04-26 14:16:08.475872 resty_client-0.0.6/resty/types.py
+-rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 resty_client-0.0.6/PKG-INFO
```

### Comparing `resty_client-0.0.5/LICENSE` & `resty_client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.5/pyproject.toml` & `resty_client-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resty-client"
-version = "0.0.5"
+version = "0.0.6"
 description = "RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data validation and deserialization tools."
 authors = ["CrazyProger1 <crazyproger1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "resty" },
 ]
```

### Comparing `resty_client-0.0.5/README.md` & `resty_client-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -95,57 +95,58 @@
 
 from resty.clients.httpx import RESTClient
 
 
 async def main():
     client = RESTClient(httpx.AsyncClient(base_url="https://localhost:8000"))
 
-    response = await UserManager.create(
-        client=client,
+    manager = UserManager(client=client)
+
+    response = await manager.create(
         obj=UserCreateSchema(
             username="admin",
             email="admin@admin.com",
             password="admin",
             age=19,
         ),
         response_type=UserReadSchema,
     )
     print(response)  # id=1 username='admin' email='admin@admin.com' age=19
 
-    response = await UserManager.read(
-        client=client,
+    response = await manager.read(
         response_type=UserReadSchema,
     )
 
     for obj in response:
         print(obj)  # id=1 username='admin' email='admin@admin.com' age=19
 
-    response = await UserManager.read_one(
-        client=client,
+    response = await manager.read_one(
         obj_or_pk=1,
         response_type=UserReadSchema,
     )
 
     print(response)  # id=1 username='admin' email='admin@admin.com' age=19
 
-    response = await UserManager.update(
-        client=client,
-        obj=UserUpdateSchema(id=1, username="admin123", ),
+    response = await manager.update(
+        obj=UserUpdateSchema(
+            id=1,
+            username="admin123",
+        ),
         response_type=UserReadSchema,
     )
 
     print(response)  # id=1 username='admin123' email='admin@admin.com' age=19
 
-    await UserManager.delete(
-        client=client,
+    await manager.delete(
         obj_or_pk=1,
         expected_status=204,
     )
 
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## Status
 
 ``0.0.5`` - **RELEASED**
```

### Comparing `resty_client-0.0.5/resty/clients/httpx/clients.py` & `resty_client-0.0.6/resty/clients/httpx/clients.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from urllib.parse import urljoin
 
 import httpx
 
 from resty.clients.types import (
     BaseRESTClient,
     Request,
     Response,
@@ -16,18 +17,18 @@
 )
 from resty.exceptions import ConnectError
 
 
 class RESTClient(BaseRESTClient):
 
     def __init__(
-        self,
-        httpx_client: httpx.AsyncClient = None,
-        check_status: bool = True,
-        middleware_manager: BaseMiddlewareManager = None,
+            self,
+            httpx_client: httpx.AsyncClient = None,
+            check_status: bool = True,
+            middleware_manager: BaseMiddlewareManager = None,
     ):
         self.middlewares = middleware_manager or MiddlewareManager()
         self._xclient = httpx_client or httpx.AsyncClient()
 
         if check_status:
             self.middlewares.add_middleware(StatusCheckingMiddleware())
 
@@ -41,27 +42,27 @@
                 data=request.data,
                 params=request.params,
                 cookies=request.cookies,
                 follow_redirects=request.redirects,
                 timeout=request.timeout,
             )
         except httpx.ConnectError:
-            raise ConnectError(url=request.url)
+            raise ConnectError(url=urljoin(str(self._xclient.base_url), request.url))
 
     @staticmethod
     def _extract_json_data(xresponse: httpx.Response) -> dict | list:
         try:
             data = xresponse.json()
         except json.decoder.JSONDecodeError:
             data = {}
 
         return data
 
     async def _parse_xresponse(
-        self, request: Request, xresponse: httpx.Response
+            self, request: Request, xresponse: httpx.Response
     ) -> Response:
         return Response(
             request=request,
             status=xresponse.status_code,
             json=self._extract_json_data(xresponse=xresponse),
             content=xresponse.content,
             text=xresponse.text,
```

### Comparing `resty_client-0.0.5/resty/exceptions.py` & `resty_client-0.0.6/resty/exceptions.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.5/resty/managers/builders.py` & `resty_client-0.0.6/resty/managers/builders.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,27 +21,24 @@
 
     @classmethod
     @cache
     def _normalize_url(cls, url: str | None) -> str:
         if not url:
             return ""
 
-        if not url.endswith('/'):
-            return url + '/'
+        if not url.endswith("/"):
+            return url + "/"
         return url
 
     @classmethod
     def build(
-            cls, endpoints: Endpoints, endpoint: Endpoint, base_url: str = None, **kwargs
+        cls, endpoints: Endpoints, endpoint: Endpoint, base_url: str = None, **kwargs
     ) -> str:
 
         endpoint_url = cls._get_endpoint_url(endpoints=endpoints, endpoint=endpoint)
 
         if endpoint_url:
-            url = urljoin(
-                cls._normalize_url(url=base_url),
-                endpoint_url
-            )
+            url = urljoin(cls._normalize_url(url=base_url), endpoint_url)
         else:
             url = base_url or ""
 
         return cls._inject_params(url=url, **kwargs)
```

### Comparing `resty_client-0.0.5/resty/managers/managers.py` & `resty_client-0.0.6/resty/managers/managers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,187 +1,226 @@
 import inspect
-from typing import Mapping, Iterable, Callable
+from typing import Mapping, Iterable
 
 from resty.clients import BaseRESTClient
 from resty.enums import Endpoint, Method, Field
 from resty.types import Schema, Response, Request
 from resty.serializers import Serializer, BaseSerializer
 from resty.managers.types import BaseManager, ResponseType
 from resty.managers.builders import URLBuilder
 
 
 class Manager(BaseManager):
     serializer_class = Serializer
     url_builder_class = URLBuilder
 
-    @classmethod
-    def get_serializer(cls, **kwargs) -> type[BaseSerializer]:
-        serializer = kwargs.pop('serializer', cls.serializer_class)
+    def __init__(self, client: BaseRESTClient = None):
+        self._client = client
+
+    def get_serializer(self, **kwargs) -> type[BaseSerializer]:
+        serializer = kwargs.pop("serializer", self.serializer_class)
 
         if not serializer:
-            raise RuntimeError('Serializer not specified')
+            raise RuntimeError("Serializer not specified")
 
         if not (
-                isinstance(serializer, BaseSerializer)
-                or inspect.isclass(serializer)
-                and issubclass(serializer, BaseSerializer)
+            isinstance(serializer, BaseSerializer)
+            or inspect.isclass(serializer)
+            and issubclass(serializer, BaseSerializer)
         ):
-            raise RuntimeError('The serializer must be a subclass of BaseSerializer')
+            raise RuntimeError("The serializer must be a subclass of BaseSerializer")
 
         return serializer
 
-    @classmethod
-    def get_method(cls, endpoint: Endpoint, **kwargs) -> Method:
-        method = cls.methods.get(endpoint)
+    def get_method(self, endpoint: Endpoint, **kwargs) -> Method:
+        method = self.methods.get(endpoint)
         if not method:
-            raise RuntimeError(f'Method not specified for endpoint: {endpoint}')
+            raise RuntimeError(f"Method not specified for endpoint: {endpoint}")
 
         return method
 
-    @classmethod
-    def get_field(cls, field: Field) -> str:
-        field = cls.fields.get(field)
+    def get_field(self, field: Field) -> str:
+        field = self.fields.get(field)
 
         if not field:
-            raise RuntimeError(f'Field not specified: {field}')
+            raise RuntimeError(f"Field not specified: {field}")
 
         return field
 
-    @classmethod
-    def get_pk(cls, obj: Schema | Mapping) -> any:
-        field = cls.get_field(Field.PRIMARY)
+    def get_pk(self, obj: Schema | Mapping) -> any:
+        field = self.get_field(Field.PRIMARY)
 
         if isinstance(obj, Mapping):
             return obj.get(field)
 
         return getattr(obj, field, None)
 
-    @classmethod
-    def _get_pk(cls, obj_or_pk: any) -> any:
+    def _get_pk(self, obj_or_pk: any) -> any:
         if isinstance(obj_or_pk, Mapping | Schema):
-            return cls.get_pk(obj=obj_or_pk)
+            return self.get_pk(obj=obj_or_pk)
         return obj_or_pk
 
-    @classmethod
-    def _deserialize(cls, schema: type[Schema], data: any, **kwargs):
-        serializer = cls.get_serializer(**kwargs)
+    def _deserialize(self, schema: type[Schema], data: any, **kwargs):
+        serializer = self.get_serializer(**kwargs)
         if isinstance(data, Mapping):
             return serializer.deserialize(schema=schema, data=data, **kwargs)
         return serializer.deserialize_many(schema=schema, data=data, **kwargs)
 
-    @classmethod
-    def _serialize(cls, obj: Schema, **kwargs):
-        serializer = cls.get_serializer(**kwargs)
+    def _serialize(self, obj: Schema, **kwargs):
+        serializer = self.get_serializer(**kwargs)
         return serializer.serialize(obj=obj, **kwargs)
 
-    @classmethod
-    async def _make_request(cls, client: BaseRESTClient, request: Request) -> Response:
+    def _get_client(self, **kwargs) -> BaseRESTClient:
+        client = kwargs.pop("client", self._client)
+
+        if not client:
+            raise TypeError(
+                "REST Client not specified. Pass it to the constructor or via kwargs"
+            )
+
+        if not isinstance(client, BaseRESTClient):
+            raise TypeError("Client must inherit from BaseRESTClient")
+
+        return client
+
+    async def _make_request(self, request: Request, **kwargs) -> Response:
+        client = self._get_client(**kwargs)
         return await client.request(request=request)
 
-    @classmethod
-    def _prepare_url(cls, endpoint: Endpoint, **kwargs) -> str:
-        url = kwargs.pop('url', None)
-        base_url = kwargs.pop('base_url', None)
+    def _prepare_url(self, endpoint: Endpoint, **kwargs) -> str:
+        url = kwargs.pop("url", None)
+        base_url = kwargs.pop("base_url", None)
 
         if isinstance(url, str):
             return url
 
-        return cls.url_builder_class.build(
-            endpoints=cls.endpoints,
+        return self.url_builder_class.build(
+            endpoints=self.endpoints,
             endpoint=endpoint,
-            base_url=base_url or cls.url,
-            **kwargs
+            base_url=base_url or self.url,
+            **kwargs,
         )
 
-    @classmethod
-    def _prepare_json(cls, **kwargs):
-        obj = kwargs.pop('obj', None)
+    def _prepare_json(self, **kwargs):
+        obj = kwargs.pop("obj", None)
 
         if isinstance(obj, dict | list | set | tuple):
             return obj
         elif isinstance(obj, Schema):
-            return cls._serialize(obj, **kwargs)
+            return self._serialize(obj, **kwargs)
         return {}
 
-    @classmethod
-    def _prepare_request(cls, endpoint: Endpoint, **kwargs) -> Request:
+    def _prepare_request(self, endpoint: Endpoint, **kwargs) -> Request:
         return Request(
-            url=cls._prepare_url(endpoint=endpoint, **kwargs),
-            method=cls.get_method(endpoint, **kwargs),
+            url=self._prepare_url(endpoint=endpoint, **kwargs),
+            method=self.get_method(endpoint, **kwargs),
             endpoint=endpoint,
-            data=kwargs.pop('data', {}),
-            json=cls._prepare_json(**kwargs),
-            timeout=kwargs.pop('timeout', None),
-            params=kwargs.pop('params', {}),
-            headers=kwargs.pop('headers', {}),
-            cookies=kwargs.pop('cookies', {}),
-            redirects=kwargs.pop('redirects', False),
+            data=kwargs.pop("data", {}),
+            json=self._prepare_json(**kwargs),
+            timeout=kwargs.pop("timeout", None),
+            params=kwargs.pop("params", {}),
+            headers=kwargs.pop("headers", {}),
+            cookies=kwargs.pop("cookies", {}),
+            redirects=kwargs.pop("redirects", False),
             middleware_options=kwargs.copy(),
         )
 
-    @classmethod
-    def _handle_response(cls, response: Response, response_type: ResponseType, **kwargs) -> any:
+    def _handle_response(
+        self, response: Response, response_type: ResponseType, **kwargs
+    ) -> any:
         if not response:
             return
 
         if inspect.isclass(response_type):
             if issubclass(response_type, dict | list | tuple | set):
                 return response_type(response.json)
             elif issubclass(response_type, Schema):
-                return cls._deserialize(schema=response_type, data=response.json, **kwargs)
+                return self._deserialize(
+                    schema=response_type, data=response.json, **kwargs
+                )
 
         if callable(response_type):
             try:
                 return response_type(response)
             except TypeError:
                 pass
 
         return response.json
 
-    @classmethod
-    async def create[T: Schema](cls, client: BaseRESTClient, obj: Schema | Mapping, response_type: ResponseType = None,
-                                **kwargs) -> T | None:
-        request = cls._prepare_request(endpoint=Endpoint.CREATE, obj=obj, **kwargs)
-        response = await cls._make_request(client=client, request=request)
-        return cls._handle_response(response=response, response_type=response_type, **kwargs)
-
-    @classmethod
-    async def read[T: Schema](cls, client: BaseRESTClient, response_type: ResponseType = None, **kwargs) -> Iterable[T]:
-        request = cls._prepare_request(endpoint=Endpoint.READ, **kwargs)
-        response = await cls._make_request(client=client, request=request)
-        return cls._handle_response(response=response, response_type=response_type, **kwargs)
-
-    @classmethod
-    async def read_one[T: Schema](cls, client: BaseRESTClient, obj_or_pk: Schema | Mapping | any,
-                                  response_type: ResponseType = None, **kwargs) -> T:
-
-        request = cls._prepare_request(
-            endpoint=Endpoint.READ_ONE,
-            pk=cls._get_pk(obj_or_pk=obj_or_pk),
-            **kwargs
-        )
-        response = await cls._make_request(client=client, request=request)
-        return cls._handle_response(response=response, response_type=response_type, **kwargs)
-
-    @classmethod
-    async def update[T: Schema](cls, client: BaseRESTClient, obj: Schema | Mapping, response_type: ResponseType = None,
-                                **kwargs) -> T | None:
-        request = cls._prepare_request(
+    async def create[
+        T: Schema
+    ](
+        self,
+        obj: Schema | Mapping,
+        response_type: ResponseType = None,
+        **kwargs,
+    ) -> (
+        T | None
+    ):
+        request = self._prepare_request(endpoint=Endpoint.CREATE, obj=obj, **kwargs)
+        response = await self._make_request(request=request, **kwargs)
+        return self._handle_response(
+            response=response, response_type=response_type, **kwargs
+        )
+
+    async def read[
+        T: Schema
+    ](self, response_type: ResponseType = None, **kwargs) -> Iterable[T]:
+        request = self._prepare_request(endpoint=Endpoint.READ, **kwargs)
+        response = await self._make_request(request=request, **kwargs)
+        return self._handle_response(
+            response=response, response_type=response_type, **kwargs
+        )
+
+    async def read_one[
+        T: Schema
+    ](
+        self,
+        obj_or_pk: Schema | Mapping | any,
+        response_type: ResponseType = None,
+        **kwargs,
+    ) -> T:
+
+        request = self._prepare_request(
+            endpoint=Endpoint.READ_ONE, pk=self._get_pk(obj_or_pk=obj_or_pk), **kwargs
+        )
+        response = await self._make_request(request=request, **kwargs)
+        return self._handle_response(
+            response=response, response_type=response_type, **kwargs
+        )
+
+    async def update[
+        T: Schema
+    ](
+        self,
+        obj: Schema | Mapping,
+        response_type: ResponseType = None,
+        **kwargs,
+    ) -> (
+        T | None
+    ):
+        request = self._prepare_request(
             endpoint=Endpoint.UPDATE,
-            pk=kwargs.pop('pk', cls.get_pk(obj)),
+            pk=kwargs.pop("pk", self.get_pk(obj)),
             obj=obj,
-            **kwargs
+            **kwargs,
+        )
+        response = await self._make_request(request=request, **kwargs)
+        return self._handle_response(
+            response=response, response_type=response_type, **kwargs
         )
-        response = await cls._make_request(client=client, request=request)
-        return cls._handle_response(response=response, response_type=response_type, **kwargs)
 
-    @classmethod
-    async def delete[T: Schema](cls, client: BaseRESTClient, obj_or_pk: Schema | Mapping | any,
-                                response_type: ResponseType = None,
-                                **kwargs) -> T | None:
-        request = cls._prepare_request(
-            endpoint=Endpoint.DELETE,
-            pk=cls._get_pk(obj_or_pk=obj_or_pk),
-            **kwargs
+    async def delete[
+        T: Schema
+    ](
+        self,
+        obj_or_pk: Schema | Mapping | any,
+        response_type: ResponseType = None,
+        **kwargs,
+    ) -> (T | None):
+        request = self._prepare_request(
+            endpoint=Endpoint.DELETE, pk=self._get_pk(obj_or_pk=obj_or_pk), **kwargs
+        )
+        response = await self._make_request(request=request, **kwargs)
+        return self._handle_response(
+            response=response, response_type=response_type, **kwargs
         )
-        response = await cls._make_request(client=client, request=request)
-        return cls._handle_response(response=response, response_type=response_type, **kwargs)
```

### Comparing `resty_client-0.0.5/resty/managers/types.py` & `resty_client-0.0.6/resty/managers/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,71 +34,57 @@
         Endpoint.DELETE: Method.DELETE,
     }
     endpoints: Endpoints = {}
     fields: Fields = {}
     serializer_class: BaseSerializer
     url_builder_class: BaseURLBuilder
 
-    @classmethod
     @abstractmethod
-    def get_serializer(cls, **kwargs) -> type[BaseSerializer]: ...
+    def get_serializer(self, **kwargs) -> type[BaseSerializer]: ...
 
-    @classmethod
     @abstractmethod
-    def get_method(cls, endpoint: Endpoint, **kwargs) -> Method: ...
+    def get_method(self, endpoint: Endpoint, **kwargs) -> Method: ...
 
-    @classmethod
     @abstractmethod
-    def get_field(cls, field: Field) -> str: ...
+    def get_field(self, field: Field) -> str: ...
 
-    @classmethod
     @abstractmethod
-    def get_pk(cls, obj: Schema | Mapping) -> any: ...
+    def get_pk(self, obj: Schema | Mapping) -> any: ...
 
-    @classmethod
     @abstractmethod
     async def create[T: Schema](
-            cls,
-            client: BaseRESTClient,
+            self,
             obj: Schema | Mapping,
             response_type: ResponseType = None,
             **kwargs,
     ) -> T | None: ...
 
-    @classmethod
     @abstractmethod
     async def read[T: Schema](
-            cls,
-            client: BaseRESTClient,
+            self,
             response_type: ResponseType = None,
             **kwargs,
     ) -> Iterable[T]: ...
 
-    @classmethod
     @abstractmethod
     async def read_one[T: Schema](
-            cls,
-            client: BaseRESTClient,
+            self,
             obj_or_pk: Schema | Mapping | any,
             response_type: ResponseType = None,
             **kwargs,
     ) -> T: ...
 
-    @classmethod
     @abstractmethod
     async def update[T: Schema](
-            cls,
-            client: BaseRESTClient,
+            self,
             obj: Schema | Mapping,
             response_type: ResponseType = None,
             **kwargs,
     ) -> T | None: ...
 
-    @classmethod
     @abstractmethod
     async def delete[T: Schema](
-            cls,
-            client: BaseRESTClient,
+            self,
             obj_or_pk: Schema | Mapping | any,
             response_type: ResponseType = None,
             **kwargs,
     ) -> T | None: ...
```

### Comparing `resty_client-0.0.5/resty/middlewares/managers.py` & `resty_client-0.0.6/resty/middlewares/managers.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.5/resty/middlewares/status.py` & `resty_client-0.0.6/resty/middlewares/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from resty.types import Response
 from resty.constants import STATUS_ERRORS
 from resty.exceptions import HTTPError
 
 
 class StatusCheckingMiddleware(BaseResponseMiddleware):
     def __init__(
-            self,
-            errors: Mapping[int, type[Exception]] = None,
-            default_error: type[Exception] = HTTPError,
+        self,
+        errors: Mapping[int, type[Exception]] = None,
+        default_error: type[Exception] = HTTPError,
     ):
         self._errors = errors or STATUS_ERRORS
         self._default_error = default_error
 
     @staticmethod
     def _check_status(actual: int, expected: int | Container[int] = 200) -> bool:
         if isinstance(expected, Container):
```

### Comparing `resty_client-0.0.5/resty/middlewares/types.py` & `resty_client-0.0.6/resty/middlewares/types.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.5/resty/serializers/serializers.py` & `resty_client-0.0.6/resty/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.5/resty/serializers/types.py` & `resty_client-0.0.6/resty/serializers/types.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.5/resty/types.py` & `resty_client-0.0.6/resty/types.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.5/PKG-INFO` & `resty_client-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resty-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data validation and deserialization tools.
 License: MIT
 Author: CrazyProger1
 Author-email: crazyproger1@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -109,57 +109,58 @@
 
 from resty.clients.httpx import RESTClient
 
 
 async def main():
     client = RESTClient(httpx.AsyncClient(base_url="https://localhost:8000"))
 
-    response = await UserManager.create(
-        client=client,
+    manager = UserManager(client=client)
+
+    response = await manager.create(
         obj=UserCreateSchema(
             username="admin",
             email="admin@admin.com",
             password="admin",
             age=19,
         ),
         response_type=UserReadSchema,
     )
     print(response)  # id=1 username='admin' email='admin@admin.com' age=19
 
-    response = await UserManager.read(
-        client=client,
+    response = await manager.read(
         response_type=UserReadSchema,
     )
 
     for obj in response:
         print(obj)  # id=1 username='admin' email='admin@admin.com' age=19
 
-    response = await UserManager.read_one(
-        client=client,
+    response = await manager.read_one(
         obj_or_pk=1,
         response_type=UserReadSchema,
     )
 
     print(response)  # id=1 username='admin' email='admin@admin.com' age=19
 
-    response = await UserManager.update(
-        client=client,
-        obj=UserUpdateSchema(id=1, username="admin123", ),
+    response = await manager.update(
+        obj=UserUpdateSchema(
+            id=1,
+            username="admin123",
+        ),
         response_type=UserReadSchema,
     )
 
     print(response)  # id=1 username='admin123' email='admin@admin.com' age=19
 
-    await UserManager.delete(
-        client=client,
+    await manager.delete(
         obj_or_pk=1,
         expected_status=204,
     )
 
 
+
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## Status
 
 ``0.0.5`` - **RELEASED**
```

