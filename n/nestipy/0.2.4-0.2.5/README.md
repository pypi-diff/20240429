# Comparing `tmp/nestipy-0.2.4.tar.gz` & `tmp/nestipy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.2.4.tar", max compression
+gzip compressed data, was "nestipy-0.2.5.tar", max compression
```

## Comparing `nestipy-0.2.4.tar` & `nestipy-0.2.5.tar`

### file list

```diff
@@ -1,118 +1,119 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.2.4/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy-0.2.4/README.md
--rw-r--r--   0        0        0      767 2024-04-29 10:54:11.896554 nestipy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.2.4/src/nestipy/__init__.py
--rw-r--r--   0        0        0     1151 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-27 15:32:43.416679 nestipy-0.2.4/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.2.4/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0      978 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/config/__init__.py
--rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     2957 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/decorator/class_.py
--rw-r--r--   0        0        0     1204 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/decorator/method.py
--rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/exception/__init__.py
--rw-r--r--   0        0        0      732 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/exception/decorator.py
--rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/exception/http.py
--rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/exception/interface.py
--rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/exception/message.py
--rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/exception/meta.py
--rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/exception/status.py
--rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/guards/__init__.py
--rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/guards/can_activate.py
--rw-r--r--   0        0        0      332 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/guards/decorator.py
--rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/guards/meta.py
--rw-r--r--   0        0        0      719 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/helpers/__init__.py
--rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/http_/__init__.py
--rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/http_/multipart.py
--rw-r--r--   0        0        0     4231 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/http_/request.py
--rw-r--r--   0        0        0     4989 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/http_/response.py
--rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/http_/test.py
--rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/http_/upload_file.py
--rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/http_/websocket.py
--rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/interceptor/__init__.py
--rw-r--r--   0        0        0      489 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/interceptor/decorator.py
--rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/interceptor/interface.py
--rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/interceptor/meta.py
--rw-r--r--   0        0        0      168 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/middleware/__init__.py
--rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/middleware/cors.py
--rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/middleware/interface.py
--rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/middleware/meta.py
--rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/template/__init__.py
--rw-r--r--   0        0        0      274 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/template/decorator.py
--rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/template/interface.py
--rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/template/meta.py
--rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/common/utils.py
--rw-r--r--   0        0        0      882 2024-04-27 15:32:43.416679 nestipy-0.2.4/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-29 10:02:54.487800 nestipy-0.2.4/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.2.4/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.2.4/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.2.4/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/adapter/__init__.py
--rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/adapter/blacksheep_adapter.py
--rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/adapter/fastapi_adapter.py
--rw-r--r--   0        0        0     5666 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/adapter/http_adapter.py
--rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/constant.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/context/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/context/argument_host.py
--rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/context/execution_context.py
--rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/context/http_argument_host.py
--rw-r--r--   0        0        0      730 2024-04-27 15:32:43.416679 nestipy-0.2.4/src/nestipy/core/discover.py
--rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/exception/__init__.py
--rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.156372 nestipy-0.2.4/src/nestipy/core/exception/processor.py
--rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/guards/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/guards/processor.py
--rw-r--r--   0        0        0     3739 2024-04-27 15:32:43.416679 nestipy-0.2.4/src/nestipy/core/instance_loader.py
--rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/interceptor/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/interceptor/processor.py
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/meta/__init__.py
--rw-r--r--   0        0        0      380 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/meta/controller_metadata_creator.py
--rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/meta/metadata_creator.py
--rw-r--r--   0        0        0      771 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/meta/module_metadata_creator.py
--rw-r--r--   0        0        0      374 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/meta/provider_metadata_creator.py
--rw-r--r--   0        0        0      162 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/middleware/__init__.py
--rw-r--r--   0        0        0     3949 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/middleware/executor.py
--rw-r--r--   0        0        0     8889 2024-04-27 15:32:43.416679 nestipy-0.2.4/src/nestipy/core/nestipy_application.py
--rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/nestipy_factory.py
--rw-r--r--   0        0        0      107 2024-04-27 15:32:43.416679 nestipy-0.2.4/src/nestipy/core/on_init.py
--rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      608 2024-04-27 15:32:43.416679 nestipy-0.2.4/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.2.4/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.2.4/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.2.4/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/router/__init__.py
--rw-r--r--   0        0        0     2879 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/router/route_explorer.py
--rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/router/route_extractor.py
--rw-r--r--   0        0        0     7920 2024-04-27 15:32:43.416679 nestipy-0.2.4/src/nestipy/core/router/router_proxy.py
--rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/template/__init__.py
--rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/template/minimal_jinja.py
--rw-r--r--   0        0        0     1457 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/core/template/processor.py
--rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/__init__.py
--rw-r--r--   0        0        0     1533 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/decorator.py
--rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/graphql_adapter.py
--rw-r--r--   0        0        0     1111 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/graphql_asgi.py
--rw-r--r--   0        0        0     1871 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/graphql_explorer.py
--rw-r--r--   0        0        0      547 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/graphql_module.py
--rw-r--r--   0        0        0     4326 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/graphql_proxy.py
--rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/meta.py
--rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/playground/graphql-playground-default.html
--rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/playground/graphql-playground-graphiql.html
--rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/pubsub.py
--rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/strawberry/__init__.py
--rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/strawberry/strawberry_adapter.py
--rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/strawberry/strawberry_asgi.py
--rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/graphql/test.py
--rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/openapi/__init__.py
--rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/openapi/constant.py
--rw-r--r--   0        0        0     3139 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/openapi/decorator.py
--rw-r--r--   0        0        0     1500 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/openapi/document_builder.py
--rw-r--r--   0        0        0      423 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/openapi/explorer.py
--rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/openapi/swagger.html
--rw-r--r--   0        0        0     2195 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/openapi/swagger_module.py
--rw-r--r--   0        0        0     2728 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/openapi/test.py
--rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/types_/__init__.py
--rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/types_/handler.py
--rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/types_/http.py
--rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/websocket/__init__.py
--rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/websocket/adapter.py
--rw-r--r--   0        0        0      716 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/websocket/decorator.py
--rw-r--r--   0        0        0     4517 2024-04-26 12:17:55.160372 nestipy-0.2.4/src/nestipy/websocket/proxy.py
--rw-r--r--   0        0        0     2995 1970-01-01 00:00:00.000000 nestipy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy-0.2.5/README.md
+-rw-r--r--   0        0        0      767 2024-04-29 11:25:59.911384 nestipy-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-29 12:35:05.153461 nestipy-0.2.5/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1151 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-27 15:32:43.416679 nestipy-0.2.5/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-03-29 11:21:44.572810 nestipy-0.2.5/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0      978 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      719 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4503 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     4231 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     4989 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1403 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0      168 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0      167 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      933 2024-04-29 11:25:01.889396 nestipy-0.2.5/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-29 10:02:54.487800 nestipy-0.2.5/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-03-29 11:21:44.576810 nestipy-0.2.5/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-03-29 11:21:44.576810 nestipy-0.2.5/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-03-29 11:21:44.576810 nestipy-0.2.5/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0      802 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      369 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0      730 2024-04-27 15:32:43.416679 nestipy-0.2.5/src/nestipy/core/discover.py
+-rw-r--r--   0        0        0       90 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.156372 nestipy-0.2.5/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     3777 2024-04-29 11:25:27.712482 nestipy-0.2.5/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3949 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     8889 2024-04-27 15:32:43.416679 nestipy-0.2.5/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0      913 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0       64 2024-04-29 11:24:26.410705 nestipy-0.2.5/src/nestipy/core/on_destroy.py
+-rw-r--r--   0        0        0       60 2024-04-29 11:24:33.962421 nestipy-0.2.5/src/nestipy/core/on_init.py
+-rw-r--r--   0        0        0       89 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-27 15:32:43.416679 nestipy-0.2.5/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-03-29 11:21:44.576810 nestipy-0.2.5/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-03-29 11:21:44.576810 nestipy-0.2.5/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-03-29 11:21:44.576810 nestipy-0.2.5/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     2879 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     7920 2024-04-27 15:32:43.416679 nestipy-0.2.5/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      282 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1111 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      547 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4326 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0     1105 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     3139 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1500 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      423 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0     1323 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2195 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     2728 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      254 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     2988 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4517 2024-04-26 12:17:55.160372 nestipy-0.2.5/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0     2995 1970-01-01 00:00:00.000000 nestipy-0.2.5/PKG-INFO
```

### Comparing `nestipy-0.2.4/LICENSE` & `nestipy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/README.md` & `nestipy-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/pyproject.toml` & `nestipy-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.2.4"
+version = "0.2.5"
 description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nestipy-0.2.4/src/nestipy/common/__init__.py` & `nestipy-0.2.5/src/nestipy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/common/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/config/__init__.py` & `nestipy-0.2.5/src/nestipy/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/decorator/class_.py` & `nestipy-0.2.5/src/nestipy/common/decorator/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/decorator/method.py` & `nestipy-0.2.5/src/nestipy/common/decorator/method.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/exception/decorator.py` & `nestipy-0.2.5/src/nestipy/common/exception/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/exception/message.py` & `nestipy-0.2.5/src/nestipy/common/exception/message.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/exception/status.py` & `nestipy-0.2.5/src/nestipy/common/exception/status.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/helpers/__init__.py` & `nestipy-0.2.5/src/nestipy/common/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/http_/multipart.py` & `nestipy-0.2.5/src/nestipy/common/http_/multipart.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/http_/request.py` & `nestipy-0.2.5/src/nestipy/common/http_/request.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/http_/response.py` & `nestipy-0.2.5/src/nestipy/common/http_/response.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/http_/upload_file.py` & `nestipy-0.2.5/src/nestipy/common/http_/upload_file.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/middleware/cors.py` & `nestipy-0.2.5/src/nestipy/common/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/template/interface.py` & `nestipy-0.2.5/src/nestipy/common/template/interface.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/common/utils.py` & `nestipy-0.2.5/src/nestipy/common/utils.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/__init__.py` & `nestipy-0.2.5/src/nestipy/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .constant import AppKey
 from .context.execution_context import ExecutionContext, ArgumentHost, HttpArgumentHost
 from .discover import DiscoverService
 from .middleware import MiddlewareConsumer
 from .nestipy_application import NestipyApplication, NestipyApplicationConfig
 from .nestipy_factory import NestipyFactory
 from .on_init import OnInit
