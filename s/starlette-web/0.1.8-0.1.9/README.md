# Comparing `tmp/starlette_web-0.1.8.tar.gz` & `tmp/starlette_web-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_web-0.1.8.tar", last modified: Wed Feb  7 19:20:07 2024, max compression
+gzip compressed data, was "starlette_web-0.1.9.tar", last modified: Mon Apr 29 18:23:32 2024, max compression
```

## Comparing `starlette_web-0.1.8.tar` & `starlette_web-0.1.9.tar`

### file list

```diff
@@ -1,212 +1,214 @@
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.830325 starlette_web-0.1.8/
--rw-rw-rw-   0        0        0     1108 2023-04-15 07:48:43.000000 starlette_web-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      274 2024-02-07 19:19:49.000000 starlette_web-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5337 2024-02-07 19:20:07.830325 starlette_web-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2329 2023-03-26 13:41:03.000000 starlette_web-0.1.8/README.md
--rw-rw-rw-   0        0        0     2514 2024-02-07 19:06:32.000000 starlette_web-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-07 19:20:07.830325 starlette_web-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.715539 starlette_web-0.1.8/starlette_web/
--rw-rw-rw-   0        0        0       23 2022-12-29 14:13:54.000000 starlette_web-0.1.8/starlette_web/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.720578 starlette_web-0.1.8/starlette_web/common/
--rw-rw-rw-   0        0        0       52 2022-04-25 19:06:18.000000 starlette_web-0.1.8/starlette_web/common/__init__.py
--rw-rw-rw-   0        0        0     5349 2024-01-19 21:25:05.000000 starlette_web-0.1.8/starlette_web/common/app.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.720578 starlette_web-0.1.8/starlette_web/common/authorization/
--rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.8/starlette_web/common/authorization/__init__.py
--rw-rw-rw-   0        0        0      697 2023-09-02 09:03:31.000000 starlette_web-0.1.8/starlette_web/common/authorization/backends.py
--rw-rw-rw-   0        0        0      356 2024-02-07 16:41:35.000000 starlette_web-0.1.8/starlette_web/common/authorization/base_user.py
--rw-rw-rw-   0        0        0     3025 2023-03-25 08:05:20.000000 starlette_web-0.1.8/starlette_web/common/authorization/permissions.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.730602 starlette_web-0.1.8/starlette_web/common/caches/
--rw-rw-rw-   0        0        0       80 2023-03-16 18:44:56.000000 starlette_web-0.1.8/starlette_web/common/caches/__init__.py
--rw-rw-rw-   0        0        0     2162 2023-03-25 08:05:20.000000 starlette_web-0.1.8/starlette_web/common/caches/base.py
--rw-rw-rw-   0        0        0     3893 2024-01-14 18:56:11.000000 starlette_web-0.1.8/starlette_web/common/caches/base_lock.py
--rw-rw-rw-   0        0        0     1125 2024-02-04 19:20:30.000000 starlette_web-0.1.8/starlette_web/common/caches/cache_handler.py
--rw-rw-rw-   0        0        0     5291 2023-12-23 12:48:54.000000 starlette_web-0.1.8/starlette_web/common/caches/local_memory.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.730602 starlette_web-0.1.8/starlette_web/common/channels/
--rw-rw-rw-   0        0        0       54 2023-03-12 16:44:21.000000 starlette_web-0.1.8/starlette_web/common/channels/__init__.py
--rw-rw-rw-   0        0        0     4182 2024-02-07 18:42:53.000000 starlette_web-0.1.8/starlette_web/common/channels/base.py
--rw-rw-rw-   0        0        0      447 2023-03-12 16:44:21.000000 starlette_web-0.1.8/starlette_web/common/channels/event.py
--rw-rw-rw-   0        0        0      181 2023-03-22 16:38:31.000000 starlette_web-0.1.8/starlette_web/common/channels/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.730602 starlette_web-0.1.8/starlette_web/common/channels/layers/
--rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.8/starlette_web/common/channels/layers/__init__.py
--rw-rw-rw-   0        0        0      783 2024-01-03 18:26:13.000000 starlette_web-0.1.8/starlette_web/common/channels/layers/base.py
--rw-rw-rw-   0        0        0     2217 2024-02-07 18:46:50.000000 starlette_web-0.1.8/starlette_web/common/channels/layers/local_memory.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.730602 starlette_web-0.1.8/starlette_web/common/conf/
--rw-rw-rw-   0        0        0     2221 2023-09-02 09:01:37.000000 starlette_web-0.1.8/starlette_web/common/conf/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-04-13 17:27:54.000000 starlette_web-0.1.8/starlette_web/common/conf/app_manager.py
--rw-rw-rw-   0        0        0      198 2023-03-03 17:32:15.000000 starlette_web-0.1.8/starlette_web/common/conf/base_app_config.py
--rw-rw-rw-   0        0        0     2282 2024-02-07 18:54:15.000000 starlette_web-0.1.8/starlette_web/common/conf/global_settings.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.742218 starlette_web-0.1.8/starlette_web/common/database/
--rw-rw-rw-   0        0        0      282 2023-09-10 14:15:25.000000 starlette_web-0.1.8/starlette_web/common/database/__init__.py
--rw-rw-rw-   0        0        0     1822 2023-12-23 14:33:06.000000 starlette_web-0.1.8/starlette_web/common/database/columns.py
--rw-rw-rw-   0        0        0       81 2022-05-09 11:25:06.000000 starlette_web-0.1.8/starlette_web/common/database/model_base.py
--rw-rw-rw-   0        0        0     1550 2024-01-05 17:38:23.000000 starlette_web-0.1.8/starlette_web/common/database/session_maker.py
--rw-rw-rw-   0        0        0     2206 2023-09-10 11:51:19.000000 starlette_web-0.1.8/starlette_web/common/database/types.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.742218 starlette_web-0.1.8/starlette_web/common/email/
--rw-rw-rw-   0        0        0      169 2022-05-22 18:14:32.000000 starlette_web-0.1.8/starlette_web/common/email/__init__.py
--rw-rw-rw-   0        0        0     1728 2024-01-06 08:49:22.000000 starlette_web-0.1.8/starlette_web/common/email/base_sender.py
--rw-rw-rw-   0        0        0     2049 2024-01-06 09:11:16.000000 starlette_web-0.1.8/starlette_web/common/email/email_manager.py
--rw-rw-rw-   0        0        0     2183 2024-01-14 18:56:11.000000 starlette_web-0.1.8/starlette_web/common/email/smtp.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.742218 starlette_web-0.1.8/starlette_web/common/files/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.8/starlette_web/common/files/__init__.py
--rw-rw-rw-   0        0        0     6989 2024-01-14 18:56:11.000000 starlette_web-0.1.8/starlette_web/common/files/cache.py
--rw-rw-rw-   0        0        0     3930 2023-09-02 09:01:37.000000 starlette_web-0.1.8/starlette_web/common/files/filelock.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.750249 starlette_web-0.1.8/starlette_web/common/files/storages/
--rw-rw-rw-   0        0        0      217 2023-04-22 07:33:53.000000 starlette_web-0.1.8/starlette_web/common/files/storages/__init__.py
--rw-rw-rw-   0        0        0     6158 2024-01-04 22:28:51.000000 starlette_web-0.1.8/starlette_web/common/files/storages/base.py
--rw-rw-rw-   0        0        0     4532 2023-04-01 16:31:26.000000 starlette_web-0.1.8/starlette_web/common/files/storages/filesystem.py
--rw-rw-rw-   0        0        0     2552 2023-04-22 15:22:16.000000 starlette_web-0.1.8/starlette_web/common/files/storages/storage_manager.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.750249 starlette_web-0.1.8/starlette_web/common/http/
--rw-rw-rw-   0        0        0        0 2022-05-03 08:01:50.000000 starlette_web-0.1.8/starlette_web/common/http/__init__.py
--rw-rw-rw-   0        0        0     6821 2024-02-07 19:03:14.000000 starlette_web-0.1.8/starlette_web/common/http/base_endpoint.py
--rw-rw-rw-   0        0        0     3878 2024-02-07 18:59:25.000000 starlette_web-0.1.8/starlette_web/common/http/exception_handlers.py
--rw-rw-rw-   0        0        0     3304 2023-09-02 09:01:37.000000 starlette_web-0.1.8/starlette_web/common/http/exceptions.py
--rw-rw-rw-   0        0        0     1075 2022-05-09 11:25:06.000000 starlette_web-0.1.8/starlette_web/common/http/renderers.py
--rw-rw-rw-   0        0        0      336 2022-10-03 19:19:24.000000 starlette_web-0.1.8/starlette_web/common/http/responses.py
--rw-rw-rw-   0        0        0     1009 2023-04-17 17:33:36.000000 starlette_web-0.1.8/starlette_web/common/http/schemas.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.750249 starlette_web-0.1.8/starlette_web/common/i18n/
--rw-rw-rw-   0        0        0      163 2023-04-18 19:56:04.000000 starlette_web-0.1.8/starlette_web/common/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.750249 starlette_web-0.1.8/starlette_web/common/management/
--rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.8/starlette_web/common/management/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-09-03 17:56:27.000000 starlette_web-0.1.8/starlette_web/common/management/admin_util.py
--rw-rw-rw-   0        0        0     1080 2023-04-06 12:18:07.000000 starlette_web-0.1.8/starlette_web/common/management/alembic_mixin.py
--rw-rw-rw-   0        0        0     6056 2023-12-21 20:10:11.000000 starlette_web-0.1.8/starlette_web/common/management/base.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.760415 starlette_web-0.1.8/starlette_web/common/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-21 19:56:59.000000 starlette_web-0.1.8/starlette_web/common/management/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.760415 starlette_web-0.1.8/starlette_web/common/management/commands/_app_defaults/
--rw-rw-rw-   0        0        0        0 2023-03-26 18:53:46.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_app_defaults/__init__.py
--rw-rw-rw-   0        0        0      376 2023-03-26 18:59:14.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_app_defaults/admin.py
--rw-rw-rw-   0        0        0      224 2023-03-26 18:55:02.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_app_defaults/apps.py
--rw-rw-rw-   0        0        0      310 2023-09-03 19:08:18.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_app_defaults/models.py
--rw-rw-rw-   0        0        0       95 2023-03-26 19:00:40.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_app_defaults/routes.py
--rw-rw-rw-   0        0        0      154 2023-03-26 19:00:00.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_app_defaults/views.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.760415 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/
--rw-rw-rw-   0        0        0      192 2024-01-14 18:56:17.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/.env_template
--rw-rw-rw-   0        0        0        0 2023-03-26 17:54:43.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.760415 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/alembic/
--rw-rw-rw-   0        0        0     3575 2024-01-14 18:56:17.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/alembic/env.py-tpl
--rw-rw-rw-   0        0        0      549 2023-12-23 14:33:07.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/asgi.py
--rw-rw-rw-   0        0        0      867 2023-12-23 14:33:07.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/command.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.770426 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/core/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/core/__init__.py
--rw-rw-rw-   0        0        0      881 2023-09-02 09:01:37.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/core/routes.py
--rw-rw-rw-   0        0        0     3479 2023-09-02 09:01:37.000000 starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/core/settings.py
--rw-rw-rw-   0        0        0     1652 2024-02-02 19:03:08.000000 starlette_web-0.1.8/starlette_web/common/management/commands/makemigrations.py
--rw-rw-rw-   0        0        0     1294 2023-04-06 16:46:56.000000 starlette_web-0.1.8/starlette_web/common/management/commands/migrate.py
--rw-rw-rw-   0        0        0     2099 2023-09-02 09:01:37.000000 starlette_web-0.1.8/starlette_web/common/management/commands/startapp.py
--rw-rw-rw-   0        0        0     4189 2024-01-14 18:56:17.000000 starlette_web-0.1.8/starlette_web/common/management/commands/startproject.py
--rw-rw-rw-   0        0        0     1989 2023-09-02 09:01:37.000000 starlette_web-0.1.8/starlette_web/common/management/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.770426 starlette_web-0.1.8/starlette_web/common/utils/
--rw-rw-rw-   0        0        0      506 2023-04-01 19:36:50.000000 starlette_web-0.1.8/starlette_web/common/utils/__init__.py
--rw-rw-rw-   0        0        0     2778 2023-12-23 14:33:07.000000 starlette_web-0.1.8/starlette_web/common/utils/choices.py
--rw-rw-rw-   0        0        0     1265 2023-03-18 14:43:23.000000 starlette_web-0.1.8/starlette_web/common/utils/crypto.py
--rw-rw-rw-   0        0        0      187 2023-04-01 19:33:59.000000 starlette_web-0.1.8/starlette_web/common/utils/encoding.py
--rw-rw-rw-   0        0        0      633 2023-02-17 20:46:29.000000 starlette_web-0.1.8/starlette_web/common/utils/importing.py
--rw-rw-rw-   0        0        0      477 2023-09-02 09:01:37.000000 starlette_web-0.1.8/starlette_web/common/utils/inspect.py
--rw-rw-rw-   0        0        0     2324 2022-05-09 11:25:06.000000 starlette_web-0.1.8/starlette_web/common/utils/json.py
--rw-rw-rw-   0        0        0     2273 2023-09-02 09:01:38.000000 starlette_web-0.1.8/starlette_web/common/utils/regex.py
--rw-rw-rw-   0        0        0     1828 2023-03-25 08:05:10.000000 starlette_web-0.1.8/starlette_web/common/utils/serializers.py
--rw-rw-rw-   0        0        0      246 2022-05-09 11:25:06.000000 starlette_web-0.1.8/starlette_web/common/utils/singleton.py
--rw-rw-rw-   0        0        0      217 2022-10-03 19:19:24.000000 starlette_web-0.1.8/starlette_web/common/utils/urls.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.770426 starlette_web-0.1.8/starlette_web/common/ws/
--rw-rw-rw-   0        0        0        0 2022-12-29 14:13:54.000000 starlette_web-0.1.8/starlette_web/common/ws/__init__.py
--rw-rw-rw-   0        0        0     6902 2023-05-18 17:18:16.000000 starlette_web-0.1.8/starlette_web/common/ws/base_endpoint.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.770426 starlette_web-0.1.8/starlette_web/contrib/
--rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.8/starlette_web/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.780541 starlette_web-0.1.8/starlette_web/contrib/admin/
--rw-rw-rw-   0        0        0      185 2023-02-26 15:17:29.000000 starlette_web-0.1.8/starlette_web/contrib/admin/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-12-23 14:33:07.000000 starlette_web-0.1.8/starlette_web/contrib/admin/admin.py
--rw-rw-rw-   0        0        0      564 2023-03-03 17:32:15.000000 starlette_web-0.1.8/starlette_web/contrib/admin/apps.py
--rw-rw-rw-   0        0        0     4146 2024-01-06 09:17:57.000000 starlette_web-0.1.8/starlette_web/contrib/admin/auth_provider.py
--rw-rw-rw-   0        0        0     5200 2023-09-02 09:36:34.000000 starlette_web-0.1.8/starlette_web/contrib/admin/middleware.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.780541 starlette_web-0.1.8/starlette_web/contrib/apispec/
--rw-rw-rw-   0        0        0        0 2022-10-03 19:19:24.000000 starlette_web-0.1.8/starlette_web/contrib/apispec/__init__.py
--rw-rw-rw-   0        0        0     3498 2024-01-19 20:11:59.000000 starlette_web-0.1.8/starlette_web/contrib/apispec/apps.py
--rw-rw-rw-   0        0        0     8251 2024-01-19 21:56:54.000000 starlette_web-0.1.8/starlette_web/contrib/apispec/introspection.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.780541 starlette_web-0.1.8/starlette_web/contrib/apispec/marshmallow/
--rw-rw-rw-   0        0        0      352 2024-01-19 19:53:55.000000 starlette_web-0.1.8/starlette_web/contrib/apispec/marshmallow/__init__.py
--rw-rw-rw-   0        0        0     1545 2024-01-19 18:56:24.000000 starlette_web-0.1.8/starlette_web/contrib/apispec/marshmallow/converters.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.700494 starlette_web-0.1.8/starlette_web/contrib/apispec/static/
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.780541 starlette_web-0.1.8/starlette_web/contrib/apispec/static/apispec/
--rw-rw-rw-   0        0        0   879592 2022-10-03 19:19:24.000000 starlette_web-0.1.8/starlette_web/contrib/apispec/static/apispec/redoc.js
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.700494 starlette_web-0.1.8/starlette_web/contrib/apispec/templates/
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.790382 starlette_web-0.1.8/starlette_web/contrib/apispec/templates/apispec/
--rw-rw-rw-   0        0        0      539 2023-04-22 13:29:35.000000 starlette_web-0.1.8/starlette_web/contrib/apispec/templates/apispec/redoc.html
--rw-rw-rw-   0        0        0     1924 2023-12-23 14:26:52.000000 starlette_web-0.1.8/starlette_web/contrib/apispec/views.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.790382 starlette_web-0.1.8/starlette_web/contrib/auth/
--rw-rw-rw-   0        0        0        0 2023-04-13 17:15:05.000000 starlette_web-0.1.8/starlette_web/contrib/auth/__init__.py
--rw-rw-rw-   0        0        0     3484 2023-02-26 16:10:52.000000 starlette_web-0.1.8/starlette_web/contrib/auth/admin.py
--rw-rw-rw-   0        0        0      261 2023-03-17 18:16:19.000000 starlette_web-0.1.8/starlette_web/contrib/auth/apps.py
--rw-rw-rw-   0        0        0     4527 2023-09-10 10:02:48.000000 starlette_web-0.1.8/starlette_web/contrib/auth/backend.py
--rw-rw-rw-   0        0        0     3981 2023-09-10 10:24:50.000000 starlette_web-0.1.8/starlette_web/contrib/auth/hashers.py
--rw-rw-rw-   0        0        0     2513 2024-02-07 17:06:46.000000 starlette_web-0.1.8/starlette_web/contrib/auth/jwt_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.790382 starlette_web-0.1.8/starlette_web/contrib/auth/management/
--rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.8/starlette_web/contrib/auth/management/__init__.py
--rw-rw-rw-   0        0        0     1308 2023-04-01 16:41:19.000000 starlette_web-0.1.8/starlette_web/contrib/auth/management/auth_command_mixin.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.800168 starlette_web-0.1.8/starlette_web/contrib/auth/management/commands/
--rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.8/starlette_web/contrib/auth/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1367 2023-09-02 09:26:41.000000 starlette_web-0.1.8/starlette_web/contrib/auth/management/commands/changepassword.py
--rw-rw-rw-   0        0        0     1529 2023-09-02 07:19:23.000000 starlette_web-0.1.8/starlette_web/contrib/auth/management/commands/createsuperuser.py
--rw-rw-rw-   0        0        0     3176 2024-02-07 16:46:54.000000 starlette_web-0.1.8/starlette_web/contrib/auth/models.py
--rw-rw-rw-   0        0        0     3399 2024-02-07 16:46:54.000000 starlette_web-0.1.8/starlette_web/contrib/auth/password_validation.py
--rw-rw-rw-   0        0        0      624 2023-02-26 15:17:30.000000 starlette_web-0.1.8/starlette_web/contrib/auth/permissions.py
--rw-rw-rw-   0        0        0      654 2022-05-09 11:25:06.000000 starlette_web-0.1.8/starlette_web/contrib/auth/routes.py
--rw-rw-rw-   0        0        0     2724 2022-10-01 11:03:47.000000 starlette_web-0.1.8/starlette_web/contrib/auth/schemas.py
--rw-rw-rw-   0        0        0     1718 2024-02-07 17:08:02.000000 starlette_web-0.1.8/starlette_web/contrib/auth/utils.py
--rw-rw-rw-   0        0        0    19331 2023-09-02 09:01:38.000000 starlette_web-0.1.8/starlette_web/contrib/auth/views.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.800168 starlette_web-0.1.8/starlette_web/contrib/camel_case/
--rw-rw-rw-   0        0        0      249 2022-05-03 14:50:29.000000 starlette_web-0.1.8/starlette_web/contrib/camel_case/__init__.py
--rw-rw-rw-   0        0        0      389 2023-04-09 20:47:08.000000 starlette_web-0.1.8/starlette_web/contrib/camel_case/parser.py
--rw-rw-rw-   0        0        0      262 2022-05-03 14:50:29.000000 starlette_web-0.1.8/starlette_web/contrib/camel_case/renderer.py
--rw-rw-rw-   0        0        0     4103 2022-10-03 19:19:24.000000 starlette_web-0.1.8/starlette_web/contrib/camel_case/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.800168 starlette_web-0.1.8/starlette_web/contrib/constance/
--rw-rw-rw-   0        0        0     3889 2023-09-10 10:25:42.000000 starlette_web-0.1.8/starlette_web/contrib/constance/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-12-21 20:06:49.000000 starlette_web-0.1.8/starlette_web/contrib/constance/apps.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.800168 starlette_web-0.1.8/starlette_web/contrib/constance/backends/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:01:30.000000 starlette_web-0.1.8/starlette_web/contrib/constance/backends/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-04-06 19:49:34.000000 starlette_web-0.1.8/starlette_web/contrib/constance/backends/base.py
--rw-rw-rw-   0        0        0     1626 2023-09-02 09:01:38.000000 starlette_web-0.1.8/starlette_web/contrib/constance/backends/caching_mixin.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.810130 starlette_web-0.1.8/starlette_web/contrib/constance/backends/database/
--rw-rw-rw-   0        0        0     2553 2023-09-02 09:05:33.000000 starlette_web-0.1.8/starlette_web/contrib/constance/backends/database/__init__.py
--rw-rw-rw-   0        0        0      152 2023-03-03 17:32:15.000000 starlette_web-0.1.8/starlette_web/contrib/constance/backends/database/apps.py
--rw-rw-rw-   0        0        0      344 2023-08-30 17:42:12.000000 starlette_web-0.1.8/starlette_web/contrib/constance/backends/database/models.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.810130 starlette_web-0.1.8/starlette_web/contrib/mqtt/
--rw-rw-rw-   0        0        0        0 2024-01-01 21:35:50.000000 starlette_web-0.1.8/starlette_web/contrib/mqtt/__init__.py
--rw-rw-rw-   0        0        0     8813 2024-01-04 17:03:34.000000 starlette_web-0.1.8/starlette_web/contrib/mqtt/channel_layers.py
--rw-rw-rw-   0        0        0     1156 2024-01-05 18:55:02.000000 starlette_web-0.1.8/starlette_web/contrib/mqtt/serializers.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.810130 starlette_web-0.1.8/starlette_web/contrib/postgres/
--rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.8/starlette_web/contrib/postgres/__init__.py
--rw-rw-rw-   0        0        0     3561 2024-01-03 18:26:13.000000 starlette_web-0.1.8/starlette_web/contrib/postgres/channel_layers.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.810130 starlette_web-0.1.8/starlette_web/contrib/redis/
--rw-rw-rw-   0        0        0      137 2022-05-14 13:30:44.000000 starlette_web-0.1.8/starlette_web/contrib/redis/__init__.py
--rw-rw-rw-   0        0        0     4680 2023-12-24 12:01:20.000000 starlette_web-0.1.8/starlette_web/contrib/redis/cache.py
--rw-rw-rw-   0        0        0     2292 2024-01-03 18:26:13.000000 starlette_web-0.1.8/starlette_web/contrib/redis/channel_layers.py
--rw-rw-rw-   0        0        0     1196 2023-03-27 18:37:04.000000 starlette_web-0.1.8/starlette_web/contrib/redis/redislock.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.810130 starlette_web-0.1.8/starlette_web/contrib/scheduler/
--rw-rw-rw-   0        0        0      133 2023-03-04 19:50:46.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/__init__.py
--rw-rw-rw-   0        0        0     2217 2023-03-04 19:50:46.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/app_settings.py
--rw-rw-rw-   0        0        0     2084 2023-04-03 20:00:17.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/apps.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.810130 starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/
--rw-rw-rw-   0        0        0      843 2023-03-31 19:10:23.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/__init__.py
--rw-rw-rw-   0        0        0     3700 2023-08-30 18:34:06.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/base.py
--rw-rw-rw-   0        0        0     2659 2024-01-06 09:17:43.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/posix.py
--rw-rw-rw-   0        0        0     7287 2023-03-31 19:15:38.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/win32.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.820138 starlette_web-0.1.8/starlette_web/contrib/scheduler/management/
--rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.820138 starlette_web-0.1.8/starlette_web/contrib/scheduler/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1458 2023-09-02 09:01:38.000000 starlette_web-0.1.8/starlette_web/contrib/scheduler/management/commands/scheduler.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.820138 starlette_web-0.1.8/starlette_web/contrib/staticfiles/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.8/starlette_web/contrib/staticfiles/__init__.py
--rw-rw-rw-   0        0        0      136 2023-03-03 17:32:15.000000 starlette_web-0.1.8/starlette_web/contrib/staticfiles/apps.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.820138 starlette_web-0.1.8/starlette_web/contrib/staticfiles/management/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.8/starlette_web/contrib/staticfiles/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.820138 starlette_web-0.1.8/starlette_web/contrib/staticfiles/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.8/starlette_web/contrib/staticfiles/management/commands/__init__.py
--rw-rw-rw-   0        0        0     4229 2023-03-03 17:32:15.000000 starlette_web-0.1.8/starlette_web/contrib/staticfiles/management/commands/collectstatic.py
-drwxrwxrwx   0        0        0        0 2024-02-07 19:20:07.820138 starlette_web-0.1.8/starlette_web.egg-info/
--rw-rw-rw-   0        0        0     5337 2024-02-07 19:20:07.000000 starlette_web-0.1.8/starlette_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7407 2024-02-07 19:20:07.000000 starlette_web-0.1.8/starlette_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-07 19:20:07.000000 starlette_web-0.1.8/starlette_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-02-07 19:20:07.000000 starlette_web-0.1.8/starlette_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1002 2024-02-07 19:20:07.000000 starlette_web-0.1.8/starlette_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       79 2024-02-07 19:20:07.000000 starlette_web-0.1.8/starlette_web.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.855178 starlette_web-0.1.9/
+-rw-rw-rw-   0        0        0     1108 2023-04-15 07:48:43.000000 starlette_web-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      274 2024-02-07 19:19:49.000000 starlette_web-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5341 2024-04-29 18:23:32.855178 starlette_web-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2329 2023-03-26 13:41:03.000000 starlette_web-0.1.9/README.md
+-rw-rw-rw-   0        0        0     2545 2024-04-29 18:20:40.000000 starlette_web-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 18:23:32.855178 starlette_web-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.664775 starlette_web-0.1.9/starlette_web/
+-rw-rw-rw-   0        0        0       23 2022-12-29 14:13:54.000000 starlette_web-0.1.9/starlette_web/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.674850 starlette_web-0.1.9/starlette_web/common/
+-rw-rw-rw-   0        0        0       52 2022-04-25 19:06:18.000000 starlette_web-0.1.9/starlette_web/common/__init__.py
+-rw-rw-rw-   0        0        0     5388 2024-04-29 14:39:49.000000 starlette_web-0.1.9/starlette_web/common/app.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.685047 starlette_web-0.1.9/starlette_web/common/authorization/
+-rw-rw-rw-   0        0        0       99 2024-02-08 18:43:17.000000 starlette_web-0.1.9/starlette_web/common/authorization/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-09-02 09:03:31.000000 starlette_web-0.1.9/starlette_web/common/authorization/backends.py
+-rw-rw-rw-   0        0        0      357 2024-03-07 19:45:04.000000 starlette_web-0.1.9/starlette_web/common/authorization/base_user.py
+-rw-rw-rw-   0        0        0     3025 2024-02-08 18:40:59.000000 starlette_web-0.1.9/starlette_web/common/authorization/jwt_utils.py
+-rw-rw-rw-   0        0        0     3025 2023-03-25 08:05:20.000000 starlette_web-0.1.9/starlette_web/common/authorization/permissions.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.695014 starlette_web-0.1.9/starlette_web/common/caches/
+-rw-rw-rw-   0        0        0       80 2023-03-16 18:44:56.000000 starlette_web-0.1.9/starlette_web/common/caches/__init__.py
+-rw-rw-rw-   0        0        0     2162 2023-03-25 08:05:20.000000 starlette_web-0.1.9/starlette_web/common/caches/base.py
+-rw-rw-rw-   0        0        0     3893 2024-01-14 18:56:11.000000 starlette_web-0.1.9/starlette_web/common/caches/base_lock.py
+-rw-rw-rw-   0        0        0     1125 2024-02-04 19:20:30.000000 starlette_web-0.1.9/starlette_web/common/caches/cache_handler.py
+-rw-rw-rw-   0        0        0     5291 2023-12-23 12:48:54.000000 starlette_web-0.1.9/starlette_web/common/caches/local_memory.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.695014 starlette_web-0.1.9/starlette_web/common/channels/
+-rw-rw-rw-   0        0        0       54 2023-03-12 16:44:21.000000 starlette_web-0.1.9/starlette_web/common/channels/__init__.py
+-rw-rw-rw-   0        0        0     4541 2024-02-09 16:41:05.000000 starlette_web-0.1.9/starlette_web/common/channels/base.py
+-rw-rw-rw-   0        0        0      447 2023-03-12 16:44:21.000000 starlette_web-0.1.9/starlette_web/common/channels/event.py
+-rw-rw-rw-   0        0        0      181 2023-03-22 16:38:31.000000 starlette_web-0.1.9/starlette_web/common/channels/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.695014 starlette_web-0.1.9/starlette_web/common/channels/layers/
+-rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.9/starlette_web/common/channels/layers/__init__.py
+-rw-rw-rw-   0        0        0      783 2024-01-03 18:26:13.000000 starlette_web-0.1.9/starlette_web/common/channels/layers/base.py
+-rw-rw-rw-   0        0        0     2217 2024-02-07 18:46:50.000000 starlette_web-0.1.9/starlette_web/common/channels/layers/local_memory.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.704724 starlette_web-0.1.9/starlette_web/common/conf/
+-rw-rw-rw-   0        0        0     2221 2023-09-02 09:01:37.000000 starlette_web-0.1.9/starlette_web/common/conf/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-04-13 17:27:54.000000 starlette_web-0.1.9/starlette_web/common/conf/app_manager.py
+-rw-rw-rw-   0        0        0      198 2023-03-03 17:32:15.000000 starlette_web-0.1.9/starlette_web/common/conf/base_app_config.py
+-rw-rw-rw-   0        0        0     2246 2024-04-29 14:28:48.000000 starlette_web-0.1.9/starlette_web/common/conf/global_settings.py
+-rw-rw-rw-   0        0        0      706 2024-04-29 14:26:01.000000 starlette_web-0.1.9/starlette_web/common/conf/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.704724 starlette_web-0.1.9/starlette_web/common/database/
+-rw-rw-rw-   0        0        0      282 2023-09-10 14:15:25.000000 starlette_web-0.1.9/starlette_web/common/database/__init__.py
+-rw-rw-rw-   0        0        0     1822 2023-12-23 14:33:06.000000 starlette_web-0.1.9/starlette_web/common/database/columns.py
+-rw-rw-rw-   0        0        0       81 2022-05-09 11:25:06.000000 starlette_web-0.1.9/starlette_web/common/database/model_base.py
+-rw-rw-rw-   0        0        0     1550 2024-01-05 17:38:23.000000 starlette_web-0.1.9/starlette_web/common/database/session_maker.py
+-rw-rw-rw-   0        0        0     2206 2023-09-10 11:51:19.000000 starlette_web-0.1.9/starlette_web/common/database/types.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.704724 starlette_web-0.1.9/starlette_web/common/email/
+-rw-rw-rw-   0        0        0      169 2022-05-22 18:14:32.000000 starlette_web-0.1.9/starlette_web/common/email/__init__.py
+-rw-rw-rw-   0        0        0     1728 2024-01-06 08:49:22.000000 starlette_web-0.1.9/starlette_web/common/email/base_sender.py
+-rw-rw-rw-   0        0        0     2049 2024-01-06 09:11:16.000000 starlette_web-0.1.9/starlette_web/common/email/email_manager.py
+-rw-rw-rw-   0        0        0     2183 2024-01-14 18:56:11.000000 starlette_web-0.1.9/starlette_web/common/email/smtp.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.714812 starlette_web-0.1.9/starlette_web/common/files/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.9/starlette_web/common/files/__init__.py
+-rw-rw-rw-   0        0        0     6989 2024-01-14 18:56:11.000000 starlette_web-0.1.9/starlette_web/common/files/cache.py
+-rw-rw-rw-   0        0        0     3930 2023-09-02 09:01:37.000000 starlette_web-0.1.9/starlette_web/common/files/filelock.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.714812 starlette_web-0.1.9/starlette_web/common/files/storages/
+-rw-rw-rw-   0        0        0      217 2023-04-22 07:33:53.000000 starlette_web-0.1.9/starlette_web/common/files/storages/__init__.py
+-rw-rw-rw-   0        0        0     6164 2024-04-28 19:46:21.000000 starlette_web-0.1.9/starlette_web/common/files/storages/base.py
+-rw-rw-rw-   0        0        0     4532 2023-04-01 16:31:26.000000 starlette_web-0.1.9/starlette_web/common/files/storages/filesystem.py
+-rw-rw-rw-   0        0        0     2552 2023-04-22 15:22:16.000000 starlette_web-0.1.9/starlette_web/common/files/storages/storage_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.724998 starlette_web-0.1.9/starlette_web/common/http/
+-rw-rw-rw-   0        0        0        0 2022-05-03 08:01:50.000000 starlette_web-0.1.9/starlette_web/common/http/__init__.py
+-rw-rw-rw-   0        0        0     7115 2024-04-28 20:35:14.000000 starlette_web-0.1.9/starlette_web/common/http/base_endpoint.py
+-rw-rw-rw-   0        0        0     3878 2024-02-07 18:59:25.000000 starlette_web-0.1.9/starlette_web/common/http/exception_handlers.py
+-rw-rw-rw-   0        0        0     3304 2023-09-02 09:01:37.000000 starlette_web-0.1.9/starlette_web/common/http/exceptions.py
+-rw-rw-rw-   0        0        0     1075 2022-05-09 11:25:06.000000 starlette_web-0.1.9/starlette_web/common/http/renderers.py
+-rw-rw-rw-   0        0        0      336 2022-10-03 19:19:24.000000 starlette_web-0.1.9/starlette_web/common/http/responses.py
+-rw-rw-rw-   0        0        0     1009 2023-04-17 17:33:36.000000 starlette_web-0.1.9/starlette_web/common/http/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.724998 starlette_web-0.1.9/starlette_web/common/i18n/
+-rw-rw-rw-   0        0        0      163 2023-04-18 19:56:04.000000 starlette_web-0.1.9/starlette_web/common/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.724998 starlette_web-0.1.9/starlette_web/common/management/
+-rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.9/starlette_web/common/management/__init__.py
+-rw-rw-rw-   0        0        0     1383 2024-04-29 14:26:24.000000 starlette_web-0.1.9/starlette_web/common/management/admin_util.py
+-rw-rw-rw-   0        0        0     1080 2023-04-06 12:18:07.000000 starlette_web-0.1.9/starlette_web/common/management/alembic_mixin.py
+-rw-rw-rw-   0        0        0     6006 2024-04-29 14:02:44.000000 starlette_web-0.1.9/starlette_web/common/management/base.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.738177 starlette_web-0.1.9/starlette_web/common/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-21 19:56:59.000000 starlette_web-0.1.9/starlette_web/common/management/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.738177 starlette_web-0.1.9/starlette_web/common/management/commands/_app_defaults/
+-rw-rw-rw-   0        0        0        0 2023-03-26 18:53:46.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_app_defaults/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-03-26 18:59:14.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_app_defaults/admin.py
+-rw-rw-rw-   0        0        0      224 2023-03-26 18:55:02.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_app_defaults/apps.py
+-rw-rw-rw-   0        0        0      310 2023-09-03 19:08:18.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_app_defaults/models.py
+-rw-rw-rw-   0        0        0       95 2023-03-26 19:00:40.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_app_defaults/routes.py
+-rw-rw-rw-   0        0        0      154 2023-03-26 19:00:00.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_app_defaults/views.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.744702 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/
+-rw-rw-rw-   0        0        0      192 2024-01-14 18:56:17.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/.env_template
+-rw-rw-rw-   0        0        0        0 2023-03-26 17:54:43.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.744702 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/alembic/
+-rw-rw-rw-   0        0        0     3575 2024-01-14 18:56:17.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/alembic/env.py-tpl
+-rw-rw-rw-   0        0        0      478 2024-04-29 14:37:46.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/asgi.py
+-rw-rw-rw-   0        0        0      793 2024-04-29 14:26:44.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/command.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.754843 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/core/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/core/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-09-02 09:01:37.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/core/routes.py
+-rw-rw-rw-   0        0        0     3479 2023-09-02 09:01:37.000000 starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/core/settings.py
+-rw-rw-rw-   0        0        0     1652 2024-02-02 19:03:08.000000 starlette_web-0.1.9/starlette_web/common/management/commands/makemigrations.py
+-rw-rw-rw-   0        0        0     1294 2023-04-06 16:46:56.000000 starlette_web-0.1.9/starlette_web/common/management/commands/migrate.py
+-rw-rw-rw-   0        0        0     2099 2023-09-02 09:01:37.000000 starlette_web-0.1.9/starlette_web/common/management/commands/startapp.py
+-rw-rw-rw-   0        0        0     4189 2024-01-14 18:56:17.000000 starlette_web-0.1.9/starlette_web/common/management/commands/startproject.py
+-rw-rw-rw-   0        0        0     1989 2023-09-02 09:01:37.000000 starlette_web-0.1.9/starlette_web/common/management/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.764978 starlette_web-0.1.9/starlette_web/common/utils/
+-rw-rw-rw-   0        0        0      506 2023-04-01 19:36:50.000000 starlette_web-0.1.9/starlette_web/common/utils/__init__.py
+-rw-rw-rw-   0        0        0     2778 2023-12-23 14:33:07.000000 starlette_web-0.1.9/starlette_web/common/utils/choices.py
+-rw-rw-rw-   0        0        0     1265 2023-03-18 14:43:23.000000 starlette_web-0.1.9/starlette_web/common/utils/crypto.py
+-rw-rw-rw-   0        0        0      187 2023-04-01 19:33:59.000000 starlette_web-0.1.9/starlette_web/common/utils/encoding.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 20:46:29.000000 starlette_web-0.1.9/starlette_web/common/utils/importing.py
+-rw-rw-rw-   0        0        0      477 2023-09-02 09:01:37.000000 starlette_web-0.1.9/starlette_web/common/utils/inspect.py
+-rw-rw-rw-   0        0        0     2324 2022-05-09 11:25:06.000000 starlette_web-0.1.9/starlette_web/common/utils/json.py
+-rw-rw-rw-   0        0        0     2273 2023-09-02 09:01:38.000000 starlette_web-0.1.9/starlette_web/common/utils/regex.py
+-rw-rw-rw-   0        0        0     1828 2023-03-25 08:05:10.000000 starlette_web-0.1.9/starlette_web/common/utils/serializers.py
+-rw-rw-rw-   0        0        0      246 2022-05-09 11:25:06.000000 starlette_web-0.1.9/starlette_web/common/utils/singleton.py
+-rw-rw-rw-   0        0        0      217 2022-10-03 19:19:24.000000 starlette_web-0.1.9/starlette_web/common/utils/urls.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.764978 starlette_web-0.1.9/starlette_web/common/ws/
+-rw-rw-rw-   0        0        0        0 2022-12-29 14:13:54.000000 starlette_web-0.1.9/starlette_web/common/ws/__init__.py
+-rw-rw-rw-   0        0        0     7001 2024-03-07 20:26:08.000000 starlette_web-0.1.9/starlette_web/common/ws/base_endpoint.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.764978 starlette_web-0.1.9/starlette_web/contrib/
+-rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.9/starlette_web/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.764978 starlette_web-0.1.9/starlette_web/contrib/admin/
+-rw-rw-rw-   0        0        0      185 2023-02-26 15:17:29.000000 starlette_web-0.1.9/starlette_web/contrib/admin/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-12-23 14:33:07.000000 starlette_web-0.1.9/starlette_web/contrib/admin/admin.py
+-rw-rw-rw-   0        0        0      564 2023-03-03 17:32:15.000000 starlette_web-0.1.9/starlette_web/contrib/admin/apps.py
+-rw-rw-rw-   0        0        0     4146 2024-01-06 09:17:57.000000 starlette_web-0.1.9/starlette_web/contrib/admin/auth_provider.py
+-rw-rw-rw-   0        0        0     5200 2023-09-02 09:36:34.000000 starlette_web-0.1.9/starlette_web/contrib/admin/middleware.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.774702 starlette_web-0.1.9/starlette_web/contrib/apispec/
+-rw-rw-rw-   0        0        0        0 2022-10-03 19:19:24.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/__init__.py
+-rw-rw-rw-   0        0        0     3498 2024-04-29 14:27:35.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/apps.py
+-rw-rw-rw-   0        0        0     8251 2024-01-19 21:56:54.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/introspection.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.774702 starlette_web-0.1.9/starlette_web/contrib/apispec/marshmallow/
+-rw-rw-rw-   0        0        0      486 2024-04-29 17:49:16.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/marshmallow/__init__.py
+-rw-rw-rw-   0        0        0     2948 2024-04-29 17:35:34.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/marshmallow/converters.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.644932 starlette_web-0.1.9/starlette_web/contrib/apispec/static/
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.774702 starlette_web-0.1.9/starlette_web/contrib/apispec/static/apispec/
+-rw-rw-rw-   0        0        0   879592 2022-10-03 19:19:24.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/static/apispec/redoc.js
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.644932 starlette_web-0.1.9/starlette_web/contrib/apispec/templates/
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.805103 starlette_web-0.1.9/starlette_web/contrib/apispec/templates/apispec/
+-rw-rw-rw-   0        0        0      539 2023-04-22 13:29:35.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/templates/apispec/redoc.html
+-rw-rw-rw-   0        0        0      402 2024-04-29 16:33:01.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/utils.py
+-rw-rw-rw-   0        0        0     1924 2023-12-23 14:26:52.000000 starlette_web-0.1.9/starlette_web/contrib/apispec/views.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.815154 starlette_web-0.1.9/starlette_web/contrib/auth/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:15:05.000000 starlette_web-0.1.9/starlette_web/contrib/auth/__init__.py
+-rw-rw-rw-   0        0        0     3484 2023-02-26 16:10:52.000000 starlette_web-0.1.9/starlette_web/contrib/auth/admin.py
+-rw-rw-rw-   0        0        0      261 2023-03-17 18:16:19.000000 starlette_web-0.1.9/starlette_web/contrib/auth/apps.py
+-rw-rw-rw-   0        0        0     4527 2023-09-10 10:02:48.000000 starlette_web-0.1.9/starlette_web/contrib/auth/backend.py
+-rw-rw-rw-   0        0        0     3981 2023-09-10 10:24:50.000000 starlette_web-0.1.9/starlette_web/contrib/auth/hashers.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.815154 starlette_web-0.1.9/starlette_web/contrib/auth/management/
+-rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.9/starlette_web/contrib/auth/management/__init__.py
+-rw-rw-rw-   0        0        0     1308 2023-04-01 16:41:19.000000 starlette_web-0.1.9/starlette_web/contrib/auth/management/auth_command_mixin.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.815154 starlette_web-0.1.9/starlette_web/contrib/auth/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.9/starlette_web/contrib/auth/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1367 2023-09-02 09:26:41.000000 starlette_web-0.1.9/starlette_web/contrib/auth/management/commands/changepassword.py
+-rw-rw-rw-   0        0        0     1529 2023-09-02 07:19:23.000000 starlette_web-0.1.9/starlette_web/contrib/auth/management/commands/createsuperuser.py
+-rw-rw-rw-   0        0        0     3176 2024-02-07 16:46:54.000000 starlette_web-0.1.9/starlette_web/contrib/auth/models.py
+-rw-rw-rw-   0        0        0     3399 2024-02-07 16:46:54.000000 starlette_web-0.1.9/starlette_web/contrib/auth/password_validation.py
+-rw-rw-rw-   0        0        0      624 2023-02-26 15:17:30.000000 starlette_web-0.1.9/starlette_web/contrib/auth/permissions.py
+-rw-rw-rw-   0        0        0      654 2022-05-09 11:25:06.000000 starlette_web-0.1.9/starlette_web/contrib/auth/routes.py
+-rw-rw-rw-   0        0        0     2724 2022-10-01 11:03:47.000000 starlette_web-0.1.9/starlette_web/contrib/auth/schemas.py
+-rw-rw-rw-   0        0        0     1479 2024-02-08 18:31:03.000000 starlette_web-0.1.9/starlette_web/contrib/auth/utils.py
+-rw-rw-rw-   0        0        0    19331 2023-09-02 09:01:38.000000 starlette_web-0.1.9/starlette_web/contrib/auth/views.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.824666 starlette_web-0.1.9/starlette_web/contrib/camel_case/
+-rw-rw-rw-   0        0        0      249 2022-05-03 14:50:29.000000 starlette_web-0.1.9/starlette_web/contrib/camel_case/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-04-09 20:47:08.000000 starlette_web-0.1.9/starlette_web/contrib/camel_case/parser.py
+-rw-rw-rw-   0        0        0      262 2022-05-03 14:50:29.000000 starlette_web-0.1.9/starlette_web/contrib/camel_case/renderer.py
+-rw-rw-rw-   0        0        0     4103 2022-10-03 19:19:24.000000 starlette_web-0.1.9/starlette_web/contrib/camel_case/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.824666 starlette_web-0.1.9/starlette_web/contrib/constance/
+-rw-rw-rw-   0        0        0     3889 2023-09-10 10:25:42.000000 starlette_web-0.1.9/starlette_web/contrib/constance/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-12-21 20:06:49.000000 starlette_web-0.1.9/starlette_web/contrib/constance/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.824666 starlette_web-0.1.9/starlette_web/contrib/constance/backends/
+-rw-rw-rw-   0        0        0        0 2023-02-20 07:01:30.000000 starlette_web-0.1.9/starlette_web/contrib/constance/backends/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-04-06 19:49:34.000000 starlette_web-0.1.9/starlette_web/contrib/constance/backends/base.py
+-rw-rw-rw-   0        0        0     1626 2023-09-02 09:01:38.000000 starlette_web-0.1.9/starlette_web/contrib/constance/backends/caching_mixin.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.824666 starlette_web-0.1.9/starlette_web/contrib/constance/backends/database/
+-rw-rw-rw-   0        0        0     2553 2023-09-02 09:05:33.000000 starlette_web-0.1.9/starlette_web/contrib/constance/backends/database/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-03-03 17:32:15.000000 starlette_web-0.1.9/starlette_web/contrib/constance/backends/database/apps.py
+-rw-rw-rw-   0        0        0      344 2023-08-30 17:42:12.000000 starlette_web-0.1.9/starlette_web/contrib/constance/backends/database/models.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.824666 starlette_web-0.1.9/starlette_web/contrib/mqtt/
+-rw-rw-rw-   0        0        0        0 2024-01-01 21:35:50.000000 starlette_web-0.1.9/starlette_web/contrib/mqtt/__init__.py
+-rw-rw-rw-   0        0        0     8813 2024-01-04 17:03:34.000000 starlette_web-0.1.9/starlette_web/contrib/mqtt/channel_layers.py
+-rw-rw-rw-   0        0        0     1156 2024-01-05 18:55:02.000000 starlette_web-0.1.9/starlette_web/contrib/mqtt/serializers.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.834757 starlette_web-0.1.9/starlette_web/contrib/postgres/
+-rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.9/starlette_web/contrib/postgres/__init__.py
+-rw-rw-rw-   0        0        0     3561 2024-01-03 18:26:13.000000 starlette_web-0.1.9/starlette_web/contrib/postgres/channel_layers.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.838309 starlette_web-0.1.9/starlette_web/contrib/redis/
+-rw-rw-rw-   0        0        0      137 2022-05-14 13:30:44.000000 starlette_web-0.1.9/starlette_web/contrib/redis/__init__.py
+-rw-rw-rw-   0        0        0     4680 2023-12-24 12:01:20.000000 starlette_web-0.1.9/starlette_web/contrib/redis/cache.py
+-rw-rw-rw-   0        0        0     2292 2024-01-03 18:26:13.000000 starlette_web-0.1.9/starlette_web/contrib/redis/channel_layers.py
+-rw-rw-rw-   0        0        0     1196 2023-03-27 18:37:04.000000 starlette_web-0.1.9/starlette_web/contrib/redis/redislock.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.838309 starlette_web-0.1.9/starlette_web/contrib/scheduler/
+-rw-rw-rw-   0        0        0      133 2023-03-04 19:50:46.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     2217 2023-03-04 19:50:46.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/app_settings.py
+-rw-rw-rw-   0        0        0     2084 2023-04-03 20:00:17.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.844822 starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/
+-rw-rw-rw-   0        0        0      843 2023-03-31 19:10:23.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/__init__.py
+-rw-rw-rw-   0        0        0     3767 2024-04-28 19:46:44.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/base.py
+-rw-rw-rw-   0        0        0     2659 2024-01-06 09:17:43.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/posix.py
+-rw-rw-rw-   0        0        0     7296 2024-04-28 20:13:50.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/win32.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.844822 starlette_web-0.1.9/starlette_web/contrib/scheduler/management/
+-rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.844822 starlette_web-0.1.9/starlette_web/contrib/scheduler/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1458 2023-09-02 09:01:38.000000 starlette_web-0.1.9/starlette_web/contrib/scheduler/management/commands/scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.844822 starlette_web-0.1.9/starlette_web/contrib/staticfiles/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.9/starlette_web/contrib/staticfiles/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-03-03 17:32:15.000000 starlette_web-0.1.9/starlette_web/contrib/staticfiles/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.844822 starlette_web-0.1.9/starlette_web/contrib/staticfiles/management/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.9/starlette_web/contrib/staticfiles/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.844822 starlette_web-0.1.9/starlette_web/contrib/staticfiles/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.9/starlette_web/contrib/staticfiles/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     4229 2023-03-03 17:32:15.000000 starlette_web-0.1.9/starlette_web/contrib/staticfiles/management/commands/collectstatic.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:23:32.844822 starlette_web-0.1.9/starlette_web.egg-info/
+-rw-rw-rw-   0        0        0     5341 2024-04-29 18:23:32.000000 starlette_web-0.1.9/starlette_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7489 2024-04-29 18:23:32.000000 starlette_web-0.1.9/starlette_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 18:23:32.000000 starlette_web-0.1.9/starlette_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-29 18:23:32.000000 starlette_web-0.1.9/starlette_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1021 2024-04-29 18:23:32.000000 starlette_web-0.1.9/starlette_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       79 2024-04-29 18:23:32.000000 starlette_web-0.1.9/starlette_web.egg-info/top_level.txt
```

### Comparing `starlette_web-0.1.8/LICENSE` & `starlette_web-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/PKG-INFO` & `starlette_web-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette_web
-Version: 0.1.8
+Version: 0.1.9
 Summary: Asynchronous web framework, based on Starlette and inspired by Django
 Author-email: Sergey Sayamov <dolamroth@mail.ru>, Dmitry Burnaev <dmitry.burnaev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/dolamroth/starlette-web
 Project-URL: Issues, https://github.com/dolamroth/starlette-web/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,46 +13,46 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: anyio<4.3,>=4.2.0
