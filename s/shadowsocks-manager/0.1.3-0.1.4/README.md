# Comparing `tmp/shadowsocks_manager-0.1.3.tar.gz` & `tmp/shadowsocks_manager-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowsocks_manager-0.1.3.tar", last modified: Fri Apr 26 20:03:28 2024, max compression
+gzip compressed data, was "shadowsocks_manager-0.1.4.tar", last modified: Mon Apr 29 19:12:34 2024, max compression
```

## Comparing `shadowsocks_manager-0.1.3.tar` & `shadowsocks_manager-0.1.4.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.816147 shadowsocks_manager-0.1.3/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/bin/ssm-dev-start
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/bin/ssm-dev-stop
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/bin/ssm-setup
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/bin/ssm-test
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-26 20:03:25.000000 shadowsocks_manager-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/.env
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/fixtures/nameserver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.820147 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/auth.group.json
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/sites.site.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/fixtures/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/notification/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/retry/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/retry/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.824147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/fixtures/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36547 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.828147 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/createsuperuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-26 20:03:14.000000 shadowsocks_manager-0.1.3/shadowsocks_manager/utils/uwsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:03:28.832147 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 20:03:28.000000 shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20803 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.848405 shadowsocks_manager-0.1.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/bin/ssm-dev-start
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/bin/ssm-dev-stop
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/bin/ssm-setup
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/bin/ssm-test
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-29 19:12:30.000000 shadowsocks_manager-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.848405 shadowsocks_manager-0.1.4/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/.env
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/fixtures/nameserver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.852405 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/auth.group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/sites.site.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/fixtures/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/notification/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/retry/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.856405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/fixtures/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36795 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21089 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.860405 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 19:12:13.000000 shadowsocks_manager-0.1.4/shadowsocks_manager/utils/uwsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:12:34.864405 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20803 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 19:12:34.000000 shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/top_level.txt
```

### Comparing `shadowsocks_manager-0.1.3/LICENSE` & `shadowsocks_manager-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/PKG-INFO` & `shadowsocks_manager-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.3
+Version: 0.1.4
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
@@ -60,15 +60,15 @@
 Requires-Dist: six
 Requires-Dist: boto3
 Requires-Dist: celery
 Requires-Dist: Django<4
 Requires-Dist: django-allowedsites-dynamic
 Requires-Dist: django-cache-lock
 Requires-Dist: django-celery-beat==1.6.0; python_version <= "2.7"
-Requires-Dist: django-celery-beat<2.6.0; python_version < "3.8"
+Requires-Dist: django-celery-beat<2.6.0; python_version > "2.7" and python_version < "3.8"
 Requires-Dist: django-celery-beat; python_version >= "3.8"
 Requires-Dist: django-celery-results==2.0.1; python_version <= "2.7"
 Requires-Dist: django-celery-results; python_version > "2.7"
 Requires-Dist: django-enumfield<3.0; python_version <= "2.7"
 Requires-Dist: django-enumfield; python_version > "2.7"
 Requires-Dist: django-filter~=1.1; python_version <= "2.7"
 Requires-Dist: django-filter; python_version > "2.7"
@@ -79,15 +79,14 @@
 Requires-Dist: psutil
 Requires-Dist: python-crontab==2.6.0; python_version <= "2.7"
 Requires-Dist: python-crontab; python_version > "2.7"
 Requires-Dist: python-decouple
 Requires-Dist: python-memcached==1.59
 Requires-Dist: pytz
 Requires-Dist: requests
-Requires-Dist: shadowsocks-alexforks
 Requires-Dist: uWSGI
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: codecov-cli; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -127,25 +126,26 @@
 * How's the Shadowsocks supported:
     * libev edition:
         * Full functional.
         * No builtin service manager, you need to install it and start the service by yourself.
     * python edition:
         * Lacks the collection of traffic statistics.
         * Lacks the ability to test user port creation status.
-        * Pre-installed, and have a builtin service manager.
+        * ~~Pre-installed, and have a builtin service manager.~~
+        * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
 Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