+from .on_destroy import OnDestroy
 from .platform import NestipyFastApiApplication, NestipyBlackSheepApplication
 from .template import MinimalJinjaTemplateEngine
 
 __all__ = [
     "NestipyFactory",
     "NestipyApplication",
     "NestipyApplicationConfig",
@@ -19,9 +20,10 @@
     "HttpArgumentHost",
     "NestipyFastApiApplication",
     "NestipyBlackSheepApplication",
     "MinimalJinjaTemplateEngine",
     "AppKey",
     "MiddlewareConsumer",
     "DiscoverService",
-    "OnInit"
+    "OnInit",
+    "OnDestroy"
 ]
```

### Comparing `nestipy-0.2.4/src/nestipy/core/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/core/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/adapter/blacksheep_adapter.py` & `nestipy-0.2.5/src/nestipy/core/adapter/blacksheep_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/adapter/fastapi_adapter.py` & `nestipy-0.2.5/src/nestipy/core/adapter/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/adapter/http_adapter.py` & `nestipy-0.2.5/src/nestipy/core/adapter/http_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/context/argument_host.py` & `nestipy-0.2.5/src/nestipy/core/context/argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/context/execution_context.py` & `nestipy-0.2.5/src/nestipy/core/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/discover.py` & `nestipy-0.2.5/src/nestipy/core/discover.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/exception/processor.py` & `nestipy-0.2.5/src/nestipy/core/exception/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/guards/processor.py` & `nestipy-0.2.5/src/nestipy/core/guards/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/instance_loader.py` & `nestipy-0.2.5/src/nestipy/core/instance_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Type, Any
 
 from nestipy_dynamic_module import DynamicModule, MiddlewareConsumer, NestipyModule
 from nestipy_ioc import NestipyContainer, ModuleProviderDict
 from nestipy_metadata import ModuleMetadata, Reflect
 
 from .discover import DiscoverService
