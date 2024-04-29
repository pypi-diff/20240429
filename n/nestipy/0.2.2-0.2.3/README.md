# Comparing `tmp/nestipy-0.2.2.tar.gz` & `tmp/nestipy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.2.2.tar", max compression
+gzip compressed data, was "nestipy-0.2.3.tar", max compression
```

## Comparing `nestipy-0.2.2.tar` & `nestipy-0.2.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.2.2/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy-0.2.2/README.md
--rw-r--r--   0        0        0      767 2024-04-29 10:02:35.395943 nestipy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.2.2/src/nestipy/__init__.py
--rw-r--r--   0        0        0     1151 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-27 15:32:43.416679 nestipy-0.2.2/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.2.2/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0      978 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/config/__init__.py
--rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     2957 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/decorator/class_.py
--rw-r--r--   0        0        0     1204 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/decorator/method.py
--rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/exception/__init__.py
--rw-r--r--   0        0        0      732 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/exception/decorator.py
--rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/exception/http.py
--rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/exception/interface.py
--rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/exception/message.py
--rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/exception/meta.py
--rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/exception/status.py
--rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/guards/__init__.py
--rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/guards/can_activate.py
--rw-r--r--   0        0        0      332 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/guards/decorator.py
--rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/guards/meta.py
--rw-r--r--   0        0        0      719 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/helpers/__init__.py
--rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/http_/__init__.py
--rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/http_/multipart.py
--rw-r--r--   0        0        0     4231 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/http_/request.py
--rw-r--r--   0        0        0     4989 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/http_/response.py
--rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/http_/test.py
--rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/http_/upload_file.py
--rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/http_/websocket.py
--rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/interceptor/__init__.py
--rw-r--r--   0        0        0      489 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/interceptor/decorator.py
--rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/interceptor/interface.py
--rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/interceptor/meta.py
--rw-r--r--   0        0        0      168 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/middleware/__init__.py
--rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/middleware/cors.py
--rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/middleware/interface.py
--rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/middleware/meta.py
--rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/template/__init__.py
--rw-r--r--   0        0        0      274 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/template/decorator.py
--rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/template/interface.py
--rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/template/meta.py
--rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/common/utils.py
--rw-r--r--   0        0        0      882 2024-04-27 15:32:43.416679 nestipy-0.2.2/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-29 10:02:54.487800 nestipy-0.2.2/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.2.2/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.2.2/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.2.2/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/adapter/__init__.py
--rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/adapter/blacksheep_adapter.py
--rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/adapter/fastapi_adapter.py
--rw-r--r--   0        0        0     5666 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/adapter/http_adapter.py
--rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/constant.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/context/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/context/argument_host.py
--rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/context/execution_context.py
--rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/context/http_argument_host.py
--rw-r--r--   0        0        0      730 2024-04-27 15:32:43.416679 nestipy-0.2.2/src/nestipy/core/discover.py
--rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/exception/__init__.py
--rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.156372 nestipy-0.2.2/src/nestipy/core/exception/processor.py
--rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/guards/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/guards/processor.py
--rw-r--r--   0        0        0     3739 2024-04-27 15:32:43.416679 nestipy-0.2.2/src/nestipy/core/instance_loader.py
--rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/interceptor/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/interceptor/processor.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/meta/__init__.py
--rw-r--r--   0        0        0      380 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/meta/controller_metadata_creator.py
--rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/meta/metadata_creator.py
--rw-r--r--   0        0        0      771 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/meta/module_metadata_creator.py
--rw-r--r--   0        0        0      374 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/meta/provider_metadata_creator.py
--rw-r--r--   0        0        0      162 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/middleware/__init__.py
--rw-r--r--   0        0        0     3949 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/middleware/executor.py
--rw-r--r--   0        0        0     8889 2024-04-27 15:32:43.416679 nestipy-0.2.2/src/nestipy/core/nestipy_application.py
--rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/nestipy_factory.py
--rw-r--r--   0        0        0      107 2024-04-27 15:32:43.416679 nestipy-0.2.2/src/nestipy/core/on_init.py
--rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      608 2024-04-27 15:32:43.416679 nestipy-0.2.2/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.2.2/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.2.2/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.2.2/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/router/__init__.py
--rw-r--r--   0        0        0     2879 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/router/route_explorer.py
--rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/router/route_extractor.py
--rw-r--r--   0        0        0     7920 2024-04-27 15:32:43.416679 nestipy-0.2.2/src/nestipy/core/router/router_proxy.py
--rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/template/__init__.py
--rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/template/minimal_jinja.py
--rw-r--r--   0        0        0     1457 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/core/template/processor.py
--rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/__init__.py
--rw-r--r--   0        0        0     1533 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/decorator.py
--rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/graphql_adapter.py
--rw-r--r--   0        0        0     1111 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/graphql_asgi.py
--rw-r--r--   0        0        0     1871 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/graphql_explorer.py
--rw-r--r--   0        0        0      547 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/graphql_module.py
--rw-r--r--   0        0        0     4326 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/graphql_proxy.py
--rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/meta.py
--rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/playground/graphql-playground-default.html
--rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/playground/graphql-playground-graphiql.html
--rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/pubsub.py
--rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/strawberry/__init__.py
--rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/strawberry/strawberry_adapter.py
--rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/strawberry/strawberry_asgi.py
--rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/graphql/test.py
--rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/openapi/__init__.py
--rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/openapi/constant.py
--rw-r--r--   0        0        0     3139 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/openapi/decorator.py
--rw-r--r--   0        0        0     1500 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/openapi/document_builder.py
--rw-r--r--   0        0        0      423 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/openapi/explorer.py
--rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/openapi/swagger.html
--rw-r--r--   0        0        0     2195 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/openapi/swagger_module.py
--rw-r--r--   0        0        0     2728 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/openapi/test.py
--rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/types_/__init__.py
--rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/types_/handler.py
--rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/types_/http.py
--rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/websocket/__init__.py
--rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/websocket/adapter.py
--rw-r--r--   0        0        0      716 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/websocket/decorator.py
--rw-r--r--   0        0        0     4517 2024-04-26 12:17:55.160372 nestipy-0.2.2/src/nestipy/websocket/proxy.py
--rw-r--r--   0        0        0     2995 1970-01-01 00:00:00.000000 nestipy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy-0.2.3/README.md
+-rw-r--r--   0        0        0      767 2024-04-29 10:30:25.394933 nestipy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.2.3/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1151 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-27 15:32:43.416679 nestipy-0.2.3/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.2.3/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0      978 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      719 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     4231 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     4989 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0      168 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      882 2024-04-27 15:32:43.416679 nestipy-0.2.3/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-29 10:02:54.487800 nestipy-0.2.3/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.2.3/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.2.3/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.2.3/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0      730 2024-04-27 15:32:43.416679 nestipy-0.2.3/src/nestipy/core/discover.py
+-rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.156372 nestipy-0.2.3/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     3739 2024-04-27 15:32:43.416679 nestipy-0.2.3/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3949 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     8889 2024-04-27 15:32:43.416679 nestipy-0.2.3/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0      107 2024-04-27 15:32:43.416679 nestipy-0.2.3/src/nestipy/core/on_init.py
+-rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-27 15:32:43.416679 nestipy-0.2.3/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.2.3/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.2.3/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.2.3/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     2879 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     7920 2024-04-27 15:32:43.416679 nestipy-0.2.3/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1111 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      547 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4326 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     3139 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1500 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      423 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2195 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     2728 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4517 2024-04-26 12:17:55.160372 nestipy-0.2.3/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0     2995 1970-01-01 00:00:00.000000 nestipy-0.2.3/PKG-INFO
```

### Comparing `nestipy-0.2.2/LICENSE` & `nestipy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/README.md` & `nestipy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/pyproject.toml` & `nestipy-0.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.2.2"
+version = "0.2.3"
 description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-minijinja = "^1.0.8"
 pyee = "^11.1.0"
 snakecase = "^1.0.1"
 python-socketio = "^5.11.1"
 blacksheep = "^2.0.7"
 aiofiles = "^23.2.1"
 fastapi = "^0.110.0"
 uvicorn = { extras = ["standard"], version = "^0.29.0" }
 strawberry-graphql = "^0.225.0"
 ujson = "^5.9.0"
 nestipy-ioc = "^0.1.30"
 nestipy-metadata = "^0.1.1"
 nestipy-dynamic-module = "^0.1.3"