-Requires-Dist: starlette<1.0,>=0.35.1
+Requires-Dist: anyio<4.4,>=4.3.0
+Requires-Dist: starlette<1.0,>=0.37.2
 Requires-Dist: webargs-starlette<2.2,>=2.1
-Requires-Dist: python-multipart==0.0.6
-Requires-Dist: uvicorn[standard]<0.26,>=0.25.0
-Requires-Dist: sqlalchemy<2.1,>=2.0.23
+Requires-Dist: python-multipart==0.0.9
+Requires-Dist: uvicorn[standard]<0.30,>=0.29.0
+Requires-Dist: sqlalchemy<2.1,>=2.0.29
 Requires-Dist: alembic<1.14,>=1.13.1
 Requires-Dist: Jinja2<3.2,>=3.1
 Requires-Dist: httpx<0.27,>=0.26.0
 Requires-Dist: python-dotenv<0.22,>=0.21
 Requires-Dist: traceback-with-variables<2.1,>=2.0.4
 Requires-Dist: aiosmtplib<3.1,>=3.0.1
 Requires-Dist: filelock<3.14,>=3.13.1
 Requires-Dist: marshmallow<3.21,>=3.20.1
 Requires-Dist: chardet<5.3,>=5.2.0
+Requires-Dist: PyJWT[crypto]<2.9,>=2.8
+Requires-Dist: exceptiongroup<2.0,>=1.2.1
 Provides-Extra: apispec
 Requires-Dist: apispec<6.4,>=6.3.1; extra == "apispec"
 Requires-Dist: pyyaml<6.1,>=6.0.1; extra == "apispec"
 Requires-Dist: openapi-spec-validator<0.8,>=0.7.1; extra == "apispec"
 Provides-Extra: admin
 Requires-Dist: starlette-admin<0.12,>=0.11.2; extra == "admin"