+from .on_destroy import OnDestroy
 from .on_init import OnInit
 from ..graphql.graphql_module import GraphqlModule
 
 
 class InstanceType(enum.Enum):
     providers: str = 'Provider'
     controller: str = 'Controller',
@@ -72,24 +73,24 @@
     @classmethod
     async def initialize_instance(cls, class_ref: Type, instance: Any) -> None:
         # call configure for module
         if issubclass(class_ref, NestipyModule):
             consumer = MiddlewareConsumer(module=class_ref)
             module = typing.cast(NestipyModule, instance)
             module.configure(consumer)
-            # await module.on_startup()
+            await module.on_startup()
         elif issubclass(class_ref, OnInit):
             ins = typing.cast(OnInit, instance)
             await ins.on_startup()
 
     async def destroy(self):
         for module in self.discover.get_all_module():
             if isinstance(module, NestipyModule):
                 await module.on_shutdown()
 
         for provider in self.discover.get_all_provider():
-            if isinstance(provider, OnInit):
+            if isinstance(provider, OnDestroy):
                 await provider.on_shutdown()
 
         for controller in self.discover.get_all_controller():
-            if isinstance(controller, OnInit):
+            if isinstance(controller, OnDestroy):
                 await controller.on_shutdown()
```

### Comparing `nestipy-0.2.4/src/nestipy/core/interceptor/processor.py` & `nestipy-0.2.5/src/nestipy/core/interceptor/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/meta/metadata_creator.py` & `nestipy-0.2.5/src/nestipy/core/meta/metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/meta/module_metadata_creator.py` & `nestipy-0.2.5/src/nestipy/core/meta/module_metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/middleware/executor.py` & `nestipy-0.2.5/src/nestipy/core/middleware/executor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/nestipy_application.py` & `nestipy-0.2.5/src/nestipy/core/nestipy_application.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/nestipy_factory.py` & `nestipy-0.2.5/src/nestipy/core/nestipy_factory.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.2.5/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/router/route_explorer.py` & `nestipy-0.2.5/src/nestipy/core/router/route_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/router/router_proxy.py` & `nestipy-0.2.5/src/nestipy/core/router/router_proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/template/minimal_jinja.py` & `nestipy-0.2.5/src/nestipy/core/template/minimal_jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/core/template/processor.py` & `nestipy-0.2.5/src/nestipy/core/template/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/decorator.py` & `nestipy-0.2.5/src/nestipy/graphql/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/graphql_adapter.py` & `nestipy-0.2.5/src/nestipy/graphql/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/graphql_asgi.py` & `nestipy-0.2.5/src/nestipy/graphql/graphql_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/graphql_explorer.py` & `nestipy-0.2.5/src/nestipy/graphql/graphql_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/graphql_module.py` & `nestipy-0.2.5/src/nestipy/graphql/graphql_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/graphql_proxy.py` & `nestipy-0.2.5/src/nestipy/graphql/graphql_proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/playground/graphql-playground-default.html` & `nestipy-0.2.5/src/nestipy/graphql/playground/graphql-playground-default.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/playground/graphql-playground-graphiql.html` & `nestipy-0.2.5/src/nestipy/graphql/playground/graphql-playground-graphiql.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/pubsub.py` & `nestipy-0.2.5/src/nestipy/graphql/pubsub.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/strawberry/__init__.py` & `nestipy-0.2.5/src/nestipy/graphql/strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/strawberry/strawberry_adapter.py` & `nestipy-0.2.5/src/nestipy/graphql/strawberry/strawberry_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/graphql/strawberry/strawberry_asgi.py` & `nestipy-0.2.5/src/nestipy/graphql/strawberry/strawberry_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/openapi/__init__.py` & `nestipy-0.2.5/src/nestipy/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/openapi/decorator.py` & `nestipy-0.2.5/src/nestipy/openapi/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/openapi/document_builder.py` & `nestipy-0.2.5/src/nestipy/openapi/document_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/openapi/swagger.html` & `nestipy-0.2.5/src/nestipy/openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/openapi/swagger_module.py` & `nestipy-0.2.5/src/nestipy/openapi/swagger_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/openapi/test.py` & `nestipy-0.2.5/src/nestipy/openapi/test.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/websocket/adapter.py` & `nestipy-0.2.5/src/nestipy/websocket/adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/websocket/decorator.py` & `nestipy-0.2.5/src/nestipy/websocket/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/src/nestipy/websocket/proxy.py` & `nestipy-0.2.5/src/nestipy/websocket/proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.2.4/PKG-INFO` & `nestipy-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.2.4 Summary: Nestipy is a Python
+Metadata-Version: 2.1 Name: nestipy Version: 0.2.5 Summary: Nestipy is a Python
 framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: minijinja
```