+![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
 
 Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
+![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
@@ -163,26 +163,28 @@
 ### 2.2. Manual installation
 
 ```sh
 # create a docker network
 docker network create ssm-network
 
 # run memcached, used by django cache
-docker run -d -p 11211:11211 --network ssm-network --name ssm-memcached memcached
+docker run -d --network ssm-network --name ssm-memcached memcached
 
 # run rabbitmq, used by celery
-docker run -d -p 5672:5672 --network ssm-network --name ssm-rabbitmq rabbitmq
+docker run -d --network ssm-network --name ssm-rabbitmq rabbitmq
 
-# create a directory to store the data, it will be mounted to the container
+# create a directory to store the data, it will be mounted to the shadowsocks-manager container
 mkdir -p ~/ssm-volume
 
 # run the shadowsocks-manager
-docker run -d -p 80:80 --network ssm-network -v ~/ssm-volume:/var/local/ssm --name ssm alexzhangs/shadowsocks-manager \
-           -e SSM_SECRET_KEY=yourkey -e SSM_DEBUG=False -e SSM_MEMCACHED_HOST=ssm-memcached -e SSM_RABBITMQ_HOST=ssm-rabbitmq \
-           -u admin -p yourpassword -M admin@yourdomain.com
+docker run -d -p 80:80 -v ~/ssm-volume:/var/local/ssm \
+    --network ssm-network --name ssm alexzhangs/shadowsocks-manager \
+    -e SSM_SECRET_KEY=yourkey -e SSM_DEBUG=False \
+    -e SSM_MEMCACHED_HOST=ssm-memcached -e SSM_RABBITMQ_HOST=ssm-rabbitmq \
+    -u admin -p yourpassword -M admin@yourdomain.com
 ```
 
 ### 2.3. Install with script
 
 ```sh
 git clone https://github.com/alexzhangs/shadowsocks-manager
 bash shadowsocks-manager/install.sh -u admin -p yourpassword -M admin@yourdomain.com
@@ -205,48 +207,43 @@
 ## 3. Using shadowsocks-manager
 
 1. Shadowsocks server
 
     First, you need to have a Shadowsocks server with the multi-user API
 enabled.
 
-    About how to install and configure Shadowsocks server in AWS, refer
-to the repo
-[aws-ec2-shadowsocks-libev](https://github.com/alexzhangs/aws-ec2-shadowsocks-libev)
-
-    After the server is installed and started, there should be a
-running process named `ss-manager`. Write down the IP address and
-the port that the `ss-manager` is listening on, and also the public IP
-address of the server, the encryption method that Shadowsocks is using,
-they are going to be used in the next step.
+    Install it with docker on the same server with shadowsocks-manager.
+
+    ```sh
+    # run shadowsocks-libev
+    MGR_PORT=6001
+    SS_PORTS=8381-8480
+    ENCRYPT=aes-256-cfb
+    docker run -d -p $SS_PORTS:$SS_PORTS/UDP -p $SS_PORTS:$SS_PORTS \
+        --network ssm-network --name ssm-ss-libev shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+
+    # Use below command to get the private IP address of the shadowsocks-libev container for later configuration.
+    docker inspect ssm-ss-libev | grep IPAddress
+    ```
 
 1. Add Shadowsocks server to shadowsocks-manager
 
     Add the Shadowsocks server as a Node of shadowsocks-manager from
 web admin console: `Home › Shadowsocks › Shadowsocks Nodes`.
 
 1. Create users(ports) and assign Shadowsocks Node
 
     Create users from web admin console: `Home › Shadowsocks ›
 Shadowsocks Accounts` and assign the existing nodes to them.
 
     After a few seconds, the created user ports should be available to your
 Shadowsocks client.
 
-1. The builtin local service manager for Shadowsocks python edition
-
-    There's a builtin local service manager available for the Shadowsocks `python edition`. 
-
-    The `python edition` is pre-installed with `shadowsocks-manager`. With the service manager, you can start&stop
-the local service daemon on-the-fly. Check it out from the web admin console `Home › Shadowsocks › Shadowsocks Nodes`, 
-under the `SHADOWSOCKS MANAGERS` tab.
-
-    However the `traffice statistics` and `user port creation status` features are not available for the 
-`python edition`.
-
 
 ## 4. Sendmail (Optional)
 
 `sendmail` is used to send account notification Email, it should
 be configured on the same server with shadowsocks-manager.
 
 About how to configure `sendmail` client to use AWS SES as SMTP server on AWS EC2 instance, refer to repo
@@ -289,23 +286,14 @@
 * The Python edition lacks the `list` commands. A pull request was opened years ago but never merged.
 * The Python edition's `stat` command has a very different way to use, I didn't figure the usage syntax out by looking into the code.
 * The Python edition's `ping` command returns a simple string `pong` rather than a list of ports.
 * The Python edition's `ping` command has to be sent as the syntax: `ping:{}` in order to work if tested with `nc`. It caused by the tailing newline: `ping\n`.
 
 So either you get some change on your own or stick with the libev edition.
 
-### Update for Shadowsocks Python edition on 2024-04
-
-Both the pypi version (2.8.2) and the github master branch (3.0.0) failed to start `ssserver` due to the upstream and dependency changes.
-
-Since the Python edition is pre-installed in this project, mainly for running test cases, I have to make a patch to make it work.
-
-The fix based on github master branch 3.0.0, and would be minimal, just to make the `ssserver` start without any error, no more features added.
-After the fix, the pre-installed Python edition will be changed from the [original pypi version](https://pypi.org/project/shadowsocks/) to [my fork](https://pypi.org/project/shadowsocks-alexforks/).
-
 
 ## 7. Known Issues
 
 1. DNS records matching for Node may not be accurate on macOS.
     For unknown reason sometimes DNS query returns only one IP address
 while multiple IP addresses were configured for the domain.
 
@@ -367,18 +355,46 @@
 
 ### 8.1. Development Environment Setup
 
 1. Install the dependencies
 
     ```sh
     # run memcached, used by django cache
-    docker run -d -p 11211:11211 --name ssm-memcached memcached
+    docker run -d -p 11211:11211 --name ssm-dev-memcached memcached
 
     # run rabbitmq, used by celery
-    docker run -d -p 5672:5672 --name ssm-rabbitmq rabbitmq
+    docker run -d -p 5672:5672 --name ssm-dev-rabbitmq rabbitmq
+
+    # run shadowsocks-libev, simulate localhost node
+    MGR_PORT=6001 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    docker run -d -p 127.0.0.1:$MGR_PORT:$MGR_PORT/UDP \
+        -p 127.0.0.1:$SS_PORTS:$SS_PORTS/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+
+    # get the private IP address of the host, double check the result, it might not be correct
+    PRIVATE_IP=$(ipconfig getifaddr en0 2>/dev/null || hostname -i | awk '{print $1}' 2>/dev/null)
+    echo "PRIVATE_IP=$PRIVATE_IP"
+
+    # run shadowsocks-libev, simulate private IP node
+    MGR_PORT=6002 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
+        -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-private shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+        
+    # run shadowsocks-libev, simulate public IP node
+    MGR_PORT=6003 SS_PORTS=8480 ENCRYPT=aes-256-cfb
+    docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
+        -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-public shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
     ```
 
 1. Link the project code in your workspace to the Python environment
 
     ```sh
     cd shadowsocks-manager
     pip install -e .
@@ -388,26 +404,30 @@
 
     ```sh
     ssm-setup -c -m -l -u admin -p yourpassword
     ```
 
 1. Run the development server
 
+    Make sure the memcached and rabbitmq are running.
+
     ```sh
     ssm-dev-start
     ```
 
 1. Stop the development server
 
     ```sh
     ssm-dev-stop
     ```
 
 1. Test the Django code
 
+    Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
+
     ```sh
     ssm-test -t
     ```
 
 1. Test the Django code with coverage
 
     ```sh
@@ -515,18 +535,34 @@
 
     # uWSGI
     supervisorctl start ssm-uwsgi
 
     # Celery
     supervisorctl start ssm-celery-worker
     supervisorctl start ssm-celery-beat
+
+    # Docker
+    docker ps
     ```
 
-1. Check the listening ports (Linux)
+1. Check the listening ports and processes (Linux)
 
     ```
     # TCP
-    netstat -tan
+    netstat -tanp
 
     # UDP
-    netstat -uan
+    netstat -uanp
+    ```
+
+1. Check the listening ports (MacOS)
+
+    ```
+    # TCP
+    netstat -anp tcp
+
+    # UDP
+    netstat -anp udp
+
+    # find the process by port
+    lsof -i :80 -P
     ```
```

### Comparing `shadowsocks_manager-0.1.3/README.md` & `shadowsocks_manager-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,25 +31,26 @@
 * How's the Shadowsocks supported:
     * libev edition:
         * Full functional.
         * No builtin service manager, you need to install it and start the service by yourself.
     * python edition:
         * Lacks the collection of traffic statistics.
         * Lacks the ability to test user port creation status.
-        * Pre-installed, and have a builtin service manager.
+        * ~~Pre-installed, and have a builtin service manager.~~
+        * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
 Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
+![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
 
 Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
+![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
@@ -67,26 +68,28 @@
 ### 2.2. Manual installation
 
 ```sh
 # create a docker network
 docker network create ssm-network
 
 # run memcached, used by django cache
-docker run -d -p 11211:11211 --network ssm-network --name ssm-memcached memcached
+docker run -d --network ssm-network --name ssm-memcached memcached
 
 # run rabbitmq, used by celery
-docker run -d -p 5672:5672 --network ssm-network --name ssm-rabbitmq rabbitmq
+docker run -d --network ssm-network --name ssm-rabbitmq rabbitmq
 
-# create a directory to store the data, it will be mounted to the container
+# create a directory to store the data, it will be mounted to the shadowsocks-manager container
 mkdir -p ~/ssm-volume
 
 # run the shadowsocks-manager
-docker run -d -p 80:80 --network ssm-network -v ~/ssm-volume:/var/local/ssm --name ssm alexzhangs/shadowsocks-manager \
-           -e SSM_SECRET_KEY=yourkey -e SSM_DEBUG=False -e SSM_MEMCACHED_HOST=ssm-memcached -e SSM_RABBITMQ_HOST=ssm-rabbitmq \
-           -u admin -p yourpassword -M admin@yourdomain.com
+docker run -d -p 80:80 -v ~/ssm-volume:/var/local/ssm \
+    --network ssm-network --name ssm alexzhangs/shadowsocks-manager \
+    -e SSM_SECRET_KEY=yourkey -e SSM_DEBUG=False \
+    -e SSM_MEMCACHED_HOST=ssm-memcached -e SSM_RABBITMQ_HOST=ssm-rabbitmq \
+    -u admin -p yourpassword -M admin@yourdomain.com
 ```
 
 ### 2.3. Install with script
 
 ```sh
 git clone https://github.com/alexzhangs/shadowsocks-manager
 bash shadowsocks-manager/install.sh -u admin -p yourpassword -M admin@yourdomain.com
@@ -109,48 +112,43 @@
 ## 3. Using shadowsocks-manager
 
 1. Shadowsocks server
 
     First, you need to have a Shadowsocks server with the multi-user API
 enabled.
 
-    About how to install and configure Shadowsocks server in AWS, refer
-to the repo
-[aws-ec2-shadowsocks-libev](https://github.com/alexzhangs/aws-ec2-shadowsocks-libev)
-
-    After the server is installed and started, there should be a
-running process named `ss-manager`. Write down the IP address and
-the port that the `ss-manager` is listening on, and also the public IP
-address of the server, the encryption method that Shadowsocks is using,
-they are going to be used in the next step.
+    Install it with docker on the same server with shadowsocks-manager.
+
+    ```sh
+    # run shadowsocks-libev
+    MGR_PORT=6001
+    SS_PORTS=8381-8480
+    ENCRYPT=aes-256-cfb
+    docker run -d -p $SS_PORTS:$SS_PORTS/UDP -p $SS_PORTS:$SS_PORTS \
+        --network ssm-network --name ssm-ss-libev shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+
+    # Use below command to get the private IP address of the shadowsocks-libev container for later configuration.
+    docker inspect ssm-ss-libev | grep IPAddress
+    ```
 
 1. Add Shadowsocks server to shadowsocks-manager
 
     Add the Shadowsocks server as a Node of shadowsocks-manager from
 web admin console: `Home › Shadowsocks › Shadowsocks Nodes`.
 
 1. Create users(ports) and assign Shadowsocks Node
 
     Create users from web admin console: `Home › Shadowsocks ›
 Shadowsocks Accounts` and assign the existing nodes to them.
 
     After a few seconds, the created user ports should be available to your
 Shadowsocks client.
 
-1. The builtin local service manager for Shadowsocks python edition
-
-    There's a builtin local service manager available for the Shadowsocks `python edition`. 
-
-    The `python edition` is pre-installed with `shadowsocks-manager`. With the service manager, you can start&stop
-the local service daemon on-the-fly. Check it out from the web admin console `Home › Shadowsocks › Shadowsocks Nodes`, 
-under the `SHADOWSOCKS MANAGERS` tab.
-
-    However the `traffice statistics` and `user port creation status` features are not available for the 
-`python edition`.
-
 
 ## 4. Sendmail (Optional)
 
 `sendmail` is used to send account notification Email, it should
 be configured on the same server with shadowsocks-manager.
 
 About how to configure `sendmail` client to use AWS SES as SMTP server on AWS EC2 instance, refer to repo
@@ -193,23 +191,14 @@
 * The Python edition lacks the `list` commands. A pull request was opened years ago but never merged.
 * The Python edition's `stat` command has a very different way to use, I didn't figure the usage syntax out by looking into the code.
 * The Python edition's `ping` command returns a simple string `pong` rather than a list of ports.
 * The Python edition's `ping` command has to be sent as the syntax: `ping:{}` in order to work if tested with `nc`. It caused by the tailing newline: `ping\n`.
 
 So either you get some change on your own or stick with the libev edition.
 
-### Update for Shadowsocks Python edition on 2024-04
-
-Both the pypi version (2.8.2) and the github master branch (3.0.0) failed to start `ssserver` due to the upstream and dependency changes.
-
-Since the Python edition is pre-installed in this project, mainly for running test cases, I have to make a patch to make it work.
-
-The fix based on github master branch 3.0.0, and would be minimal, just to make the `ssserver` start without any error, no more features added.
-After the fix, the pre-installed Python edition will be changed from the [original pypi version](https://pypi.org/project/shadowsocks/) to [my fork](https://pypi.org/project/shadowsocks-alexforks/).
-
 
 ## 7. Known Issues
 
 1. DNS records matching for Node may not be accurate on macOS.
     For unknown reason sometimes DNS query returns only one IP address
 while multiple IP addresses were configured for the domain.
 
@@ -271,18 +260,46 @@
 
 ### 8.1. Development Environment Setup
 
 1. Install the dependencies
 
     ```sh
     # run memcached, used by django cache
-    docker run -d -p 11211:11211 --name ssm-memcached memcached
+    docker run -d -p 11211:11211 --name ssm-dev-memcached memcached
 
     # run rabbitmq, used by celery
-    docker run -d -p 5672:5672 --name ssm-rabbitmq rabbitmq
+    docker run -d -p 5672:5672 --name ssm-dev-rabbitmq rabbitmq
+
+    # run shadowsocks-libev, simulate localhost node
+    MGR_PORT=6001 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    docker run -d -p 127.0.0.1:$MGR_PORT:$MGR_PORT/UDP \
+        -p 127.0.0.1:$SS_PORTS:$SS_PORTS/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+
+    # get the private IP address of the host, double check the result, it might not be correct
+    PRIVATE_IP=$(ipconfig getifaddr en0 2>/dev/null || hostname -i | awk '{print $1}' 2>/dev/null)
+    echo "PRIVATE_IP=$PRIVATE_IP"
+
+    # run shadowsocks-libev, simulate private IP node
+    MGR_PORT=6002 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
+        -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-private shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+        
+    # run shadowsocks-libev, simulate public IP node
+    MGR_PORT=6003 SS_PORTS=8480 ENCRYPT=aes-256-cfb
+    docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
+        -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-public shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
     ```
 
 1. Link the project code in your workspace to the Python environment
 
     ```sh
     cd shadowsocks-manager
     pip install -e .
@@ -292,26 +309,30 @@
 
     ```sh
     ssm-setup -c -m -l -u admin -p yourpassword
     ```
 
 1. Run the development server
 
+    Make sure the memcached and rabbitmq are running.
+
     ```sh
     ssm-dev-start
     ```
 
 1. Stop the development server
 
     ```sh
     ssm-dev-stop
     ```
 
 1. Test the Django code
 
+    Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
+
     ```sh
     ssm-test -t
     ```
 
 1. Test the Django code with coverage
 
     ```sh
@@ -419,18 +440,34 @@
 
     # uWSGI
     supervisorctl start ssm-uwsgi
 
     # Celery
     supervisorctl start ssm-celery-worker
     supervisorctl start ssm-celery-beat
+
+    # Docker
+    docker ps
     ```
 
-1. Check the listening ports (Linux)
+1. Check the listening ports and processes (Linux)
 
     ```
     # TCP
-    netstat -tan
+    netstat -tanp
 
     # UDP
-    netstat -uan
+    netstat -uanp
+    ```
+
+1. Check the listening ports (MacOS)
+
     ```
+    # TCP
+    netstat -anp tcp
+
+    # UDP
+    netstat -anp udp
+
+    # find the process by port
+    lsof -i :80 -P
+    ```
```

### Comparing `shadowsocks_manager-0.1.3/bin/ssm-dev-start` & `shadowsocks_manager-0.1.4/bin/ssm-dev-start`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/bin/ssm-setup` & `shadowsocks_manager-0.1.4/bin/ssm-setup`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/bin/ssm-test` & `shadowsocks_manager-0.1.4/bin/ssm-test`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/pyproject.toml` & `shadowsocks_manager-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shadowsocks-manager"
-version = "0.1.3"
+version = "0.1.4"
 requires-python = ">=2.7"
 dependencies = [
     "future",
     "six",
     "boto3",
     "celery",
     "Django<4",
@@ -16,15 +16,15 @@
     "django-allowedsites-dynamic",
 
     "django-cache-lock",
 
     # 20210314 - py2.7 - workaround for: ERROR: Could not find a version that satisfies the requirement django-timezone-field<5.0,>=4.1.0 (from django-celery-beat->-r requirements.txt (line 10)) (from versions: 0.3.1, 0.3.2, 0.4, 1.0, 1.1, 1.2, 1.3, 2.0rc1, 2.0, 2.1, 3.0rc1, 3.0, 3.1)
     "django-celery-beat==1.6.0; python_version <= '2.7'",
     # 20240319 - py3.8 - workaround for: Exception: django-celery-beat 2.6.0 requires CPython 3.8 or later!
-    "django-celery-beat<2.6.0; python_version < '3.8'",
+    "django-celery-beat<2.6.0; python_version > '2.7' and python_version < '3.8'",
     "django-celery-beat; python_version >= '3.8'",
 
     # 20210917 - py2.7 - workaround for: ERROR: django-celery-results 2.2.0 requires celery<6.0,>=5.0, but you'll have celery 4.4.7 which is incompatible.
     "django-celery-results==2.0.1; python_version <= '2.7'",
     "django-celery-results; python_version > '2.7'",
 
     # 20220622 - py2.7 - workaround for: ImportError: No module named enum
@@ -55,18 +55,19 @@
     # "python-memcached==1.59; python_version <= '2.7'",
     # "python-memcached; python_version > '2.7'",
     "python-memcached==1.59",
 
     "pytz",
     "requests",
 
+    # 20240430 - removed. the installation of Shadowsocks service should be handled outside of this project.
     # 20240417 - workaround for: AttributeError: dlsym(0x8c358790, EVP_CIPHER_CTX_cleanup): symbol not found: File python3.12/site-packages/shadowsocks/crypto/openssl.py, line 52
     # 20240417 - py3.10+ - workaround for: AttributeError: module 'collections' has no attribute 'MutableMapping': File python3.12/site-packages/shadowsocks/lru_cache.py, line 34
     # "shadowsocks",
-    "shadowsocks-alexforks",
+    # "shadowsocks-alexforks",
 
     "uWSGI",
 ]
 authors = [{name = "Alex", email = "alexzhangs@gmail.com"}]
 maintainers = []
 readme = "README.md"
 license = {file = "LICENSE"}
@@ -135,15 +136,15 @@
 [tool.setuptools.package-data]
 shadowsocks_manager = ["fixtures/*", "**/fixtures/*", ".env"]
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.bumpversion]
-current_version = "0.1.3"
+current_version = "0.1.4"
 parse = """
     (?P<major>\\d+)\\.
     (?P<minor>\\d+)\\.
     (?P<patch>\\d+)
     (
         \\-                         # separator
         (?P<suffix>[0-9]\\d*)       # suffix Number
```

### Comparing `shadowsocks_manager-0.1.3/setup.cfg` & `shadowsocks_manager-0.1.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shadowsocks-manager
-version = 0.1.3
+version = 0.1.4
 description = A shadowsocks manager for multi-user and traffic statistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Alex
 author_email = alexzhangs@gmail.com
 url = https://github.com/alexzhangs/shadowsocks-manager
 license = MIT
@@ -54,15 +54,15 @@
 	Django<4
 	
 	django-allowedsites-dynamic
 	
 	django-cache-lock
 	
 	django-celery-beat==1.6.0; python_version <= '2.7'
-	django-celery-beat<2.6.0; python_version < '3.8'
+	django-celery-beat<2.6.0; python_version > '2.7' and python_version < '3.8'
 	django-celery-beat; python_version >= '3.8'
 	
 	django-celery-results==2.0.1; python_version <= '2.7'
 	django-celery-results; python_version > '2.7'
 	
 	django-enumfield<3.0; python_version <= '2.7'
 	django-enumfield; python_version > '2.7'
```

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/__main__.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/__init__.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/args_formatter/tests.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/args_formatter/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/admin.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/models.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/serializers.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/tests.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/domain/views.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/domain/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/dynamicmethod/models.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/dynamicmethod/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json` & `shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json` & `shadowsocks_manager-0.1.4/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/manage.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/notification/fixtures/template.json` & `shadowsocks_manager-0.1.4/shadowsocks_manager/notification/fixtures/template.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/notification/models.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/notification/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/notification/tests.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/notification/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/retry/__init__.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/retry/tests.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/retry/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/celery.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/settings.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/settings.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocks_manager/urls.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocks_manager/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/admin.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,28 +53,22 @@
 
 class SSManagerInline(admin.TabularInline):
     model = SSManager
     extra = 1
     max_num = 1
 
     fields = ('interface', 'port', 'encrypt', 'timeout', 'fastopen', 'is_accessible',
-              'server_edition', 'is_v2ray_enabled', 'server_version', 'is_server_enabled', 'server_status',)
-    readonly_fields = ('is_accessible', 'is_v2ray_enabled', 'server_version', 'server_status', 'dt_created', 'dt_updated')
+              'server_edition', 'is_v2ray_enabled',)
+    readonly_fields = ('is_accessible', 'is_v2ray_enabled', 'dt_created', 'dt_updated')
 
     def is_accessible(self, obj):
         return obj.is_accessible
 
     is_accessible.boolean = True
 
-    def server_version(self, obj):
-        return obj.server.version
-
-    def server_status(self, obj):
-        return obj.server.status
-
 
 @admin.register(Node)
 class NodeAdmin(admin.ModelAdmin):
     readonly_fields = ('transferred_totally', 'dt_collected', 'dt_created', 'dt_updated')
     fields = ('name', 'record', 'public_ip', 'private_ip', 'is_active', 'location',)
     list_display = fields + ('is_matching_dns_query',) + readonly_fields
     fields = fields + ('sns_endpoint', 'sns_access_key', 'sns_secret_key',) + readonly_fields
```

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/management/commands/shadowsocks_config.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/models.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,17 @@
 
 
 class Node(StatisticMethod):
     name = models.CharField(unique=True, max_length=32, help_text='Give the node a name.')
     record = models.ForeignKey(Record, null=True, blank=True, on_delete=models.SET_NULL, related_name='nodes',
         help_text='Domain name resolved to the node public IP.')
     public_ip = models.GenericIPAddressField('Public IP', protocol='both', unpack_ipv4=True,
-        unique=True, null=True, blank=True, help_text='Public IP address for the node.')
+        null=True, blank=True, help_text='Public IP address for the node. The non-manager service '
+            'port testing is always based on this IP address since listening on private IP makes no sense. '
+            'So make sure this IP address is set, even as 127.0.0.1 or a private IP address for testing nodes.')
     private_ip = models.GenericIPAddressField('Private IP', protocol='both', unpack_ipv4=True,
         null=True, blank=True, help_text='Private IP address for the node.')
     location = models.CharField(max_length=64, null=True, blank=True,
         help_text='Geography location for the node, appears in the account notification '
             'Email if not blank, example: Hongkong.')
     is_active = models.BooleanField(default=True, help_text='Is this node ready to be online')
     sns_endpoint = models.CharField(max_length=128, null=True, blank=True,
@@ -537,29 +539,28 @@
     interface = enum.EnumField(InterfaceList, default=InterfaceList.LOCALHOST,
         help_text='Network interface bound to Manager API on the node, use an internal '
             'interface if possible.')
     port = models.PositiveIntegerField(default=6001,
         help_text='Port number bound to Manager API.')
     encrypt = models.CharField(max_length=32, default='aes-256-cfb',
         help_text='Encrypt method: rc4-md5, aes-128-gcm, aes-192-gcm, aes-256-gcm, '
-        'aes-128-cfb, aes-192-cfb, aes-256-cfb, aes-128-ctr, aes-192-ctr, aes-256-ctr, '
-        'camellia-128-cfb, camellia-192-cfb, camellia-256-cfb, bf-cfb, chacha20-ietf-poly1305, '
-        'xchacha20-ietf-poly1305, salsa20, chacha20 and chacha20-ietf.')
+            'aes-128-cfb, aes-192-cfb, aes-256-cfb, aes-128-ctr, aes-192-ctr, aes-256-ctr, '
+            'camellia-128-cfb, camellia-192-cfb, camellia-256-cfb, bf-cfb, chacha20-ietf-poly1305, '
+            'xchacha20-ietf-poly1305, salsa20, chacha20 and chacha20-ietf. '
+            'The changes made here will not affect the plugin status on server.')
     timeout = models.PositiveIntegerField(default=30,
-        help_text='Socket timeout in seconds for Shadowsocks client.')
+        help_text='Socket timeout in seconds for Shadowsocks client. '
+            'The changes made here will not affect the plugin status on server.')
     fastopen = models.BooleanField('Fast Open', default=False,
         help_text='Enable TCP fast open, with Linux kernel > 3.7.0.')
     server_edition = enum.EnumField(ServerEditionList, default=ServerEditionList.LIBEV,
         help_text='The Shadowsocks server edition. The libev edition is recommended.')
     is_v2ray_enabled = models.BooleanField(default=False,
         help_text='Whether the v2ray-plugin is enabled for Shadowsocks server. The changes made here will not '
             'affect the plugin status on server.')
-    is_server_enabled = models.BooleanField(default=False,
-        help_text='Control the Shadowsocks server up or down. Works only with the Shadowsocks python edition '
-            'local node.')
     dt_created = models.DateTimeField('Created', auto_now_add=True)
     dt_updated = models.DateTimeField('Updated', auto_now=True)
 
     class Meta:
         verbose_name = 'Shadowsocks Manager'
 
     def __str__(self):
@@ -571,22 +572,14 @@
         self._original_server_edition = self.server_edition
 
     def clean(self):
         if not self._ip:
             raise ValidationError({
                 self.node.get_ip_field_by_interface(self.interface):
                 [_('There is no IP address set for selected interface on the node.')]})
-        if self.is_server_enabled and self.server_edition != ServerEditionList.PYTHON:
-            raise ValidationError({
-                'is_server_enabled':
-                [_('is_server_enabled was set without Shadowsocks python edition.')]})
-
-    @property
-    def server(self):
-        return SSServer(self)
 
     @property
     def _ip(self):
         """
         Return the node's IP address on the network interface that the Manager API is listening on.
         """
         return self.node.get_ip_by_interface(self.interface)
@@ -804,33 +797,27 @@
         """
         Test if the manager is in service.
         Internally using ping_ex().
         """
         return self.ping_ex() is not None
 
     def on_update(self):
-        if self.server_edition != self._original_server_edition and self._original_server_edition == ServerEditionList.PYTHON:
-            self.server.stop()
-            self.clear_cache()
-            NodeAccount.clear_caches(node=self.node)
-        if self.server_edition == ServerEditionList.PYTHON:
-            if self.is_server_enabled:
-                self.server.restart()
-            else:
-                self.server.stop()
-            self.clear_cache()
-            NodeAccount.clear_caches(node=self.node)
+        self.clear_cache()
+        NodeAccount.clear_caches(node=self.node)
 
     def on_delete(self):
-        self.server.stop()
         self.clear_cache()
         NodeAccount.clear_caches(node=self.node)
 
 
-class SSServer(object):
+class SSServer(object):  # pragma: no cover
+    """
+    This class is used to manage the local Shadowsocks server python edition.
+    The usage of this class is removed from the SSManager model.
+    """
 
     def __init__(self, manager, *args, **kwargs):
         super(SSServer, self).__init__(*args, **kwargs)
         self.manager = manager
         # the lift_pip_shadowsocks is no longer needed after the django app shadowsocks was renamed to shadowsocksz
         # self.lift_pip_shadowsocks()
 
@@ -839,15 +826,16 @@
 
     def logfile(self, original=False):
         return '/tmp/shadowsocks-{}.log'.format(self.manager._original_port if original else self.manager.port)
 
     @classmethod
     def lift_pip_shadowsocks(cls):
         """
-        Workaround for the package naming conflict between the Django app `shadowsocks` and the pip package `shadowsocks`.
+        Workaround for the package naming conflict between the Django app `shadowsocks` and the Shadowsocks
+        python editon installed with pip package `shadowsocks`.
         Lower the searching priority of the Django project app home dir in sys.path.
         """
         import shadowsocks
         # get the package's path
         p = shadowsocks.__path__[0]
         if not p.endswith('/shadowsocks_manager/shadowsocks'):
             # shadowsocks is not referring to the Django app, nothing to do
@@ -875,14 +863,22 @@
         if flag:
             # add the Django project app home dir back to the end
             os.putenv('PYTHONPATH', ':'.join(pythonpath + sys.path + [p]))
 
         # unimport the package
         del sys.modules['shadowsocks']
 
+    @classmethod
+    def random_password(cls, length=16):
+        """
+        Return a random password string.
+        """
+        import random, string
+        return ''.join(random.choices(string.ascii_letters + string.digits, k=length))
+
     def call(self, command, *args, **kwargs):
         """
         Call Shadowsocks server command by subprocess.Popen().
         Return (exit_code, stdout, stderr)
         """
         proc = subprocess.Popen(command, *args, stdout=PIPE, stderr=PIPE,
                                 **kwargs)
@@ -950,15 +946,19 @@
         """
         command = [
             'ssserver',
             '--pid-file', self.pidfile(),
             '--log-file', self.logfile(),
             '-d', 'start',
             '--manager-address', '{}:{}'.format(self.manager._ip, self.manager.port),  # the options order matters
-            '-k', 'passw0rd',
+            # The shadowsocks python edition does not support to run the manager without a server port.
+            # So, the server port is set to 65500, which is not supposed to be used by any client.
+            # And the password is set to a random string, which is not supposed to be known by any client.
+            '-p 65500',  
+            '-k', self.random_password(),
             '-m', self.manager.encrypt,
             '-t', str(self.manager.timeout),
             '--fast-open', str(self.manager.fastopen),
         ]
         """
         * close_fds=True: For Python 2.7, should not inherit the parent process's fds. The inherit fds won't be released
                           after the parent process was exited but the child process remains.
```

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/serializers.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,11 +31,11 @@
         model = models.NodeAccount
         fields = ('id', 'node', 'account', 'is_active', 'dt_created', 'dt_updated')
 
 
 class SSManagerSerializer(serializers.ModelSerializer):
     class Meta:
         model = models.SSManager
-        fields = ('id', 'node', 'interface', 'port', 'encrypt', 'timeout', 'fastopen', 'server_edition', 'is_v2ray_enabled', 'is_server_enabled', 'dt_created', 'dt_updated')
+        fields = ('id', 'node', 'interface', 'port', 'encrypt', 'timeout', 'fastopen', 'server_edition', 'is_v2ray_enabled', 'dt_created', 'dt_updated')
 
     interface = EnumField(models.InterfaceList)
     server_edition = EnumField(models.ServerEditionList)
```

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/tests.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 
 import logging
 # disable logging for the test module to make the output clean
 logging.disable(logging.CRITICAL)
 
 
 import socket
-def get_ip():
+def get_local_ip():
     """
     Get the local ip address.
     https://github.com/mayermakes/Get_IP
     """
     ip = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         ip.connect(('10.255.255.255', 1))
         IP = ip.getsockname()[0]
     except:
-        IP = '127.0.0.1'
+        raise
     finally:
         ip.close()
     return IP
-ip = get_ip()
+local_ip = get_local_ip()
 
 
 """
 Feature matrix for methods in unittest.TestCase class:
 +-------------+------------------+---------------------+----------------+----------------------------------+---------------------------+
 | Provider    | Method           | When is Called      | Class Method   | Manual Cleanup Needed            | When is Cleanup Done      |
 +=============+==================+=====================+================+==================================+===========================+
@@ -159,23 +159,22 @@
 class AccountTestCase(AppTestCase):
     @classmethod
     def up(cls):
         config = models.Config.load()
 
         # generate 2 accounts
         for port in [config.port_begin, config.port_end]:
-            obj = models.Account(
+            models.Account(
                 username=port,
                 password='mock-password',
                 email='mock@mock-example.com',
                 first_name=str(port),
                 last_name='mock',
                 is_active=True,
-            )
-            obj.save()
+            ).save()
 
     @classmethod
     def setUpTestData(cls):
         cls.allup()
 
     def test_account_clean_less(self):
         obj = models.Account.objects.first()
@@ -184,28 +183,43 @@
 
     def test_account_clean_great(self):
         obj = models.Account.objects.last()
         obj.username = str(int(obj.username) + 1)  # set the port out of the config range
         self.assertRaises(ValidationError, obj.clean)
 
     def test_account_port_accessible(self):
-        # The ssserver's live ports are affected by the ssmanager's restart comes from the other test cases.
         # Perform the heartbeat once to recreate the ssmanager ports.
         # Seems that the rollback performed by django.test.TestCase.setUpTestData() method's isolation mechanism
-        # doesn't trigger the django's signal mechanism, so the ssserver ports are not created.
+        # doesn't trigger the django's signal mechanism, so the shadowsocks ports are not created.
         models.NodeAccount.heartbeat()
 
-        for obj in models.Account.objects.all():
-            self.assertTrue(obj.nodes_ref.get(node__name='localhost').is_accessible_ex())
+        for accout in models.Account.objects.all():
+            for na in accout.nodes_ref.all():
+                self.assertTrue(na.is_accessible)
+
+    def test_account_port_accessible_ex(self):
+        models.NodeAccount.heartbeat()
+
+        for accout in models.Account.objects.all():
+            for na in accout.nodes_ref.all():
+                self.assertTrue(na.is_accessible_ex())
 
     def test_account_port_accessible_after_update(self):
         obj = models.Account.objects.first()
         obj.username = str(int(obj.username) + 1)
         obj.save()
-        self.assertTrue(obj.nodes_ref.get(node__name='localhost').is_accessible_ex())
+        for na in obj.nodes_ref.all():
+            self.assertTrue(na.is_accessible)
+
+    def test_account_port_accessible_ex_after_update(self):
+        obj = models.Account.objects.first()
+        obj.username = str(int(obj.username) + 1)
+        obj.save()
+        for na in obj.nodes_ref.all():
+            self.assertTrue(na.is_accessible_ex())
 
     def test_account_notify(self):
         for obj in models.Account.objects.all():
             self.assertTrue(obj.notify(sender=obj))
 
     def test_account_notify_validation_email(self):
         obj = models.Account.objects.first()
@@ -213,37 +227,14 @@
         self.assertRaisesRegex(ValidationError, 'email', obj.notify, sender=obj)
 
     def test_account_notify_validation_is_active(self):
         obj = models.Account.objects.first()
         obj.is_active = False
         self.assertRaisesRegex(ValidationError, 'is_active', obj.notify, sender=obj)
 
-    def test_account_toggle_active(self):
-        # make all accounts inactive
-        for obj in models.Account.objects.all():
-            obj.toggle_active()
-            self.assertFalse(obj.is_active)
-
-        # all nas are inactive now
-        for na in models.NodeAccount.objects.all():
-            self.assertFalse(na.is_active)
-
-        # make all accounts active
-        for obj in models.Account.objects.all():
-            obj.toggle_active()
-            self.assertTrue(obj.is_active)
-
-        # all nas are active now
-        for na in models.NodeAccount.objects.all():
-            self.assertTrue(na.is_active)
-
-    def test_account_serializer(self):
-        obj = serializers.AccountSerializer()
-        json.loads(json.dumps(obj.to_representation(models.Account.objects.first())))
-
     def test_account_notify_validation_node(self):
         # make all nodes inactive
         for node in models.Node.objects.all():
             node.is_active = False
             node.save()
         obj = models.Account.objects.first()
         self.assertRaisesRegex(ValidationError, 'no active node', obj.notify, sender=obj)
@@ -260,75 +251,99 @@
         # make all nodes' record None
         for node in models.Node.objects.all():
             node.record = None
             node.save()
         obj = models.Account.objects.first()
         self.assertTrue(obj.notify(sender=obj))
 
+    def test_account_toggle_active(self):
+        # make all accounts inactive
+        for obj in models.Account.objects.all():
+            obj.toggle_active()
+            self.assertFalse(obj.is_active)
+
+        # all nas are inactive now
+        for na in models.NodeAccount.objects.all():
+            self.assertFalse(na.is_active)
+
+        # make all accounts active
+        for obj in models.Account.objects.all():
+            obj.toggle_active()
+            self.assertTrue(obj.is_active)
+
+        # all nas are active now
+        for na in models.NodeAccount.objects.all():
+            self.assertTrue(na.is_active)
+
+    def test_account_serializer(self):
+        obj = serializers.AccountSerializer()
+        json.loads(json.dumps(obj.to_representation(models.Account.objects.first())))
+
 
 class NodeTestCase(AppTestCase):
     @classmethod
     def up(cls):
-        DomainAppTestCase.allup()
-        record = Record.objects.first()
-
-        # generate one localhost node
-        obj = models.Node(
-            name='localhost',
+        # add a ss-libev node for the ssmanager listening on localhost
+        models.Node(
+            name='ss-libev-localhost',
             record=None,
-            public_ip=ip,
-            private_ip=ip,
+            public_ip='127.0.0.1',
+            private_ip='127.0.0.1',
             location='Local',
-            sns_endpoint=None,
-            sns_access_key=None,
-            sns_secret_key=None,
+            sns_endpoint='arn:aws:sns:ap-northeast-1:0:topic', # mock sns endpoint
+            sns_access_key='mock-sns_access_key',
+            sns_secret_key='mock-sns_secret_key',
             is_active=True,
-        )
-        obj.save()
+        ).save()
 
-        # generate 2 mock nodes
-        for i in list(range(1, 3)):
-            obj = models.Node(
-                name='mock-node-{}'.format(i),
-                record=record,
-                public_ip='.'.join([str(i) for j in list(range(4))]), # mock ip address here
-                private_ip=ip,
-                location='mock-locaction-{}'.format(i),
-                sns_endpoint='arn:aws:sns:ap-northeast-1:{}:topic'.format(i), # mock sns endpoint
-                sns_access_key='mock-sns_access_key-{}'.format(i),
-                sns_secret_key='mock-sns_secret_key-{}'.format(i),
-                is_active=True,
-            )
-            obj.save()
+        # add a ss-libev node for the ssmanager listening on private ip
+        models.Node(
+            name='ss-libev-private',
+            record=None,
+            public_ip=local_ip,
+            private_ip=local_ip,
+            location='Private',
+            sns_endpoint='arn:aws:sns:ap-northeast-1:0:topic', # mock sns endpoint
+            sns_access_key='mock-sns_access_key',
+            sns_secret_key='mock-sns_secret_key',
+            is_active=True,
+        ).save()
+
+        DomainAppTestCase.allup()
+        record = Record.objects.first()
+        # add a ss-libev node for the ssmanager listening on public ip
+        models.Node(
+            name='ss-libev-public',
+            record=record,
+            public_ip=local_ip,  # using private ip as public ip
+            private_ip=local_ip,
+            location='Public',
+            sns_endpoint='arn:aws:sns:ap-northeast-1:0:topic', # mock sns endpoint
+            sns_access_key='mock-sns_access_key',
+            sns_secret_key='mock-sns_secret_key',
+            is_active=True,
+        ).save()
 
     @classmethod
     def setUpTestData(cls):
         cls.allup()
 
-    def test_node_is_matching_record(self):
-        for obj in models.Node.objects.all():
-            if obj.record:
-                self.assertTrue(obj.is_matching_record)
-            else:
-                self.assertFalse(obj.is_matching_record)
+    def test_node_is_matching_record_positive(self):
+        for obj in models.Node.objects.filter(record__isnull=False):
+            self.assertTrue(obj.is_matching_record)
+
+    def test_node_is_matching_record_negative(self):
+        for obj in models.Node.objects.filter(record__isnull=True):
+            self.assertFalse(obj.is_matching_record)
 
-    def test_node_is_matching_dns_query(self):
+    def test_node_is_matching_dns_query_negitive(self):
         for obj in models.Node.objects.all():
             self.assertFalse(obj.is_matching_dns_query)
 
-    def test_node_record_sync(self):
-        # ip addresses are synced between node and record
-        for obj in models.Node.objects.filter(record__isnull=False):
-            self.assertTrue(obj.is_matching_record)
-
     def test_node_toggle_active(self):
-        # all nas are active before test
-        for na in models.NodeAccount.objects.all():
-            self.assertTrue(na.is_active)
-
         # make all nodes inactive
         for obj in models.Node.objects.all():
             obj.toggle_active()
             self.assertFalse(obj.is_active)
 
         # all nas are inactive now
         for na in models.NodeAccount.objects.all():
@@ -342,15 +357,16 @@
         # all nas are active now
         for na in models.NodeAccount.objects.all():
             self.assertTrue(na.is_active)
 
     def test_node_record_sync(self):
         # change nodes's public_ip
         for obj in models.Node.objects.filter(record__isnull=False):
-            obj.public_ip = '.'.join(str(int(part)+100) for part in obj.public_ip.split('.'))
+            # plus 1 to the last part of public ip address
+            obj.public_ip = '.'.join(obj.public_ip.split('.')[0:3] + [str(int(obj.public_ip.split('.')[-1]) + 1)])
             obj.save()
             self.assertTrue(obj.is_matching_record)
 
     def test_node_record_sync_after_toggle_active(self):
         # make nodes inactive
         for obj in models.Node.objects.filter(record__isnull=False):
             obj.toggle_active()
@@ -365,101 +381,122 @@
         obj = serializers.NodeSerializer()
         json.loads(json.dumps(obj.to_representation(models.Node.objects.first())))
 
 
 class NodeAccountTestCase(AppTestCase):
     @classmethod
     def up(cls):
-        # add the localhost node to all accounts
-        for account in models.Account.objects.all():
-            node = models.Node.objects.get(name='localhost')
-            if models.NodeAccount.objects.filter(node=node, account=account).count() == 0:
-                na = models.NodeAccount(node=node, account=account, is_active=(account.is_active and node.is_active))
-                na.save()
+        # Add the first account to the localhost node and the private node
+        account = models.Account.objects.all().first()
+        node = models.Node.objects.get(name='ss-libev-localhost')
+        na = models.NodeAccount(node=node, account=account, is_active=(account.is_active and node.is_active))
+        na.save()
+
+        node = models.Node.objects.get(name='ss-libev-private')
+        na = models.NodeAccount(node=node, account=account, is_active=(account.is_active and node.is_active))
+        na.save()
+        
+        # Add the last account to the public node
+        # The public node is using the private ip to mock public ip, using different account to avoid the port conflict
+        account = models.Account.objects.all().last()
+        node = models.Node.objects.get(name='ss-libev-public')
+        na = models.NodeAccount(node=node, account=account, is_active=(account.is_active and node.is_active))
+        na.save()
 
     @classmethod
     def setUpTestData(cls):
         cls.allup()
 
     def test_nodeaccount_is_accessible_positive(self):
-        models.NodeAccount.heartbeat()
-        # get the nas that have node.ssmanager listening on localhost
-        for obj in models.NodeAccount.objects.filter(node__ssmanagers__interface=models.InterfaceList.LOCALHOST):
+        #models.NodeAccount.heartbeat()
+        for obj in models.NodeAccount.objects.all():
+            self.assertTrue(obj.is_accessible)
+
+    def test_nodeaccount_is_accessible_ex_positive(self):
+        #models.NodeAccount.heartbeat()
+        for obj in models.NodeAccount.objects.all():
             self.assertTrue(obj.is_accessible_ex())
 
-    def test_nodeaccount_is_accessible_negative(self):
-        # get the nas that don't have node.ssmanager listening on localhost
-        for obj in models.NodeAccount.objects.exclude(node__ssmanagers__interface=models.InterfaceList.LOCALHOST):
-            self.assertFalse(obj.is_accessible_ex())
-
     def test_nodeaccount_is_created(self):
-        # get the nas that have node.ssmanager listening on localhost
-        for obj in models.NodeAccount.objects.filter(node__ssmanagers__interface=models.InterfaceList.LOCALHOST):
-            # the Shadowsocks python edition's list command doesn't work, so the is_created() method is always None
-            self.assertFalse(obj.is_created())
+        for obj in models.NodeAccount.objects.all():
+            self.assertTrue(obj.is_created())
 
     def test_nodeaccount_serializer(self):
         obj = serializers.NodeAccountSerializer()
         json.loads(json.dumps(obj.to_representation(models.NodeAccount.objects.first())))
 
 
 class SSManagerTestCase(AppTestCase):
     @classmethod
     def up(cls):
-        # add a ssmanager to localhost node, using python edition, auto install&start
-        obj = models.SSManager(
-            node=models.Node.objects.get(name='localhost'),
+        # Add a libev edition manager to the localhost node
+        # Make sure this manager is running and accessible at localhost before the test.
+        # Example command:
+        # MGR_PORT=6001 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+        # docker run -d -p 127.0.0.1:$MGR_PORT:$MGR_PORT/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS \
+        #   --name ssm-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
+        #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+
+        models.SSManager(
+            node=models.Node.objects.get(name='ss-libev-localhost'),
             interface=models.InterfaceList.LOCALHOST,
             port=6001,
             fastopen=False,
             encrypt='aes-256-cfb',
-            server_edition=models.ServerEditionList.PYTHON,
+            server_edition=models.ServerEditionList.LIBEV,
             is_v2ray_enabled=False,
-            is_server_enabled=True,
-        )
-        obj.save()
+        ).save()
 
-        # add a ssmanager to each mock node, using libev edition
-        for node in models.Node.objects.exclude(name='localhost'):
-            obj = models.SSManager(
-                node=node,
-                interface=node.pk % 2 + 2,  # limit the interface within: [2, 3]
-                port=6001,
-                fastopen=False,
-                encrypt='aes-256-cfb',
-                server_edition=models.ServerEditionList.LIBEV,
-                is_v2ray_enabled=False,
-            )
-            obj.save()
+        # Add a libev edition manager to the private node
+        # Make sure this manager is running and accessible at private ip before the test.
+        # Example command:
+        # MGR_PORT=6002 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+        # docker run -d -p <private_ip>:$MGR_PORT:$MGR_PORT/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS \
+        #   --name ssm-ss-libev-private shadowsocks/shadowsocks-libev:edge \
+        #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+        models.SSManager(
+            node=models.Node.objects.get(name='ss-libev-private'),
+            interface=models.InterfaceList.PRIVATE,
+            port=6002,
+            fastopen=False,
+            encrypt='aes-256-cfb',
+            server_edition=models.ServerEditionList.LIBEV,
+            is_v2ray_enabled=False,
+        ).save()
+
+        # Add a libev edition manager to the public node
+        # Make sure this manager is running and accessible at private ip before the test.
+        # Example command:
+        # MGR_PORT=6003 SS_PORTS=8480 ENCRYPT=aes-256-cfb
+        # docker run -d -p <private_ip>:$MGR_PORT:$MGR_PORT/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS \
+        #   --name ssm-ss-libev-public shadowsocks/shadowsocks-libev:edge \
+        #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+        models.SSManager(
+            node=models.Node.objects.get(name='ss-libev-public'),
+            interface=models.InterfaceList.PUBLIC,
+            port=6003,
+            fastopen=False,
+            encrypt='aes-256-cfb',
+            server_edition=models.ServerEditionList.LIBEV,
+            is_v2ray_enabled=False,
+        ).save()
 
     @classmethod
     def setUpTestData(cls):
         cls.allup()
 
     def test_ssmanager_is_accessible(self):
-        obj = models.SSManager.objects.filter(interface=models.InterfaceList.LOCALHOST).first()
-        self.assertTrue(obj.is_accessible)
-
-    def test_ssmanager_is_server_enabled(self):
-        obj = models.SSManager.objects.filter(interface=models.InterfaceList.LOCALHOST).first()
-        self.assertTrue(obj.is_server_enabled)
-
-    def test_ssmanager_server_version(self):
-        obj = models.SSManager.objects.filter(interface=models.InterfaceList.LOCALHOST).first()
-        #self.assertTrue(obj.server.version)
-
-    def test_ssmanager_server_status(self):
-        obj = models.SSManager.objects.filter(interface=models.InterfaceList.LOCALHOST).first()
-        self.assertTrue(re.match('(running|sleeping)', obj.server.status or ''))
+        for obj in models.SSManager.objects.all():
+            self.assertTrue(obj.is_accessible)
 
     def test_ssmanager_add_and_remove(self):
-        obj = models.SSManager.objects.filter(interface=models.InterfaceList.LOCALHOST).first()
-        port=8388
-        obj.add(port, 'mock-password')
-        self.assertTrue(obj.is_port_created_or_accessible(port))
+        for obj in models.SSManager.objects.all():
+            port=8388
+            obj.add(port, 'mock-password')
+            self.assertTrue(obj.is_port_created_or_accessible(port))
 
         obj.remove(port)
         self.assertFalse(obj.is_port_created_or_accessible(port))
 
     def test_ssmanager_clean(self):
         obj = models.SSManager.objects.filter(interface=models.InterfaceList.PUBLIC).first()
         obj.node.public_ip = None
```

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/urls.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/shadowsocksz/views.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/shadowsocksz/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,8 +46,8 @@
 
 class SSManagerViewSet(viewsets.ModelViewSet):
     """
     This viewset automatically provides `list` and `detail` actions.
     """
     queryset = models.SSManager.objects.all()
     serializer_class = serializers.SSManagerSerializer
-    filter_fields = ['node', 'node__name', 'server_edition', 'is_v2ray_enabled', 'is_server_enabled']
+    filter_fields = ['node', 'node__name', 'server_edition', 'is_v2ray_enabled']
```

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/singleton/models.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/singleton/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/admin.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/models.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/serializers.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/tests.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/statistic/views.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/statistic/views.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/utils/celery.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/utils/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/utils/createsuperuser.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/utils/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/utils/dotenv.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager/utils/manage.py` & `shadowsocks_manager-0.1.4/shadowsocks_manager/utils/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/PKG-INFO` & `shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.3
+Version: 0.1.4
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
@@ -60,15 +60,15 @@
 Requires-Dist: six
 Requires-Dist: boto3
 Requires-Dist: celery
 Requires-Dist: Django<4
 Requires-Dist: django-allowedsites-dynamic
 Requires-Dist: django-cache-lock
 Requires-Dist: django-celery-beat==1.6.0; python_version <= "2.7"
-Requires-Dist: django-celery-beat<2.6.0; python_version < "3.8"
+Requires-Dist: django-celery-beat<2.6.0; python_version > "2.7" and python_version < "3.8"
 Requires-Dist: django-celery-beat; python_version >= "3.8"
 Requires-Dist: django-celery-results==2.0.1; python_version <= "2.7"
 Requires-Dist: django-celery-results; python_version > "2.7"
 Requires-Dist: django-enumfield<3.0; python_version <= "2.7"
 Requires-Dist: django-enumfield; python_version > "2.7"
 Requires-Dist: django-filter~=1.1; python_version <= "2.7"
 Requires-Dist: django-filter; python_version > "2.7"
@@ -79,15 +79,14 @@
 Requires-Dist: psutil
 Requires-Dist: python-crontab==2.6.0; python_version <= "2.7"
 Requires-Dist: python-crontab; python_version > "2.7"
 Requires-Dist: python-decouple
 Requires-Dist: python-memcached==1.59
 Requires-Dist: pytz
 Requires-Dist: requests
-Requires-Dist: shadowsocks-alexforks
 Requires-Dist: uWSGI
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: codecov-cli; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -127,25 +126,26 @@
 * How's the Shadowsocks supported:
     * libev edition:
         * Full functional.
         * No builtin service manager, you need to install it and start the service by yourself.
     * python edition:
         * Lacks the collection of traffic statistics.
         * Lacks the ability to test user port creation status.
-        * Pre-installed, and have a builtin service manager.
+        * ~~Pre-installed, and have a builtin service manager.~~
+        * No builtin service manager, you need to install it and start the service by yourself.
 
 Code in Python, base on Django, Django REST framework, Celery, and SQLite.
 
 The development status can be found at: [project home](https://github.com/alexzhangs/shadowsocks-manager/projects/1).
 
 Node List:
-![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-list.png)
+![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-list.png)
 
 Node's Shadowsocks Manager:
-![Home › Shadowsocks › Shadowsocks Nodes](https://www.0xbeta.com/shadowsocks-manager/assets/images/shadowsocks-node-ssmanager.png)
+![Home › Shadowsocks › Shadowsocks Nodes](/assets/images/shadowsocks-node-ssmanager.png)
 
 
 ## 1. Requirements
 
 * Python 2.7, Python 3.x
 * Django 1.11.x, Django 3.x
 * Docker
@@ -163,26 +163,28 @@
 ### 2.2. Manual installation
 
 ```sh
 # create a docker network
 docker network create ssm-network
 
 # run memcached, used by django cache
-docker run -d -p 11211:11211 --network ssm-network --name ssm-memcached memcached
+docker run -d --network ssm-network --name ssm-memcached memcached
 
 # run rabbitmq, used by celery
-docker run -d -p 5672:5672 --network ssm-network --name ssm-rabbitmq rabbitmq
+docker run -d --network ssm-network --name ssm-rabbitmq rabbitmq
 
-# create a directory to store the data, it will be mounted to the container
+# create a directory to store the data, it will be mounted to the shadowsocks-manager container
 mkdir -p ~/ssm-volume
 
 # run the shadowsocks-manager
-docker run -d -p 80:80 --network ssm-network -v ~/ssm-volume:/var/local/ssm --name ssm alexzhangs/shadowsocks-manager \
-           -e SSM_SECRET_KEY=yourkey -e SSM_DEBUG=False -e SSM_MEMCACHED_HOST=ssm-memcached -e SSM_RABBITMQ_HOST=ssm-rabbitmq \
-           -u admin -p yourpassword -M admin@yourdomain.com
+docker run -d -p 80:80 -v ~/ssm-volume:/var/local/ssm \
+    --network ssm-network --name ssm alexzhangs/shadowsocks-manager \
+    -e SSM_SECRET_KEY=yourkey -e SSM_DEBUG=False \
+    -e SSM_MEMCACHED_HOST=ssm-memcached -e SSM_RABBITMQ_HOST=ssm-rabbitmq \
+    -u admin -p yourpassword -M admin@yourdomain.com
 ```
 
 ### 2.3. Install with script
 
 ```sh
 git clone https://github.com/alexzhangs/shadowsocks-manager
 bash shadowsocks-manager/install.sh -u admin -p yourpassword -M admin@yourdomain.com
@@ -205,48 +207,43 @@
 ## 3. Using shadowsocks-manager
 
 1. Shadowsocks server
 
     First, you need to have a Shadowsocks server with the multi-user API
 enabled.
 
-    About how to install and configure Shadowsocks server in AWS, refer
-to the repo
-[aws-ec2-shadowsocks-libev](https://github.com/alexzhangs/aws-ec2-shadowsocks-libev)
-
-    After the server is installed and started, there should be a
-running process named `ss-manager`. Write down the IP address and
-the port that the `ss-manager` is listening on, and also the public IP
-address of the server, the encryption method that Shadowsocks is using,
-they are going to be used in the next step.
+    Install it with docker on the same server with shadowsocks-manager.
+
+    ```sh
+    # run shadowsocks-libev
+    MGR_PORT=6001
+    SS_PORTS=8381-8480
+    ENCRYPT=aes-256-cfb
+    docker run -d -p $SS_PORTS:$SS_PORTS/UDP -p $SS_PORTS:$SS_PORTS \
+        --network ssm-network --name ssm-ss-libev shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+
+    # Use below command to get the private IP address of the shadowsocks-libev container for later configuration.
+    docker inspect ssm-ss-libev | grep IPAddress
+    ```
 
 1. Add Shadowsocks server to shadowsocks-manager
 
     Add the Shadowsocks server as a Node of shadowsocks-manager from
 web admin console: `Home › Shadowsocks › Shadowsocks Nodes`.
 
 1. Create users(ports) and assign Shadowsocks Node
 
     Create users from web admin console: `Home › Shadowsocks ›
 Shadowsocks Accounts` and assign the existing nodes to them.
 
     After a few seconds, the created user ports should be available to your
 Shadowsocks client.
 
-1. The builtin local service manager for Shadowsocks python edition
-
-    There's a builtin local service manager available for the Shadowsocks `python edition`. 
-
-    The `python edition` is pre-installed with `shadowsocks-manager`. With the service manager, you can start&stop
-the local service daemon on-the-fly. Check it out from the web admin console `Home › Shadowsocks › Shadowsocks Nodes`, 
-under the `SHADOWSOCKS MANAGERS` tab.
-
-    However the `traffice statistics` and `user port creation status` features are not available for the 
-`python edition`.
-
 
 ## 4. Sendmail (Optional)
 
 `sendmail` is used to send account notification Email, it should
 be configured on the same server with shadowsocks-manager.
 
 About how to configure `sendmail` client to use AWS SES as SMTP server on AWS EC2 instance, refer to repo
@@ -289,23 +286,14 @@
 * The Python edition lacks the `list` commands. A pull request was opened years ago but never merged.
 * The Python edition's `stat` command has a very different way to use, I didn't figure the usage syntax out by looking into the code.
 * The Python edition's `ping` command returns a simple string `pong` rather than a list of ports.
 * The Python edition's `ping` command has to be sent as the syntax: `ping:{}` in order to work if tested with `nc`. It caused by the tailing newline: `ping\n`.
 
 So either you get some change on your own or stick with the libev edition.
 
-### Update for Shadowsocks Python edition on 2024-04
-
-Both the pypi version (2.8.2) and the github master branch (3.0.0) failed to start `ssserver` due to the upstream and dependency changes.
-
-Since the Python edition is pre-installed in this project, mainly for running test cases, I have to make a patch to make it work.
-
-The fix based on github master branch 3.0.0, and would be minimal, just to make the `ssserver` start without any error, no more features added.
-After the fix, the pre-installed Python edition will be changed from the [original pypi version](https://pypi.org/project/shadowsocks/) to [my fork](https://pypi.org/project/shadowsocks-alexforks/).
-
 
 ## 7. Known Issues
 
 1. DNS records matching for Node may not be accurate on macOS.
     For unknown reason sometimes DNS query returns only one IP address
 while multiple IP addresses were configured for the domain.
 
@@ -367,18 +355,46 @@
 
 ### 8.1. Development Environment Setup
 
 1. Install the dependencies
 
     ```sh
     # run memcached, used by django cache
-    docker run -d -p 11211:11211 --name ssm-memcached memcached
+    docker run -d -p 11211:11211 --name ssm-dev-memcached memcached
 
     # run rabbitmq, used by celery
-    docker run -d -p 5672:5672 --name ssm-rabbitmq rabbitmq
+    docker run -d -p 5672:5672 --name ssm-dev-rabbitmq rabbitmq
+
+    # run shadowsocks-libev, simulate localhost node
+    MGR_PORT=6001 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    docker run -d -p 127.0.0.1:$MGR_PORT:$MGR_PORT/UDP \
+        -p 127.0.0.1:$SS_PORTS:$SS_PORTS/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+
+    # get the private IP address of the host, double check the result, it might not be correct
+    PRIVATE_IP=$(ipconfig getifaddr en0 2>/dev/null || hostname -i | awk '{print $1}' 2>/dev/null)
+    echo "PRIVATE_IP=$PRIVATE_IP"
+
+    # run shadowsocks-libev, simulate private IP node
+    MGR_PORT=6002 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
+        -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-private shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
+        
+    # run shadowsocks-libev, simulate public IP node
+    MGR_PORT=6003 SS_PORTS=8480 ENCRYPT=aes-256-cfb
+    docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
+        -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
+        --name ssm-dev-ss-libev-public shadowsocks/shadowsocks-libev:edge \
+        ss-manager --manager-address 0.0.0.0:$MGR_PORT \
+        --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
     ```
 
 1. Link the project code in your workspace to the Python environment
 
     ```sh
     cd shadowsocks-manager
     pip install -e .
@@ -388,26 +404,30 @@
 
     ```sh
     ssm-setup -c -m -l -u admin -p yourpassword
     ```
 
 1. Run the development server
 
+    Make sure the memcached and rabbitmq are running.
+
     ```sh
     ssm-dev-start
     ```
 
 1. Stop the development server
 
     ```sh
     ssm-dev-stop
     ```
 
 1. Test the Django code
 
+    Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
+
     ```sh
     ssm-test -t
     ```
 
 1. Test the Django code with coverage
 
     ```sh
@@ -515,18 +535,34 @@
 
     # uWSGI
     supervisorctl start ssm-uwsgi
 
     # Celery
     supervisorctl start ssm-celery-worker
     supervisorctl start ssm-celery-beat
+
+    # Docker
+    docker ps
     ```
 
-1. Check the listening ports (Linux)
+1. Check the listening ports and processes (Linux)
 
     ```
     # TCP
-    netstat -tan
+    netstat -tanp
 
     # UDP
-    netstat -uan
+    netstat -uanp
+    ```
+
+1. Check the listening ports (MacOS)
+
+    ```
+    # TCP
+    netstat -anp tcp
+
+    # UDP
+    netstat -anp udp
+
+    # find the process by port
+    lsof -i :80 -P
     ```
```

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/SOURCES.txt` & `shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.3/shadowsocks_manager.egg-info/requires.txt` & `shadowsocks_manager-0.1.4/shadowsocks_manager.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,36 +9,35 @@
 djangorestframework
 docopt
 psutil
 python-decouple
 python-memcached==1.59
 pytz
 requests
-shadowsocks-alexforks
 uWSGI
 
 [:python_version < "3.3"]
 ipaddress
 
-[:python_version < "3.8"]
-django-celery-beat<2.6.0
-
 [:python_version <= "2.7"]
 django-celery-beat==1.6.0
 django-celery-results==2.0.1
 django-enumfield<3.0
 django-filter~=1.1
 python-crontab==2.6.0
 
 [:python_version > "2.7"]
 django-celery-results
 django-enumfield
 django-filter
 python-crontab
 
+[:python_version > "2.7" and python_version < "3.8"]
+django-celery-beat<2.6.0
+
 [:python_version >= "3.8"]
 django-celery-beat
 
 [dev]
 build
 bump-my-version
 codecov-cli
```