-Provides-Extra: auth
-Requires-Dist: PyJWT[crypto]<2.9,>=2.8; extra == "auth"
 Provides-Extra: mqtt
 Requires-Dist: gmqtt<0.7,>=0.6.13; extra == "mqtt"
 Provides-Extra: postgres
 Requires-Dist: asyncpg<0.30,>=0.29; extra == "postgres"
 Provides-Extra: redis
 Requires-Dist: redis<5.1,>=5.0.1; extra == "redis"
 Provides-Extra: scheduler
 Requires-Dist: croniter<2.1,>=2.0.1; extra == "scheduler"
-Requires-Dist: py-win-task-scheduler==0.2.0; sys_platform == "win32" and extra == "scheduler"
+Requires-Dist: py-win-task-scheduler==0.2.1; sys_platform == "win32" and extra == "scheduler"
 Provides-Extra: ssh
 Requires-Dist: asyncssh<2.15,>=2.14.2; extra == "ssh"
 Provides-Extra: deploy
 Requires-Dist: gunicorn<22.0,>=21.2.0; extra == "deploy"
 Provides-Extra: develop
 Requires-Dist: black~=22.10.0; extra == "develop"
 Provides-Extra: testing
```

### Comparing `starlette_web-0.1.8/README.md` & `starlette_web-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/pyproject.toml` & `starlette_web-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "starlette_web"
-version = "0.1.8"
+version = "0.1.9"
 description = "Asynchronous web framework, based on Starlette and inspired by Django"
 readme = "README.md"
 authors = [
     {name = "Sergey Sayamov", email = "dolamroth@mail.ru"},
     {name = "Dmitry Burnaev", email = "dmitry.burnaev@gmail.com"},
 ]
 license = { text = "MIT" }