+minijinja = "^2.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nestipy-0.2.2/src/nestipy/common/__init__.py` & `nestipy-0.2.3/src/nestipy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/common/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/config/__init__.py` & `nestipy-0.2.3/src/nestipy/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/decorator/class_.py` & `nestipy-0.2.3/src/nestipy/common/decorator/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/decorator/method.py` & `nestipy-0.2.3/src/nestipy/common/decorator/method.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/exception/decorator.py` & `nestipy-0.2.3/src/nestipy/common/exception/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/exception/message.py` & `nestipy-0.2.3/src/nestipy/common/exception/message.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/exception/status.py` & `nestipy-0.2.3/src/nestipy/common/exception/status.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/helpers/__init__.py` & `nestipy-0.2.3/src/nestipy/common/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/http_/multipart.py` & `nestipy-0.2.3/src/nestipy/common/http_/multipart.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/http_/request.py` & `nestipy-0.2.3/src/nestipy/common/http_/request.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/http_/response.py` & `nestipy-0.2.3/src/nestipy/common/http_/response.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/http_/upload_file.py` & `nestipy-0.2.3/src/nestipy/common/http_/upload_file.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/middleware/cors.py` & `nestipy-0.2.3/src/nestipy/common/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/template/interface.py` & `nestipy-0.2.3/src/nestipy/common/template/interface.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/common/utils.py` & `nestipy-0.2.3/src/nestipy/common/utils.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/__init__.py` & `nestipy-0.2.3/src/nestipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/core/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/adapter/blacksheep_adapter.py` & `nestipy-0.2.3/src/nestipy/core/adapter/blacksheep_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/adapter/fastapi_adapter.py` & `nestipy-0.2.3/src/nestipy/core/adapter/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/adapter/http_adapter.py` & `nestipy-0.2.3/src/nestipy/core/adapter/http_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/context/argument_host.py` & `nestipy-0.2.3/src/nestipy/core/context/argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/context/execution_context.py` & `nestipy-0.2.3/src/nestipy/core/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/discover.py` & `nestipy-0.2.3/src/nestipy/core/discover.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/exception/processor.py` & `nestipy-0.2.3/src/nestipy/core/exception/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/guards/processor.py` & `nestipy-0.2.3/src/nestipy/core/guards/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/instance_loader.py` & `nestipy-0.2.3/src/nestipy/core/instance_loader.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/interceptor/processor.py` & `nestipy-0.2.3/src/nestipy/core/interceptor/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/meta/metadata_creator.py` & `nestipy-0.2.3/src/nestipy/core/meta/metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/meta/module_metadata_creator.py` & `nestipy-0.2.3/src/nestipy/core/meta/module_metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/middleware/executor.py` & `nestipy-0.2.3/src/nestipy/core/middleware/executor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/nestipy_application.py` & `nestipy-0.2.3/src/nestipy/core/nestipy_application.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/nestipy_factory.py` & `nestipy-0.2.3/src/nestipy/core/nestipy_factory.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.2.3/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/router/route_explorer.py` & `nestipy-0.2.3/src/nestipy/core/router/route_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/router/router_proxy.py` & `nestipy-0.2.3/src/nestipy/core/router/router_proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/template/minimal_jinja.py` & `nestipy-0.2.3/src/nestipy/core/template/minimal_jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/core/template/processor.py` & `nestipy-0.2.3/src/nestipy/core/template/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/decorator.py` & `nestipy-0.2.3/src/nestipy/graphql/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/graphql_adapter.py` & `nestipy-0.2.3/src/nestipy/graphql/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/graphql_asgi.py` & `nestipy-0.2.3/src/nestipy/graphql/graphql_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/graphql_explorer.py` & `nestipy-0.2.3/src/nestipy/graphql/graphql_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/graphql_module.py` & `nestipy-0.2.3/src/nestipy/graphql/graphql_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/graphql_proxy.py` & `nestipy-0.2.3/src/nestipy/graphql/graphql_proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/playground/graphql-playground-default.html` & `nestipy-0.2.3/src/nestipy/graphql/playground/graphql-playground-default.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/playground/graphql-playground-graphiql.html` & `nestipy-0.2.3/src/nestipy/graphql/playground/graphql-playground-graphiql.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/pubsub.py` & `nestipy-0.2.3/src/nestipy/graphql/pubsub.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/strawberry/__init__.py` & `nestipy-0.2.3/src/nestipy/graphql/strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/strawberry/strawberry_adapter.py` & `nestipy-0.2.3/src/nestipy/graphql/strawberry/strawberry_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/graphql/strawberry/strawberry_asgi.py` & `nestipy-0.2.3/src/nestipy/graphql/strawberry/strawberry_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/openapi/__init__.py` & `nestipy-0.2.3/src/nestipy/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/openapi/decorator.py` & `nestipy-0.2.3/src/nestipy/openapi/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/openapi/document_builder.py` & `nestipy-0.2.3/src/nestipy/openapi/document_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/openapi/swagger.html` & `nestipy-0.2.3/src/nestipy/openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/openapi/swagger_module.py` & `nestipy-0.2.3/src/nestipy/openapi/swagger_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/openapi/test.py` & `nestipy-0.2.3/src/nestipy/openapi/test.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/websocket/adapter.py` & `nestipy-0.2.3/src/nestipy/websocket/adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/websocket/decorator.py` & `nestipy-0.2.3/src/nestipy/websocket/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/src/nestipy/websocket/proxy.py` & `nestipy-0.2.3/src/nestipy/websocket/proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.2/PKG-INFO` & `nestipy-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
-Requires-Dist: minijinja (>=1.0.8,<2.0.0)
+Requires-Dist: minijinja (>=2.0.1,<3.0.0)
 Requires-Dist: nestipy-dynamic-module (>=0.1.3,<0.2.0)
 Requires-Dist: nestipy-ioc (>=0.1.30,<0.2.0)
 Requires-Dist: nestipy-metadata (>=0.1.1,<0.2.0)
 Requires-Dist: pyee (>=11.1.0,<12.0.0)
 Requires-Dist: python-socketio (>=5.11.1,<6.0.0)
 Requires-Dist: snakecase (>=1.0.1,<2.0.0)
 Requires-Dist: strawberry-graphql (>=0.225.0,<0.226.0)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.2.2 Summary: Nestipy is a Python
+Metadata-Version: 2.1 Name: nestipy Version: 0.2.3 Summary: Nestipy is a Python
 framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: minijinja
-(>=1.0.8,<2.0.0) Requires-Dist: nestipy-dynamic-module (>=0.1.3,<0.2.0)
+(>=2.0.1,<3.0.0) Requires-Dist: nestipy-dynamic-module (>=0.1.3,<0.2.0)
 Requires-Dist: nestipy-ioc (>=0.1.30,<0.2.0) Requires-Dist: nestipy-metadata
 (>=0.1.1,<0.2.0) Requires-Dist: pyee (>=11.1.0,<12.0.0) Requires-Dist: python-
 socketio (>=5.11.1,<6.0.0) Requires-Dist: snakecase (>=1.0.1,<2.0.0) Requires-
 Dist: strawberry-graphql (>=0.225.0,<0.226.0) Requires-Dist: ujson
 (>=5.9.0,<6.0.0) Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
                                 [Nestipy Logo]
```