@@ -20,29 +20,31 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 2 - Pre-Alpha",
 ]
 dependencies = [
-    "anyio>=4.2.0,<4.3",
-    "starlette>=0.35.1,<1.0",
+    "anyio>=4.3.0,<4.4",
+    "starlette>=0.37.2,<1.0",
     "webargs-starlette>=2.1,<2.2",
-    "python-multipart==0.0.6", # required by starlette dependencies
-    "uvicorn[standard]>=0.25.0,<0.26",
-    "sqlalchemy>=2.0.23,<2.1",
+    "python-multipart==0.0.9", # required by starlette dependencies
+    "uvicorn[standard]>=0.29.0,<0.30",
+    "sqlalchemy>=2.0.29,<2.1",
     "alembic>=1.13.1,<1.14",
     "Jinja2>=3.1,<3.2",
     "httpx>=0.26.0,<0.27",
     "python-dotenv>=0.21,<0.22",
     "traceback-with-variables>=2.0.4,<2.1",
     "aiosmtplib>=3.0.1,<3.1",
     "filelock>=3.13.1,<3.14",
     "marshmallow>=3.20.1,<3.21",
     "chardet>=5.2.0,<5.3",
+    "PyJWT[crypto]>=2.8,<2.9",
+    "exceptiongroup>=1.2.1,<2.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dolamroth/starlette-web"
 "Issues" = "https://github.com/dolamroth/starlette-web/issues"
 
 [project.scripts]
@@ -54,21 +56,20 @@
 [project.optional-dependencies]
 apispec = [
     "apispec>=6.3.1,<6.4",
     "pyyaml>=6.0.1,<6.1",
     "openapi-spec-validator>=0.7.1,<0.8",
 ]
 admin = ["starlette-admin>=0.11.2,<0.12"]
-auth = ["PyJWT[crypto]>=2.8,<2.9"]
 mqtt = ["gmqtt>=0.6.13,<0.7"]
 postgres = ["asyncpg>=0.29,<0.30"]
 redis = ["redis>=5.0.1,<5.1"]
 scheduler = [
     "croniter>=2.0.1,<2.1",
-    "py-win-task-scheduler==0.2.0; sys_platform == 'win32'",
+    "py-win-task-scheduler==0.2.1; sys_platform == 'win32'",
 ]
 ssh = ["asyncssh>=2.14.2,<2.15"]
 deploy = ["gunicorn>=21.2.0,<22.0"]
 develop = ["black~=22.10.0"]
 testing = [
     "pytest>=7.4.3",
     "coverage>=6.2",
```

### Comparing `starlette_web-0.1.8/starlette_web/common/app.py` & `starlette_web-0.1.9/starlette_web/common/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self._event_handlers = []
 
     def pre_app_init(self) -> None:
         """
         Extra actions before app's initialization (can be overridden)
         """
         app_manager.initialize_apps()
-        if self.run_checks:
+        if self.run_checks and (settings.SKIP_CHECKS is not True):
             app_manager.run_apps_checks()
 
     def post_app_init(self, app: AppClass) -> None:
         """
         Extra actions after app's initialization (can be overridden)
         """
         pass
```

### Comparing `starlette_web-0.1.8/starlette_web/common/authorization/backends.py` & `starlette_web-0.1.9/starlette_web/common/authorization/backends.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/authorization/permissions.py` & `starlette_web-0.1.9/starlette_web/common/authorization/permissions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/caches/base.py` & `starlette_web-0.1.9/starlette_web/common/caches/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/caches/base_lock.py` & `starlette_web-0.1.9/starlette_web/common/caches/base_lock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/caches/cache_handler.py` & `starlette_web-0.1.9/starlette_web/common/caches/cache_handler.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/caches/local_memory.py` & `starlette_web-0.1.9/starlette_web/common/caches/local_memory.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/channels/base.py` & `starlette_web-0.1.9/starlette_web/common/channels/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import anyio
 from anyio._core._tasks import TaskGroup
 from anyio.streams.memory import (
     MemoryObjectReceiveStream,
     MemoryObjectSendStream,
     EndOfStream,
     ClosedResourceError,
+    BrokenResourceError,
 )
 
 from starlette_web.common.channels.layers.base import BaseChannelLayer
 from starlette_web.common.channels.event import Event
 from starlette_web.common.channels.exceptions import ListenerClosed
 
 
@@ -46,38 +47,49 @@
     async def connect(self) -> None:
         await self._channel_layer.connect()
 
     async def disconnect(self) -> None:
         await self._channel_layer.disconnect()
 
     async def _listener(self) -> None:
+        async def _safe_send(_send_stream: MemoryObjectSendStream, _event: Event):
+            try:
+                await _send_stream.send(_event)
+            except (BrokenResourceError, ClosedResourceError):
+                pass
+
         async with anyio.create_task_group() as task_group:
             while True:
                 try:
                     event = await self._channel_layer.next_published()
                 except ListenerClosed:
                     break
 
                 async with self._manager_lock:
                     subscribers_list = list(self._subscribers.get(event.group, []))
 
                 for send_stream in subscribers_list:
-                    task_group.start_soon(send_stream.send, event)
+                    task_group.start_soon(_safe_send, send_stream, event)
 
         async with self._manager_lock:
             for group in self._subscribers.keys():
                 for recv_channel in self._subscribers[group]:
                     recv_channel.close()
 
     async def publish(self, group: str, message: Any, **kwargs) -> None:
         await self._channel_layer.publish(group, message, **kwargs)
 
     @asynccontextmanager
-    async def subscribe(self, group: str, **kwargs) -> AsyncGenerator["Subscriber", None]:
-        send_stream, receive_stream = anyio.create_memory_object_stream()
+    async def subscribe(
+        self,
+        group: str,
+        max_buffer_size: float = 0,
+        **kwargs,
+    ) -> AsyncGenerator["Subscriber", None]:
+        send_stream, receive_stream = anyio.create_memory_object_stream(max_buffer_size)
 
         try:
             async with self._manager_lock:
                 if not self._subscribers.get(group):
                     await self._channel_layer.subscribe(group, **kwargs)
                     self._subscribers[group] = {
                         send_stream,
```

### Comparing `starlette_web-0.1.8/starlette_web/common/channels/layers/base.py` & `starlette_web-0.1.9/starlette_web/common/channels/layers/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/channels/layers/local_memory.py` & `starlette_web-0.1.9/starlette_web/common/channels/layers/local_memory.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/conf/__init__.py` & `starlette_web-0.1.9/starlette_web/common/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/conf/app_manager.py` & `starlette_web-0.1.9/starlette_web/common/conf/app_manager.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/conf/global_settings.py` & `starlette_web-0.1.9/starlette_web/common/conf/global_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # TODO: for future support of i18n
 LANGUAGE_CODE = "en-us"
 
 # Database settings
 
 DB_ASYNC_SESSION_CLASS = "sqlalchemy.ext.asyncio.AsyncSession"
-DB_USE_CONNECTION_POOL_FOR_MANAGEMENT_COMMANDS = False
+SKIP_CHECKS = None
 DB_POOL_RECYCLE = 3600
 DB_ECHO = False
 
 # Must be overridden in user-defined settings
 DATABASE_DSN = None
 
 # Common.cache
```

### Comparing `starlette_web-0.1.8/starlette_web/common/database/columns.py` & `starlette_web-0.1.9/starlette_web/common/database/columns.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/database/session_maker.py` & `starlette_web-0.1.9/starlette_web/common/database/session_maker.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/database/types.py` & `starlette_web-0.1.9/starlette_web/common/database/types.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/email/base_sender.py` & `starlette_web-0.1.9/starlette_web/common/email/base_sender.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/email/email_manager.py` & `starlette_web-0.1.9/starlette_web/common/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/email/smtp.py` & `starlette_web-0.1.9/starlette_web/common/email/smtp.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/files/cache.py` & `starlette_web-0.1.9/starlette_web/common/files/cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/files/filelock.py` & `starlette_web-0.1.9/starlette_web/common/files/filelock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/files/storages/base.py` & `starlette_web-0.1.9/starlette_web/common/files/storages/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from contextlib import nullcontext
+from contextlib import AsyncExitStack
 from typing import Any, AnyStr, List, Literal, Optional
 from typing import AsyncContextManager, AsyncIterator
 
 import anyio
 
 from starlette_web.common.http.exceptions import NotSupportedError
 
@@ -96,15 +96,15 @@
 
     async def _finalize_write(self, fd: Any) -> None:
         pass
 
     def get_access_lock(self, path: str, mode="r") -> AsyncContextManager:
         # Mode parameter allows possible usage of RWLock,
         # should you find a working cross-process implementation
-        return nullcontext()
+        return AsyncExitStack()
 
 
 class _AsyncResourse(AsyncContextManager):
     def __init__(self, storage: BaseStorage, path: str, mode: str, **kwargs):
         self._storage = storage
         self._path = path
         self._mode = mode
```

### Comparing `starlette_web-0.1.8/starlette_web/common/files/storages/filesystem.py` & `starlette_web-0.1.9/starlette_web/common/files/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/files/storages/storage_manager.py` & `starlette_web-0.1.9/starlette_web/common/files/storages/storage_manager.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/http/base_endpoint.py` & `starlette_web-0.1.9/starlette_web/common/http/base_endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
-from typing import Type, Union, Iterable, ClassVar, Optional, Mapping, List, Awaitable
+from typing import (
+    Type, Union, Iterable, ClassVar, Optional, Mapping, List, Awaitable, Dict,
+)
 
 from marshmallow import Schema, ValidationError
 from sqlalchemy.ext.asyncio import AsyncSession
 from starlette import status
 from starlette.background import BackgroundTasks
 from starlette.exceptions import HTTPException
 from starlette.endpoints import HTTPEndpoint
@@ -112,22 +114,29 @@
             # Exception may be raised inside permission_class, to pass additional details
             except PermissionDeniedError as exc:
                 raise exc
             except Exception as exc:
                 raise PermissionDeniedError from exc
 
     async def _validate(
-        self, request, schema: Type[Schema] = None, partial_: bool = False, location: str = None
+        self,
+        request,
+        schema: Type[Schema] = None,
+        partial_: bool = False,
+        location: str = None,
+        context: Optional[Dict] = None,
     ) -> Optional[Mapping]:
         """Simple validation, based on marshmallow's schemas"""
 
         schema_class = schema or self.request_schema
         schema_kwargs = {}
         if partial_:
             schema_kwargs["partial"] = [field for field in schema_class().fields]
+        if context:
+            schema_kwargs["context"] = context
 
         schema_obj, cleaned_data = schema_class(**schema_kwargs), {}
         try:
             cleaned_data = await self.request_parser().parse(schema_obj, request, location=location)
             if hasattr(schema_obj, "is_valid") and callable(schema_obj.is_valid):
                 schema_obj.is_valid(cleaned_data)
 
@@ -144,23 +153,26 @@
 
     def _response(
         self,
         data: Union[ModelBase, Iterable[ModelBase], dict] = None,
         status_code: int = status.HTTP_200_OK,
         headers: Mapping[str, str] = None,
         background: Optional[BackgroundTasks] = None,
+        context: Optional[Dict] = None,
     ) -> BaseRenderer:
         """
         A shorthand for response_renderer plus serializing data and passing text status.
         To be used primarily with JSONRenderer and such.
         """
         if (data is not None) and self.response_schema:
             schema_kwargs = {}
             if isinstance(data, Iterable) and not isinstance(data, dict):
                 schema_kwargs["many"] = True
+            if context is not None:
+                schema_kwargs["context"] = context
 
             payload = self.response_schema(**schema_kwargs).dump(data)
         else:
             payload = data
 
         return self.response_renderer(
             payload,
```

### Comparing `starlette_web-0.1.8/starlette_web/common/http/exception_handlers.py` & `starlette_web-0.1.9/starlette_web/common/http/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/http/exceptions.py` & `starlette_web-0.1.9/starlette_web/common/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/http/renderers.py` & `starlette_web-0.1.9/starlette_web/common/http/renderers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/http/schemas.py` & `starlette_web-0.1.9/starlette_web/common/http/schemas.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/admin_util.py` & `starlette_web-0.1.9/starlette_web/common/management/admin_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import os
 import sys
 
+from starlette_web.common.conf.utils import parse_startapp_known_args
+
 
 def main():
     current_settings = os.environ.get("STARLETTE_SETTINGS_MODULE")
 
     try:
         # At this point, user-defined settings may not exist
         # (i.e., if user calls startproject command),
         # so pass global_settings instead
         settings_module = "starlette_web.common.conf.global_settings"
 
-        sys_argv = list(sys.argv).copy()
-        for arg in sys_argv.copy():
-            if arg.startswith("--settings="):
-                settings_module = arg[11:]
-                sys_argv.remove(arg)
+        args = parse_startapp_known_args()
+        if args.settings:
+            settings_module = args.settings
 
         os.environ.setdefault("STARLETTE_SETTINGS_MODULE", settings_module)
 
-        if len(sys_argv) < 2:
+        if len(sys.argv) < 2:
             raise Exception(
                 "Missing command name. Correct syntax is: " '"starlette-web-admin command_name ..."'
             )
 
-        from starlette_web.common.conf import settings
         from starlette_web.common.app import get_asgi_application
         from starlette_web.common.management.base import fetch_command_by_name
 
-        command = fetch_command_by_name(sys_argv[1])
-        app = get_asgi_application(use_pool=settings.DB_USE_CONNECTION_POOL_FOR_MANAGEMENT_COMMANDS)
-        command(app).run_from_command_line(sys_argv)
+        command = fetch_command_by_name(sys.argv[1])
+        app = get_asgi_application(use_pool=args.use_pool)
+        command(app).run_from_command_line(sys.argv)
     finally:
         if current_settings:
             os.environ["STARLETTE_SETTINGS_MODULE"] = current_settings
         else:
             os.unsetenv("STARLETTE_SETTINGS_MODULE")
```

### Comparing `starlette_web-0.1.8/starlette_web/common/management/alembic_mixin.py` & `starlette_web-0.1.9/starlette_web/common/management/alembic_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/base.py` & `starlette_web-0.1.9/starlette_web/common/management/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,11 +165,11 @@
         details = ""
     raise CommandError(message=error_message, details=details)
 
 
 async def call_command(command_name, command_args: List[str]):
     command = fetch_command_by_name(command_name)
     app = get_asgi_application(
-        use_pool=settings.DB_USE_CONNECTION_POOL_FOR_MANAGEMENT_COMMANDS,
+        use_pool=False,
         run_checks_on_startup=False,
     )
     await command(app).run_from_code(["command.py", command_name] + command_args)
```

### Comparing `starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/alembic/env.py-tpl` & `starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/alembic/env.py-tpl`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/command.py` & `starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import argparse
 import os
 import sys
 
 from starlette_web.common.app import get_asgi_application
+from starlette_web.common.conf.utils import parse_startapp_known_args
 from starlette_web.common.management.base import fetch_command_by_name, CommandError
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--settings", default="core.settings", required=False)
-    args, _ = parser.parse_known_args()
-    os.environ.setdefault("STARLETTE_SETTINGS_MODULE", args.settings)
+    args = parse_startapp_known_args()
+    os.environ.setdefault("STARLETTE_SETTINGS_MODULE", args.settings or "core.settings")
 
     if len(sys.argv) < 2:
         raise CommandError(
             'Missing command name. Correct syntax is: "python command.py command_name ..."'
         )
 
-    from starlette_web.common.conf import settings
-
     command = fetch_command_by_name(sys.argv[1])
-    app = get_asgi_application(use_pool=settings.DB_USE_CONNECTION_POOL_FOR_MANAGEMENT_COMMANDS)
+    app = get_asgi_application(
+        use_pool=args.use_pool,
+        run_checks_on_startup=not args.skip_checks,
+    )
     command(app).run_from_command_line(sys.argv)
```

### Comparing `starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/core/routes.py` & `starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/core/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/commands/_project_defaults/core/settings.py` & `starlette_web-0.1.9/starlette_web/common/management/commands/_project_defaults/core/settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/commands/makemigrations.py` & `starlette_web-0.1.9/starlette_web/common/management/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/commands/migrate.py` & `starlette_web-0.1.9/starlette_web/common/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/commands/startapp.py` & `starlette_web-0.1.9/starlette_web/common/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/commands/startproject.py` & `starlette_web-0.1.9/starlette_web/common/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/management/utils.py` & `starlette_web-0.1.9/starlette_web/common/management/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/utils/choices.py` & `starlette_web-0.1.9/starlette_web/common/utils/choices.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/utils/crypto.py` & `starlette_web-0.1.9/starlette_web/common/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/utils/importing.py` & `starlette_web-0.1.9/starlette_web/common/utils/importing.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/utils/json.py` & `starlette_web-0.1.9/starlette_web/common/utils/json.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/utils/regex.py` & `starlette_web-0.1.9/starlette_web/common/utils/regex.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/utils/serializers.py` & `starlette_web-0.1.9/starlette_web/common/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/common/ws/base_endpoint.py` & `starlette_web-0.1.9/starlette_web/common/ws/base_endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,21 @@
             raise WebSocketDisconnect(code=1006, reason=str(exc)) from exc
 
         # Explicitly clear db_session,
         # so that user does not use it through lengthy websocket life-state
         del websocket.state.db_session
 
         if permitted:
-            await websocket.accept()
+            await self.accept(websocket)
         else:
             raise WebSocketDisconnect(code=3000, reason=reason)
 
+    async def accept(self, websocket: WebSocket) -> None:
+        await websocket.accept()
+
     async def on_receive(self, websocket: WebSocket, data: Any) -> None:
         cleaned_data = self._validate(data)
         task_id = get_random_string(50)
         self.task_group.start_soon(self._background_handler_wrap, task_id, websocket, cleaned_data)
 
     async def on_disconnect(self, websocket: WebSocket, close_code: int) -> None:
         if self.task_group:
```

### Comparing `starlette_web-0.1.8/starlette_web/contrib/admin/admin.py` & `starlette_web-0.1.9/starlette_web/contrib/admin/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/admin/apps.py` & `starlette_web-0.1.9/starlette_web/contrib/admin/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/admin/auth_provider.py` & `starlette_web-0.1.9/starlette_web/contrib/admin/auth_provider.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/admin/middleware.py` & `starlette_web-0.1.9/starlette_web/contrib/admin/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/apispec/apps.py` & `starlette_web-0.1.9/starlette_web/contrib/apispec/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/apispec/introspection.py` & `starlette_web-0.1.9/starlette_web/contrib/apispec/introspection.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/apispec/static/apispec/redoc.js` & `starlette_web-0.1.9/starlette_web/contrib/apispec/static/apispec/redoc.js`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/apispec/templates/apispec/redoc.html` & `starlette_web-0.1.9/starlette_web/contrib/apispec/templates/apispec/redoc.html`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/apispec/views.py` & `starlette_web-0.1.9/starlette_web/contrib/apispec/views.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/admin.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/backend.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/backend.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/hashers.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/jwt_utils.py` & `starlette_web-0.1.9/starlette_web/common/authorization/jwt_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 import copy
 import datetime
 from functools import cached_property
 from typing import Tuple
 
 import jwt
 
+from starlette_web.common.conf import settings
+from starlette_web.common.utils.json import StarletteJSONEncoder
 from starlette_web.common.utils.inspect import get_available_options
 
 
 class JWTProcessor:
     def __init__(self, **kwargs):
         self.init_options = kwargs
 
     def encode_jwt(
         self,
         payload: dict,
         expires_in: int = None,
         **kwargs,
     ) -> Tuple[str, datetime.datetime]:
+        _options = {**self.init_options}
+        _options.update(kwargs)
+
         _expires_at = self._get_expires_at(
             expires_in=expires_in,
-            **self.init_options,
-            **kwargs,
+            **_options,
         )
         _payload = copy.deepcopy(payload)
         _payload["exp"] = _expires_at
         self._enhance_payload_for_encode(
             _payload,
-            **self.init_options,
-            **kwargs,
+            **_options,
         )
 
         token = jwt.encode(
             payload=_payload,
             key=self._get_encode_secret_key,
-            **self._get_encode_options(**self.init_options, **kwargs),
+            **self._get_encode_options(**_options),
         )
         return token, _expires_at
 
     def decode_jwt(self, encoded_jwt: str, **kwargs):
+        _options = {**self.init_options}
+        _options.update(kwargs)
+
         return jwt.decode(
             encoded_jwt,
             key=self._get_decode_secret_key,
-            **self._get_decode_options(**self.init_options, **kwargs),
+            **self._get_decode_options(**_options),
         )
 
     @cached_property
     def _get_encode_secret_key(self):
-        raise NotImplementedError()
+        return str(settings.SECRET_KEY)
 
     @cached_property
     def _get_decode_secret_key(self):
-        raise NotImplementedError()
+        return str(settings.SECRET_KEY)
 
     def _get_expires_at(self, expires_in: int = None, **kwargs) -> datetime.datetime:
+        if expires_in is None and kwargs.get("expires_in"):
+            expires_in = kwargs["expires_in"]
+
         return datetime.datetime.utcnow() + datetime.timedelta(seconds=expires_in)
 
     def _enhance_payload_for_encode(self, payload: dict, **kwargs) -> None:
         pass
 
     def _get_encode_options(self, **kwargs) -> dict:
         res = {}
@@ -80,7 +89,16 @@
         if "algorithm" in options and not res.get("algorithms"):
             res["algorithms"] = [options["algorithm"]]
 
         if "options" not in res:
             res["options"] = options
 
         return res
+
+
+jwt_processor = JWTProcessor(
+    algorithm=settings.AUTH_JWT_ALGORITHM,
+    verify_signature=True,
+    json_encoder=StarletteJSONEncoder,
+)
+encode_jwt = jwt_processor.encode_jwt
+decode_jwt = jwt_processor.decode_jwt
```

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/management/auth_command_mixin.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/management/auth_command_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/management/commands/changepassword.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/management/commands/changepassword.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/management/commands/createsuperuser.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/management/commands/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/models.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/models.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/password_validation.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/password_validation.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/permissions.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/routes.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/schemas.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/utils.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
 from dataclasses import dataclass
-from functools import cached_property
 
 from starlette_web.common.conf import settings
 from starlette_web.common.utils.json import StarletteJSONEncoder
-from starlette_web.contrib.auth.jwt_utils import JWTProcessor
+from starlette_web.common.authorization.jwt_utils import JWTProcessor
 
 
 TOKEN_TYPE_ACCESS = "access"
 TOKEN_TYPE_REFRESH = "refresh"
 TOKEN_TYPE_RESET_PASSWORD = "reset_password"
 
 
@@ -17,22 +16,14 @@
     refresh_token: str
     refresh_token_expired_at: datetime.datetime
     access_token: str
     access_token_expired_at: datetime.datetime
 
 
 class AuthJWTProcessor(JWTProcessor):
-    @cached_property
-    def _get_encode_secret_key(self):
-        return str(settings.SECRET_KEY)
-
-    @cached_property
-    def _get_decode_secret_key(self):
-        return str(settings.SECRET_KEY)
-
     def _get_expires_at(self, expires_in: int = None, **kwargs) -> datetime.datetime:
         token_type: str = kwargs.get("token_type", TOKEN_TYPE_ACCESS)
 
         if token_type == TOKEN_TYPE_REFRESH:
             expires_in = settings.AUTH_JWT_REFRESH_EXPIRES_IN
         else:
             expires_in = expires_in or settings.AUTH_JWT_EXPIRES_IN
```

### Comparing `starlette_web-0.1.8/starlette_web/contrib/auth/views.py` & `starlette_web-0.1.9/starlette_web/contrib/auth/views.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/camel_case/utils.py` & `starlette_web-0.1.9/starlette_web/contrib/camel_case/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/constance/__init__.py` & `starlette_web-0.1.9/starlette_web/contrib/constance/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/constance/apps.py` & `starlette_web-0.1.9/starlette_web/contrib/constance/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/constance/backends/base.py` & `starlette_web-0.1.9/starlette_web/contrib/constance/backends/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/constance/backends/caching_mixin.py` & `starlette_web-0.1.9/starlette_web/contrib/constance/backends/caching_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/constance/backends/database/__init__.py` & `starlette_web-0.1.9/starlette_web/contrib/constance/backends/database/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/mqtt/channel_layers.py` & `starlette_web-0.1.9/starlette_web/contrib/mqtt/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/mqtt/serializers.py` & `starlette_web-0.1.9/starlette_web/contrib/mqtt/serializers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/postgres/channel_layers.py` & `starlette_web-0.1.9/starlette_web/contrib/postgres/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/redis/cache.py` & `starlette_web-0.1.9/starlette_web/contrib/redis/cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/redis/channel_layers.py` & `starlette_web-0.1.9/starlette_web/contrib/redis/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/redis/redislock.py` & `starlette_web-0.1.9/starlette_web/contrib/redis/redislock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/scheduler/app_settings.py` & `starlette_web-0.1.9/starlette_web/contrib/scheduler/app_settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/scheduler/apps.py` & `starlette_web-0.1.9/starlette_web/contrib/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/__init__.py` & `starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/base.py` & `starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import hashlib
 import logging
 import os
 import tempfile
-from contextlib import nullcontext
-from typing import List, Dict, Tuple, Union
+from contextlib import ExitStack
+from typing import List, Dict, Tuple, Union, ContextManager
 
 import anyio
 from filelock import FileLock
 from traceback_with_variables import format_exc
 
 from starlette_web.common.conf import settings as project_settings
 
@@ -99,15 +99,17 @@
     def _get_job_by_hash(self, job_hash: str) -> JobType:
         for job in self.settings.PERIODIC_JOBS:
             if self._hash_job(job) == job_hash:
                 return job
 
         raise CommandError(details=f"Periodic job with hash = {job_hash} not found.")
 
-    def _get_job_mutex(self, job_hash: str):
+    def _get_job_mutex(self, job_hash: str) -> ContextManager:
+        exit_stack = ExitStack()
+
         if self.settings.LOCK_JOBS:
             lock_file = os.path.join(
                 tempfile.gettempdir(), self._get_project_level_hash() + "_" + job_hash + ".lock"
             )
-            return FileLock(lock_file, timeout=self.settings.BLOCKING_TIMEOUT)
-        else:
-            return nullcontext()
+            exit_stack.enter_context(FileLock(lock_file, timeout=self.settings.BLOCKING_TIMEOUT))
+
+        return exit_stack
```

### Comparing `starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/posix.py` & `starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/posix.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/scheduler/backends/win32.py` & `starlette_web-0.1.9/starlette_web/contrib/scheduler/backends/win32.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,19 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._project_folder_exists = False
         self._current_jobs = []
         self._root_dir = "starlette_web"
 
     def __enter__(self):
-        if self.needs_write:
-            if ctypes.windll.shell32.IsUserAnAdmin() == 0:
-                warnings.warn(
-                    "You may have insufficient privileges to make "
-                    "changes to Task Scheduler as non-administrator"
-                )
+        if ctypes.windll.shell32.IsUserAnAdmin() == 0:
+            warnings.warn(
+                "You may have insufficient privileges to make or observe "
+                "changes to Task Scheduler as non-administrator"
+            )
 
         self._ensure_project_folder_exists()
         self._read_jobs()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         return False
@@ -85,15 +84,15 @@
                     trigger_type="Daily",
                     repeat_interval="1 minute",
                     repeat_duration="1 day",
                     start_time=start_time,
                     start_date=start_date,
                 )
 
-            created = create_task(
+            created, reason = create_task(
                 name=job_hash,
                 location=location,
                 description=f"Periodic job {job_hash}",
                 enabled=True,
                 hidden=False,
                 user_name=self.settings.USERNAME,
                 password=self.settings.PASSWORD,
@@ -105,29 +104,29 @@
                 allow_demand_start=False,
                 start_when_available=True,
                 force=True,
                 restart_every=False,
                 execution_time_limit=False,
                 force_stop=True,
                 delete_after=False,
-                multiple_instances=not self.settings.LOCK_JOBS,
+                multiple_instances=["Parallel", "No New Instance"][self.settings.LOCK_JOBS],
                 action_type="Execute",
                 cmd=self.settings.PYTHON_EXECUTABLE,
                 arguments=(
                     f"command.py "
                     f"scheduler "
                     f"run "
                     f"--jobhash={job_hash} "
                     f"--settings={self.settings.SETTINGS_MODULE}"
                 ),
                 start_in=self.settings.RUN_DIRECTORY,
                 **schedule_kwargs,
             )
             if not created:
-                raise CommandError(message=f"Could not create task {job}")
+                raise CommandError(message=f"Could not create task {job}. {reason}")
 
             logger.info(f"Created scheduled task {job}")
 
     def _ensure_project_folder_exists(self):
         if self._project_folder_exists:
             return
 
@@ -172,15 +171,15 @@
         location = "\\" + self._root_dir + "\\" + project_hash
 
         for job in self.settings.PERIODIC_JOBS:
             task_name = self._hash_job(job)
             if task_name in self._current_jobs:
                 task_info = get_task_info(task_name, location=location)
                 logger.info("%s -> %s" % (job, location + task_name))
-                logger.info(json.dumps(task_info, indent=2))
+                logger.debug(json.dumps(task_info, indent=2))
 
     def remove_jobs(self):
         project_hash = self._get_project_level_hash()
         location = "\\" + self._root_dir + "\\" + project_hash
 
         for job_hash in self._current_jobs:
             deleted = delete_task(name=job_hash, location=location)
```

### Comparing `starlette_web-0.1.8/starlette_web/contrib/scheduler/management/commands/scheduler.py` & `starlette_web-0.1.9/starlette_web/contrib/scheduler/management/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web/contrib/staticfiles/management/commands/collectstatic.py` & `starlette_web-0.1.9/starlette_web/contrib/staticfiles/management/commands/collectstatic.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.8/starlette_web.egg-info/PKG-INFO` & `starlette_web-0.1.9/starlette_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette_web
-Version: 0.1.8
+Version: 0.1.9
 Summary: Asynchronous web framework, based on Starlette and inspired by Django
 Author-email: Sergey Sayamov <dolamroth@mail.ru>, Dmitry Burnaev <dmitry.burnaev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/dolamroth/starlette-web
 Project-URL: Issues, https://github.com/dolamroth/starlette-web/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,46 +13,46 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: anyio<4.3,>=4.2.0
-Requires-Dist: starlette<1.0,>=0.35.1
+Requires-Dist: anyio<4.4,>=4.3.0
+Requires-Dist: starlette<1.0,>=0.37.2
 Requires-Dist: webargs-starlette<2.2,>=2.1
-Requires-Dist: python-multipart==0.0.6
-Requires-Dist: uvicorn[standard]<0.26,>=0.25.0
-Requires-Dist: sqlalchemy<2.1,>=2.0.23
+Requires-Dist: python-multipart==0.0.9
+Requires-Dist: uvicorn[standard]<0.30,>=0.29.0
+Requires-Dist: sqlalchemy<2.1,>=2.0.29
 Requires-Dist: alembic<1.14,>=1.13.1
 Requires-Dist: Jinja2<3.2,>=3.1
 Requires-Dist: httpx<0.27,>=0.26.0
 Requires-Dist: python-dotenv<0.22,>=0.21
 Requires-Dist: traceback-with-variables<2.1,>=2.0.4
 Requires-Dist: aiosmtplib<3.1,>=3.0.1
 Requires-Dist: filelock<3.14,>=3.13.1
 Requires-Dist: marshmallow<3.21,>=3.20.1
 Requires-Dist: chardet<5.3,>=5.2.0
+Requires-Dist: PyJWT[crypto]<2.9,>=2.8
+Requires-Dist: exceptiongroup<2.0,>=1.2.1
 Provides-Extra: apispec
 Requires-Dist: apispec<6.4,>=6.3.1; extra == "apispec"
 Requires-Dist: pyyaml<6.1,>=6.0.1; extra == "apispec"
 Requires-Dist: openapi-spec-validator<0.8,>=0.7.1; extra == "apispec"
 Provides-Extra: admin
 Requires-Dist: starlette-admin<0.12,>=0.11.2; extra == "admin"
-Provides-Extra: auth
-Requires-Dist: PyJWT[crypto]<2.9,>=2.8; extra == "auth"
 Provides-Extra: mqtt
 Requires-Dist: gmqtt<0.7,>=0.6.13; extra == "mqtt"
 Provides-Extra: postgres
 Requires-Dist: asyncpg<0.30,>=0.29; extra == "postgres"
 Provides-Extra: redis
 Requires-Dist: redis<5.1,>=5.0.1; extra == "redis"
 Provides-Extra: scheduler
 Requires-Dist: croniter<2.1,>=2.0.1; extra == "scheduler"
-Requires-Dist: py-win-task-scheduler==0.2.0; sys_platform == "win32" and extra == "scheduler"
+Requires-Dist: py-win-task-scheduler==0.2.1; sys_platform == "win32" and extra == "scheduler"
 Provides-Extra: ssh
 Requires-Dist: asyncssh<2.15,>=2.14.2; extra == "ssh"
 Provides-Extra: deploy
 Requires-Dist: gunicorn<22.0,>=21.2.0; extra == "deploy"
 Provides-Extra: develop
 Requires-Dist: black~=22.10.0; extra == "develop"
 Provides-Extra: testing
```

### Comparing `starlette_web-0.1.8/starlette_web.egg-info/SOURCES.txt` & `starlette_web-0.1.9/starlette_web.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 starlette_web.egg-info/requires.txt
 starlette_web.egg-info/top_level.txt
 starlette_web/common/__init__.py
 starlette_web/common/app.py
 starlette_web/common/authorization/__init__.py
 starlette_web/common/authorization/backends.py
 starlette_web/common/authorization/base_user.py
+starlette_web/common/authorization/jwt_utils.py
 starlette_web/common/authorization/permissions.py
 starlette_web/common/caches/__init__.py
 starlette_web/common/caches/base.py
 starlette_web/common/caches/base_lock.py
 starlette_web/common/caches/cache_handler.py
 starlette_web/common/caches/local_memory.py
 starlette_web/common/channels/__init__.py
@@ -27,14 +28,15 @@
 starlette_web/common/channels/layers/__init__.py
 starlette_web/common/channels/layers/base.py
 starlette_web/common/channels/layers/local_memory.py
 starlette_web/common/conf/__init__.py
 starlette_web/common/conf/app_manager.py
 starlette_web/common/conf/base_app_config.py
 starlette_web/common/conf/global_settings.py
+starlette_web/common/conf/utils.py
 starlette_web/common/database/__init__.py
 starlette_web/common/database/columns.py
 starlette_web/common/database/model_base.py
 starlette_web/common/database/session_maker.py
 starlette_web/common/database/types.py
 starlette_web/common/email/__init__.py
 starlette_web/common/email/base_sender.py
@@ -97,25 +99,25 @@
 starlette_web/contrib/admin/admin.py
 starlette_web/contrib/admin/apps.py
 starlette_web/contrib/admin/auth_provider.py
 starlette_web/contrib/admin/middleware.py
 starlette_web/contrib/apispec/__init__.py
 starlette_web/contrib/apispec/apps.py
 starlette_web/contrib/apispec/introspection.py
+starlette_web/contrib/apispec/utils.py
 starlette_web/contrib/apispec/views.py
 starlette_web/contrib/apispec/marshmallow/__init__.py
 starlette_web/contrib/apispec/marshmallow/converters.py
 starlette_web/contrib/apispec/static/apispec/redoc.js
 starlette_web/contrib/apispec/templates/apispec/redoc.html
 starlette_web/contrib/auth/__init__.py
 starlette_web/contrib/auth/admin.py
 starlette_web/contrib/auth/apps.py
 starlette_web/contrib/auth/backend.py
 starlette_web/contrib/auth/hashers.py
-starlette_web/contrib/auth/jwt_utils.py
 starlette_web/contrib/auth/models.py
 starlette_web/contrib/auth/password_validation.py
 starlette_web/contrib/auth/permissions.py
 starlette_web/contrib/auth/routes.py
 starlette_web/contrib/auth/schemas.py
 starlette_web/contrib/auth/utils.py
 starlette_web/contrib/auth/views.py
```

### Comparing `starlette_web-0.1.8/starlette_web.egg-info/requires.txt` & `starlette_web-0.1.9/starlette_web.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-anyio<4.3,>=4.2.0
-starlette<1.0,>=0.35.1
+anyio<4.4,>=4.3.0
+starlette<1.0,>=0.37.2
 webargs-starlette<2.2,>=2.1
-python-multipart==0.0.6
-uvicorn[standard]<0.26,>=0.25.0
-sqlalchemy<2.1,>=2.0.23
+python-multipart==0.0.9
+uvicorn[standard]<0.30,>=0.29.0
+sqlalchemy<2.1,>=2.0.29
 alembic<1.14,>=1.13.1
 Jinja2<3.2,>=3.1
 httpx<0.27,>=0.26.0
 python-dotenv<0.22,>=0.21
 traceback-with-variables<2.1,>=2.0.4
 aiosmtplib<3.1,>=3.0.1
 filelock<3.14,>=3.13.1
 marshmallow<3.21,>=3.20.1
 chardet<5.3,>=5.2.0
+PyJWT[crypto]<2.9,>=2.8
+exceptiongroup<2.0,>=1.2.1
 
 [admin]
 starlette-admin<0.12,>=0.11.2
 
 [all]
 starlette-web[admin,apispec,auth,deploy,develop,mqtt,postgres,redis,scheduler,testing]
 
 [apispec]
 apispec<6.4,>=6.3.1
 pyyaml<6.1,>=6.0.1
 openapi-spec-validator<0.8,>=0.7.1
 
-[auth]
-PyJWT[crypto]<2.9,>=2.8
-
 [deploy]
 gunicorn<22.0,>=21.2.0
 
 [develop]
 black~=22.10.0
 
 [full]
@@ -46,15 +45,15 @@
 [redis]
 redis<5.1,>=5.0.1
 
 [scheduler]
 croniter<2.1,>=2.0.1
 
 [scheduler:sys_platform == "win32"]
-py-win-task-scheduler==0.2.0
+py-win-task-scheduler==0.2.1
 
 [ssh]
 asyncssh<2.15,>=2.14.2
 
 [testing]
 pytest>=7.4.3
 coverage>=6.2
```

