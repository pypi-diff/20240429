# Comparing `tmp/trytond-7.0.9.tar.gz` & `tmp/trytond-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond-7.0.9.tar", last modified: Thu Apr  4 07:37:34 2024, max compression
+gzip compressed data, was "trytond-7.2.0.tar", last modified: Mon Apr 29 15:55:40 2024, max compression
```

## Comparing `trytond-7.0.9.tar` & `trytond-7.2.0.tar`

### file list

```diff
@@ -1,607 +1,609 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.558808 trytond-7.0.9/
--rw-r--r--   0 ced       (1000) ced       (1000)    40883 2024-04-04 07:37:31.000000 trytond-7.0.9/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-04-04 07:37:31.000000 trytond-7.0.9/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:39.000000 trytond-7.0.9/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      204 2023-10-30 17:06:39.000000 trytond-7.0.9/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3944 2024-04-04 07:37:34.558808 trytond-7.0.9/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-30 17:06:39.000000 trytond-7.0.9/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.415478 trytond-7.0.9/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2880 2023-10-30 17:06:39.000000 trytond-7.0.9/bin/trytond
--rwxr-xr-x   0 ced       (1000) ced       (1000)      807 2024-02-05 16:24:27.000000 trytond-7.0.9/bin/trytond-admin
--rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2023-10-30 17:06:39.000000 trytond-7.0.9/bin/trytond-console
--rwxr-xr-x   0 ced       (1000) ced       (1000)      889 2023-10-30 17:06:39.000000 trytond-7.0.9/bin/trytond-cron
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2023-10-30 17:06:39.000000 trytond-7.0.9/bin/trytond-stat
--rwxr-xr-x   0 ced       (1000) ced       (1000)      898 2024-02-05 16:24:27.000000 trytond-7.0.9/bin/trytond-worker
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.415478 trytond-7.0.9/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2367 2024-03-03 16:24:03.000000 trytond-7.0.9/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.418811 trytond-7.0.9/doc/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/modules/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.418811 trytond-7.0.9/doc/modules/res/
--rw-r--r--   0 ced       (1000) ced       (1000)     3741 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/modules/res/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2024-03-03 16:24:03.000000 trytond-7.0.9/doc/modules/res/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1546 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/modules/res/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3146 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/modules/res/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.422145 trytond-7.0.9/doc/ref/
--rw-r--r--   0 ced       (1000) ced       (1000)    10247 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/ref/backend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3269 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2656 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/cache.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/exceptions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    31979 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1171 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/filestore.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/i18n.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    32945 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/ref/models.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/pool.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8787 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/pyson.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1559 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/ref/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/sendmail.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4623 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/ref/tests.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.425478 trytond-7.0.9/doc/ref/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)      565 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/tools/barcode.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/tools/email.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/tools/immutabledict.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/tools/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/tools/logging.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/ref/tools/misc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/tools/qrcode.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/tools/singleton.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      608 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/tools/timezone.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5550 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/transaction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6064 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/ref/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.432144 trytond-7.0.9/doc/topics/
--rw-r--r--   0 ced       (1000) ced       (1000)     3717 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/topics/access_rights.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/actions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4014 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/backend_types.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14772 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/topics/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1431 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/cron.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7848 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/domain.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/topics/install.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1108 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/logs.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.432144 trytond-7.0.9/doc/topics/models/
--rw-r--r--   0 ced       (1000) ced       (1000)      840 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/models/fields_default_value.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1197 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/models/fields_on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1376 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/models/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.432144 trytond-7.0.9/doc/topics/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)     6022 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/modules/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3887 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/pyson.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.432144 trytond-7.0.9/doc/topics/reports/
--rw-r--r--   0 ced       (1000) ced       (1000)     8742 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/reports/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/start_server.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2229 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/task_queue.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2880 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/topics/testing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2191 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/translation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/triggers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/user_application.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2034 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/user_errors_warnings.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.435478 trytond-7.0.9/doc/topics/views/
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/views/extension.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    25396 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/views/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1669 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/topics/wizard.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.435478 trytond-7.0.9/doc/tutorial/
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.438811 trytond-7.0.9/doc/tutorial/module/
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/anatomy.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1843 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/default_values.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3334 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/domains.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2917 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/extend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3524 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/function_fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3935 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/tutorial/module/model.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2662 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3727 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1712 2024-02-05 16:24:27.000000 trytond-7.0.9/doc/tutorial/module/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/states.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4746 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/table_query.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6258 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5047 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4773 2023-10-30 17:06:39.000000 trytond-7.0.9/doc/tutorial/module/workflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:37:34.558808 trytond-7.0.9/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5616 2024-03-03 16:24:20.000000 trytond-7.0.9/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      624 2023-10-30 17:06:39.000000 trytond-7.0.9/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.445477 trytond-7.0.9/trytond/
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-03-03 11:59:43.000000 trytond-7.0.9/trytond/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6931 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/admin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1370 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/application.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.448811 trytond-7.0.9/trytond/backend/
--rw-r--r--   0 ced       (1000) ced       (1000)     1115 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4390 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/database.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.448811 trytond-7.0.9/trytond/backend/postgresql/
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/postgresql/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26454 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/postgresql/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3631 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/postgresql/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    27887 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/postgresql/table.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.452144 trytond-7.0.9/trytond/backend/sqlite/
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/sqlite/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20692 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/sqlite/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2209 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/sqlite/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    15130 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/sqlite/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4200 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/backend/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9431 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16924 2024-03-12 15:42:43.000000 trytond-7.0.9/trytond/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7521 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/commandline.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6270 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/config.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2280 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/console.py
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-01-26 18:15:24.000000 trytond-7.0.9/trytond/const.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31266 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/convert.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2098 2023-11-15 17:02:43.000000 trytond-7.0.9/trytond/filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1116 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/i18n.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.462144 trytond-7.0.9/trytond/ir/
--rw-r--r--   0 ced       (1000) ced       (1000)     3329 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    40010 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/ir/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10524 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/action.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2865 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1960 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/attachment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4282 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/calendar_.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1459 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7823 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/cron.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      596 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4525 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/email.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20601 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6087 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/error.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3592 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/error.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4213 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/export.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/export.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.462144 trytond-7.0.9/trytond/ir/fonts/
--rw-r--r--   0 ced       (1000) ced       (1000)     4384 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/fonts/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    58284 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/fonts/karla.ttf
--rw-r--r--   0 ced       (1000) ced       (1000)     1323 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22311 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/lang.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27227 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/lang.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.478810 trytond-7.0.9/trytond/ir/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   101854 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   101350 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    88207 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   102980 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   102212 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82922 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    94943 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   104084 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    87882 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   103053 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97828 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    87571 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97430 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93329 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93295 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100776 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100556 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    98264 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93442 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   104186 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    95382 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    88018 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   112965 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97736 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/message.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22145 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/ir/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    60624 2024-02-10 10:25:12.000000 trytond-7.0.9/trytond/ir/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16085 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/model.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    18462 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8376 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/module.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4199 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/note.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/queue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9445 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/ir/queue_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7910 2024-02-10 10:24:25.000000 trytond-7.0.9/trytond/ir/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10185 2024-01-08 10:55:00.000000 trytond-7.0.9/trytond/ir/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11140 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/rule.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16164 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4927 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5562 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/session.py
--rw-r--r--   0 ced       (1000) ced       (1000)    67397 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/translation.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7726 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/translation.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11517 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/trigger.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.482143 trytond-7.0.9/trytond/ir/ui/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5531 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/board.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    18063 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/board.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/calendar.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     3508 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/calendar.rng
--rw-r--r--   0 ced       (1000) ced       (1000)    10340 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/form.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    35278 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/form.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/graph.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5214 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/graph.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2520 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icon.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1521 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icon.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.485476 trytond-7.0.9/trytond/ir/ui/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/tryton-board.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/tryton-calendar.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/tryton-folder.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/tryton-form.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/tryton-graph.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/tryton-list.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/tryton-settings.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/icons/tryton-tree.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    10200 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2962 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/menu.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3895 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/tree.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    13567 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/tree.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/ui.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    23740 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/view.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7956 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/ui/view.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.492143 trytond-7.0.9/trytond/ir/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_act_window_domain_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_act_window_domain_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_act_window_domain_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1120 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_act_window_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_act_window_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_act_window_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_act_window_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_act_window_view_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      952 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1299 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_report_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_report_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_url_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_url_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_wizard_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/action_wizard_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/attachment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/attachment_form_preview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/attachment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1204 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/email_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/error_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/error_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/export_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/export_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/icon_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/icon_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/lang_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/lang_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/lang_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_button_click_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_button_click_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      676 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_button_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_button_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      534 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_button_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_button_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      870 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_data_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_data_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_field_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_field_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      679 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_field_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_field_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_log_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_log_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/model_print_model_graph_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_activate_upgrade_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_activate_upgrade_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_config_wizard_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_config_wizard_first_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_config_wizard_item_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_config_wizard_other_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_dependency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_dependency_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/module_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/note_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/note_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1064 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/rule_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/rule_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/sequence_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_clean_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_clean_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_export_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_export_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_set_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_set_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/translation_update_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1035 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/trigger_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/trigger_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_menu_favorite_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_menu_favorite_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_menu_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_menu_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_menu_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_search_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_search_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_tree_optional_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_tree_optional_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_tree_state_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_tree_state_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_tree_width_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/ir/view/ui_view_tree_width_list.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.498809 trytond-7.0.9/trytond/model/
--rw-r--r--   0 ced       (1000) ced       (1000)     1199 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/active.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3105 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1050 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9327 2023-12-27 10:58:12.000000 trytond-7.0.9/trytond/model/dictschema.py
--rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/digits.py
--rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.508809 trytond-7.0.9/trytond/model/fields/
--rw-r--r--   0 ced       (1000) ced       (1000)     1216 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4592 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9426 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7104 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8365 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26874 2024-02-29 15:47:56.000000 trytond-7.0.9/trytond/model/fields/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2603 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8403 2023-12-10 21:35:04.000000 trytond-7.0.9/trytond/model/fields/function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18790 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/model/fields/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14146 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4401 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16083 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/model/fields/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2116 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8415 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7508 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3439 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/fields/text.py
--rw-r--r--   0 ced       (1000) ced       (1000)      899 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/match.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17379 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/model/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4605 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    88864 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/model/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    82808 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/model/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    37242 2023-12-27 10:57:51.000000 trytond-7.0.9/trytond/model/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3773 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2712 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/order.py
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/symbol.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7250 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/union.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/model/workflow.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.508809 trytond-7.0.9/trytond/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)    13828 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/modules/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9444 2024-03-12 15:42:54.000000 trytond-7.0.9/trytond/pool.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.508809 trytond-7.0.9/trytond/protocols/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/protocols/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8248 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/protocols/dispatcher.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5827 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/protocols/jsonrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9823 2024-02-29 11:40:49.000000 trytond-7.0.9/trytond/protocols/wrappers.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5602 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/protocols/xmlrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22590 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/pyson.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.508809 trytond-7.0.9/trytond/report/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/report/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19852 2024-01-28 21:07:57.000000 trytond-7.0.9/trytond/report/report.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.515476 trytond-7.0.9/trytond/res/
--rw-r--r--   0 ced       (1000) ced       (1000)     1235 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1301 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/res/email_reset_password.html
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2476 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/group.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8325 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23683 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.522142 trytond-7.0.9/trytond/res/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    13517 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13817 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11796 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13991 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13962 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11406 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12866 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13876 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11757 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14183 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13277 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12306 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12624 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15248 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13378 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13751 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13646 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12905 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13708 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13703 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13714 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11757 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15565 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13277 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1570 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2458 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)    43139 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/res/user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8012 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/user.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.522142 trytond-7.0.9/trytond/res/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1153 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/user_application_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/user_application_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/user_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1527 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1386 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/user_form_preferences.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/user_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/user_warning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/res/view/user_warning_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3905 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4804 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/security.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5253 2023-12-10 12:57:53.000000 trytond-7.0.9/trytond/sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3227 2023-12-10 12:48:47.000000 trytond-7.0.9/trytond/status.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.555474 trytond-7.0.9/trytond/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     2433 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1202 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/copy_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2023 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/export_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)      943 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_function.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1162 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7491 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1354 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5212 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3161 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1489 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1224 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1063 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)        9 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/forbidden.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      917 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5599 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/import_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/import_data.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1069 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1083 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/mixin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4442 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1493 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/model_log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8123 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7720 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8965 2023-12-27 10:57:51.000000 trytond-7.0.9/trytond/tests/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3695 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/modelview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1116 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/path.py
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)      971 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)      584 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36330 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6920 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_backend.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4725 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10644 2024-01-26 18:15:57.000000 trytond-7.0.9/trytond/tests/test_cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12243 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_copy.py
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15266 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_exportdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7404 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22837 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1021 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13633 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15520 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7608 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_depends.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27461 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13029 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3641 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10439 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25081 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15080 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12677 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16994 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23583 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9820 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20599 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9360 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19472 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15036 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3019 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15175 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3834 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_i18n.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19311 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_importdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18556 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4610 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_mixins.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16417 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6973 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_model_index.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8288 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_model_log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4808 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_model_match.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    58690 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31235 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26545 2023-12-27 10:57:51.000000 trytond-7.0.9/trytond/tests/test_modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3450 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8733 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_order.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_path.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3726 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_protocols.py
--rw-r--r--   0 ced       (1000) ced       (1000)    34938 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2340 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_report.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2413 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_res.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3214 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6365 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4377 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27797 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4323 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5462 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)    47191 2024-02-29 11:44:54.000000 trytond-7.0.9/trytond/tests/test_tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4766 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12469 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15386 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)    44530 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_tryton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3353 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_union.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11988 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/test_user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3171 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/test_wsgi.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1187 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1180 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      928 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tests/workflow.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.558808 trytond-7.0.9/trytond/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)     1748 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tools/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1902 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/barcode.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/decimal_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-02-29 11:44:54.000000 trytond-7.0.9/trytond/tools/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2293 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/gevent.py
--rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/immutabledict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3677 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/logging.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9534 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/tools/misc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1595 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/qrcode.py
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/singleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3864 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/string_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1144 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tools/timezone.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12694 2024-03-12 15:42:43.000000 trytond-7.0.9/trytond/transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1445 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tryton.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/tryton.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2754 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/url.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.558808 trytond-7.0.9/trytond/wizard/
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/wizard/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14525 2023-10-30 17:06:39.000000 trytond-7.0.9/trytond/wizard/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6885 2024-03-12 15:42:43.000000 trytond-7.0.9/trytond/worker.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9486 2024-02-05 16:24:27.000000 trytond-7.0.9/trytond/wsgi.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:37:34.558808 trytond-7.0.9/trytond.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3944 2024-04-04 07:37:33.000000 trytond-7.0.9/trytond.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    16488 2024-04-04 07:37:34.000000 trytond-7.0.9/trytond.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:37:33.000000 trytond-7.0.9/trytond.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:28.000000 trytond-7.0.9/trytond.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      592 2024-04-04 07:37:33.000000 trytond-7.0.9/trytond.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:37:33.000000 trytond-7.0.9/trytond.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.988837 trytond-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)    41204 2024-04-29 15:31:10.000000 trytond-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-04-29 15:31:09.000000 trytond-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      204 2023-04-15 07:12:15.000000 trytond-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-04-29 15:55:40.988837 trytond-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-04-15 07:12:16.000000 trytond-7.2.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.942172 trytond-7.2.0/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2890 2024-04-27 16:30:39.000000 trytond-7.2.0/bin/trytond
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      878 2024-04-22 12:14:37.000000 trytond-7.2.0/bin/trytond-admin
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2023-04-15 07:12:15.000000 trytond-7.2.0/bin/trytond-console
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      949 2024-04-27 16:30:39.000000 trytond-7.2.0/bin/trytond-cron
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2023-04-15 07:12:16.000000 trytond-7.2.0/bin/trytond-stat
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     1088 2024-04-27 16:30:39.000000 trytond-7.2.0/bin/trytond-worker
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.942172 trytond-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2367 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.942172 trytond-7.2.0/doc/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/modules/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.942172 trytond-7.2.0/doc/modules/res/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3741 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/modules/res/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/modules/res/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1546 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/modules/res/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3146 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/modules/res/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/ref/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10444 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/backend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3269 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2656 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/cache.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2632 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/exceptions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    32469 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1171 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/ref/filestore.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/ref/i18n.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    33575 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/models.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/pool.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8787 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/ref/pyson.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1712 2024-03-17 11:01:36.000000 trytond-7.2.0/doc/ref/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2640 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/sendmail.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4738 2024-04-26 10:28:17.000000 trytond-7.2.0/doc/ref/tests.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/ref/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/tools/barcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/ref/tools/email.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/tools/immutabledict.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/tools/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/tools/logging.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1959 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/ref/tools/misc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/ref/tools/qrcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/tools/singleton.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      608 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/ref/tools/timezone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5550 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/ref/transaction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6064 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/ref/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-02-04 18:51:27.000000 trytond-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/topics/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4008 2024-04-13 17:12:23.000000 trytond-7.2.0/doc/topics/access_rights.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/actions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4014 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/topics/backend_types.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14914 2024-03-17 11:01:36.000000 trytond-7.2.0/doc/topics/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1431 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/cron.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7848 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/domain.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/topics/install.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1108 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/logs.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/topics/models/
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/topics/models/fields_default_value.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/models/fields_on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1376 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/models/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/topics/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6022 2023-10-24 13:25:05.000000 trytond-7.2.0/doc/topics/modules/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3887 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/pyson.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.945505 trytond-7.2.0/doc/topics/reports/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8742 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/topics/reports/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1381 2024-02-26 09:40:58.000000 trytond-7.2.0/doc/topics/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/start_server.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2229 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/task_queue.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2884 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/topics/testing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/translation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/triggers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2024-04-26 10:38:57.000000 trytond-7.2.0/doc/topics/user_application.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2034 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/user_errors_warnings.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.948838 trytond-7.2.0/doc/topics/views/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/topics/views/extension.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    25819 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/topics/views/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1669 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/topics/wizard.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.948838 trytond-7.2.0/doc/tutorial/
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.948838 trytond-7.2.0/doc/tutorial/module/
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/tutorial/module/anatomy.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1843 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/default_values.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3334 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/domains.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2917 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/extend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3524 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/tutorial/module/function_fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/tutorial/module/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3949 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/tutorial/module/model.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2662 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3727 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/tutorial/module/report.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-04-22 12:14:37.000000 trytond-7.2.0/doc/tutorial/module/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-04-15 07:12:16.000000 trytond-7.2.0/doc/tutorial/module/states.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4746 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/tutorial/module/table_query.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6258 2023-04-15 07:12:15.000000 trytond-7.2.0/doc/tutorial/module/view.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5047 2024-01-27 09:58:52.000000 trytond-7.2.0/doc/tutorial/module/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4727 2024-04-27 16:30:39.000000 trytond-7.2.0/doc/tutorial/module/workflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:55:40.988837 trytond-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5625 2024-04-27 16:30:39.000000 trytond-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      624 2024-03-17 11:01:36.000000 trytond-7.2.0/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.952171 trytond-7.2.0/trytond/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-29 15:31:05.000000 trytond-7.2.0/trytond/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6968 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/admin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1455 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/application.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.952171 trytond-7.2.0/trytond/backend/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/backend/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4455 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/backend/database.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.952171 trytond-7.2.0/trytond/backend/postgresql/
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/backend/postgresql/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26951 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/backend/postgresql/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4829 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/postgresql/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    29327 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/postgresql/table.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.952171 trytond-7.2.0/trytond/backend/sqlite/
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/backend/sqlite/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20807 2024-04-01 22:30:57.000000 trytond-7.2.0/trytond/backend/sqlite/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4030 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/sqlite/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    15183 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/sqlite/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4248 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/backend/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9431 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16924 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7715 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/commandline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-13 17:12:23.000000 trytond-7.2.0/trytond/config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2280 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/console.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/const.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31204 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/convert.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1500 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-10-07 21:28:39.000000 trytond-7.2.0/trytond/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2098 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1116 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/i18n.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.955505 trytond-7.2.0/trytond/ir/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3372 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    40622 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10524 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/action.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2865 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1960 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/attachment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6508 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-01 10:31:26.000000 trytond-7.2.0/trytond/ir/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/ir/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4282 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/calendar_.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1459 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7912 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1931 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/cron.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      596 2024-02-07 17:19:02.000000 trytond-7.2.0/trytond/ir/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4502 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/email.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20520 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6087 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/error.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3523 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/error.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4213 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/export.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.955505 trytond-7.2.0/trytond/ir/fonts/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4384 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/fonts/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    58284 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/fonts/karla.ttf
+-rw-r--r--   0 ced       (1000) ced       (1000)     1323 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22311 2024-04-07 14:43:04.000000 trytond-7.2.0/trytond/ir/lang.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27181 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/lang.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.958838 trytond-7.2.0/trytond/ir/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   101916 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   101483 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    88269 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103114 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   102346 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82984 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    95005 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   104146 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    87944 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103187 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97890 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    87741 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97492 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    93391 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    93357 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100910 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100618 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    98326 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100578 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   104248 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96213 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    88080 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   113027 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97870 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1490 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/message.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22606 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    64603 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15908 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/model.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    18462 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/ir/module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8238 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/module.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4199 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/ir/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/note.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/queue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9479 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/queue_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7910 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10185 2024-04-26 10:38:57.000000 trytond-7.2.0/trytond/ir/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12027 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/ir/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/rule.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16164 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4927 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5562 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/ir/session.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    67671 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/translation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7726 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/translation.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11517 2024-04-03 14:12:24.000000 trytond-7.2.0/trytond/ir/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/trigger.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.958838 trytond-7.2.0/trytond/ir/ui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/board.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    18063 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/ir/ui/board.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/ui/calendar.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     3508 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/ir/ui/calendar.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)    10397 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/form.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    35542 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/form.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/graph.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5214 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/ir/ui/graph.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2682 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/icon.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1521 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/icon.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.958838 trytond-7.2.0/trytond/ir/ui/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/ui/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-board.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-calendar.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-folder.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-form.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-graph.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-list.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-settings.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/ui/icons/tryton-tree.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    10200 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/ui/menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2962 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/menu.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3895 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/ui/tree.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    13567 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/ir/ui/tree.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/ui/ui.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    26813 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/view.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8412 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/ui/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.968838 trytond-7.2.0/trytond/ir/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_domain_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_domain_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_domain_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1136 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_act_window_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_act_window_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-06-23 11:39:44.000000 trytond-7.2.0/trytond/ir/view/action_act_window_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/action_act_window_view_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      952 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/action_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/action_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1358 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_report_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_report_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_url_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_url_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/action_wizard_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/action_wizard_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/attachment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/attachment_form_preview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/attachment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1204 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/email_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/error_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/error_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/export_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/export_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      510 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/icon_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/icon_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/lang_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/lang_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/lang_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/model_button_click_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-04-15 07:12:15.000000 trytond-7.2.0/trytond/ir/view/model_button_click_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_button_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_button_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      534 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/model_button_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/model_button_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_data_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_data_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_field_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_field_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      682 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_field_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_field_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      388 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/model_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/view/model_log_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/view/model_log_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/model_print_model_graph_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_activate_upgrade_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_activate_upgrade_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/module_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_config_wizard_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_config_wizard_first_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/module_config_wizard_item_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_config_wizard_other_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_dependency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_dependency_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/module_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/module_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/note_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/note_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1072 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/rule_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/rule_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/ir/view/sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/sequence_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_clean_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_clean_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_export_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/translation_export_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/translation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/translation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_set_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/translation_set_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/translation_update_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1035 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/trigger_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/trigger_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/ui_menu_favorite_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/ui_menu_favorite_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/ir/view/ui_menu_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/ui_menu_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/ui_menu_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      859 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_list_extension.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_search_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_search_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_optional_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_optional_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_state_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_state_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_width_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/ir/view/ui_view_tree_width_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.968838 trytond-7.2.0/trytond/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1199 2024-02-22 16:15:03.000000 trytond-7.2.0/trytond/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/active.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1050 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/model/descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9327 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/dictschema.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/digits.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/model/fields/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4592 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/fields/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/model/fields/boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9426 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/model/fields/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7052 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8365 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/model/fields/dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26432 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2603 2023-06-12 14:04:21.000000 trytond-7.2.0/trytond/model/fields/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3164 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/fmany2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8403 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/fields/function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/fields/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18816 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/fields/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14114 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/fields/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4401 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/fields/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/fields/numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16101 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/fields/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2116 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/model/fields/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8415 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/model/fields/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7508 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/fields/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3439 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/fields/text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      899 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/model/match.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17673 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/model/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4605 2024-04-07 14:43:13.000000 trytond-7.2.0/trytond/model/modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    90408 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    84791 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/model/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    38145 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/model/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2712 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/symbol.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/model/union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/model/workflow.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13764 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/modules/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8803 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/pool.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/protocols/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/protocols/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9185 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/protocols/dispatcher.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5827 2024-04-18 16:40:25.000000 trytond-7.2.0/trytond/protocols/jsonrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10447 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/protocols/wrappers.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5602 2023-10-07 21:54:42.000000 trytond-7.2.0/trytond/protocols/xmlrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24260 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/pyson.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/report/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/report/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20078 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/report/report.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.972171 trytond-7.2.0/trytond/res/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1235 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1496 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/res/email_reset_password.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2430 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/res/group.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8327 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22621 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/res/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.975504 trytond-7.2.0/trytond/res/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13763 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14072 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12042 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14246 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14217 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11652 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13112 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14122 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14674 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13523 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12552 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12870 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15494 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13624 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14006 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13892 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13151 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13963 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13949 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13969 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15820 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13532 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/res/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1570 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2458 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)    43182 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/res/user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7748 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/res/user.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.975504 trytond-7.2.0/trytond/res/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/res/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1153 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/view/group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/view/group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-08-27 09:41:33.000000 trytond-7.2.0/trytond/res/view/user_application_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-08-27 09:41:33.000000 trytond-7.2.0/trytond/res/view/user_application_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/res/view/user_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1527 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/res/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1386 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/res/view/user_form_preferences.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/res/view/user_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/res/view/user_warning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/res/view/user_warning_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3973 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6000 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/security.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5662 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3227 2024-04-13 17:12:23.000000 trytond-7.2.0/trytond/status.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.985504 trytond-7.2.0/trytond/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2433 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1202 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/copy_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2023 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/export_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2372 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2676 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_function.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1162 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7491 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1354 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5212 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3161 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1489 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1224 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1063 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)        9 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/forbidden.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      917 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5599 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/import_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/import_data.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1069 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1083 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/mixin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4719 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1493 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8936 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7720 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8965 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3695 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/modelview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1116 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      971 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      584 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36123 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6920 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/tests/test_backend.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4725 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12678 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_copy.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15266 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_exportdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7404 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22837 2023-10-21 11:43:01.000000 trytond-7.2.0/trytond/tests/test_field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1021 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13633 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15520 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7608 2023-08-15 21:07:26.000000 trytond-7.2.0/trytond/tests/test_field_depends.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27461 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13029 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3641 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10446 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25088 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15103 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12677 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17303 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23590 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9827 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20622 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9360 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19472 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15036 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3019 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17308 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tests/test_history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3794 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_i18n.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20525 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/tests/test_importdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19232 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4610 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_mixins.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17190 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6973 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_model_index.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8288 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4808 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_model_match.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    61345 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31037 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31080 2024-04-29 13:17:17.000000 trytond-7.2.0/trytond/tests/test_modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3450 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8733 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3726 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_protocols.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    36764 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2340 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_report.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2413 2024-02-26 09:40:58.000000 trytond-7.2.0/trytond/tests/test_res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3214 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6365 2024-02-25 16:44:42.000000 trytond-7.2.0/trytond/tests/test_routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4377 2023-08-16 08:35:53.000000 trytond-7.2.0/trytond/tests/test_rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25750 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4299 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5462 2024-02-04 18:51:27.000000 trytond-7.2.0/trytond/tests/test_sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    48966 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5859 2024-03-17 11:01:36.000000 trytond-7.2.0/trytond/tests/test_transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12469 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tests/test_tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15386 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    45182 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_tryton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3353 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11366 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5406 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/test_wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3171 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/test_wsgi.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1307 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1180 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-07-23 09:59:26.000000 trytond-7.2.0/trytond/tests/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      928 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tests/workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tests/workflow.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.985504 trytond-7.2.0/trytond/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2592 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tools/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tools/barcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tools/decimal_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tools/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2562 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/tools/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tools/gevent.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tools/immutabledict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3677 2024-04-18 16:16:44.000000 trytond-7.2.0/trytond/tools/logging.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9631 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/tools/misc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1595 2024-01-27 09:58:52.000000 trytond-7.2.0/trytond/tools/qrcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-01-16 14:00:21.000000 trytond-7.2.0/trytond/tools/singleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3864 2024-04-07 14:01:56.000000 trytond-7.2.0/trytond/tools/string_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tools/timezone.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12819 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1445 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/tryton.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5501 2024-04-07 15:53:45.000000 trytond-7.2.0/trytond/tryton.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2754 2024-02-26 09:40:58.000000 trytond-7.2.0/trytond/url.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.985504 trytond-7.2.0/trytond/wizard/
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:16.000000 trytond-7.2.0/trytond/wizard/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15037 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/wizard/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7318 2024-04-27 16:30:39.000000 trytond-7.2.0/trytond/worker.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9735 2024-04-22 12:14:37.000000 trytond-7.2.0/trytond/wsgi.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:40.985504 trytond-7.2.0/trytond.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    16565 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond-7.2.0/trytond.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:55:40.000000 trytond-7.2.0/trytond.egg-info/top_level.txt
```

### Comparing `trytond-7.0.9/CHANGELOG` & `trytond-7.2.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,37 @@
 
-Version 7.0.9 - 2024-04-04
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.8 - 2024-03-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.7 - 2024-02-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.6 - 2024-02-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.5 - 2024-01-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.4 - 2024-01-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.3 - 2023-12-16
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.2 - 2023-12-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2023-11-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
+* Do not accept compressed content from unauthenticated request (#13142)
+* Set loading eager to visible xxx2many on form view
+* Add loading attribute to form view
+* Add a contextual read limit on Model.read
+* Add a contextual read limit for related fields
+* Add xml_id field on ModelStorage
+* Add send_message methods
+* Store model on ir.rule.group
+* Store model on ir.model.button
+* Store model and field name on ir.model.field.access
+* Store model name on ir.model.access
+* Store model name on ir.model.field
+* Add fmany2one field
+* Allow creation of foreign key on non primary key
+* Include context information in access error
+* Remove trytond-worker max tasks per child option for Python <= 3.10
+* Do not copy readonly relational fields
+* Support list of single value in sortable_values tools
+* Allow resetting password of user via RPC
+* Support cached_property on object with __slots__
+* Allow creating indexes concurrently
+* Allow skipping index creation
+* Add assert methods to test tools
+* Set ELLIPSIS option flag on doctest
+* Set IGNORE_EXCEPTION_DETAIL option flag on doctest
+* Add timeout parameter on RPC definitions
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add pairwise_longest tools
 * Add support for Python 3.12
 * Support default values for autocomplete
```

### Comparing `trytond-7.0.9/COPYRIGHT` & `trytond-7.2.0/COPYRIGHT`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Copyright (C) 2004-2008 Tiny SPRL.
 Copyright (C) 2007-2024 Cédric Krier.
 Copyright (C) 2007-2013 Bertrand Chenal.
 Copyright (C) 2008-2024 B2CK SPRL.
 Copyright (C) 2011 Openlabs Technologies & Consulting (P) Ltd.
-Copyright (C) 2011-2023 Nicolas Évrard.
-Copyright (C) 2020-2023 Maxime Richez
-Copyright (C) 2020-2023 SALUC SA
+Copyright (C) 2011-2024 Nicolas Évrard.
+Copyright (C) 2020-2024 Maxime Richez
+Copyright (C) 2020-2024 SALUC SA
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond-7.0.9/LICENSE` & `trytond-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/PKG-INFO` & `trytond-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 7.0.9
+Version: 7.2.0
 Summary: Tryton server
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/latest/server/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -60,14 +60,15 @@
 Requires-Dist: python-sql>=1.3
 Requires-Dist: werkzeug>=0.12
 Requires-Dist: passlib>=1.7.0
 Requires-Dist: pytz; python_version < "3.9"
 Requires-Dist: backports.entry-points-selectable; python_version < "3.10"
 Provides-Extra: test
 Requires-Dist: pillow; extra == "test"
+Requires-Dist: pydot; extra == "test"
 Provides-Extra: postgresql
 Requires-Dist: psycopg2>=2.7.0; extra == "postgresql"
 Provides-Extra: graphviz
 Requires-Dist: pydot; extra == "graphviz"
 Provides-Extra: levenshtein
 Requires-Dist: python-Levenshtein; extra == "levenshtein"
 Provides-Extra: bcrypt
```

### Comparing `trytond-7.0.9/bin/trytond` & `trytond-7.2.0/bin/trytond`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # Import trytond things after it is configured
 from trytond.wsgi import app
 
 with commandline.pidfile(options):
     Pool.start()
     threads = []
     for name in options.database_names:
-        thread = threading.Thread(target=Pool(name).init)
+        thread = threading.Thread(target=lambda: Pool(name).init())
         thread.start()
         threads.append(thread)
     for thread in threads:
         thread.join()
     hostname, port = split_netloc(config.get('web', 'listen'))
     certificate = config.get('ssl', 'certificate')
     try:
```

### Comparing `trytond-7.0.9/bin/trytond-admin` & `trytond-7.2.0/bin/trytond-admin`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 import trytond.commandline as commandline
 from trytond.config import config
 
 parser = commandline.get_parser_admin()
 if argcomplete:
     argcomplete.autocomplete(parser)
 options = parser.parse_args()
+if options.indexes is None:
+    options.indexes = bool(options.update)
 config.update_etc(options.configfile)
 commandline.config_log(options)
 
 # Import after application is configured
 import trytond.admin as admin
 
 admin.run(options)
```

### Comparing `trytond-7.0.9/bin/trytond-console` & `trytond-7.2.0/bin/trytond-console`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/bin/trytond-cron` & `trytond-7.2.0/bin/trytond-cron`

 * *Files 10% similar despite different names*

```diff
@@ -26,9 +26,12 @@
 commandline.config_log(options)
 
 import trytond.cron as cron
 # Import after application is configured
 from trytond.pool import Pool
 
 with commandline.pidfile(options):
-    Pool.start()
-    cron.run(options)
+    try:
+        Pool.start()
+        cron.run(options)
+    except KeyboardInterrupt:
+        pass
```

### Comparing `trytond-7.0.9/bin/trytond-stat` & `trytond-7.2.0/bin/trytond-stat`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/bin/trytond-worker` & `trytond-7.2.0/bin/trytond-worker`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,15 @@
 config.update_etc(options.configfile)
 commandline.config_log(options)
 
 import trytond.worker as worker
 # Import after application is configured
 from trytond.pool import Pool
 
-with commandline.pidfile(options):
-    Pool.start()
-    worker.work(options)
+# Ensure main module can be safely imported by a new interpreter
+if __name__ == '__main__':
+    with commandline.pidfile(options):
+        try:
+            Pool.start()
+            worker.work(options)
+        except (KeyboardInterrupt, SystemExit):
+            pass
```

### Comparing `trytond-7.0.9/doc/conf.py` & `trytond-7.2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/index.rst` & `trytond-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/modules/res/design.rst` & `trytond-7.2.0/doc/modules/res/design.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/modules/res/setup.rst` & `trytond-7.2.0/doc/modules/res/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/modules/res/usage.rst` & `trytond-7.2.0/doc/modules/res/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/backend.rst` & `trytond-7.2.0/doc/ref/backend.rst`

 * *Files 2% similar despite different names*

```diff
@@ -275,23 +275,24 @@
 
 .. method:: TableHandler.add_column(column_name, abstract_type[, default[, comment]])
 
    Add the named column of abstract type.
    The ``default`` is a method that return the value to fill the new column.
    ``comment`` set as comment for the column.
 
-.. method:: TableHandler.add_fk(column_name, reference[, on_delete])
+.. method:: TableHandler.add_fk(columns, reference[, ref_columns[, on_delete])
 
-   Add a foreign key constraint on the named column to target the ``reference``
-   table name.
+   Add a foreign key constraint on the named columns to target the
+   ``ref_columns`` of ``reference`` table name.
    ``on_delete`` defines the method to use when foreign record is deleted.
 
-.. method:: TableHandler.drop_fk(column_name[, table])
+.. method:: TableHandler.drop_fk(columns[, ref_columns[, table])
 
-   Drop the foreign key constrant on the named column.
+   Drop the foreign key constraint on the named columns targeting the
+   ``ref_columns``.
    ``table`` can be used to alter another table.
 
 .. method:: TableHandler.not_null_action(column_name[, action])
 
    Add or remove ``NOT NULL`` on the named column.
 
 .. method:: TableHandler.add_constraint(ident, constraint)
@@ -300,19 +301,22 @@
    table.
 
 .. method:: TableHandler.drop_constraint(ident[, table])
 
    Drop the named ``ident`` constraint.
    ``table`` can be used to alter another table.
 
-.. method:: TableHandler.set_indexes(indexes)
+.. method:: TableHandler.set_indexes(indexes[, concurrently])
 
    Create the :class:`indexes <trytond.model.Index>` if possible and drop
    others having ``idx_`` as prefix or ``_index`` as suffix.
 
+   If ``concurrently`` is set indexes are created concurrently if possible.
+   It defaults to ``False``.
+
 .. method:: TableHandler.drop_column(column_name)
 
    Drop the named column.
 
 .. classmethod:: TableHandler.drop_table(model, table[, cascade])
 
    Drop the named ``table`` and clean ``ir.model.data`` from the given
```

### Comparing `trytond-7.0.9/doc/ref/bus.rst` & `trytond-7.2.0/doc/ref/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/cache.rst` & `trytond-7.2.0/doc/ref/cache.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/exceptions.rst` & `trytond-7.2.0/doc/ref/exceptions.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/fields.rst` & `trytond-7.2.0/doc/ref/fields.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1170,7 +1170,21 @@
 
 .. method:: Dict.translated([name[, type_]])
 
    Return a descriptor for the translated ``values`` or ``keys`` of the field
    following ``type_``.
    The descriptor must be used on the same class as the field.
    Default ``type_`` is ``values``.
+
+fmany2one
+---------
+
+.. function:: fmany2one(name, sources, target[, string[, ondelete[, \**options]]])
+
+Return a mixin_ class which adds a :class:`Function` field to a
+:class:`~trytond.model.ModelSQL` class that emulate a :class:`Many2One` that
+refers to the ``target`` record having the ``sources`` as value.
+``target`` is composed of the name of the model and the name of the fields
+separated by a comma.
+The target fields must be unique.
+
+.. _mixin: http://en.wikipedia.org/wiki/Mixin
```

### Comparing `trytond-7.0.9/doc/ref/filestore.rst` & `trytond-7.2.0/doc/ref/filestore.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/i18n.rst` & `trytond-7.2.0/doc/ref/i18n.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/models.rst` & `trytond-7.2.0/doc/ref/models.rst`

 * *Files 0% similar despite different names*

```diff
@@ -320,14 +320,17 @@
    Return a list of dictionary for the record ids.
    The dictionary is composed of the fields as key and their values.
 
    ``fields_names`` can contain dereferenced fields from related models.
    Their values will be returned under the referencing field suffixed by a
    ``.``.
    The number of *dots* in the name is not limited.
+   The number of records read using *dots* can be limited with the
+   ``related_read_limit`` key in the context.
+   The remaining records will only contain the ``id`` field.
 
    ``fields_names`` can also contain ``<field>:string`` for
    :class:`~fields.Selection` or :class:`~fields.MultiSelection` fields.
    Their human-readable value are returned.
 
    The virtual fields ``_write`` and ``_delete`` can be used the read the
    writeable and deleteable state of the records.
@@ -386,14 +389,21 @@
 
    The keys of ``default`` may use the dotted notation for the
    :class:`~fields.One2Many` to define the default to pass to its ``copy``
    operation.
 
    New records are returned following the input order.
 
+   .. note::
+
+      The :class:`~fields.One2Many` and :class:`~fields.Many2Many` relation
+      fields are not copied if their :attr:`~fields.Field.readonly` attribute
+      is ``True`` or if their relationional :class:`Model` is not a
+      :class:`ModelStorage` or if it has a :meth:`ModelSQL.table_query`.
+
 .. classmethod:: ModelStorage.search(domain[, offset[, limit[, order[, count]]]])
 
    Return a list of records that match the :ref:`domain <topics-domain>`.
 
    If ``offset`` or ``limit`` are set, the result starts at the offset and has
    the length of the limit.
 
@@ -569,14 +579,19 @@
       The message id for :meth:`~trytond.i18n.gettext`
 
 .. attribute:: ModelSQL._sql_indexes
 
    A :py:class:`set <set>` containing the :class:`Index` that are created on
    the table.
 
+.. attribute:: ModelSQL._history_sql_indexes
+
+   A :py:class:`set <set>` containing the :class:`Index` that are created on
+   the history table.
+
 Class methods:
 
 .. classmethod:: ModelSQL.__table__()
 
    Return a SQL Table instance for the Model.
 
 .. classmethod:: ModelSQL.__table_history__()
```

### Comparing `trytond-7.0.9/doc/ref/pool.rst` & `trytond-7.2.0/doc/ref/pool.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 
    Stop the pool by removing instances for the database.
 
 .. classmethod:: Pool.database_list()
 
    List all started databases.
 
+.. classmethod:: Pool.refresh(database_name, modules)
+
+   Stop the pool if it contains any of the modules.
+
 Instance methods:
 
 .. method:: Pool.get(name[, type])
 
    Return the named object of ``type`` from the pool.
 
 .. method:: Pool.iterobject([type])
```

### Comparing `trytond-7.0.9/doc/ref/pyson.rst` & `trytond-7.2.0/doc/ref/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/rpc.rst` & `trytond-7.2.0/doc/ref/rpc.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _ref-rpc:
 .. module:: trytond.rpc
 
 RPC
 ===
 
-.. class:: RPC([readonly[, instantiate[, [decorator, result[, check_access[, unique[, fresh_session[, cache]]]]]]]])
+.. class:: RPC([readonly[, instantiate[, [decorator, result[, check_access[, unique[, fresh_session[, cache[, timeout]]]]]]]]])
 
    Define the behavior of Remote Procedure Call.
 
 Instance attributes are:
 
 .. attribute:: RPC.readonly
 
@@ -42,14 +42,20 @@
    If set, it requires a fresh session.
    Default is ``False``.
 
 .. attribute:: RPC.cache
 
    A :class:`RPCCache` instance to compute the cache duration for the answer.
 
+.. attribute:: RPC.timeout
+
+   The timeout in second for the call.
+   ``0`` or ``None`` means no timeout is applied.
+   Default is ``None``.
+
 
 RPCCache
 --------
 
 .. class:: RPCCache([days[, seconds])
 
    Define cache duration of RPC result.
```

### Comparing `trytond-7.0.9/doc/ref/sendmail.rst` & `trytond-7.2.0/doc/ref/sendmail.rst`

 * *Files 14% similar despite different names*

```diff
@@ -6,36 +6,47 @@
 
 .. function:: sendmail_transactional(from_addr, to_addrs, msg[, transaction[, datamanager[, strict]]])
 
    Send email message only if the current transaction is successfully committed.
 
    The required arguments are an :rfc:`5322` from-address string, a list of
    :rfc:`5322` to-address strings (a bare string is treated as a list with 1
-   address), and an email message.
+   address), and an :py:class:`email.message.Message`.
    The caller may pass a :class:`~trytond.transaction.Transaction` instance to
    join otherwise the current one is joined.
    A specific data manager can be specified otherwise the default
    :class:`SMTPDataManager` is used for sending email.
    The strict value is passed to instantiate the default :class:`SMTPDataManager`.
 
    .. warning::
 
       An SMTP failure is only logged without raising any exception.
 
+.. function:: send_message_transactional(msg[, from_addr[, to_addrs[, transaction[, datamanager[, strict]]]]])
+
+   It is a convenience method for calling :func:`sendmail_transactional`.
+   If ``from_addr`` is ``None`` or ``to_addrs`` is ``None``, if fills those
+   arguments with addresses extracted from the headers of ``msg``.
+
 .. function:: sendmail(from_addr, to_addrs, msg[, server[, strict]])
 
    Send email message like :meth:`sendmail_transactional` but directly without
    caring about the transaction and return the ``server``.
 
    The caller may pass a server instance from `smtplib`_.
    It may return a new server instance if a reconnection was needed and if the
    instance comes from :meth:`get_smtp_server`.
    If strict is ``True``, an exception is raised if it is not possible to
    connect to the server.
 
+.. function:: send_message(msg[, from_addr[, to_addrs[, server[, strict]]]])
+
+   Same convenience method as :func:`send_message_transactional` but for
+   calling :func:`sendmail`.
+
 .. function:: get_smtp_server([uri[, strict]])
 
    Return a SMTP instance from `smtplib`_ using the ``uri`` or the one defined
    in the ``email`` section of the :ref:`configuration <topics-configuration>`.
    If strict is ``True``, an exception is raised if it is not possible to
    connect to the server.
```

### Comparing `trytond-7.0.9/doc/ref/tests.rst` & `trytond-7.2.0/doc/ref/tests.rst`

 * *Files 2% similar despite different names*

```diff
@@ -159,7 +159,10 @@
 .. function:: activate_modules(modules)
 
    Activate a list of ``modules`` for scenario based on proteus doctests.
 
 .. function:: set_user(user, config)
 
    Set the user of the ``config`` proteus connection to ``user``.
+
+The module exposes also all the assert methods of :py:class:`unittest.TestCase`
+that can be run doctest scenario.
```

### Comparing `trytond-7.0.9/doc/ref/tools/barcode.rst` & `trytond-7.2.0/doc/ref/tools/barcode.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/tools/logging.rst` & `trytond-7.2.0/doc/ref/tools/logging.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/tools/misc.rst` & `trytond-7.2.0/doc/ref/tools/misc.rst`

 * *Files 13% similar despite different names*

```diff
@@ -52,14 +52,18 @@
    This is the case when the value starts and ends with a ``%`` or does not
    contain any wild cards.
 
 .. function:: likify(string[, escape])
 
    Convert the string for full text if it does not contain any wild cards.
 
+.. function:: sortable_values(func)
+
+   Decorator that makes returned list of values sortable.
+
 .. function:: sql_pairing(x, y)
 
    Return an SQL expression that pairs SQL integers x and y.
 
 .. function:: firstline(text)
 
    Return first non-empty line of a text field.
```

### Comparing `trytond-7.0.9/doc/ref/tools/timezone.rst` & `trytond-7.2.0/doc/ref/tools/timezone.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/transaction.rst` & `trytond-7.2.0/doc/ref/transaction.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/ref/wizard.rst` & `trytond-7.2.0/doc/ref/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/access_rights.rst` & `trytond-7.2.0/doc/topics/access_rights.rst`

 * *Files 8% similar despite different names*

```diff
@@ -78,31 +78,36 @@
 Record Rule
 ===========
 
 The record rules are conditions that records must meet for the user to be
 granted permission to use them.
 They are defined by records of ``ir.rule.group`` which contains:
 
-    - a model on which it applies
-    - the permissions granted
-    - a set of user groups to which the rule applies
-    - a global flag to always enforce
-    - a default flag to add to all users
-    - a list of ``ir.rule`` with a :ref:`domain <topics-domain>` to select the
-      records to which the rule applies.
+    - The model the rule applies to.
+    - The type of permissions to be granted.
+    - A set of user groups to which the rule applies.
+    - A global flag to always enforce the rule even if there are other rules
+      that are less restrictive.
+    - A default flag to apply the rule, by default, to all users.
+      This then allows other less restrictive rules, that apply to the user,
+      to grant them additional permissions.
+    - A list of ``ir.rule`` records, each with a :ref:`domain <topics-domain>`
+      that is used to select the records to which the rule applies.
 
 A rule group matches a record if the record is validated by at least one of the
 domains.
-The access is granted to a record:
+Access is only granted to a record:
 
     - if the user belongs to a group which has at least one matching rule group
       that has the permission,
 
     - or if there is a default matching rule group with the permission,
 
     - or if there is a global matching rule group with the permission.
 
-Otherwise the access is denied if there is any matching rule group.
+    - or if there are no matching rule groups and no global rule groups for
+      the model.
+
 
 .. note::
     Records for which the user has no ``read`` access are filtered out from the
     :meth:`~trytond.model.ModelStorage.search` result.
```

### Comparing `trytond-7.0.9/doc/topics/actions.rst` & `trytond-7.2.0/doc/topics/actions.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/backend_types.rst` & `trytond-7.2.0/doc/topics/backend_types.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/bus.rst` & `trytond-7.2.0/doc/topics/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/configuration.rst` & `trytond-7.2.0/doc/topics/configuration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -267,14 +267,21 @@
 max_size_authenticated
 ~~~~~~~~~~~~~~~~~~~~~~
 
 The maximum size in bytes of an authenticated request (zero means no limit).
 
 Default: 2GB
 
+timeout
+~~~~~~~
+
+The timeout in seconds before aborting requests that have their execution time
+depending on the parameters.
+
+Default: ``60``
 
 cache
 -----
 
 Defines size of various cache.
 
 transaction
```

### Comparing `trytond-7.0.9/doc/topics/cron.rst` & `trytond-7.2.0/doc/topics/cron.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/domain.rst` & `trytond-7.2.0/doc/topics/domain.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/index.rst` & `trytond-7.2.0/doc/topics/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/install.rst` & `trytond-7.2.0/doc/topics/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
     * Install the published package.
       You first need to have `pip <https://pip.pypa.io/>`_ installed.
       Then to install ``trytond`` run:
 
       .. code-block:: console
 
-         $ python -m pip install trytond
+         $ python3 -m pip install trytond
 
       You can also install for example the ``sale`` module with:
 
       .. code-block:: console
 
-         $ python -m pip install trytond_sale
+         $ python3 -m pip install trytond_sale
 
     * Without installation, you need to make sure you have all the dependencies
       installed and then run:
 
       .. code-block:: console
 
-         $ python bin/trytond
+         $ python3 bin/trytond
 
       You can register modules by linking them into the ``trytond/modules``
       folder.
```

### Comparing `trytond-7.0.9/doc/topics/logs.rst` & `trytond-7.2.0/doc/topics/logs.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/models/fields_default_value.rst` & `trytond-7.2.0/doc/topics/models/fields_default_value.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/models/fields_on_change.rst` & `trytond-7.2.0/doc/topics/models/fields_on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/models/index.rst` & `trytond-7.2.0/doc/topics/models/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/modules/index.rst` & `trytond-7.2.0/doc/topics/modules/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/pyson.rst` & `trytond-7.2.0/doc/topics/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/reports/index.rst` & `trytond-7.2.0/doc/topics/reports/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/rpc.rst` & `trytond-7.2.0/doc/topics/rpc.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/setup_database.rst` & `trytond-7.2.0/doc/topics/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/start_server.rst` & `trytond-7.2.0/doc/topics/start_server.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/task_queue.rst` & `trytond-7.2.0/doc/topics/task_queue.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/testing.rst` & `trytond-7.2.0/doc/topics/testing.rst`

 * *Files 8% similar despite different names*

```diff
@@ -55,37 +55,37 @@
 Running trytond's tests
 -----------------------
 
 You can run a specific test file using ``unittest`` command line like:
 
 .. code-block:: console
 
-   $ python -m unittest trytond.tests.test_tools
+   $ python3 -m unittest trytond.tests.test_tools
 
 To run all trytond's tests using discover of ``unittest`` with:
 
 .. code-block:: console
 
-   $ python -m unittest discover -s trytond.tests
+   $ python3 -m unittest discover -s trytond.tests
 
 To run all modules tests:
 
 .. code-block:: console
 
-   $ python -m unittest discover -s trytond.modules
+   $ python3 -m unittest discover -s trytond.modules
 
 
 Running your module's tests
 ---------------------------
 
 You just need to replace the directory path with the one of your module:
 
 .. code-block:: console
 
-   $ python -m unittest discover -s trytond.modules.my_module.tests
+   $ python3 -m unittest discover -s trytond.modules.my_module.tests
 
 Extending trytond's tests
 -------------------------
 
 Python modules extending ``trytond`` core can define additional classes to
 register in ``tests`` module.
 Those modules must create an entry point ``trytond.tests`` which defines a
```

### Comparing `trytond-7.0.9/doc/topics/translation.rst` & `trytond-7.2.0/doc/topics/translation.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/triggers.rst` & `trytond-7.2.0/doc/topics/triggers.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/user_application.rst` & `trytond-7.2.0/doc/topics/user_application.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/user_errors_warnings.rst` & `trytond-7.2.0/doc/topics/user_errors_warnings.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/views/extension.rst` & `trytond-7.2.0/doc/topics/views/extension.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/topics/views/index.rst` & `trytond-7.2.0/doc/topics/views/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -361,14 +361,22 @@
    evaluated to the language code for which spell checking must be done.
 
 ``border``
    The type of border for the image widget. Available values are ``square``,
    ``rounded`` or ``circle``.
    The default value is ``square``.
 
+``loading``
+   Override the :attr:`~trytond.model.fields.Field.loading` of the field.
+   When ``eager`` for :class:`~trytond.model.fields.One2Many` and
+   :class:`~trytond.model.fields.Many2Many` the client may try to read the
+   fields of the related model using dotted notation.
+   This result in less round trip between the client and the server at the
+   expense of a bigger payload and a bigger query execution time.
+
 :ref:`yexpand <common-attributes-yexpand>`,
 :ref:`yfill <common-attributes-yfill>`,
 :ref:`xexpand <common-attributes-xexpand>`,
 :ref:`xfill <common-attributes-xfill>`,
 :ref:`colspan <common-attributes-colspan>`,
 :ref:`help <common-attributes-help>`,
 :ref:`pre_validate <common-attributes-pre_validate>`,
```

### Comparing `trytond-7.0.9/doc/topics/wizard.rst` & `trytond-7.2.0/doc/topics/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/anatomy.rst` & `trytond-7.2.0/doc/tutorial/module/anatomy.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/default_values.rst` & `trytond-7.2.0/doc/tutorial/module/default_values.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/domains.rst` & `trytond-7.2.0/doc/tutorial/module/domains.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/extend.rst` & `trytond-7.2.0/doc/tutorial/module/extend.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/function_fields.rst` & `trytond-7.2.0/doc/tutorial/module/function_fields.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/index.rst` & `trytond-7.2.0/doc/tutorial/module/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/model.rst` & `trytond-7.2.0/doc/tutorial/module/model.rst`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
       ir
       party
 
 As we defined a new dependency, we must refresh the installation with:
 
 .. code-block:: console
 
-   $ python -m pip install --editable opportunity
+   $ python3 -m pip install --use-pep517 --editable opportunity
 
 Now we can activate the ``opportunity`` module and its dependencies:
 
 .. code-block:: console
 
     $ trytond-admin -d test -u opportunity --activate-dependencies
```

### Comparing `trytond-7.0.9/doc/tutorial/module/on_change.rst` & `trytond-7.2.0/doc/tutorial/module/on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/report.rst` & `trytond-7.2.0/doc/tutorial/module/report.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/setup.rst` & `trytond-7.2.0/doc/tutorial/module/setup.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 This step will cover the installation of tryton from a developer perspective.
 We will assume that you are already fluent with venv_ and pip_.
 
 Let's create a virtual environment inside your working directory:
 
 .. code-block:: console
 
-   $ python -m venv .venv
+   $ python3 -m venv .venv
    $ source .venv/bin/activate
+   $ python -m pip install --upgrade pip
 
 Install cookiecutter and mercurial
 ----------------------------------
 
 To bootstrap the module, we provide a cookiecutter_ template.
 First we install cookiecutter_ and mercurial_ with:
 
 .. code-block:: console
 
-   $ python -m pip install cookiecutter mercurial
+   $ python3 -m pip install cookiecutter mercurial
 
 Setup module
 ------------
 
 The Tryton template can be rendered into a module with:
 
 .. code-block:: console
@@ -53,15 +54,15 @@
 Install module
 --------------
 
 Now we can install the new module in editable mode:
 
 .. code-block:: console
 
-   $ python -m pip install --editable opportunity
+   $ python3 -m pip install --use-pep517 --editable opportunity
 
 Continue with :ref:`initializing the database <tutorial-module-setup-database>`
 
 .. _pip: https://pip.pypa.io/
 .. _venv: https://docs.python.org/library/venv.html
 .. _cookiecutter: https://pypi.org/project/cookiecutter/
 .. _mercurial: https://www.mercurial-scm.org/
```

### Comparing `trytond-7.0.9/doc/tutorial/module/setup_database.rst` & `trytond-7.2.0/doc/tutorial/module/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/states.rst` & `trytond-7.2.0/doc/tutorial/module/states.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/table_query.rst` & `trytond-7.2.0/doc/tutorial/module/table_query.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/view.rst` & `trytond-7.2.0/doc/tutorial/module/view.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/wizard.rst` & `trytond-7.2.0/doc/tutorial/module/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/doc/tutorial/module/workflow.rst` & `trytond-7.2.0/doc/tutorial/module/workflow.rst`

 * *Files 9% similar despite different names*

```diff
@@ -104,23 +104,23 @@
 
 .. code-block:: xml
 
    <tryton>
       <data>
          ...
          <record model="ir.model.button" id="opportunity_convert_button">
+            <field name="model">training.opportunity</field>
             <field name="name">convert</field>
             <field name="string">Convert</field>
-            <field name="model" search="[('model', '=', 'training.opportunity')]"/>
          </record>
 
          <record model="ir.model.button" id="opportunity_lost_button">
+            <field name="model">training.opportunity</field>
             <field name="name">lost</field>
             <field name="string">Lost</field>
-            <field name="model" search="[('model', '=', 'training.opportunity')]"/>
          </record>
       </data>
    </tryton>
 
 Now we can add the ``state`` field and the buttons in the form view.
 The buttons can be grouped under a ``group`` tag.
 This is how the ``view/opportunity_form.xml`` must be adapted:
```

### Comparing `trytond-7.0.9/setup.py` & `trytond-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 if minor_version % 2:
     download_url = ''
 else:
     download_url = 'http://downloads.tryton.org/%s.%s/' % (
         major_version, minor_version)
 
-tests_require = ['pillow']
+tests_require = ['pillow', 'pydot']
 
 setup(name=name,
     version=version,
     description='Tryton server',
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
```

### Comparing `trytond-7.0.9/tox.ini` & `trytond-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/__init__.py` & `trytond-7.2.0/trytond/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from lxml import etree, objectify
 
 try:
     from requests import utils as requests_utils
 except ImportError:
     requests_utils = None
 
-__version__ = "7.0.9"
+__version__ = "7.2.0"
 
 os.environ.setdefault(
     'TRYTOND_APPNAME',
     os.path.basename(getattr(__main__, '__file__', 'trytond')))
 os.environ.setdefault('TRYTOND_TZ', os.environ.get('TZ', 'UTC'))
 os.environ['TZ'] = 'UTC'
 if hasattr(time, 'tzset'):
```

### Comparing `trytond-7.0.9/trytond/admin.py` & `trytond-7.2.0/trytond/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
                 lang = set([x[0] for x in cursor])
             lang.add(main_lang)
         else:
             lang = set()
         lang |= set(options.languages)
         pool = Pool(db_name)
         pool.init(update=options.update, lang=list(lang),
-            activatedeps=options.activatedeps)
+            activatedeps=options.activatedeps,
+            indexes=options.indexes)
 
         if options.update_modules_list:
             with Transaction().start(db_name, 0) as transaction:
                 Module = pool.get('ir.module')
                 Module.update_list()
 
         if lang:
```

### Comparing `trytond-7.0.9/trytond/application.py` & `trytond-7.2.0/trytond/application.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,12 +32,14 @@
 # TRYTOND_CONFIG it's managed by importing config
 db_names = os.environ.get('TRYTOND_DATABASE_NAMES')
 if db_names:
     # Read with csv so database name can include special chars
     reader = csv.reader(StringIO(db_names))
     threads = []
     for name in next(reader):
-        thread = threading.Thread(target=Pool(name).init)
+        thread = threading.Thread(target=lambda: Pool(name).init())
         thread.start()
         threads.append(thread)
     for thread in threads:
         thread.join()
+
+assert len(threads := threading.enumerate()) == 1, f"len({threads}) != 1"
```

### Comparing `trytond-7.0.9/trytond/backend/__init__.py` & `trytond-7.2.0/trytond/backend/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 except ImportError:
     from importlib.metadata import entry_points
 
 from trytond.config import config
 
 __all__ = [
     'name', 'Database', 'TableHandler',
-    'DatabaseIntegrityError', 'DatabaseDataError', 'DatabaseOperationalError']
+    'DatabaseIntegrityError', 'DatabaseDataError', 'DatabaseOperationalError',
+    'DatabaseTimeoutError']
 
 
 name = urllib.parse.urlparse(config.get('database', 'uri', default='')).scheme
 
 _modname = 'trytond.backend.%s' % name
 try:
     _module = importlib.import_module(_modname)
@@ -30,8 +31,9 @@
     else:
         raise
 
 Database = _module.Database
 DatabaseIntegrityError = _module.DatabaseIntegrityError
 DatabaseDataError = _module.DatabaseDataError
 DatabaseOperationalError = _module.DatabaseOperationalError
+DatabaseTimeoutError = _module.DatabaseTimeoutError
 TableHandler = _module.TableHandler
```

### Comparing `trytond-7.0.9/trytond/backend/database.py` & `trytond-7.2.0/trytond/backend/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # this repository contains the full copyright notices and license terms.
 from collections import namedtuple
 
 from sql import For
 
 DatabaseIntegrityError = None
 DatabaseOperationalError = None
+DatabaseTimeoutError = None
 
 SQLType = namedtuple('SQLType', 'base type')
 
 
 class DatabaseInterface(object):
     '''
     Define generic interface for database connection
@@ -22,15 +23,16 @@
 
     def __init__(self, name=''):
         self.name = name
 
     def connect(self):
         raise NotImplementedError
 
-    def get_connection(self, autocommit=False, readonly=False):
+    def get_connection(
+            self, autocommit=False, readonly=False, statement_timeout=None):
         raise NotImplementedError
 
     def put_connection(self, connection, close=False):
         raise NotImplementedError
 
     def close(self):
         raise NotImplementedError
```

### Comparing `trytond-7.0.9/trytond/backend/postgresql/database.py` & `trytond-7.2.0/trytond/backend/postgresql/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,32 @@
 
 try:
     from psycopg2.extensions import PYDATE, PYDATETIME, PYINTERVAL, PYTIME
 except ImportError:
     PYDATE, PYDATETIME, PYTIME, PYINTERVAL = None, None, None, None
 from psycopg2 import DataError as DatabaseDataError
 from psycopg2 import IntegrityError as DatabaseIntegrityError
+from psycopg2 import InterfaceError
 from psycopg2 import OperationalError as DatabaseOperationalError
 from psycopg2 import ProgrammingError
+from psycopg2.errors import QueryCanceled as DatabaseTimeoutError
 from psycopg2.extras import register_default_json, register_default_jsonb
 from sql import Cast, Flavor, For, Table
 from sql.conditionals import Coalesce
 from sql.functions import Function
 from sql.operators import BinaryOperator, Concat
 
 from trytond.backend.database import DatabaseInterface, SQLType
 from trytond.config import config, parse_uri
 from trytond.tools.gevent import is_gevent_monkey_patched
 
 __all__ = [
     'Database',
-    'DatabaseIntegrityError', 'DatabaseDataError', 'DatabaseOperationalError']
+    'DatabaseIntegrityError', 'DatabaseDataError', 'DatabaseOperationalError',
+    'DatabaseTimeoutError']
 
 logger = logging.getLogger(__name__)
 
 os.environ['PGTZ'] = os.environ.get('TZ', '')
 _timeout = config.getint('database', 'timeout')
 _minconn = config.getint('database', 'minconn', default=1)
 _maxconn = config.getint('database', 'maxconn', default=64)
@@ -250,15 +253,16 @@
                 'TRYTOND_APPNAME', 'trytond'),
             }
         return params
 
     def connect(self):
         return self
 
-    def get_connection(self, autocommit=False, readonly=False):
+    def get_connection(
+            self, autocommit=False, readonly=False, statement_timeout=None):
         retry = max(config.getint('database', 'retry'), _maxconn)
         for count in range(retry, -1, -1):
             try:
                 conn = self._connpool.getconn()
             except PoolError:
                 if count and not self._connpool.closed:
                     logger.info('waiting a connection')
@@ -270,23 +274,32 @@
                     'connection to "%s" failed', self.name, exc_info=True)
                 raise
             try:
                 conn.set_session(
                     isolation_level=ISOLATION_LEVEL_REPEATABLE_READ,
                     readonly=readonly,
                     autocommit=autocommit)
-                # Detect disconnection
-                conn.cursor().execute('SELECT 1')
+                with conn.cursor() as cur:
+                    if statement_timeout:
+                        cur.execute('SET statement_timeout=%s' %
+                            (statement_timeout * 1000))
+                    else:
+                        # Detect disconnection
+                        cur.execute('SELECT 1')
             except DatabaseOperationalError:
                 self._connpool.putconn(conn, close=True)
                 continue
             break
         return conn
 
     def put_connection(self, connection, close=False):
+        try:
+            connection.reset()
+        except InterfaceError:
+            pass
         self._connpool.putconn(connection, close=close)
 
     def close(self):
         with self._lock:
             logger.info('disconnection from "%s"', self.name)
             self._connpool.closeall()
             self._databases[os.getpid()].pop(self.name)
```

### Comparing `trytond-7.0.9/trytond/backend/postgresql/table.py` & `trytond-7.2.0/trytond/backend/postgresql/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -392,59 +392,82 @@
                     SQL('UPDATE {} SET {} = %s').format(
                         Identifier(self.table_name),
                         Identifier(column_name)),
                     (default(),))
 
         self._update_definitions(columns=True)
 
-    def add_fk(self, column_name, reference, on_delete=None):
+    def add_fk(self, columns, reference, ref_columns=None, on_delete=None):
         if on_delete is not None:
             on_delete = on_delete.upper()
         else:
             on_delete = 'SET NULL'
+        if isinstance(columns, str):
+            columns = [columns]
 
         cursor = Transaction().connection.cursor()
-        name = self.convert_name(self.table_name + '_' + column_name + '_fkey')
+        if ref_columns:
+            ref_columns_name = '_' + '_'.join(ref_columns)
+        else:
+            ref_columns_name = ''
+        name = self.convert_name(
+            self.table_name + '_' + '_'.join(columns)
+            + ref_columns_name + '_fkey')
         if name in self._constraints:
-            if self._fk_deltypes.get(column_name) != on_delete:
-                self.drop_fk(column_name)
-                add = True
+            for column_name in columns:
+                if self._fk_deltypes.get(column_name) != on_delete:
+                    self.drop_fk(columns, ref_columns)
+                    add = True
+                    break
             else:
                 add = False
         else:
             add = True
         if add:
+            columns = SQL(', ').join(map(Identifier, columns))
+            if not ref_columns:
+                ref_columns = ['id']
+            ref_columns = SQL(', ').join(map(Identifier, ref_columns))
             cursor.execute(
                 SQL(
                     "ALTER TABLE {table} "
                     "ADD CONSTRAINT {constraint} "
-                    "FOREIGN KEY ({column}) REFERENCES {reference} "
+                    "FOREIGN KEY ({columns}) "
+                    "REFERENCES {reference} ({ref_columns}) "
                     "ON DELETE {action}"
                     )
                 .format(
                     table=Identifier(self.table_name),
                     constraint=Identifier(name),
-                    column=Identifier(column_name),
+                    columns=columns,
                     reference=Identifier(reference),
+                    ref_columns=ref_columns,
                     action=SQL(on_delete)))
             self._update_definitions(constraints=True)
 
-    def drop_fk(self, column_name, table=None):
-        self.drop_constraint(column_name + '_fkey', table=table)
+    def drop_fk(self, columns, ref_columns=None, table=None):
+        if isinstance(columns, str):
+            columns = [columns]
+        if ref_columns:
+            ref_columns_name = '_' + '_'.join(ref_columns)
+        else:
+            ref_columns_name = ''
+        self.drop_constraint(
+            '_'.join(columns) + ref_columns_name + '_fkey', table=table)
 
     def not_null_action(self, column_name, action='add'):
         if not self.column_exist(column_name):
             return
 
         with Transaction().connection.cursor() as cursor:
             if action == 'add':
                 if self._columns[column_name]['notnull']:
                     return
                 cursor.execute(SQL(
-                        'SELECT id FROM {} WHERE {} IS NULL').format(
+                        'SELECT id FROM {} WHERE {} IS NULL LIMIT 1').format(
                         Identifier(self.table_name),
                         Identifier(column_name)))
                 if not cursor.rowcount:
                     cursor.execute(
                         SQL(
                             'ALTER TABLE {} ALTER COLUMN {} SET NOT NULL')
                         .format(
@@ -490,25 +513,36 @@
             return
         cursor = Transaction().connection.cursor()
         cursor.execute(
             SQL('ALTER TABLE {} DROP CONSTRAINT {}').format(
                 Identifier(self.table_name), Identifier(ident)))
         self._update_definitions(constraints=True)
 
-    def set_indexes(self, indexes):
+    def set_indexes(self, indexes, concurrently=False):
         cursor = Transaction().connection.cursor()
         old = set(self._indexes)
         for index in indexes:
             translator = self.index_translator_for(index)
             if translator:
                 name, query, params = translator.definition(index)
                 name = '_'.join([self.table_name, name])
                 name = 'idx_' + self.convert_name(name, reserved=len('idx_'))
                 cursor.execute(
-                    SQL('CREATE INDEX IF NOT EXISTS {} ON {} USING {}').format(
+                    'SELECT idx.indisvalid '
+                    'FROM pg_index idx '
+                    'JOIN pg_class cls ON cls.oid = idx.indexrelid '
+                    'WHERE cls.relname = %s',
+                    (name,))
+                if (idx_valid := cursor.fetchone()) and not idx_valid[0]:
+                    cursor.execute(
+                        SQL("DROP INDEX {}").format(Identifier(name)))
+                cursor.execute(
+                    SQL('CREATE INDEX {} IF NOT EXISTS {} ON {} USING {}')
+                    .format(
+                        SQL('CONCURRENTLY' if concurrently else ''),
                         Identifier(name),
                         Identifier(self.table_name),
                         query),
                     params)
                 old.discard(name)
         for name in old:
             if name.startswith('idx_') or name.endswith('_index'):
```

### Comparing `trytond-7.0.9/trytond/backend/sqlite/database.py` & `trytond-7.2.0/trytond/backend/sqlite/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,24 +25,29 @@
 from trytond.backend.database import DatabaseInterface, SQLType
 from trytond.config import config, parse_uri
 from trytond.tools import safe_join
 from trytond.transaction import Transaction
 
 __all__ = [
     'Database',
-    'DatabaseIntegrityError', 'DatabaseDataError', 'DatabaseOperationalError']
+    'DatabaseIntegrityError', 'DatabaseDataError', 'DatabaseOperationalError',
+    'DatabaseTimeoutError']
 logger = logging.getLogger(__name__)
 
 _default_name = config.get('database', 'default_name', default=':memory:')
 
 
 class DatabaseDataError(DatabaseError):
     pass
 
 
+class DatabaseTimeoutError(Exception):
+    pass
+
+
 class SQLiteExtract(Function):
     __slots__ = ()
     _function = 'EXTRACT'
 
     @staticmethod
     def extract(lookup_type, date):
         if date is None:
@@ -441,15 +446,16 @@
 
         # Use unparse before replacing sqlite with file because SQLite accepts
         # a relative path URI like file:db/test.sqlite which doesn't conform to
         # RFC8089 which urllib follows and enforces when the scheme is 'file'
         db_uri = urllib.parse.urlunparse(db_uri)
         return db_uri.replace('sqlite', 'file', 1)
 
-    def get_connection(self, autocommit=False, readonly=False):
+    def get_connection(
+            self, autocommit=False, readonly=False, statement_timeout=None):
         if self._conn is None:
             self.connect()
         if autocommit:
             self._conn.isolation_level = None
         else:
             self._conn.isolation_level = 'IMMEDIATE'
         return self._conn
```

### Comparing `trytond-7.0.9/trytond/backend/sqlite/table.py` & `trytond-7.2.0/trytond/backend/sqlite/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,18 +251,18 @@
                 # Populate column with default values:
                 cursor.execute('UPDATE ' + _escape_identifier(self.table_name)
                     + ' SET ' + _escape_identifier(column_name) + ' = ?',
                     (default(),))
 
         self._update_definitions(columns=True)
 
-    def add_fk(self, column_name, reference, on_delete=None):
+    def add_fk(self, columns, reference, ref_columns=None, on_delete=None):
         warnings.warn('Unable to add foreign key with SQLite backend')
 
-    def drop_fk(self, column_name, table=None):
+    def drop_fk(self, columns=None, ref_columns=None, table=None):
         warnings.warn('Unable to drop foreign key with SQLite backend')
 
     def not_null_action(self, column_name, action='add'):
         if not self.column_exist(column_name):
             return
 
         if action == 'add':
@@ -274,15 +274,15 @@
 
     def add_constraint(self, ident, constraint):
         warnings.warn('Unable to add constraint with SQLite backend')
 
     def drop_constraint(self, ident, table=None):
         warnings.warn('Unable to drop constraint with SQLite backend')
 
-    def set_indexes(self, indexes):
+    def set_indexes(self, indexes, concurrently=False):
         cursor = Transaction().connection.cursor()
         old = set(self._indexes)
         for index in indexes:
             translator = self.index_translator_for(index)
             if translator:
                 name, query, params = translator.definition(index)
                 name = '_'.join([self.table_name, name])
```

### Comparing `trytond-7.0.9/trytond/backend/table.py` & `trytond-7.2.0/trytond/backend/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,18 +66,18 @@
 
     def db_default(self, column_name, value):
         raise NotImplementedError
 
     def add_column(self, column_name, abstract_type, default=None, comment=''):
         raise NotImplementedError
 
-    def add_fk(self, column_name, reference, on_delete=None):
+    def add_fk(self, columns, reference, ref_columns=None, on_delete=None):
         raise NotImplementedError
 
-    def drop_fk(self, column_name, table=None):
+    def drop_fk(self, columns, ref_columns=None, table=None):
         raise NotImplementedError
 
     def not_null_action(self, column_name, action='add'):
         raise NotImplementedError
 
     def add_constraint(self, ident, constraint):
         raise NotImplementedError
@@ -103,15 +103,15 @@
                 raise ValueError
             if len(name) >= length:
                 if isinstance(name, str):
                     name = name.encode('utf-8')
                 name = hashlib.sha256(name).hexdigest()[:length - 1]
         return name
 
-    def set_indexes(self, indexes):
+    def set_indexes(self, indexes, concurrently=False):
         raise NotImplementedError
 
     def index_translator_for(self, index):
         return next(
             filter(
                 lambda t: t.score(index) > 0,
                 sorted(
```

### Comparing `trytond-7.0.9/trytond/bus.py` & `trytond-7.2.0/trytond/bus.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/cache.py` & `trytond-7.2.0/trytond/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
             try:
                 inst = cls._instances[name]
             except KeyError:
                 continue
             inst_timestamp = inst._timestamp.get(dbname)
             if not inst_timestamp or timestamp > inst_timestamp:
                 inst._clear(dbname, timestamp)
-        Pool(dbname).refresh(modules)
+        Pool.refresh(dbname, modules)
         cls._clean_last = dt.datetime.now()
 
     def sync_since(self, value):
         return self._clean_last > value
 
     @classmethod
     def commit(cls, transaction):
@@ -380,26 +380,26 @@
                 "listening on channel '%s' of '%s'", cls._channel, dbname)
             conn = database.get_connection(autocommit=True)
             selector = selectors.DefaultSelector()
 
             cursor = conn.cursor()
             cursor.execute('LISTEN "%s"' % cls._channel)
             # Clear everything in case we missed a payload
-            Pool(dbname).refresh(_get_modules(cursor))
+            Pool.refresh(dbname, _get_modules(cursor))
             cls._clear_all(dbname)
             current_thread.listening = True
 
             selector.register(conn, selectors.EVENT_READ)
             while cls._listener.get((pid, dbname)) == current_thread:
                 selector.select(timeout=60)
                 conn.poll()
                 while conn.notifies:
                     notification = conn.notifies.pop()
                     if notification.payload == 'refresh pool':
-                        Pool(dbname).refresh(_get_modules(cursor))
+                        Pool.refresh(dbname, _get_modules(cursor))
                     elif notification.payload:
                         reset = json.loads(notification.payload)
                         for name in reset:
                             inst = cls._instances[name]
                             inst._clear(dbname)
                 cls._clean_last = dt.datetime.now()
         except Exception:
```

### Comparing `trytond-7.0.9/trytond/commandline.py` & `trytond-7.2.0/trytond/commandline.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,64 +36,64 @@
 
 def get_base_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--version', action='version',
         version='%(prog)s ' + __version__)
     parser.add_argument("-c", "--config", dest="configfile", metavar='FILE',
         nargs='+', default=[os.environ.get('TRYTOND_CONFIG')],
-        help='Specify configuration files')
+        help="specify configuration files")
     return parser
 
 
 def get_parser():
     parser = get_base_parser()
 
     parser.add_argument("-v", "--verbose", action='count',
-        dest="verbose", default=0, help="enable verbose mode")
+        dest="verbose", default=0, help="increase verbosity")
     parser.add_argument('--dev', dest='dev', action='store_true',
         help='enable development mode')
 
     logging_config = os.environ.get('TRYTOND_LOGGING_CONFIG')
     db_names = os.environ.get('TRYTOND_DATABASE_NAMES')
     if db_names:
         db_names = list(next(csv.reader(StringIO(db_names))))
     else:
         db_names = []
     parser.add_argument(
         "-d", "--database", dest="database_names", nargs='+',
         default=db_names, metavar='DATABASE',
-        help="specify the database name").completer = database_completer
+        help="specify the database names").completer = database_completer
     parser.add_argument(
         "--logconf", dest="logconf", default=logging_config, metavar='FILE',
-        help="logging configuration file (ConfigParser format)")
+        help="set logging configuration file (ConfigParser format)")
 
     return parser
 
 
 def get_parser_daemon():
     parser = get_parser()
     parser.add_argument("--pidfile", dest="pidfile", metavar='FILE',
-        help="file where the server pid will be stored")
+        help="set file to store the process id")
     parser.add_argument(
         "--coroutine", action="store_true", dest="coroutine",
         default=bool(os.environ.get('TRYTOND_COROUTINE', False)),
         help="use coroutine for concurrency")
     return parser
 
 
 def get_parser_worker():
     parser = get_parser_daemon()
     parser.add_argument("--name", dest='name',
         help="work only on the named queue")
     parser.add_argument("-n", dest='processes', type=int,
-        help="number of processes to use")
+        help="set number of processes to use")
     parser.add_argument("--max", dest='maxtasksperchild', type=int,
-        help="number of tasks a worker process before being replaced")
+        help="set number of tasks a worker process before being replaced")
     parser.add_argument("-t", "--timeout", dest='timeout', default=60,
-        type=int, help="maximum timeout when waiting notification")
+        type=int, help="set maximum timeout when waiting notification")
     return parser
 
 
 def get_parser_cron():
     parser = get_parser_daemon()
     parser.add_argument("-1", "--once", dest='once', action='store_true',
         help="run pending tasks and halt")
@@ -102,35 +102,39 @@
 
 def get_parser_admin():
     parser = get_parser()
 
     parser.add_argument(
         "-u", "--update", dest="update", nargs='+', default=[],
         metavar='MODULE',
-        help="activate or update a module").completer = module_completer
+        help="activate or update modules").completer = module_completer
+    parser.add_argument(
+        "--indexes", dest="indexes",
+        action=getattr(argparse, 'BooleanOptionalAction', 'store_true'),
+        default=None, help="update indexes")
     parser.add_argument("--all", dest="update", action="append_const",
         const="ir", help="update all activated modules")
     parser.add_argument("--activate-dependencies", dest="activatedeps",
         action="store_true",
-        help="Activate missing dependencies of updated modules")
+        help="activate missing dependencies of updated modules")
     parser.add_argument("--email", dest="email", help="set the admin email")
     parser.add_argument("-p", "--password", dest="password",
         action='store_true', help="set the admin password")
     parser.add_argument("--reset-password", dest='reset_password',
         action='store_true', help="reset the admin password")
     parser.add_argument("--test-email", dest='test_email',
-        help="Send a test email to the specified address.")
+        help="send a test email to the specified address")
     parser.add_argument("-m", "--update-modules-list", action="store_true",
-        dest="update_modules_list", help="Update list of tryton modules")
+        dest="update_modules_list", help="update the list of tryton modules")
     parser.add_argument(
         "-l", "--language", dest="languages", nargs='+',
         default=[], metavar='CODE',
-        help="Load language translations").completer = language_completer
+        help="load language translations").completer = language_completer
     parser.add_argument("--hostname", dest="hostname", default=None,
-        help="Limit database listing to the hostname")
+        help="limit database listing to the hostname")
     parser.add_argument("--validate", dest="validate", nargs='*',
         metavar='MODEL', help="validate records of models")
     parser.add_argument("--validate-percentage", dest="validate_percentage",
         type=float, default=100, metavar="PERCENTAGE",
         help="percentage of records to validate (default: 100)")
 
     parser.epilog = ('The first time a database is initialized '
@@ -147,20 +151,20 @@
 def get_parser_console():
     parser = get_base_parser()
     parser.add_argument(
         "-d", "--database", dest="database_name",
         required=True, metavar='DATABASE',
         help="specify the database name").completer = database_completer
     parser.add_argument("--histsize", dest="histsize", type=int, default=500,
-        help="The number of commands to remember in the command history")
+        help="set the number of commands to remember in the command history")
     parser.add_argument("--readonly", dest="readonly", action='store_true',
-        help="Start a readonly transaction")
+        help="start a readonly transaction")
     parser.add_argument(
         "--lock-table", dest="lock_tables", nargs='+', default=[],
-        metavar='TABLE', help="Lock tables")
+        metavar='TABLE', help="lock tables")
     parser.epilog = "To store changes, `transaction.commit()` must be called."
     return parser
 
 
 def get_parser_stat():
     parser = get_base_parser()
     parser.epilog = "To exit press 'q', to inverse sort order press 'r'."
```

### Comparing `trytond-7.0.9/trytond/config.py` & `trytond-7.2.0/trytond/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         self.set('database', 'language', 'en')
         self.set('database', 'timeout', str(30 * 60))
         self.set('database', 'subquery_threshold', str(1_000))
         self.add_section('request')
         self.set('request', 'max_size', str(2 * 1024 * 1024))
         self.set('request', 'max_size_authenticated',
             str(2 * 1024 * 1024 * 1024))
+        self.set('request', 'timeout', str(60))
         self.add_section('cache')
         self.set('cache', 'transaction', '10')
         self.set('cache', 'model', '200')
         self.set('cache', 'record', '2000')
         self.set('cache', 'field', '100')
         self.set('cache', 'default', '1024')
         self.set('cache', 'ir.message', '10240')
```

### Comparing `trytond-7.0.9/trytond/console.py` & `trytond-7.2.0/trytond/console.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/convert.py` & `trytond-7.2.0/trytond/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -796,45 +796,46 @@
             ('fs_id', 'in', to_delete),
             ('module', '=', module),
             ], order=[('id', 'DESC')])
 
     for mrec in mdata:
         model, db_id, fs_id = mrec.model, mrec.db_id, mrec.fs_id
 
-        logger.info('Deleting %s@%s from %s.%s', db_id, model, module, fs_id)
         try:
             # Deletion of the record
             try:
                 Model = pool.get(model)
             except KeyError:
                 Model = None
             if Model:
                 Model.delete([Model(db_id)])
                 mdata_delete.append(mrec)
             else:
                 logger.warning(
-                    'Could not delete id %d of model %s because model no '
-                    'longer exists.', db_id, model)
-        except Exception:
+                    "could not delete %d@%s from %s.%s "
+                    "because model no longer exists",
+                    db_id, model, module, fs_id)
+        except Exception as e:
             transaction.rollback()
-            logger.error(
-                "Could not delete id %d from model %s.\n"
-                "There may be a relation that points to this resource "
-                "that must be manually fixed before restarting the update.",
-                db_id, model, exc_info=True)
+            logger.warning(
+                "could not delete %d@%s from %s.%s (%s).",
+                db_id, model, module, fs_id, e)
             if 'active' in Model._fields:
                 try:
                     Model.write([Model(db_id)], {
                             'active': False,
                             })
-                except Exception:
+                except Exception as e:
                     transaction.rollback()
                     logger.error(
-                        'Could not inactivate id: %d of model %s\n',
-                        db_id, model, exc_info=True)
+                        "could not deactivate %d@%s from %s.%s (%s)",
+                        db_id, model, module, fs_id, e)
+        else:
+            logger.info(
+                "deleted %s@%s from %s.%s", db_id, model, module, fs_id)
         transaction.commit()
 
     # Clean model_data:
     if mdata_delete:
         ModelData.delete(mdata_delete)
         transaction.commit()
```

### Comparing `trytond-7.0.9/trytond/cron.py` & `trytond-7.2.0/trytond/cron.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __all__ = ['run']
 logger = logging.getLogger(__name__)
 
 
 def run(options):
     threads = []
     for name in options.database_names:
-        thread = threading.Thread(target=Pool(name).init)
+        thread = threading.Thread(target=lambda: Pool(name).init())
         thread.start()
         threads.append(thread)
     for thread in threads:
         thread.join()
 
     threads = {}
     while True:
```

### Comparing `trytond-7.0.9/trytond/exceptions.py` & `trytond-7.2.0/trytond/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/filestore.py` & `trytond-7.2.0/trytond/filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/i18n.py` & `trytond-7.2.0/trytond/i18n.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/__init__.py` & `trytond-7.2.0/trytond/ir/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     rule, sequence, session, translation, trigger, ui)
 
 __all__ = ['register', 'routes']
 
 
 def register():
     Pool.register(
+        model.ModelField,  # register first for model char migration
         configuration.Configuration,
         translation.Translation,
         translation.TranslationSetStart,
         translation.TranslationSetSucceed,
         translation.TranslationCleanStart,
         translation.TranslationCleanSucceed,
         translation.TranslationUpdateStart,
@@ -38,15 +39,14 @@
         action.ActionReport,
         action.ActionActWindow,
         action.ActionActWindowView,
         action.ActionActWindowDomain,
         action.ActionWizard,
         action.ActionURL,
         model.Model,
-        model.ModelField,
         model.ModelAccess,
         model.ModelFieldAccess,
         model.ModelButton,
         model.ModelButtonRule,
         model.ModelButtonClick,
         model.ModelButtonReset,
         model.ModelData,
```

### Comparing `trytond-7.0.9/trytond/ir/action.py` & `trytond-7.2.0/trytond/ir/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     DeactivableMixin, Index, ModelSingleton, ModelSQL, ModelStorage, ModelView,
     fields, sequence_ordered)
 from trytond.model.exceptions import ValidationError
 from trytond.pool import Pool
 from trytond.pyson import PYSON, Eval, PYSONDecoder, PYSONEncoder
 from trytond.rpc import RPC
 from trytond.tools import file_open
-from trytond.transaction import Transaction, inactive_records
+from trytond.transaction import (
+    Transaction, inactive_records, without_check_access)
 
 if not config.get('html', 'plugins-ir.action.report-report_content_html'):
     config.set(
         'html', 'plugins-ir.action.report-report_content_html', 'fullpage')
 
 
 class WizardModelError(ValidationError):
@@ -95,14 +96,15 @@
     def write(cls, actions, values, *args):
         pool = Pool()
         super(Action, cls).write(actions, values, *args)
         pool.get('ir.action.keyword')._get_keyword_cache.clear()
 
     @classmethod
     @inactive_records
+    @without_check_access
     def get_action_id(cls, action_id):
         pool = Pool()
         if cls.search([
                     ('id', '=', action_id),
                     ]):
             return action_id
         for action_type in (
@@ -144,16 +146,17 @@
                 if (values['res_model']
                         and issubclass(
                             pool.get(values['res_model']), ModelSingleton)):
                     values['res_id'] = 1
         return actions
 
     def get_action_value(self):
-        return self.get_action_values(
-            self.type, [self.get_action_id(self.id)])[0]
+        action_id = self.get_action_id(self.id)
+        if action_id is not None:
+            return self.get_action_values(self.type, [action_id])[0]
 
 
 class ActionKeyword(ModelSQL, ModelView):
     "Action keyword"
     __name__ = 'ir.action.keyword'
     keyword = fields.Selection([
             ('tree_open', 'Open tree'),
@@ -461,15 +464,22 @@
     @classmethod
     def fetch_action(cls, action_id):
         fields = list(cls._fields.keys())
         return cls.search_read(
             [('action', '=', action_id)], fields_names=fields, limit=1)
 
 
-class ActionReport(ActionMixin, ModelSQL, ModelView):
+class ActionReport(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            ondelete='CASCADE'),
+        fields.fmany2one(
+            'module_ref', 'module', 'ir.module,name', "Module",
+            readonly=True, ondelete='CASCADE'),
+        ActionMixin, ModelSQL, ModelView):
     "Action report"
     __name__ = 'ir.action.report'
     _action_name = 'report_name'
     model = fields.Char('Model')
     report_name = fields.Char('Internal Name', required=True)
     report = fields.Char(
         "Path",
@@ -608,15 +618,15 @@
 
     @staticmethod
     def default_extension():
         return ''
 
     @staticmethod
     def default_module():
-        return Transaction().context.get('module') or ''
+        return Transaction().context.get('module')
 
     def get_is_custom(self, name):
         return bool(self.report_content_custom)
 
     @classmethod
     def get_report_content(cls, reports, name):
         contents = {}
@@ -671,24 +681,18 @@
 
     @classmethod
     def copy(cls, reports, default=None):
         if default is None:
             default = {}
         default = default.copy()
         default.setdefault('module', None)
-
-        new_reports = []
-        for report in reports:
-            if report.report:
-                default['report_content'] = None
-                default['report'] = None
-            default['report_name'] = report.report_name
-            new_reports.extend(super(ActionReport, cls).copy([report],
-                    default=default))
-        return new_reports
+        default.setdefault(
+            'report_content_custom',
+            lambda o: None if o['report'] else o['report_content_custom'])
+        return super().copy(reports, default=default)
 
     @classmethod
     def write(cls, reports, values, *args):
         context = Transaction().context
         if 'module' in context:
             actions = iter((reports, values) + args)
             args = []
@@ -724,15 +728,22 @@
             except Exception as exception:
                 raise ValidationError(gettext(
                         'ir.msg_report_invalid_record_name',
                         report=report.rec_name,
                         exception=exception)) from exception
 
 
-class ActionActWindow(ActionMixin, ModelSQL, ModelView):
+class ActionActWindow(
+        fields.fmany2one(
+            'res_model_ref', 'res_model', 'ir.model,model', "Model",
+            ondelete='CASCADE'),
+        fields.fmany2one(
+            'context_model_ref', 'context_model', 'ir.model,model',
+            "Context Model", ondelete='CASCADE'),
+        ActionMixin, ModelSQL, ModelView):
     "Action act window"
     __name__ = 'ir.action.act_window'
     domain = fields.Char('Domain Value')
     context = fields.Char('Context Value')
     order = fields.Char('Order Value')
     res_model = fields.Char('Model')
     context_model = fields.Char('Context Model')
@@ -932,15 +943,15 @@
 class ActionActWindowView(
         sequence_ordered(), DeactivableMixin, ModelSQL, ModelView):
     "Action act window view"
     __name__ = 'ir.action.act_window.view'
     view = fields.Many2One(
         'ir.ui.view', "View", required=True, ondelete='CASCADE',
         domain=[
-            ('model', '=', Eval('model')),
+            ('model', '=', Eval('model', None)),
             ])
     act_window = fields.Many2One('ir.action.act_window', 'Action',
             ondelete='CASCADE')
     model = fields.Function(fields.Char("Model"), 'on_change_with_model')
 
     @classmethod
     def __setup__(cls):
@@ -1064,15 +1075,19 @@
     @classmethod
     def delete(cls, domains):
         pool = Pool()
         super(ActionActWindowDomain, cls).delete(domains)
         pool.get('ir.action.keyword')._get_keyword_cache.clear()
 
 
-class ActionWizard(ActionMixin, ModelSQL, ModelView):
+class ActionWizard(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            ondelete='CASCADE'),
+        ActionMixin, ModelSQL, ModelView):
     "Action wizard"
     __name__ = 'ir.action.wizard'
     _action_name = 'wiz_name'
     wiz_name = fields.Char('Wizard name', required=True)
     model = fields.Char('Model')
     window = fields.Boolean('Window', help='Run wizard in a new window.')
```

### Comparing `trytond-7.0.9/trytond/ir/action.xml` & `trytond-7.2.0/trytond/ir/action.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/attachment.py` & `trytond-7.2.0/trytond/ir/attachment.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/attachment.xml` & `trytond-7.2.0/trytond/ir/attachment.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/avatar.py` & `trytond-7.2.0/trytond/ir/avatar.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,15 +125,18 @@
                 (width - size) // 2,
                 (height - size) // 2,
                 (width + size) // 2,
                 (height + size) // 2))
         if size > 2048:
             img = img.resize((2048, 2048))
         if img.mode in {'RGBA', 'P'}:
-            img = img.convert('RGB')
+            img.convert('RGBA')
+            background = Image.new('RGBA', img.size, (255, 255, 255))
+            background.alpha_composite(img)
+            img = background.convert('RGB')
         img.save(data, format='jpeg', optimize=True, **_params)
         return data.getvalue()
 
     def _resize(self, size=64, **_params):
         if not PIL:
             return self.image
         data = io.BytesIO()
```

### Comparing `trytond-7.0.9/trytond/ir/calendar_.py` & `trytond-7.2.0/trytond/ir/calendar_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/calendar_.xml` & `trytond-7.2.0/trytond/ir/calendar_.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/configuration.py` & `trytond-7.2.0/trytond/ir/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/cron.py` & `trytond-7.2.0/trytond/ir/cron.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,34 +181,36 @@
                 while True:
                     if count:
                         time.sleep(0.02 * (retry - count))
                     try:
                         with processing(name), \
                                 transaction.new_transaction(
                                     **transaction_extras) as cron_trans:
-                            cron.run_once()
-                            cron_trans.commit()
-                    except Exception as e:
-                        if isinstance(e, TransactionError):
-                            cron_trans.rollback()
-                            e.fix(transaction_extras)
-                            continue
-                        if (isinstance(e, backend.DatabaseOperationalError)
-                                and count < retry):
-                            cron_trans.rollback()
-                            count += 1
-                            logger.debug("Retry: %i", count)
-                            continue
-                        if isinstance(e, (UserError, UserWarning)):
-                            Error.report(cron, e)
-                            logger.info(
-                                "%s failed after %i ms", name, duration())
-                        else:
-                            logger.exception(
-                                "%s failed after %i ms", name, duration())
+                            try:
+                                cron.run_once()
+                                cron_trans.commit()
+                            except TransactionError as e:
+                                cron_trans.rollback()
+                                e.fix(transaction_extras)
+                                continue
+                            except backend.DatabaseOperationalError:
+                                if count < retry:
+                                    cron_trans.rollback()
+                                    count += 1
+                                    logger.debug("Retry: %i", count)
+                                    continue
+                                else:
+                                    raise
+                    except (UserError, UserWarning) as e:
+                        Error.report(cron, e)
+                        logger.info(
+                            "%s failed after %i ms", name, duration())
+                    except Exception:
+                        logger.exception(
+                            "%s failed after %i ms", name, duration())
                     cron.next_call = cron.compute_next_call(now)
                     cron.save()
                     break
                 logger.info("%s in %i ms", name, duration())
         while transaction.tasks:
             task_id = transaction.tasks.pop()
             run_task(db_name, task_id)
```

### Comparing `trytond-7.0.9/trytond/ir/cron.xml` & `trytond-7.2.0/trytond/ir/cron.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/cron.xml` & `trytond-7.2.0/trytond/ir/cron.xml`

```diff
@@ -27,13 +27,13 @@
     <record model="ir.action.act_window.view" id="act_cron_form_view2">
       <field name="sequence" eval="2"/>
       <field name="view" ref="cron_view_form"/>
       <field name="act_window" ref="act_cron_form"/>
     </record>
     <menuitem parent="ir.menu_scheduler" action="act_cron_form" sequence="10" id="menu_cron_form"/>
     <record model="ir.model.button" id="cron_run_once_button">
+      <field name="model">ir.cron</field>
       <field name="name">run_once</field>
       <field name="string">Run Once</field>
-      <field name="model" search="[('model', '=', 'ir.cron')]"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond-7.0.9/trytond/ir/date.py` & `trytond-7.2.0/trytond/ir/date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/email.xml` & `trytond-7.2.0/trytond/ir/email.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/email.xml` & `trytond-7.2.0/trytond/ir/email.xml`

```diff
@@ -25,15 +25,15 @@
     <record model="ir.action.act_window.view" id="act_email_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="email_view_form"/>
       <field name="act_window" ref="act_email_form"/>
     </record>
     <menuitem parent="menu_models" action="act_email_form" sequence="50" id="menu_email_form"/>
     <record model="ir.model.access" id="access_email">
-      <field name="model" search="[('model', '=', 'ir.email')]"/>
+      <field name="model">ir.email</field>
       <field name="perm_create" eval="True"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.act_window" id="act_email_form_relate">
       <field name="name">E-mail Archives</field>
```

### Comparing `trytond-7.0.9/trytond/ir/email_.py` & `trytond-7.2.0/trytond/ir/email_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import heapq
 import mimetypes
 import re
-from email.encoders import encode_base64
-from email.header import Header
-from email.mime.application import MIMEApplication
-from email.mime.multipart import MIMEMultipart
-from email.mime.nonmultipart import MIMENonMultipart
-from email.mime.text import MIMEText
-from email.utils import formataddr, getaddresses
+from email.message import EmailMessage
+from email.utils import getaddresses
 
 try:
     import html2text
 except ImportError:
     html2text = None
 from genshi.template import TextTemplate
 
@@ -21,17 +16,18 @@
 from trytond.i18n import gettext
 from trytond.model import EvalEnvironment, ModelSQL, ModelView, fields
 from trytond.model.exceptions import AccessError, ValidationError
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, PYSONDecoder
 from trytond.report import Report
 from trytond.rpc import RPC
-from trytond.sendmail import sendmail_transactional
+from trytond.sendmail import send_message_transactional
 from trytond.tools import escape_wildcard
-from trytond.tools.email_ import convert_ascii_email, set_from_header
+from trytond.tools.email_ import (
+    convert_ascii_email, format_address, set_from_header)
 from trytond.tools.string_ import StringMatcher
 from trytond.transaction import Transaction
 
 from .resource import ResourceAccessMixin
 
 HTML_EMAIL = """<!DOCTYPE html>
 <html>
@@ -44,19 +40,14 @@
 escapesre = re.compile(r'[\\"]')
 
 
 class EmailTemplateError(ValidationError):
     pass
 
 
-def _get_emails(value):
-    "Return list of email from the comma separated list"
-    return [e for n, e in getaddresses([value]) if e]
-
-
 def _formataddr(pair):
     "Format address without encoding"
     name, address = pair
     convert_ascii_email(address).encode('ascii')
     if name:
         quotes = ''
         if specialsre.search(name):
@@ -105,37 +96,37 @@
         Attachment = pool.get('ir.attachment')
         transaction = Transaction()
         user = User(transaction.user)
 
         Model = pool.get(record[0])
         record = Model(record[1])
 
+        msg = EmailMessage()
+
         body_html = HTML_EMAIL % {
             'subject': subject,
             'body': body,
             'signature': user.signature or '',
             }
-        content = MIMEMultipart('alternative')
         if html2text:
             body_text = HTML_EMAIL % {
                 'subject': subject,
                 'body': body,
                 'signature': '',
                 }
             converter = html2text.HTML2Text()
             body_text = converter.handle(body_text)
             if user.signature:
                 body_text += '\n-- \n' + converter.handle(user.signature)
-            part = MIMEText(body_text, 'plain', _charset='utf-8')
-            content.attach(part)
-        part = MIMEText(body_html, 'html', _charset='utf-8')
-        content.attach(part)
+            msg.add_alternative(body_text, subtype='plain')
+        if msg.is_multipart():
+            msg.add_alternative(body_html, subtype='html')
+        else:
+            msg.set_content(body_html, subtype='html')
         if files or reports or attachments:
-            msg = MIMEMultipart('mixed')
-            msg.attach(content)
             if files is None:
                 files = []
             else:
                 files = list(files)
 
             for report_id in (reports or []):
                 report = ActionReport(report_id)
@@ -148,50 +139,33 @@
                 if isinstance(content, str):
                     content = content.encode('utf-8')
                 files.append((name, content))
             if attachments:
                 files += [
                     (a.name, a.data) for a in Attachment.browse(attachments)]
             for name, data in files:
-                mimetype, _ = mimetypes.guess_type(name)
-                if mimetype:
-                    attachment = MIMENonMultipart(*mimetype.split('/'))
-                    attachment.set_payload(data)
-                    encode_base64(attachment)
-                else:
-                    attachment = MIMEApplication(data)
-                attachment.add_header(
-                    'Content-Disposition', 'attachment',
+                ctype, _ = mimetypes.guess_type(name)
+                if not ctype:
+                    ctype = 'application/octet-stream'
+                maintype, subtype = ctype.split('/', 1)
+                msg.add_attachment(
+                    data,
+                    maintype=maintype,
+                    subtype=subtype,
                     filename=('utf-8', '', name))
-                msg.attach(attachment)
-        else:
-            msg = content
         from_ = config.get('email', 'from')
         set_from_header(msg, from_, user.email or from_)
-        msg['To'] = ', '.join(
-            formataddr((n, convert_ascii_email(a)))
-            for n, a in getaddresses([to]))
-        msg['Cc'] = ', '.join(
-            formataddr((n, convert_ascii_email(a)))
-            for n, a in getaddresses([cc]))
-        msg['Subject'] = Header(subject, 'utf-8')
-
-        to_addrs = list(filter(None, map(
-                    str.strip,
-                    _get_emails(to) + _get_emails(cc) + _get_emails(bcc))))
-        sendmail_transactional(from_, to_addrs, msg, strict=True)
-
-        email = cls(
-            recipients=to,
-            recipients_secondary=cc,
-            recipients_hidden=bcc,
-            addresses=[{'address': a} for a in to_addrs],
-            subject=subject,
-            body=body,
-            resource=record)
+        msg['To'] = [format_address(a, n) for n, a in getaddresses([to])]
+        msg['Cc'] = [format_address(a, n) for n, a in getaddresses([cc])]
+        msg['Bcc'] = [format_address(a, n) for n, a in getaddresses([bcc])]
+        msg['Subject'] = subject
+
+        send_message_transactional(msg, strict=True)
+
+        email = cls.from_message(msg, body=body, resource=record)
         email.save()
         if files:
             attachments_ = []
             for name, data in files:
                 attachments_.append(
                     Attachment(resource=email, name=name, data=data))
             Attachment.save(attachments_)
@@ -238,14 +212,26 @@
                         (field, 'ilike', '%' + escape_wildcard(value) + '%'))
         for user in User.search([
                     ('email', '!=', ''),
                     domain,
                     ], order=[]):
             yield user.name, user.email
 
+    @classmethod
+    def from_message(cls, msg, **values):
+        to_addrs = [e for _, e in getaddresses(
+                filter(None, (msg['To'], msg['Cc'], msg['Bcc'])))]
+        return cls(
+            recipients=msg['To'],
+            recipients_secondary=msg['Cc'],
+            recipients_hidden=msg['Bcc'],
+            addresses=[{'address': a} for a in to_addrs],
+            subject=msg['Subject'],
+            **values)
+
 
 class EmailAddress(ModelSQL):
     "Email Address"
     __name__ = 'ir.email.address'
 
     email = fields.Many2One(
         'ir.email', "E-mail", required=True, ondelete='CASCADE')
@@ -322,19 +308,19 @@
         for field in [
                 'recipients',
                 'recipients_secondary',
                 'recipients_hidden',
                 ]:
             field = getattr(cls, field)
             field.domain = [
-                ('model', '=', Eval('model')),
+                ('model_ref.id', '=', Eval('model', -1)),
                 ['OR',
                     ('relation', 'in', cls.email_models()),
                     [
-                        ('model.model', 'in', cls.email_models()),
+                        ('model', 'in', cls.email_models()),
                         ('name', '=', 'id'),
                         ],
                     ]
                 ]
             field.depends.add('model')
         cls.__rpc__.update({
                 'get': RPC(instantiate=0),
@@ -571,14 +557,30 @@
     @classmethod
     def _get_language(cls, record):
         pool = Pool()
         User = pool.get('res.user')
         if isinstance(record, User) and record.language:
             return record.language
 
+    @classmethod
+    def create(cls, vlist):
+        ModelView._view_toolbar_get_cache.clear()
+        return super().create(vlist)
+
+    @classmethod
+    def write(cls, *args):
+        if any({'name', 'model'} & v.keys() for v in args[1:None:2]):
+            ModelView._view_toolbar_get_cache.clear()
+        super().write(*args)
+
+    @classmethod
+    def delete(cls, records):
+        ModelView._view_toolbar_get_cache.clear()
+        super().delete(records)
+
 
 class EmailTemplate_Report(ModelSQL):
     "Email Template - Report"
     __name__ = 'ir.email.template-ir.action.report'
 
     template = fields.Many2One(
         'ir.email.template', "Template", required=True, ondelete='CASCADE')
```

### Comparing `trytond-7.0.9/trytond/ir/error.py` & `trytond-7.2.0/trytond/ir/error.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/error.xml` & `trytond-7.2.0/trytond/ir/error.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/error.xml` & `trytond-7.2.0/trytond/ir/error.xml`

```diff
@@ -45,27 +45,27 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_error_form"/>
     </record>
     <menuitem parent="ir.menu_scheduler" action="act_error_form" sequence="50" id="menu_error_form"/>
     <record model="ir.model.button" id="error_open_button">
+      <field name="model">ir.error</field>
       <field name="name">open</field>
       <field name="string">Open</field>
-      <field name="model" search="[('model', '=', 'ir.error')]"/>
     </record>
     <record model="ir.model.button" id="error_process_button">
+      <field name="model">ir.error</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'ir.error')]"/>
     </record>
     <record model="ir.model.button" id="error_solve_button">
+      <field name="model">ir.error</field>
       <field name="name">solve</field>
       <field name="string">Solve</field>
-      <field name="model" search="[('model', '=', 'ir.error')]"/>
     </record>
   </data>
   <data noupdate="1">
     <record model="ir.cron" id="cron_error_clean">
       <field name="method">ir.error|clean</field>
       <field name="interval_number" eval="1"/>
       <field name="interval_type">months</field>
```

### Comparing `trytond-7.0.9/trytond/ir/exceptions.py` & `trytond-7.2.0/trytond/ir/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/export.py` & `trytond-7.2.0/trytond/ir/export.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/export.xml` & `trytond-7.2.0/trytond/ir/export.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/fonts/LICENSE` & `trytond-7.2.0/trytond/ir/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/fonts/karla.ttf` & `trytond-7.2.0/trytond/ir/fonts/karla.ttf`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ir.xml` & `trytond-7.2.0/trytond/ir/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/lang.py` & `trytond-7.2.0/trytond/ir/lang.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/lang.xml` & `trytond-7.2.0/trytond/ir/lang.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/lang.xml` & `trytond-7.2.0/trytond/ir/lang.xml`

```diff
@@ -527,24 +527,24 @@
     <record model="ir.action.act_window.view" id="act_lang_form_view2">
       <field name="sequence" eval="2"/>
       <field name="view" ref="lang_view_form"/>
       <field name="act_window" ref="act_lang_form"/>
     </record>
     <menuitem parent="ir.menu_localization" action="act_lang_form" sequence="10" id="menu_lang_form"/>
     <record model="ir.model.button" id="lang_load_translations_button">
+      <field name="model">ir.lang</field>
       <field name="name">load_translations</field>
       <field name="string">Load translations</field>
-      <field name="model" search="[('model', '=', 'ir.lang')]"/>
       <field name="confirm">Are you sure you want to load languages' translations?</field>
     </record>
     <record model="ir.model.button" id="lang_unload_translations_button">
+      <field name="model">ir.lang</field>
       <field name="name">unload_translations</field>
       <field name="string">Unload translations</field>
       <field name="confirm">Are you sure you want to remove languages' translations?</field>
-      <field name="model" search="[('model', '=', 'ir.lang')]"/>
     </record>
     <record model="ir.ui.view" id="lang_config_start_view_form">
       <field name="model">ir.lang.config.start</field>
       <field name="type">form</field>
       <field name="name">lang_config_start_form</field>
     </record>
     <record model="ir.action.wizard" id="act_lang_config">
```

### Comparing `trytond-7.0.9/trytond/ir/locale/bg.po` & `trytond-7.2.0/trytond/ir/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -2859,23 +2859,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
 " to its domain."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_edited_at"
@@ -2918,15 +2918,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -3041,15 +3041,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -3060,15 +3062,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
@@ -3117,23 +3119,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
@@ -3217,16 +3219,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/ca.po` & `trytond-7.2.0/trytond/ir/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -2124,15 +2124,15 @@
 
 msgctxt "model:ir.cache,name:"
 msgid "Cache"
 msgstr "Memòria cau"
 
 msgctxt "model:ir.calendar.day,abbreviation:Friday"
 msgid "Fri"
-msgstr "Div"
+msgstr "Dv"
 
 msgctxt "model:ir.calendar.day,abbreviation:Monday"
 msgid "Mon"
 msgstr "Dl"
 
 msgctxt "model:ir.calendar.day,abbreviation:Saturday"
 msgid "Sat"
@@ -2656,26 +2656,28 @@
 msgid "Type"
 msgstr "Tipus"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Si"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "El nombre de dígits del valor \"%(value)r\" del camp \"%(field)s\" del "
 "registre \"%(record)s\" de \"%(model)s\" excedeix el seu límit de "
 "\"%(digits)i\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "El valor del camp \"%(field)s\" del registre \"%(record)s\" de \"%(model)s\""
 " no és correcte segons el seu domini."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2721,17 +2723,18 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (nom del model)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "\"%(field)s (cadena)"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "El valor \"%(value)s\" del camp \"%(field)s\" del registre \"%(record)s\" de"
 " \"%(model)s\" conté caràcters invàlids \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2849,16 +2852,19 @@
 "La definició del nom de registre no és vàlida per a l'informe \"%(report)s\""
 " amb l'excepció \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Es requereix un valor pel camp \"%(field)s\" de \"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
 "Es requereix un valor pel camp \"%(field)s\" del registre \"%(record)s\" de "
 "\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Els recursos als que s'ha de copiar aquest registre."
@@ -2867,17 +2873,18 @@
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "La regla del domini \"%(name)s\" es invàlida."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Falta la funció de cerca del camp \"%(field)s\" a \"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "El valor \"%(value)s\" del camp \"%(field)s\" del registre \"%(record)s \"de"
 " \"%(model)s\" no és un dels seus valors permesos."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2927,26 +2934,28 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "El valor del camp \"%(field)s\" del registre \"%(record)s\" de \"%(model)s\""
 " es massa llarg (%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "El valor del camp \"%(field)s\" del registre \"%(record)s\" de \"%(model)s\""
 " es massa llarg (%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "El valor de temps \"%(value)s\" del camp %(field)s\" del registre "
 "\"%(record)s\" de \"%(model)s\" no és vàlid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
@@ -3035,18 +3044,19 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No podeu modificar els registres \"%(ids)s\" de \"%(model)s\" per almenys una d'aquestes regles:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "No podeu modificar el camp \"%(field)s\" del registre \"%(record)s\" de "
 "\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
```

### Comparing `trytond-7.0.9/trytond/ir/locale/cs.po` & `trytond-7.2.0/trytond/ir/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -2759,23 +2759,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
 " to its domain."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2816,15 +2816,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2937,15 +2937,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2956,15 +2958,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
@@ -3013,23 +3015,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
@@ -3112,16 +3114,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/de.po` & `trytond-7.2.0/trytond/ir/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -2669,25 +2669,27 @@
 msgid "Type"
 msgstr "Typ"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Ja"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "Die Anzahl der Nachkommastellen im Wert \"%(value)s\" für Feld \"%(field)s\""
 " von \"%(model)s\" überschreitet das Limit von \"%(digits)i\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "Der Wert \"%(value)s\" des Feldes \"%(field)s\" in \"%(record)s\" von "
 "\"%(model)s\" liegt nicht im gültigen Wertebereich (Domain)."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2733,17 +2735,18 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (Modellname)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(field)s (Zeichenkette)"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "Der Wert \"%(value)s\" für Feld \"%(field)s\" in \"%(record)s\" von "
 "\"%(model)s\" enthält die ungültigen Zeichen \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2861,16 +2864,19 @@
 "Ungültige Definition für den Berichtsnamen von Bericht \"%(report)s\" mit "
 "Fehler \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Für das Feld \"%(field)s\" von \"%(model)s\" ist ein Wert erforderlich."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
 "Für das Feld \"%(field)s\" in \"%(record)s\" von \"%(model)s\" ist ein Wert "
 "erforderlich."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Die Ressourcen zu denen dieser Datensatz kopiert werden muss."
@@ -2879,17 +2885,18 @@
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "Ungültiger Wertebereich (Domain) in Regel \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Fehlende Suchfunktion für Feld \"%(field)s\" in \"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "Der Wert \"%(value)s\" von Feld \"%(field)s\" in \"%(record)s\" von "
 "\"%(model)s\" ist nicht in der Auswahl enthalten."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2941,26 +2948,28 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "Der Wert \"%(value)s\" für Feld \"%(field)s\" in \"%(model)s\" ist zu lang "
 "(%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "Der Wert \"%(value)s\" für Feld \"%(field)s\" in \"%(record)s\" von "
 "\"%(model)s\" ist zu lang (%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "Der Wert der Zeit \"%(value)s\" für Feld \"%(field)s\" in \"%(record)s\" von"
 " \"%(model)s\" ist ungültig."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "m"
@@ -3052,18 +3061,19 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Sie sind aufgrund mindestens einer der folgenden Regeln nicht dazu berechtigt, die Datensätze \"%(ids)s\" vom Typ \"%(model)s\" zu verändern:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "Keine Berechtigung zur Änderung des Feldes \"%(field)s\" in \"%(record)s\" "
 "von \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
```

### Comparing `trytond-7.0.9/trytond/ir/locale/es.po` & `trytond-7.2.0/trytond/ir/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -2662,26 +2662,28 @@
 msgid "Type"
 msgstr "Tipo"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Sí"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "El número de dígitos en el valor \"%(value)r\" del campo \"%(field)s\" en el"
 " registro \"%(record)s\" de \"%(model)s\" excede el límite de "
 "\"%(digits)i\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "El valor \"%(value)s\" del campo \"%(field)s\" del registro \"%(record)s\" "
 "de \"%(model)s\" no es correcto según su dominio."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2727,17 +2729,18 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (nombre del modelo)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(field)s (cadena)"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "El valor \"%(value)s\" para el campo \"%(field)s\" del registro "
 "\"%(record)s\" en \"%(model)s\" contiene algunos caracteres inválidos "
 "\"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
@@ -2857,16 +2860,19 @@
 "La definición del nombre de registro no és válida en el informe "
 "\"%(report)s\" con la excepción \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Se requiere un valor para el campo \"%(field)s\" de \"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
 "Se requiere un valor para el campo \"%(field)s\" en el registro "
 "\"%(record)s\" de \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Los recursos a los que se debe copiar este registro."
@@ -2875,17 +2881,18 @@
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "El dominio de la regla \"%(name)s\" no es valido."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Falta la función de búsqueda del campo \"%(field)s\" a \"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "El valor \"%(value)s\" del campo \"%(field)s\" del registro \"%(record)s\" "
 "en \"%(model)s\" no es uno de sus valores permitidos."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2935,26 +2942,28 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "El valor del campo \"%(field)s\" del registro \"%(model)s\" en \"%(model)s\""
 " es demasiado largo (%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "El valor del campo \"%(field)s\" del registro \"%(record)s\" en "
 "\"%(model)s\" es demasiado largo (%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "El valor del tiempo \"%(value)s\" del campo \"%(field)s\" del registro "
 "\"%(record)s\" de \"%(model)s) no es valido."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
@@ -3046,18 +3055,19 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "No puede modificar los registros \"%(ids)s\" de \"%(model)s\" debido a alguna de estas reglas:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "No podéis modificar el campo \"%(field)s\" del registro \"%(record)s\" de "
 "\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
```

### Comparing `trytond-7.0.9/trytond/ir/locale/es_419.po` & `trytond-7.2.0/trytond/ir/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -2649,20 +2649,20 @@
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Creado por usuario"
@@ -2702,15 +2702,15 @@
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
@@ -2810,15 +2810,17 @@
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2827,15 +2829,15 @@
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr ""
 
@@ -2879,22 +2881,22 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
@@ -2971,16 +2973,16 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/et.po` & `trytond-7.2.0/trytond/ir/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -2713,21 +2713,21 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr "Väärtust \"%(value)s\" väljale \"%(field)s\" mudelis \"%(model)s\" ei eksisteeri."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "Selles domeenis ei ole välja \"%(field)s\" väärtus mudelis \"%(model)s\" "
 "lubatud."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_edited_at"
@@ -2773,15 +2773,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr "Väärtust \"%(value)s\" väljale \"%(field)s\" mudelis \"%(model)s\" ei eksisteeri."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
@@ -2899,15 +2899,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Mudeli \"%(model)s\" välja \"%(field)s\" jaoks on väärtus nõutud."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "Mudeli \"%(model)s\" välja \"%(field)s\" jaoks on väärtus nõutud."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2917,15 +2919,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Välja \"%(field)s\" jaoks puudub ostingufunktsioon mudelis \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr "Väärtust \"%(value)s\" väljale \"%(field)s\" mudelis \"%(model)s\" ei eksisteeri."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "Järjestus"
@@ -2975,25 +2977,25 @@
 msgstr ""
 "Väärtus on mudeli \"%(model)s\" välja \"%(field)s\" jaoks liiga pikk "
 "(%(size)i > %(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "Väärtus on mudeli \"%(model)s\" välja \"%(field)s\" jaoks liiga pikk "
 "(%(size)i > %(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr "Väärtust \"%(value)s\" väljale \"%(field)s\" mudelis \"%(model)s\" ei eksisteeri."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "EL"
 
@@ -3080,16 +3082,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "Mudeli \"%(model)s\" välja \"%(field)s\" jaoks on väärtus nõutud."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
```

### Comparing `trytond-7.0.9/trytond/ir/locale/fa.po` & `trytond-7.2.0/trytond/ir/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -2751,23 +2751,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "تعداد ارقام در مقدار:\"%(value)s\" برای فیلد :\"%(field)s\" در \"%(model)s\""
 " بیش از حد \"%(digits)i\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr "مقدار فیلد: \"%s\" در مدل: \"%s\" باتوجه به دامنه آن معتبر نیست."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "پذیرفته شده در"
@@ -2811,15 +2811,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr "مقدار زمان: \"%s\" برای فیلد : \"%s\" در مدل : \"%s\" معتبر نیست."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
@@ -2934,15 +2934,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "یک مقدار برای فیلد :\"%(field)s\" در\"%(model)s\" مورد نیاز است."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "یک مقدار برای فیلد :\"%(field)s\" در\"%(model)s\" مورد نیاز است."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2953,15 +2955,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "عملکرد جستجو برای فیلد \"٪ s\" گم شده است."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr "مقدار : \"%s\" برای فیلد : \"%s\" در مدل : \"%s\" یکی از گزینه های مجاز نیست."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "ادامه"
@@ -3011,25 +3013,25 @@
 msgstr ""
 "مقدار فیلد :\"%(field)s\" در \"%(model)s\" خیلی طولانی است (%(size)i > "
 "%(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "مقدار فیلد :\"%(field)s\" در \"%(model)s\" خیلی طولانی است (%(size)i > "
 "%(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr "مقدار زمان: \"%s\" برای فیلد : \"%s\" در مدل : \"%s\" معتبر نیست."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
@@ -3116,16 +3118,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "یک مقدار برای فیلد :\"%(field)s\" در\"%(model)s\" مورد نیاز است."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
```

### Comparing `trytond-7.0.9/trytond/ir/locale/fi.po` & `trytond-7.2.0/trytond/ir/locale/fi.po`

 * *Files 0% similar despite different names*

```diff
@@ -2734,23 +2734,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
 " to its domain."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2791,15 +2791,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2912,15 +2912,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2931,15 +2933,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
@@ -2988,23 +2990,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
@@ -3087,16 +3089,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/fr.po` & `trytond-7.2.0/trytond/ir/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -2662,26 +2662,28 @@
 msgid "Type"
 msgstr "Type"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Oui"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "Le nombre de décimales de la valeur « %(value)r » pour le champs "
 "« %(field)s » sur « %(record)s » de « %(model)s » excède la limite de "
 "« %(digits)i »."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "La valeur « %(value)s » du champ « %(field)s » sur « %(record)s » de "
 "« %(model)s » n'est pas valide selon son domaine."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2727,17 +2729,18 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (nom du modèle)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(champ)s (chaîne)"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "La valeur « %(value)s » pour le champ « %(field)s » dans « %(record)s » de "
 "« %(model)s » contient des caractères non valides « %(chars)s »."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2857,16 +2860,19 @@
 "Définition de nom d'enregistrement non valide pour le rapport « %(report)s »"
 " avec l'exception «%(exception)s »."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Une valeur est requise pour le champ « %(field)s » sur « %(model)s »."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
 "Une valeur est requise pour le champ « %(field)s » sur « %(record)s » de "
 "« %(model)s »."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Les ressources sur lesquelles cet enregistrement doit être copié."
@@ -2877,17 +2883,18 @@
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 "Fonction de recherche manquante pour le champ « %(field)s » sur "
 "« %(model)s »."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "La valeur « %(value)s » pour le champ « %(field)s » sur « %(record)s » de "
 "« %(model)s » n'est pas une des options permises."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2941,26 +2948,28 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "La valeur « %(value)s » pour le champ « %(field)s » sur « %(model)s » est "
 "trop longue (%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "La valeur « %(value)s » pour le champ « %(field)s » sur « %(record)s » de "
 "« %(model)s » est trop longue (%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "La valeur de temps « %(value)s » pour le champ « %(field)s » sur "
 "« %(record)s » de « %(model)s » n'est pas valide."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
@@ -3054,18 +3063,19 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Vous n'êtes pas autorisé à écrire sur les enregistrements « %(ids)s » de « %(model)s » à cause d'au moins une de ces règles :\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "Vous n'êtes pas autorisé à modifier le champ « %(field)s » sur "
 "« %(record)s » de « %(model)s »."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
```

### Comparing `trytond-7.0.9/trytond/ir/locale/hu.po` & `trytond-7.2.0/trytond/ir/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -2747,23 +2747,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr "A „%(model)s” elem „%(field)s” mezője hibásan van kitöltve."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Módosítás dátuma"
 
@@ -2805,15 +2805,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2939,15 +2939,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "A „%(model)s” elem „%(field)s” mezőjét ki kell tölteni."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "A „%(model)s” elem „%(field)s” mezőjét ki kell tölteni."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 #, fuzzy
@@ -2959,15 +2961,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -3020,23 +3022,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "H"
@@ -3134,16 +3136,16 @@
 msgstr ""
 "Nem tudja a „%(model)s” „%(ids)s” ID-vel rendelkező rekordjait módosítani, mert a következő szabályok legalább egyike nem teljesül:\n"
 "%(rules)s"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "A „%(model)s” elem „%(field)s” mezőjét ki kell tölteni."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/id.po` & `trytond-7.2.0/trytond/ir/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -2657,20 +2657,20 @@
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Ya"
 
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Disunting pada"
 
@@ -2708,15 +2708,15 @@
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
@@ -2820,17 +2820,20 @@
 "\"%(exception)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
-msgstr ""
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "Anda tidak diizinkan mengakses \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
 msgid "Invalid domain in rule \"%(name)s\"."
@@ -2838,15 +2841,15 @@
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "Urutan"
 
@@ -2890,23 +2893,24 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
-msgstr ""
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
+msgstr "Anda tidak diizinkan mengakses \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
 msgid "Y"
@@ -2985,16 +2989,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "Anda tidak diizinkan mengakses \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
```

### Comparing `trytond-7.0.9/trytond/ir/locale/it.po` & `trytond-7.2.0/trytond/ir/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -2807,23 +2807,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
 " to its domain."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_edited_at"
@@ -2869,15 +2869,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -3003,15 +3003,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 #, fuzzy
@@ -3023,15 +3025,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
@@ -3087,23 +3089,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
@@ -3196,16 +3198,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/lo.po` & `trytond-7.2.0/trytond/ir/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -2836,23 +2836,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
 " to its domain."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_edited_at"
@@ -2895,15 +2895,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -3016,15 +3016,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -3035,15 +3037,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
@@ -3092,23 +3094,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
@@ -3191,16 +3193,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/lt.po` & `trytond-7.2.0/trytond/ir/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -2691,23 +2691,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
 " to its domain."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2748,15 +2748,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2871,15 +2871,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2890,15 +2892,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2946,23 +2948,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "mėn."
@@ -3045,16 +3047,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/nl.po` & `trytond-7.2.0/trytond/ir/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -2662,26 +2662,28 @@
 msgid "Type"
 msgstr "Type"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Ja"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "Het aantal decimalen in de waarde \"%(value)s\" voor het veld \"%(field)s\" "
 "in \"%(record)s\" van \"%(model)s\" overschrijdt de limiet van "
 "\"%(digits)i\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "De waarde \"%(value)s\" voor veld \"%(field)s\" in \"%(record)s\" van "
 "\"%(model)s\" valt niet binnen het geldige waardebereik."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2727,17 +2729,18 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (model naam)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(field)s (tekst)"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "De waarde \"%(value)s\" voor veld \"%(field)s\" in \"%(record)s\" van "
 "\"%(model)s\" bevat ongeldige tekens \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2854,16 +2857,19 @@
 "Ongeldige recordnaamdefinitie voor rapport \"%(report)s\" met uitzondering "
 "\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Een waarde is vereist voor veld \"%(field)s\" in \"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
 "Een waarde is vereist voor veld \"%(field)s\" in \"%(record)s\" van "
 "\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "De bronnen waarnaar dit record moet worden gekopieerd."
@@ -2872,17 +2878,18 @@
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "Ongeldig domein in regel \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Zoekfunctie ontbreekt voor veld \"%(field)s\" in \"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "De waarde \"%(value)s\" voor het veld \"%(field)s\" in \"%(record)s\" van "
 "\"%(model)s\" is geen van de toegestane opties."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2934,26 +2941,28 @@
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 "De waarde voor veld \"%(field)s\" in \"%(model)s\" is te lang (%(size)i > "
 "%(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "De waarde voor veld \"%(field)s\" in \"%(record)s\" van \"%(model)s\" is te "
 "lang (%(size)i > %(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "De tijd \"%(value)s\" voor veld \"%(field)s\" in \"%(record)s\" van "
 "\"%(model)s\" is niet geldig."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
@@ -3042,18 +3051,19 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "Het is niet toegestaan om te schrijven in de records \"%(ids)s\" van \"%(model)s\"vanwege ten minste één van deze regels:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr ""
 "U hebt geen rechten om het veld \"%(field)s\" in \"%(record)s\" van "
 "\"%(model)s\" te wijzigen."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
```

### Comparing `trytond-7.0.9/trytond/ir/locale/pl.po` & `trytond-7.2.0/trytond/ir/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -2712,23 +2712,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "Liczba cyfr w wartości \"%(value)s\" w polu \"%(field)s\" modelu "
 "\"%(model)s\" przekroczyła limit \"%(digits)i\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "Wartość w polu \"%(field)s\" dla \"%(model)s\" jest nieprawidłowa względem "
 "swojej domeny."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2775,15 +2775,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "Niepoprawna wartość czasu \"%(value)s\" pola \"%(field)s\" w modelu "
 "\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2906,15 +2906,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "W polu \"%(fields)s\" w modelu \"%(model)s\" wymagana jest wartość."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "W polu \"%(fields)s\" w modelu \"%(model)s\" wymagana jest wartość."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Zasoby, do których należy skopiować ten rekord."
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2924,15 +2926,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Brak funkcji wyszukiwania w polu \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "Brak w elementach wyboru wartości \"%(value)s\" pola \"%(field)s\" dla "
 "modelu \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2986,25 +2988,25 @@
 msgstr ""
 "Wartość pola \"%(field)s\" w \"%(model)s\" jest zbyt długa (%(size)i > "
 "%(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "Wartość pola \"%(field)s\" w \"%(model)s\" jest zbyt długa (%(size)i > "
 "%(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "Niepoprawna wartość czasu \"%(value)s\" pola \"%(field)s\" w modelu "
 "\"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
@@ -3099,16 +3101,16 @@
 msgstr ""
 "Nie masz uprawnień do zapisu rekordów \"%(ids)s\" modelu \"%(model)s\" z powodu przynajmniej jednego z reguł:\n"
 "%(rules)s"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "W polu \"%(fields)s\" w modelu \"%(model)s\" wymagana jest wartość."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
```

### Comparing `trytond-7.0.9/trytond/ir/locale/pt.po` & `trytond-7.2.0/trytond/ir/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -2748,23 +2748,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "O número de dígitos no valor \"%(value)s\" para o campo \"%(field)s\" no "
 "\"%(model)s\" excede o limite de \"%(digits)i\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "O valor do campo \"%(field)s\" no \"%(model)s\" não é válido de acordo com o"
 " seu domínio."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_edited_at"
@@ -2810,15 +2810,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "O formato de hora \"%(value)s\" para o campo \"%(field)s\" em \"%(model)s\" "
 "não é valido."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2938,15 +2938,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "É necessário um valor para o campo \"%(field)s\" em \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "É necessário um valor para o campo \"%(field)s\" em \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2957,15 +2959,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "A função de busca no campo \"%(field)s\" está faltando."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "O valor \"%(value)s\" do campo \"%(field)s\" em \"%(model)s\" não está na "
 "lista de opções."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
@@ -3018,25 +3020,25 @@
 msgstr ""
 "O valor para o campo \"%(field)s\" em \"%(model)s\" é longo demais (%(size)i"
 " > %(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "O valor para o campo \"%(field)s\" em \"%(model)s\" é longo demais (%(size)i"
 " > %(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "O formato de hora \"%(value)s\" para o campo \"%(field)s\" em \"%(model)s\" "
 "não é valido."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
@@ -3128,16 +3130,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "É necessário um valor para o campo \"%(field)s\" em \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
```

### Comparing `trytond-7.0.9/trytond/ir/locale/ro.po` & `trytond-7.2.0/trytond/ir/locale/ro.po`

 * *Files 10% similar despite different names*

```diff
@@ -374,23 +374,21 @@
 msgid "Type"
 msgstr "Tip"
 
 msgctxt "field:ir.avatar,cache:"
 msgid "Cache"
 msgstr "Cache"
 
-#, fuzzy
 msgctxt "field:ir.avatar,copy_to_resources:"
 msgid "Copy to Resources"
-msgstr "Resursă"
+msgstr "Copiere în Resurse"
 
-#, fuzzy
 msgctxt "field:ir.avatar,copy_to_resources_visible:"
 msgid "Copy to Resources Visible"
-msgstr "Resursă"
+msgstr "Copiere în Resurse Vizibilă"
 
 msgctxt "field:ir.avatar,image:"
 msgid "Image"
 msgstr "Imagine"
 
 msgctxt "field:ir.avatar,image_id:"
 msgid "Image ID"
@@ -648,15 +646,14 @@
 msgid "Records"
 msgstr "Înregistrări"
 
 msgctxt "field:ir.export,resource:"
 msgid "Resource"
 msgstr "Resursă"
 
-#, fuzzy
 msgctxt "field:ir.export,user:"
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.export.line,export:"
 msgid "Export"
 msgstr "Export"
@@ -719,31 +716,32 @@
 
 msgctxt "field:ir.lang,negative_sign:"
 msgid "Negative Sign"
 msgstr "Semn negativ"
 
 msgctxt "field:ir.lang,p_cs_precedes:"
 msgid "Positive Currency Symbol Precedes"
-msgstr ""
+msgstr "Simbolul pozitiv al monedei precede"
 
 msgctxt "field:ir.lang,p_sep_by_space:"
 msgid "Positive Separate by Space"
 msgstr "Pozitiv separat de spațiu"
 
 msgctxt "field:ir.lang,p_sign_posn:"
 msgid "Positive Sign Position"
 msgstr "Poziția semnului pozitiv"
 
 msgctxt "field:ir.lang,parent:"
 msgid "Parent Code"
 msgstr "Codul părintelui"
 
+#, fuzzy
 msgctxt "field:ir.lang,pg_text_search:"
 msgid "PostgreSQL Text Search Configuration"
-msgstr ""
+msgstr "Configurație PostgreSQL de Căutare în Text"
 
 msgctxt "field:ir.lang,pm:"
 msgid "PM"
 msgstr "PM"
 
 msgctxt "field:ir.lang,positive_sign:"
 msgid "Positive Sign"
@@ -951,15 +949,15 @@
 
 msgctxt "field:ir.model.field.access,description:"
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "field:ir.model.field.access,field:"
 msgid "Field"
-msgstr "Camp"
+msgstr "Câmp"
 
 msgctxt "field:ir.model.field.access,group:"
 msgid "Group"
 msgstr "Grup"
 
 msgctxt "field:ir.model.field.access,perm_create:"
 msgid "Create Access"
@@ -973,15 +971,14 @@
 msgid "Read Access"
 msgstr "Acces citit"
 
 msgctxt "field:ir.model.field.access,perm_write:"
 msgid "Write Access"
 msgstr "Acces de scriere"
 
-#, fuzzy
 msgctxt "field:ir.model.log,action:"
 msgid "Action"
 msgstr "Acțiune"
 
 msgctxt "field:ir.model.log,event:"
 msgid "Event"
 msgstr "Eveniment"
@@ -1178,17 +1175,18 @@
 msgid "Last Timestamp"
 msgstr "Ultima Ștampila de timp"
 
 msgctxt "field:ir.sequence,name:"
 msgid "Sequence Name"
 msgstr "Numele secvenței"
 
+#, fuzzy
 msgctxt "field:ir.sequence,number_increment:"
 msgid "Increment Number"
-msgstr ""
+msgstr "Număr de increment"
 
 msgctxt "field:ir.sequence,number_next:"
 msgid "Next Number"
 msgstr "Numărul următor"
 
 msgctxt "field:ir.sequence,number_next_internal:"
 msgid "Next Number"
@@ -1200,15 +1198,15 @@
 
 msgctxt "field:ir.sequence,prefix:"
 msgid "Prefix"
 msgstr "Prefix"
 
 msgctxt "field:ir.sequence,preview:"
 msgid "Preview"
-msgstr ""
+msgstr "Previzualizare"
 
 msgctxt "field:ir.sequence,sequence_type:"
 msgid "Sequence Type"
 msgstr "Tip de secvență"
 
 msgctxt "field:ir.sequence,suffix:"
 msgid "Suffix"
@@ -1230,17 +1228,18 @@
 msgid "Last Timestamp"
 msgstr "Ultima Ștampila de timp"
 
 msgctxt "field:ir.sequence.strict,name:"
 msgid "Sequence Name"
 msgstr "Numele secvenței"
 
+#, fuzzy
 msgctxt "field:ir.sequence.strict,number_increment:"
 msgid "Increment Number"
-msgstr ""
+msgstr "Număr de increment"
 
 msgctxt "field:ir.sequence.strict,number_next:"
 msgid "Next Number"
 msgstr "Numărul următor"
 
 msgctxt "field:ir.sequence.strict,number_next_internal:"
 msgid "Next Number"
@@ -1252,20 +1251,19 @@
 
 msgctxt "field:ir.sequence.strict,prefix:"
 msgid "Prefix"
 msgstr "Prefix"
 
 msgctxt "field:ir.sequence.strict,preview:"
 msgid "Preview"
-msgstr ""
+msgstr "Previzualizare"
 
-#, fuzzy
 msgctxt "field:ir.sequence.strict,sequence_type:"
 msgid "Sequence Type"
-msgstr "Tipuri de secvență"
+msgstr "Tip de secvență"
 
 msgctxt "field:ir.sequence.strict,suffix:"
 msgid "Suffix"
 msgstr "Sufix"
 
 msgctxt "field:ir.sequence.strict,timestamp_offset:"
 msgid "Timestamp Offset"
@@ -1517,28 +1515,27 @@
 
 msgctxt "field:ir.ui.view_search,user:"
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.ui.view_tree_optional,field:"
 msgid "Field"
-msgstr "Camp"
+msgstr "Câmp"
 
 msgctxt "field:ir.ui.view_tree_optional,user:"
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.ui.view_tree_optional,value:"
 msgid "Value"
 msgstr "Valoare"
 
-#, fuzzy
 msgctxt "field:ir.ui.view_tree_optional,view_id:"
 msgid "View ID"
-msgstr "Vederi"
+msgstr "ID Vedere"
 
 msgctxt "field:ir.ui.view_tree_state,child_name:"
 msgid "Child Name"
 msgstr "Numele copilului"
 
 msgctxt "field:ir.ui.view_tree_state,domain:"
 msgid "Domain"
@@ -1558,15 +1555,15 @@
 
 msgctxt "field:ir.ui.view_tree_state,user:"
 msgid "User"
 msgstr "Utilizator"
 
 msgctxt "field:ir.ui.view_tree_width,field:"
 msgid "Field"
-msgstr "Camp"
+msgstr "Câmp"
 
 msgctxt "field:ir.ui.view_tree_width,model:"
 msgid "Model"
 msgstr "Model"
 
 msgctxt "field:ir.ui.view_tree_width,user:"
 msgid "User"
@@ -1605,14 +1602,16 @@
 "LibreOffice pentru formatul compatibil."
 
 msgctxt "help:ir.action.report,record_name:"
 msgid ""
 "A Genshi expression to compute the name using 'record'.\n"
 "Leave empty for the default name."
 msgstr ""
+"O expresie Genshi pentru a calcula numele utilizând 'record'.\n"
+"Lăsați gol pentru numele prestabilit."
 
 msgctxt "help:ir.action.report,records:"
 msgid "The records on which the action runs."
 msgstr "Înregistrările pe care se desfășoară acțiunea."
 
 msgctxt "help:ir.action.report,single:"
 msgid "Check if the template works only for one record."
@@ -1644,50 +1643,50 @@
 
 #, fuzzy
 msgctxt "help:ir.email.template,recipients_hidden_pyson:"
 msgid ""
 "A PYSON expression that generates a list of hidden recipients with the "
 "record represented by \"self\"."
 msgstr ""
-"O declarație PYSON evaluată cu înregistrarea reprezentată de „sine”. "
-"Activează regula dacă este adevărată."
+"O expresie PYSON care generează o listă de destinatari ascunși cu "
+"înregistrarea reprezentată de \"self\"."
 
 #, fuzzy
 msgctxt "help:ir.email.template,recipients_pyson:"
 msgid ""
 "A PYSON expression that generates a list of recipients with the record "
 "represented by \"self\"."
 msgstr ""
-"O declarație PYSON evaluată cu înregistrarea reprezentată de „sine”. "
-"Activează regula dacă este adevărată."
+"O expresie PYSON care generează o listă de destinatari ascunși cu "
+"înregistrarea reprezentată de \"self\"."
 
 msgctxt "help:ir.email.template,recipients_secondary:"
 msgid "The field that contains the secondary recipient(s)."
-msgstr ""
+msgstr "Câmpul care conține destinatarii secundari."
 
 #, fuzzy
 msgctxt "help:ir.email.template,recipients_secondary_pyson:"
 msgid ""
 "A PYSON expression that generates a list of secondary recipients with the "
 "record represented by \"self\"."
 msgstr ""
-"O declarație PYSON evaluată cu înregistrarea reprezentată de „sine”. "
-"Activează regula dacă este adevărată."
+"O expresie PYSON care generează o listă de destinatari secundari cu "
+"înregistrarea reprezentată de \"self\"."
 
 msgctxt "help:ir.export,header:"
 msgid "Check to include field names on the export."
-msgstr ""
+msgstr "Bifați pentru a include numele câmpurilor în export."
 
 msgctxt "help:ir.export,records:"
 msgid "The records on which the export runs."
-msgstr ""
+msgstr "Înregistrările pe care se desfășoară exportul."
 
 msgctxt "help:ir.lang,code:"
 msgid "RFC 4646 tag."
-msgstr ""
+msgstr "Eticheta RFC 4646."
 
 msgctxt "help:ir.lang,parent:"
 msgid "Code of the exceptional parent"
 msgstr "Codul părintelui excepțional"
 
 msgctxt "help:ir.model,module:"
 msgid "Module in which this model is defined."
@@ -1699,35 +1698,39 @@
 "Text pentru a solicita confirmarea utilizatorului atunci când faceți clic pe"
 " buton."
 
 msgctxt "help:ir.model.button,reset_by:"
 msgid "Button that should reset the rules."
 msgstr "Buton care ar trebui să reseteze regulile."
 
+#, fuzzy
 msgctxt "help:ir.model.button.rule,condition:"
 msgid ""
 "A PYSON statement evaluated with the record represented by \"self\"\n"
 "It activate the rule if true."
 msgstr ""
-"O declarație PYSON evaluată cu înregistrarea reprezentată de „sine”\n"
+"O declarație PYSON evaluată cu înregistrarea reprezentată de \"self\"\n"
 "Activează regula dacă este adevărată."
 
 msgctxt "help:ir.model.data,db_id:"
 msgid "The id of the record in the database."
 msgstr "ID-ul înregistrării din baza de date."
 
 msgctxt "help:ir.model.data,fs_id:"
 msgid "The id of the record as known on the file system."
 msgstr "ID-ul înregistrării, cunoscut în sistemul de fișiere."
 
+#, fuzzy
 msgctxt "help:ir.model.field,access:"
 msgid ""
 "If checked, the access right on the model of the field is also tested "
 "against the relation of the field."
 msgstr ""
+"Dacă este bifat, dreptul de acces pe modelul câmpului este, de asemenea, "
+"testat față de relația câmpului."
 
 msgctxt "help:ir.model.field,module:"
 msgid "Module in which this field is defined."
 msgstr "Modulul în care este definit acest câmp."
 
 msgctxt "help:ir.model.print_model_graph.start,filter:"
 msgid ""
@@ -1741,22 +1744,21 @@
 msgid "When the task should be done."
 msgstr "Când sarcina ar trebui să fie făcută."
 
 msgctxt "help:ir.queue,scheduled_at:"
 msgid "When the task can start."
 msgstr "Când sarcina poate începe."
 
-#, fuzzy
 msgctxt "help:ir.rule,domain:"
 msgid ""
 "Domain is evaluated with a PYSON context containing:\n"
 "- \"groups\" as list of ids from the current user"
 msgstr ""
 "Domeniul este evaluat cu un context PYSON care conține:\n"
-"- \"user” ca utilizator curent"
+"- \"groups\" ca lista de identificatori de la utilizatorul curent"
 
 msgctxt "help:ir.rule.group,default_p:"
 msgid "Add this rule to all users by default."
 msgstr "Adăugați această regulă tuturor utilizatorilor în mod implicit."
 
 msgctxt "help:ir.rule.group,global_p:"
 msgid ""
@@ -1771,68 +1773,87 @@
 msgstr ""
 "Afișată utilizatorilor când o eroare de acces apare pentru această regulă."
 
 msgctxt "help:ir.rule.group,rules:"
 msgid "The rule is satisfied if at least one test is True."
 msgstr "Regula este satisfăcută dacă cel puțin un test este adevărat."
 
+#, fuzzy
 msgctxt "help:ir.sequence,prefix:"
 msgid ""
 "The current date can be used formatted using strftime format suffixed with "
 "underscores: i.e: ${date_Y}"
 msgstr ""
+"Data curentă poate fi folosită formatată folosind formatul strftime sufixat "
+"cu underscore: exemplu - ${date_Y}"
 
+#, fuzzy
 msgctxt "help:ir.sequence,suffix:"
 msgid ""
 "The current date can be used formatted using strftime format suffixed with "
 "underscores: i.e: ${date_Y}"
 msgstr ""
+"Data curentă poate fi folosită formatată folosind formatul strftime sufixat "
+"cu underscore: exemplu - ${date_Y}"
 
+#, fuzzy
 msgctxt "help:ir.sequence.strict,prefix:"
 msgid ""
 "The current date can be used formatted using strftime format suffixed with "
 "underscores: i.e: ${date_Y}"
 msgstr ""
+"Data curentă poate fi folosită formatată folosind formatul strftime sufixat "
+"cu underscore: exemplu - ${date_Y}"
 
+#, fuzzy
 msgctxt "help:ir.sequence.strict,suffix:"
 msgid ""
 "The current date can be used formatted using strftime format suffixed with "
 "underscores: i.e: ${date_Y}"
 msgstr ""
+"Data curentă poate fi folosită formatată folosind formatul strftime sufixat "
+"cu underscore: exemplu - ${date_Y}"
 
 msgctxt "help:ir.trigger,condition:"
 msgid ""
 "A PYSON statement evaluated with record represented by \"self\"\n"
 "It triggers the action if true."
 msgstr ""
+"O declarație PYSON evaluată cu înregistrarea reprezentată de \"self\"\n"
+"Declanșează acțiunea dacă este adevărat."
 
+#, fuzzy
 msgctxt "help:ir.trigger,limit_number:"
 msgid ""
 "Limit the number of call to \"Action Function\" by records.\n"
 "0 for no limit."
 msgstr ""
+"Limitați numărul de apeluri la \"Funcția de acțiune\" în funcție de înregistrări.\n"
+"0 pentru fără limită."
 
+#, fuzzy
 msgctxt "help:ir.trigger,minimum_time_delay:"
 msgid ""
 "Set a minimum time delay between call to \"Action Function\" for the same record.\n"
 "empty for no delay."
 msgstr ""
+"Setați o întârziere minimă între apelul la \"Funcția de acțiune\" pentru aceeași înregistrare.\n"
+"Lăsați gol pentru nicio întârziere."
 
-#, fuzzy
 msgctxt "help:ir.ui.view_search,domain:"
 msgid "The PYSON domain."
 msgstr "Domeniul PYSON."
 
 msgctxt "model:ir.action,name:"
 msgid "Action"
 msgstr "Acțiune"
 
 msgctxt "model:ir.action,name:act_action_act_window_form"
 msgid "Window Actions"
-msgstr ""
+msgstr "Actiuni Fereastra"
 
 msgctxt "model:ir.action,name:act_action_form"
 msgid "Actions"
 msgstr "Acțiuni"
 
 msgctxt "model:ir.action,name:act_action_report_form"
 msgid "Reports"
@@ -1854,20 +1875,18 @@
 msgid "Config Wizard Items"
 msgstr "Configurarea articolelor de asistent"
 
 msgctxt "model:ir.action,name:act_cron_form"
 msgid "Actions"
 msgstr "Acţiuni"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_email_form"
 msgid "E-mails"
 msgstr "E-mailuri"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_email_form_relate"
 msgid "E-mail Archives"
 msgstr "Arhive E-mailuri"
 
 msgctxt "model:ir.action,name:act_email_template_form"
 msgid "E-mail Templates"
 msgstr "Șabloane E-mail"
@@ -1880,35 +1899,33 @@
 msgid "Exports"
 msgstr "Exporturi"
 
 msgctxt "model:ir.action,name:act_icon_form"
 msgid "Icons"
 msgstr "Pictograme"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_lang_config"
 msgid "Configure Languages"
-msgstr "Configurarea modulelor"
+msgstr "Configurare Limba"
 
 msgctxt "model:ir.action,name:act_lang_form"
 msgid "Languages"
 msgstr "Limbi"
 
 msgctxt "model:ir.action,name:act_menu_list"
 msgid "Menu"
 msgstr "Meniu"
 
 msgctxt "model:ir.action,name:act_menu_tree"
 msgid "Menu"
 msgstr "Meniu"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_message_form"
 msgid "Messages"
-msgstr "Mesaj"
+msgstr "Mesaje"
 
 msgctxt "model:ir.action,name:act_model_access_form"
 msgid "Models Access"
 msgstr "Acces la modele"
 
 msgctxt "model:ir.action,name:act_model_access_form_relate_model"
 msgid "Access"
@@ -1938,17 +1955,18 @@
 msgid "Fields"
 msgstr "Câmpuri"
 
 msgctxt "model:ir.action,name:act_model_form"
 msgid "Models"
 msgstr "Modele"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_model_log_form"
 msgid "Logs"
-msgstr ""
+msgstr "Registre"
 
 msgctxt "model:ir.action,name:act_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
 msgstr "Efectuați activarea / modernizarea în așteptare"
 
 msgctxt "model:ir.action,name:act_module_config"
 msgid "Configure Modules"
@@ -2010,17 +2028,18 @@
 msgid "Triggers"
 msgstr "Declanșatoare"
 
 msgctxt "model:ir.action,name:act_view_form"
 msgid "Views"
 msgstr "Vederi"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_view_search"
 msgid "View Search"
-msgstr ""
+msgstr "Vizualizare Cautare"
 
 msgctxt "model:ir.action,name:act_view_show"
 msgid "Show View"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_view_tree_optional_form"
@@ -2115,23 +2134,23 @@
 
 msgctxt "model:ir.attachment,name:"
 msgid "Attachment"
 msgstr "Atașament"
 
 msgctxt "model:ir.avatar,name:"
 msgid "Avatar"
-msgstr ""
+msgstr "Avatar"
 
 msgctxt "model:ir.avatar.cache,name:"
 msgid "Avatar Cache"
-msgstr ""
+msgstr "Cache Avatar"
 
 msgctxt "model:ir.cache,name:"
 msgid "Cache"
-msgstr ""
+msgstr "Cache"
 
 msgctxt "model:ir.calendar.day,abbreviation:Friday"
 msgid "Fri"
 msgstr "Vin"
 
 msgctxt "model:ir.calendar.day,abbreviation:Monday"
 msgid "Mon"
@@ -2297,34 +2316,33 @@
 msgid "Cron"
 msgstr "Cron"
 
 msgctxt "model:ir.date,name:"
 msgid "Date"
 msgstr "Data"
 
-#, fuzzy
 msgctxt "model:ir.email,name:"
 msgid "Email"
-msgstr "Email"
+msgstr "E-mail"
 
 msgctxt "model:ir.email.address,name:"
 msgid "Email Address"
-msgstr ""
+msgstr "Adresa de E-mail"
 
 msgctxt "model:ir.email.template,name:"
 msgid "Email Template"
-msgstr ""
+msgstr "Sablon E-mail"
 
 msgctxt "model:ir.email.template-ir.action.report,name:"
 msgid "Email Template - Report"
-msgstr ""
+msgstr "Sablon E-mail - Raport"
 
 msgctxt "model:ir.error,name:"
 msgid "Error"
-msgstr ""
+msgstr "Eroare"
 
 msgctxt "model:ir.export,name:"
 msgid "Export"
 msgstr "Export"
 
 msgctxt "model:ir.export.line,name:"
 msgid "Export line"
@@ -2364,15 +2382,15 @@
 
 msgctxt "model:ir.lang,name:lang_et"
 msgid "Estonian"
 msgstr "Eston"
 
 msgctxt "model:ir.lang,name:lang_fa"
 msgid "Persian"
-msgstr ""
+msgstr "Persana"
 
 msgctxt "model:ir.lang,name:lang_fi"
 msgid "Finnish"
 msgstr "Finlandeză"
 
 msgctxt "model:ir.lang,name:lang_fr"
 msgid "French"
@@ -2392,178 +2410,177 @@
 
 msgctxt "model:ir.lang,name:lang_lo"
 msgid "Lao"
 msgstr "Lao"
 
 msgctxt "model:ir.lang,name:lang_lt"
 msgid "Lithuanian"
-msgstr ""
+msgstr "Lituaniana"
 
 msgctxt "model:ir.lang,name:lang_nl"
 msgid "Dutch"
 msgstr "Neerlandeză"
 
 msgctxt "model:ir.lang,name:lang_pl"
 msgid "Polish"
-msgstr ""
+msgstr "Poloneza"
 
 msgctxt "model:ir.lang,name:lang_pt"
 msgid "Portuguese"
 msgstr "Portugheză"
 
-#, fuzzy
 msgctxt "model:ir.lang,name:lang_ro"
 msgid "Romanian"
-msgstr "Eston"
+msgstr "Romana"
 
 msgctxt "model:ir.lang,name:lang_ru"
 msgid "Russian"
 msgstr "Rusă"
 
 msgctxt "model:ir.lang,name:lang_sl"
 msgid "Slovenian"
-msgstr ""
+msgstr "Slovena"
 
 msgctxt "model:ir.lang,name:lang_tr"
 msgid "Turkish"
-msgstr ""
+msgstr "Turca"
 
 msgctxt "model:ir.lang,name:lang_uk"
 msgid "Ukrainian"
-msgstr ""
+msgstr "Ucraineana"
 
 msgctxt "model:ir.lang,name:lang_zh_CN"
 msgid "Chinese Simplified"
 msgstr "Chineză simplificată"
 
-#, fuzzy
 msgctxt "model:ir.lang.config.start,name:"
 msgid "Configure languages"
-msgstr "Configurarea modulelor"
+msgstr "Configurarea limbilor"
 
 msgctxt "model:ir.message,name:"
 msgid "Message"
 msgstr "Mesaj"
 
 msgctxt "model:ir.message,text:msg_ID"
 msgid "ID"
 msgstr "ID"
 
 msgctxt "model:ir.message,text:msg_access_button_error"
 msgid "Calling button \"%(button)s on \"%(model)s\" is not allowed."
-msgstr ""
+msgstr "Apelarea butonului \"%(button)s\" de pe \"%(model)s\" nu este permisă."
 
 msgctxt "model:ir.message,text:msg_access_rule_error"
 msgid "You are not allowed to access \"%(model)s\"."
 msgstr "Nu aveț voie sa accessați \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_access_rule_field_error"
 msgid "You are not allowed to access \"%(model)s.%(field)s\"."
-msgstr ""
+msgstr "Nu aveți permisiunea de a accesa \"%(model)s.%(field)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_access_wizard_error"
 msgid "You are not allowed to execute wizard \"%(wizard)s\"."
-msgstr "Nu aveț voie sa accessați \"%(model)s\"."
+msgstr "Nu aveți permisiunea să executați expertul \"%(wizard)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_access_wizard_model_error"
 msgid "You are not allowed to execute wizard \"%(wizard)s\" on \"%(model)s\"."
-msgstr "Nu aveț voie sa accessați \"%(model)s\"."
+msgstr "Nu aveți permisiunea să executați expertul \"%(wizard)s\" pe \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_action_invalid_context"
 msgid "Invalid context \"%(context)s\" for action \"%(action)s\"."
-msgstr ""
+msgstr "Context invalid \"%(context)s\" pentru actiunea \"%(action)s\"."
 
 msgctxt "model:ir.message,text:msg_action_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for action \"%(action)s\"."
 msgstr ""
+"Domeniu sau criteriu de cautare invalid \"%(domain)s\" pentru actiunea "
+"\"%(action)s\"."
 
 msgctxt "model:ir.message,text:msg_action_invalid_views"
 msgid "Invalid view \"%(view)s\" for action \"%(action)s\"."
-msgstr ""
+msgstr "Vizualizare \"%(view)s\" invalidă pentru acțiunea \"%(action)s\"."
 
 msgctxt "model:ir.message,text:msg_action_wrong_wizard_model"
 msgid "Wrong wizard model in keyword action \"%(name)s\"."
-msgstr ""
+msgstr "Model greșit de expert în acțiunea cuvântului cheie \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_active"
 msgid "Active"
-msgstr ""
+msgstr "Activ"
 
 msgctxt "model:ir.message,text:msg_active_help"
 msgid "Uncheck to exclude from future use."
-msgstr ""
+msgstr "Debifați pentru a exclude din utilizarea viitoare."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_attachments"
 msgid "Attachments"
-msgstr "Fișiere atașate"
+msgstr "Atașamente"
 
 msgctxt "model:ir.message,text:msg_avatar"
 msgid "Avatar"
-msgstr ""
+msgstr "Avatar"
 
 msgctxt "model:ir.message,text:msg_avatar_resource_unique"
 msgid "Only one avatar is allowed per resource."
-msgstr ""
+msgstr "Un singur avatar este permis per resursa."
 
 msgctxt "model:ir.message,text:msg_avatar_size_unique"
 msgid "The size of an avatar must be unique."
-msgstr ""
+msgstr "Marimea unui avatar trebuie sa fie unica."
 
 msgctxt "model:ir.message,text:msg_avatar_url"
 msgid "Avatar URL"
-msgstr ""
+msgstr "URL Avatar"
 
 msgctxt "model:ir.message,text:msg_avatars"
 msgid "Avatars"
-msgstr ""
+msgstr "Avatare"
 
 msgctxt "model:ir.message,text:msg_base_config_record"
 msgid "This record is part of the base configuration."
-msgstr ""
+msgstr "Aceasta inregistrare face parte din configuratia de baza."
 
 msgctxt "model:ir.message,text:msg_button_name_unique"
 msgid "The name of the button must be unique per model."
-msgstr ""
+msgstr "Numele butonului trebuie sa fie unic per model."
 
 msgctxt "model:ir.message,text:msg_create_rule_error"
 msgid ""
 "You are not allowed to create records of \"%(model)s\" because they fail on at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
+"Nu aveți permisiunea de a crea înregistrări pentru \"%(model)s\" deoarece nu respectă cel puțin una dintre aceste reguli:\n"
+"%(rules)s"
 
 msgctxt "model:ir.message,text:msg_created_at"
 msgid "Created at"
-msgstr ""
+msgstr "Creat la"
 
 msgctxt "model:ir.message,text:msg_created_by"
 msgid "Created by"
-msgstr ""
+msgstr "Creat de"
 
 msgctxt "model:ir.message,text:msg_delete_rule_error"
 msgid ""
 "You are not allowed to delete records \"%(ids)s\" of \"%(model)s\" because of at lease one of those rules:\n"
 "%(rules)s"
 msgstr ""
+"Nu aveți voie să ștergeți înregistrările \"%(ids)s\" din \"%(model)s\" deoarece încalcă cel puțin una dintre aceste reguli:\n"
+"%(rules)s"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_delete_xml_record"
 msgid "You are not allowed to delete the record \"%(record)s\" of \"%(model)s\"."
-msgstr "Nu aveț voie sa accessați \"%(model)s\"."
+msgstr "Nu aveți voie să ștergeți înregistrarea \"%(record)s\" din \"%(model)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_no"
 msgid "No"
-msgstr "Noi"
+msgstr "Nu"
 
 msgctxt "model:ir.message,text:msg_dict_schema_boolean"
 msgid "Boolean"
-msgstr ""
+msgstr "Boolean"
 
 msgctxt "model:ir.message,text:msg_dict_schema_char"
 msgid "Char"
 msgstr "Char"
 
 msgctxt "model:ir.message,text:msg_dict_schema_date"
 msgid "Date"
@@ -2588,57 +2605,56 @@
 msgctxt "model:ir.message,text:msg_dict_schema_help"
 msgid "Help"
 msgstr "Ajutor"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_help_selection"
 msgid "Help Selection"
-msgstr "Selecție JSON"
+msgstr "Ajutor la Selectie"
 
 msgctxt "model:ir.message,text:msg_dict_schema_help_selection_help"
 msgid "The key followed by the help text separated by a \":\", one per line."
-msgstr ""
+msgstr "Tasta urmată de textul de ajutor separat de un \":\", câte unul pe rând."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_help_selection_json"
 msgid "Help Selection JSON"
-msgstr "Selecție JSON"
+msgstr "Ajutor Selecție JSON"
 
 msgctxt "model:ir.message,text:msg_dict_schema_integer"
 msgid "Integer"
 msgstr "Întreg"
 
 msgctxt "model:ir.message,text:msg_dict_schema_invalid_domain"
 msgid "Invalid domain in schema \"%(schema)s\"."
 msgstr "Domeniu nevalid din schema \"% (schema) s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_dict_schema_invalid_help_selection"
 msgid "Invalid help selection in schema \"%(schema)s\"."
-msgstr "Domeniu nevalid din schema \"% (schema) s\"."
+msgstr "Selecție de ajutor invalidă în schema \"%(schema)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_schema_invalid_selection"
 msgid "Invalid selection in schema \"%(schema)s\"."
-msgstr ""
+msgstr "Selecție invalidă în schema \"%(schema)s\"."
 
 msgctxt "model:ir.message,text:msg_dict_schema_multiselection"
 msgid "MultiSelection"
-msgstr ""
+msgstr "Selectie Multipla"
 
 msgctxt "model:ir.message,text:msg_dict_schema_name"
 msgid "Name"
-msgstr ""
+msgstr "Nume"
 
 msgctxt "model:ir.message,text:msg_dict_schema_numeric"
 msgid "Numeric"
-msgstr ""
+msgstr "Numeric"
 
 msgctxt "model:ir.message,text:msg_dict_schema_selection"
 msgid "Selection"
-msgstr ""
+msgstr "Selectie"
 
 msgctxt "model:ir.message,text:msg_dict_schema_selection_help"
 msgid "A couple of key and label separated by \":\" per line."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_dict_schema_selection_json"
 msgid "Selection JSON"
@@ -2658,421 +2674,455 @@
 
 msgctxt "model:ir.message,text:msg_dict_schema_type"
 msgid "Type"
 msgstr "Tip"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
-msgstr ""
+msgstr "Da"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+"Numărul de cifre din valoarea \"%(value)r\" pentru câmpul \"%(field)s\" din "
+"\"%(record)s\" din \"%(model)s\" depășește limita \"%(digits)i\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+"Valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din \"%(record)s\" din "
+"\"%(model)s\" nu este validă considerând domeniul său."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
-msgstr ""
+msgstr "Editat la"
 
 msgctxt "model:ir.message,text:msg_edited_by"
 msgid "Edited by"
-msgstr ""
+msgstr "Editat de"
 
 msgctxt "model:ir.message,text:msg_email_template_invalid_body"
 msgid ""
 "Invalid body in e-mail template \"%(template)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
+"Corp nevalid în șablonul de e-mail \"%(template)s\", cu excepția "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_email_template_invalid_field_pyson"
 msgid ""
 "Invalid PYSON %(field)s in e-mail template \"%(template)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
+"PYSON %(field)s invalid în șablonul de e-mail \"%(template)s\", cu excepția "
+"\"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_email_template_invalid_field_pyson_type"
 msgid ""
 "The PYSON %(field)s in e-mail template \"%(template)s\" must generate a "
 "list."
 msgstr ""
+"PYSON %(field)s din șablonul de e-mail \"%(template)s\" trebuie să genereze "
+"o listă."
 
 msgctxt "model:ir.message,text:msg_email_template_invalid_subject"
 msgid ""
 "Invalid subject in e-mail template \"%(template)s\" with exception "
 "\"%(exception)s\"."
 msgstr ""
+"Subiect invalid în șablonul de e-mail \"%(template)s\", cu excepția "
+"\"%(exception)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_field_model_name"
 msgid "%(field)s (model name)"
-msgstr ""
+msgstr "%(field)s (nume model)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+"Valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din \"%(record)s\" din "
+"\"%(model)s\" conține unele caractere nevalide: \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
 msgstr ""
+"Înregistrările nu au putut fi șterse deoarece sunt folosite de câmpul "
+"\"%(field)s\" din \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_missing"
 msgid "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" does not exist."
-msgstr ""
+msgstr "Valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din \"%(model)s\" nu există."
 
 msgctxt "model:ir.message,text:msg_html_editor_save_fail"
 msgid "Failed to save, please retry."
-msgstr ""
+msgstr "Salvare eșuată, încercați din nou."
 
 msgctxt "model:ir.message,text:msg_id_positive"
 msgid "ID must be positive."
-msgstr ""
+msgstr "ID trebuie să fie pozitiv."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_language_code_unique"
 msgid "The code on language must be unique."
-msgstr "Limba implicită trebuie să poată fi tradusă."
+msgstr "Codul de limbă trebuie să fie unic."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_language_default_translatable"
 msgid "The default language \"%(language)s\" must be translatable."
-msgstr "Limba implicită trebuie să poată fi tradusă."
+msgstr "Limba implicită \"%(language)s\" trebuie să poată fi tradusă."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_language_delete_default"
 msgid "The default language \"%(language)s\" can not be deleted."
-msgstr "Limba implicită nu poate fi ștearsă."
+msgstr "Limba implicită \"%(language)s\" nu poate fi ștearsă."
 
 msgctxt "model:ir.message,text:msg_language_invalid_date"
 msgid "Invalid date format \"%(format)s\" for language \"%(language)s\"."
 msgstr "Format invalid de data \"%(format)s\" pentru limba \"%(language)s\"."
 
 msgctxt "model:ir.message,text:msg_language_invalid_grouping"
 msgid "Invalid grouping \"%(grouping)s\" for language \"%(language)s\"."
-msgstr ""
+msgstr "Grupare invalidă \"%(grouping)s\" pentru limba \"%(language)s\"."
 
 msgctxt "model:ir.message,text:msg_model_invalid_condition"
 msgid ""
 "The condition \"%(condition)s\" is not a valid PYSON expression for button "
 "rule \"%(rule)s\"."
 msgstr ""
+"Condiția \"%(condition)s\" nu este o expresie PYSON validă pentru regula "
+"butonului \"%(rule)s\"."
 
 msgctxt "model:ir.message,text:msg_module_deactivate_dependency"
 msgid ""
 "Some activated modules depend on the ones you are trying to deactivate:"
 msgstr ""
+"Unele module activate depind de cele pe care încercați să le dezactivați:"
 
 msgctxt "model:ir.message,text:msg_module_delete_state"
 msgid ""
 "You can not remove a module that is activated or that is about to be "
 "activated."
 msgstr ""
+"Nu puteți elimina un modul care este activat sau care urmează să fie "
+"activat."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_notes"
 msgid "Notes"
 msgstr "Notițe"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_read_error"
 msgid "You are trying to read records \"%(ids)s\" of \"%(model)s\" that don't exist."
-msgstr "Nu aveț voie sa accessați \"%(model)s\"."
+msgstr ""
+"Încercați să citiți înregistrări \"%(ids)s\" din \"%(model)s\" care nu "
+"există."
 
 msgctxt "model:ir.message,text:msg_read_rule_error"
 msgid ""
 "You are not allowed to read records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
+"Nu aveți voie să citiți înregistrările \"%(ids)s\" din \"%(model)s\" din cauza a cel puțin uneia dintre aceste reguli:\n"
+"%(rules)s"
 
 msgctxt "model:ir.message,text:msg_record_name"
 msgid "Record Name"
-msgstr ""
+msgstr "Nume Inregistrare"
 
 msgctxt "model:ir.message,text:msg_recursion_error"
 msgid ""
 "Recursion error: Record \"%(rec_name)s\" with parent \"%(parent_rec_name)s\""
 " was configured as ancestor of itself."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_reference_syntax_error"
 msgid ""
 "Syntax error for reference: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
+"Eroare de sintaxă pentru referință: %(value)r în \"%(field)s\" din "
+"\"%(model)s\" (%(column)s)."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_relation_not_found"
 msgid "Relation not found: %(value)r in \"%(model)s\" (%(column)s)."
-msgstr "Relațianu a fost găsită: \"%(value)r\" in \"%(model)s\"."
+msgstr "Relația nu a fost găsită: \"%(value)r\" in \"%(model)s\" (%(column)s)."
 
 msgctxt "model:ir.message,text:msg_report_invalid_email"
 msgid "Invalid email definition for report \"%(name)s\"."
 msgstr "Email invalid pentru raport \"%(name)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_report_invalid_record_name"
 msgid ""
 "Invalid record name definition for report \"%(report)s\" with exception "
 "\"%(exception)s\"."
-msgstr "Email invalid pentru raport \"%(name)s\"."
+msgstr ""
+"Definiție nevalidă a numelui de înregistrare pentru raportul \"%(report)s\" "
+"cu excepția \"%(exception)s\"."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
-msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+msgstr "Este necesară o valoare pentru câmpul \"%(field)s\" din \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+"Este necesară o valoare pentru câmpul \"%(field)s\" din \"%(record)s\" din "
+"\"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
-msgstr ""
+msgstr "Resursele în care trebuie copiată această înregistrare."
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
 msgid "Invalid domain in rule \"%(name)s\"."
-msgstr ""
+msgstr "Domeniu invalid in regula \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
-msgstr ""
+msgstr "Lipsește funcția de căutare pentru câmpul \"%(field)s\" din \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
 "\"%(model)s\" depășește limita de \"%(digits)i\"."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
-msgstr ""
+msgstr "Secventa"
 
 msgctxt "model:ir.message,text:msg_sequence_change_sequence_type"
 msgid ""
 "You cannot change the sequence type of a sequence instead create a new "
 "sequence."
 msgstr ""
+"Nu puteți modifica tipul de secvență al unei secvențe. Trebuie să creați o "
+"nouă secvență."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_number_increment_next"
 msgid ""
 "Invalid \"Increment Number\" (%(number_increment)s) or \"Next Number\" "
 "(%(number_next)s) with exception \"%(exception)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_prefix"
 msgid "Invalid prefix \"%(affix)s\" for sequence \"%(sequence)s\"."
-msgstr ""
+msgstr "Prefix invalid \"%(affix)s\" pentru secventa \"%(sequence)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_invalid_suffix"
 msgid "Invalid suffix \"%(affix)s\" for sequence \"%(sequence)s\"."
-msgstr ""
+msgstr "Sufix invalid \"%(affix)s\" pentru secventa \"%(sequence)s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_last_timestamp_future"
 msgid "The \"Last Timestamp\" cannot be in the future for sequence \"%s\"."
-msgstr ""
+msgstr "Ultimul \"marcaj de timp\" nu poate fi în viitor pentru secvența \"%s\"."
 
 msgctxt "model:ir.message,text:msg_sequence_missing"
 msgid "Missing sequence."
 msgstr "Secvență lipsă."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_setter_function_missing"
 msgid "Missing setter function for field \"%(field)s\" in \"%(model)s\"."
-msgstr ""
+msgstr "Lipsește funcția de setare pentru câmpul \"%(field)s\" din \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_singleton"
 msgid "Only one singleton can be created."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+"Valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din \"%(model)s\" este "
+"prea lungă (%(size)i > %(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+"Valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din \"%(record)s\" al "
+"\"%(model)s\" este prea lungă (%(size)i > %(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+"Valoarea de timp \"%(value)s\" pentru câmpul \"%(field)s\" din "
+"\"%(record)s\" al \"%(model)s\" nu este valida."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
-msgstr ""
+msgstr "M"
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
 msgid "Y"
-msgstr ""
+msgstr "Y"
 
 msgctxt "model:ir.message,text:msg_timedelta_d"
 msgid "d"
-msgstr ""
+msgstr "d"
 
 msgctxt "model:ir.message,text:msg_timedelta_h"
 msgid "h"
-msgstr ""
+msgstr "h"
 
 msgctxt "model:ir.message,text:msg_timedelta_m"
 msgid "m"
-msgstr ""
+msgstr "m"
 
 msgctxt "model:ir.message,text:msg_timedelta_s"
 msgid "s"
-msgstr ""
+msgstr "s"
 
 msgctxt "model:ir.message,text:msg_timedelta_w"
 msgid "w"
-msgstr ""
+msgstr "w"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_too_many_relations_found"
 msgid "Too many relations found: %(value)r in \"%(model)s\" (%(column)s)."
-msgstr "S-au găsit prea multe relații: \"%(value)r\" in \"%(model)s\"."
+msgstr "S-au găsit prea multe relații: %(value)r in \"%(model)s\" (%(column)s)."
 
 msgctxt "model:ir.message,text:msg_translation_overridden"
 msgid ""
 "You can not export translation \"%(name)s\" because it has been overridden "
 "by module \"%(overriding_module)s\"."
 msgstr ""
+"Nu puteți exporta traducerea \"%(name)s\" deoarece a fost înlocuită de "
+"modulul \"%(overriding_module)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_trigger_exclusive"
 msgid ""
 "You can not select \"On Time\" and any other on the same time, they are "
 "mutually exclusive."
 msgstr ""
+"Nu puteți selecta \"La Timp\" și oricare altul în același timp, acestea se "
+"exclud reciproc."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_trigger_invalid_condition"
 msgid ""
 "Condition \"%(condition)s\" is not a valid PYSON expression for trigger "
 "\"%(trigger)s\"."
 msgstr ""
+"Condiția \"%(condition)s\" nu este o expresie PYSON validă pentru "
+"declanșatorul \"%(trigger)s\"."
 
 msgctxt "model:ir.message,text:msg_value_syntax_error"
 msgid ""
 "Syntax error for value: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
+"Eroare de sintaxă pentru valoarea: %(value)r în \"%(field)s\" din "
+"%(model)s\" (%(column)s)."
 
 msgctxt "model:ir.message,text:msg_view_invalid_xml"
 msgid "Invalid XML for view \"%(name)s\"."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_view_search_invalid_domain"
 msgid "Invalid domain or search criteria \"%(domain)s\" for search \"%(search)s\"."
-msgstr "Domeniu nevalid din schema \"% (schema) s\"."
+msgstr ""
+"Domeniu sau criterii de căutare invalide \"%(domain)s\" pentru căutarea "
+"\"%(search)s\"."
 
 msgctxt "model:ir.message,text:msg_view_tree_optional_type"
 msgid "You cannot store optional on view \"%(view)s\"."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_write_error"
 msgid ""
 "You are trying to write to records \"%(ids)s\" of \"%(model)s\" that don't "
 "exist."
-msgstr "Nu aveț voie sa accessați \"%(model)s\"."
+msgstr ""
+"Încercați să scrieți în înregistrările \"%(ids)s\" din \"%(model)s\" care nu"
+" există."
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
+"Nu aveți permisiunea de a scrie în înregistrările \"%(ids)s\" din \"%(model)s\" din cauza a cel puțin uneia dintre aceste reguli:\n"
+"%(rules)s"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr ""
-"Numărul de cifre din valoarea \"%(value)s\" pentru câmpul \"%(field)s\" din "
-"\"%(model)s\" depășește limita de \"%(digits)i\"."
+"Nu aveți permisiunea de a face modificări câmpului \"%(field)s\" din "
+"\"%(record)s\" din \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
 
 msgctxt "model:ir.model,name:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "model:ir.model.access,name:"
 msgid "Model access"
-msgstr ""
+msgstr "Acces Model"
 
 msgctxt "model:ir.model.button,confirm:lang_load_translations_button"
 msgid "Are you sure you want to load languages' translations?"
-msgstr ""
+msgstr "Sigur doriți să încărcați traducerile limbilor?"
 
 msgctxt "model:ir.model.button,confirm:lang_unload_translations_button"
 msgid "Are you sure you want to remove languages' translations?"
-msgstr ""
+msgstr "Sigur doriți să eliminați traducerile limbilor?"
 
 msgctxt "model:ir.model.button,name:"
 msgid "Model Button"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:cron_run_once_button"
 msgid "Run Once"
-msgstr ""
+msgstr "Rulează o singură dată"
 
 msgctxt "model:ir.model.button,string:error_open_button"
 msgid "Open"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:error_process_button"
 msgid "Process"
-msgstr "Acces"
+msgstr "Procesare"
 
 msgctxt "model:ir.model.button,string:error_solve_button"
 msgid "Solve"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:lang_load_translations_button"
@@ -3139,15 +3189,15 @@
 msgctxt "model:ir.model.field.access,name:"
 msgid "Model Field Access"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.model.log,name:"
 msgid "Log"
-msgstr "Lao"
+msgstr "Registru"
 
 msgctxt "model:ir.model.print_model_graph.start,name:"
 msgid "Print Model Graph"
 msgstr ""
 
 msgctxt "model:ir.module,name:"
 msgid "Module"
@@ -3278,17 +3328,18 @@
 msgid "Actions"
 msgstr "Acţiuni"
 
 msgctxt "model:ir.ui.menu,name:menu_action"
 msgid "Actions"
 msgstr "Acţiuni"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_action_act_window"
 msgid "Window Actions"
-msgstr ""
+msgstr "Acțiuni Fereastră"
 
 msgctxt "model:ir.ui.menu,name:menu_action_report_form"
 msgid "Reports"
 msgstr "Rapoarte"
 
 msgctxt "model:ir.ui.menu,name:menu_action_url"
 msgid "URLs"
@@ -3314,162 +3365,168 @@
 msgctxt "model:ir.ui.menu,name:menu_cron_form"
 msgid "Actions"
 msgstr "Acţiuni"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_email_form"
 msgid "E-mails"
-msgstr "Email"
+msgstr "E-mailuri"
 
 msgctxt "model:ir.ui.menu,name:menu_email_template_form"
 msgid "E-mail Templates"
-msgstr ""
+msgstr "Șabloane E-mail"
 
 msgctxt "model:ir.ui.menu,name:menu_error_form"
 msgid "Errors"
-msgstr ""
+msgstr "Erori"
 
 msgctxt "model:ir.ui.menu,name:menu_export_form"
 msgid "Exports"
-msgstr ""
+msgstr "Exporturi"
 
 msgctxt "model:ir.ui.menu,name:menu_icon_form"
 msgid "Icons"
-msgstr ""
+msgstr "Icoane"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_ir_sequence_type"
 msgid "Types"
-msgstr "Tip"
+msgstr "Tipuri"
 
 msgctxt "model:ir.ui.menu,name:menu_lang_form"
 msgid "Languages"
 msgstr "Limbi"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_localization"
 msgid "Localization"
-msgstr ""
+msgstr "Localizare"
 
 msgctxt "model:ir.ui.menu,name:menu_menu_list"
 msgid "Menu"
-msgstr ""
+msgstr "Meniu"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_message_form"
 msgid "Messages"
-msgstr "Mesaj"
+msgstr "Mesaje"
 
 msgctxt "model:ir.ui.menu,name:menu_model_access_form"
 msgid "Models Access"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_model_button_form"
 msgid "Buttons"
-msgstr ""
+msgstr "Butoane"
 
 msgctxt "model:ir.ui.menu,name:menu_model_data_form"
 msgid "Data"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_model_field_access_form"
 msgid "Fields Access"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_model_form"
 msgid "Models"
-msgstr ""
+msgstr "Modele"
 
 msgctxt "model:ir.ui.menu,name:menu_model_log_form"
 msgid "Logs"
-msgstr ""
+msgstr "Registre"
 
 msgctxt "model:ir.ui.menu,name:menu_models"
 msgid "Models"
-msgstr ""
+msgstr "Modele"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_module_activate_upgrade"
 msgid "Perform Pending Activation/Upgrade"
-msgstr ""
+msgstr "Efectuați Activarea/Actualizarea în așteptare"
 
 msgctxt "model:ir.ui.menu,name:menu_module_form"
 msgid "Modules"
-msgstr ""
+msgstr "Module"
 
 msgctxt "model:ir.ui.menu,name:menu_modules"
 msgid "Modules"
-msgstr ""
+msgstr "Module"
 
 msgctxt "model:ir.ui.menu,name:menu_note_form"
 msgid "Notes"
-msgstr ""
+msgstr "Notiţe"
 
 msgctxt "model:ir.ui.menu,name:menu_rule_group_form"
 msgid "Record Rules"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_scheduler"
 msgid "Scheduler"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_sequence_form"
 msgid "Sequences"
-msgstr ""
+msgstr "Secvenţe"
 
 msgctxt "model:ir.ui.menu,name:menu_sequence_strict_form"
 msgid "Sequences Strict"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_sequences"
 msgid "Sequences"
-msgstr ""
+msgstr "Secvenţe"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_translation_clean"
 msgid "Clean Translations"
-msgstr ""
+msgstr "Traduceri Curate"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_translation_export"
 msgid "Export Translations"
-msgstr ""
+msgstr "Traduceri de Export"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_translation_form"
 msgid "Translations"
-msgstr ""
+msgstr "Traduceri"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_translation_set"
 msgid "Set Translations"
-msgstr ""
+msgstr "Setare Traduceri"
 
 msgctxt "model:ir.ui.menu,name:menu_translation_update"
 msgid "Synchronize Translations"
-msgstr ""
+msgstr "Sincronizare Traduceri"
 
 msgctxt "model:ir.ui.menu,name:menu_trigger_form"
 msgid "Triggers"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_ui"
 msgid "User Interface"
-msgstr ""
+msgstr "Interfață Utilizator"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_view"
 msgid "Views"
-msgstr ""
+msgstr "Vizualizări"
 
 msgctxt "model:ir.ui.menu,name:menu_view_search"
 msgid "View Search"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_view_tree_optional"
 msgid "View Tree Optional"
 msgstr "Lațime Arbore Visualizare"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_view_tree_state"
 msgid "Tree State"
-msgstr ""
+msgstr "Stare Arbore"
 
 msgctxt "model:ir.ui.menu,name:menu_view_tree_width"
 msgid "View Tree Width"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:model_model_fields_form"
 msgid "Fields"
@@ -3558,103 +3615,96 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,records:"
 msgid "Selected"
 msgstr "Noduri selectate"
 
-#, fuzzy
 msgctxt "selection:ir.action.act_window,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action.act_window,type:"
 msgid "URL"
-msgstr "URL-uri"
+msgstr "URL"
 
-#, fuzzy
 msgctxt "selection:ir.action.act_window,type:"
 msgid "Window"
 msgstr "Fereastră"
 
 #, fuzzy
 msgctxt "selection:ir.action.act_window,type:"
 msgid "Wizard"
-msgstr "Asistenți"
+msgstr "Asistent"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Action form"
 msgstr ""
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Form relate"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Open Graph"
-msgstr ""
+msgstr "Deschidere Grafic"
 
+#, fuzzy
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Open tree"
-msgstr ""
+msgstr "Deschidere Arbore"
 
 msgctxt "selection:ir.action.keyword,keyword:"
 msgid "Print form"
-msgstr ""
+msgstr "Tiparire Formular"
 
 msgctxt "selection:ir.action.report,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.report,records:"
 msgid "Selected"
-msgstr "Noduri selectate"
+msgstr "Selectat"
 
-#, fuzzy
 msgctxt "selection:ir.action.report,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action.report,type:"
 msgid "URL"
-msgstr "URL-uri"
+msgstr "URL"
 
-#, fuzzy
 msgctxt "selection:ir.action.report,type:"
 msgid "Window"
 msgstr "Fereastră"
 
 #, fuzzy
 msgctxt "selection:ir.action.report,type:"
 msgid "Wizard"
-msgstr "Asistenți"
+msgstr "Asistent"
 
 msgctxt "selection:ir.action.url,records:"
 msgid "Listed"
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.url,records:"
 msgid "Selected"
-msgstr "Noduri selectate"
+msgstr "Selectat"
 
-#, fuzzy
 msgctxt "selection:ir.action.url,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action.url,type:"
 msgid "URL"
-msgstr "URL-uri"
+msgstr "URL"
 
-#, fuzzy
 msgctxt "selection:ir.action.url,type:"
 msgid "Window"
 msgstr "Fereastră"
 
 #, fuzzy
 msgctxt "selection:ir.action.url,type:"
 msgid "Wizard"
@@ -3665,61 +3715,57 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "selection:ir.action.wizard,records:"
 msgid "Selected"
 msgstr "Noduri selectate"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,type:"
 msgid "Report"
 msgstr "Raport"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,type:"
 msgid "URL"
-msgstr "URL-uri"
+msgstr "URL"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,type:"
 msgid "Window"
 msgstr "Fereastră"
 
-#, fuzzy
 msgctxt "selection:ir.action.wizard,type:"
 msgid "Wizard"
-msgstr "Asistenți"
+msgstr "Asistent"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Data"
-msgstr ""
+msgstr "Date"
 
 msgctxt "selection:ir.attachment,type:"
 msgid "Link"
-msgstr ""
+msgstr "Legătură"
 
 msgctxt "selection:ir.cron,interval_type:"
 msgid "Days"
-msgstr ""
+msgstr "Zile"
 
 msgctxt "selection:ir.cron,interval_type:"
 msgid "Hours"
-msgstr ""
+msgstr "Ore"
 
 msgctxt "selection:ir.cron,interval_type:"
 msgid "Minutes"
-msgstr ""
+msgstr "Minute"
 
 msgctxt "selection:ir.cron,interval_type:"
 msgid "Months"
-msgstr ""
+msgstr "Luni"
 
 msgctxt "selection:ir.cron,interval_type:"
 msgid "Weeks"
-msgstr ""
+msgstr "Săptămâni"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Clean Errors"
 msgstr ""
 
 msgctxt "selection:ir.cron,method:"
 msgid "Clean Task Queue"
@@ -3808,123 +3854,124 @@
 
 msgctxt "selection:ir.module,state:"
 msgid "To be upgraded"
 msgstr ""
 
 msgctxt "selection:ir.module.config_wizard.item,state:"
 msgid "Done"
-msgstr ""
+msgstr "Terminat"
 
 msgctxt "selection:ir.module.config_wizard.item,state:"
 msgid "Open"
-msgstr ""
+msgstr "Deschis"
 
 msgctxt "selection:ir.module.dependency,state:"
 msgid "Activated"
-msgstr ""
+msgstr "Activat"
 
 msgctxt "selection:ir.module.dependency,state:"
 msgid "Not Activated"
-msgstr ""
+msgstr "Ne-Activat"
 
 msgctxt "selection:ir.module.dependency,state:"
 msgid "To be activated"
-msgstr ""
+msgstr "Va fi activat"
 
 msgctxt "selection:ir.module.dependency,state:"
 msgid "To be removed"
-msgstr ""
+msgstr "Va fi eliminat"
 
 msgctxt "selection:ir.module.dependency,state:"
 msgid "To be upgraded"
-msgstr ""
+msgstr "Va fi actualizat"
 
 msgctxt "selection:ir.module.dependency,state:"
 msgid "Unknown"
-msgstr ""
+msgstr "Necunoscut"
 
 msgctxt "selection:ir.sequence,type:"
 msgid "Decimal Timestamp"
 msgstr ""
 
 msgctxt "selection:ir.sequence,type:"
 msgid "Hexadecimal Timestamp"
 msgstr ""
 
 msgctxt "selection:ir.sequence,type:"
 msgid "Incremental"
-msgstr ""
+msgstr "Incremental"
 
 msgctxt "selection:ir.sequence.strict,type:"
 msgid "Decimal Timestamp"
 msgstr ""
 
 msgctxt "selection:ir.sequence.strict,type:"
 msgid "Hexadecimal Timestamp"
 msgstr ""
 
 msgctxt "selection:ir.sequence.strict,type:"
 msgid "Incremental"
-msgstr ""
+msgstr "Incremental"
 
 msgctxt "selection:ir.translation,type:"
 msgid "Field"
-msgstr ""
+msgstr "Câmp"
 
 msgctxt "selection:ir.translation,type:"
 msgid "Help"
-msgstr ""
+msgstr "Ajutor"
 
 msgctxt "selection:ir.translation,type:"
 msgid "Model"
-msgstr ""
+msgstr "Model"
 
 msgctxt "selection:ir.translation,type:"
 msgid "Report"
-msgstr ""
+msgstr "Raport"
 
 msgctxt "selection:ir.translation,type:"
 msgid "Selection"
-msgstr ""
+msgstr "Selecţie"
 
 msgctxt "selection:ir.translation,type:"
 msgid "View"
-msgstr ""
+msgstr "Vedere"
 
 msgctxt "selection:ir.translation,type:"
 msgid "Wizard Button"
 msgstr ""
 
 msgctxt "selection:ir.ui.view,type:"
 msgid "Board"
 msgstr ""
 
 msgctxt "selection:ir.ui.view,type:"
 msgid "Calendar"
-msgstr ""
+msgstr "Calendar"
 
 msgctxt "selection:ir.ui.view,type:"
 msgid "Form"
 msgstr "Formular"
 
 msgctxt "selection:ir.ui.view,type:"
 msgid "Graph"
-msgstr ""
+msgstr "Grafic"
 
 msgctxt "selection:ir.ui.view,type:"
 msgid "List Form"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:ir.ui.view,type:"
 msgid "Tree"
-msgstr ""
+msgstr "Arbore"
 
 msgctxt "view:ir.action.report:"
 msgid "Edit"
-msgstr ""
+msgstr "Editare"
 
 msgctxt "view:ir.action:"
 msgid "General"
 msgstr "General"
 
 msgctxt "view:ir.attachment:"
 msgid "Document"
@@ -3938,243 +3985,247 @@
 msgid "At"
 msgstr "La"
 
 msgctxt "view:ir.cron:"
 msgid "Every"
 msgstr "Fiecare"
 
-#, fuzzy
 msgctxt "view:ir.cron:"
 msgid "Next Call Date"
-msgstr "Următorul apel"
+msgstr "Data Următorului Apel"
 
-#, fuzzy
 msgctxt "view:ir.cron:"
 msgid "Next Call Time"
-msgstr "Următorul apel"
+msgstr "Ora Următorului apel"
 
 msgctxt "view:ir.cron:"
 msgid "Run Once"
 msgstr "Rulează o Singură Dată"
 
+#, fuzzy
 msgctxt "view:ir.email.template:"
 msgid "Hidden Recipients:"
-msgstr ""
+msgstr "Destinatari Ascunsi:"
 
 msgctxt "view:ir.email.template:"
 msgid "Recipients:"
-msgstr ""
+msgstr "Destinatari:"
 
 msgctxt "view:ir.email.template:"
 msgid "Secondary Recipients:"
-msgstr ""
+msgstr "Destinatari Secundari:"
 
 msgctxt "view:ir.error:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "view:ir.lang.config.start:"
 msgid "You can now load additional translations to the system."
-msgstr ""
+msgstr "Acum puteți încărca în sistem traduceri suplimentare."
 
 msgctxt "view:ir.lang:"
 msgid "Date Formatting"
-msgstr ""
+msgstr "Format Dată"
 
+#, fuzzy
 msgctxt "view:ir.lang:"
 msgid "Monetary Formatting"
-msgstr ""
+msgstr "Format Monedă"
 
+#, fuzzy
 msgctxt "view:ir.lang:"
 msgid "Numbers Formatting"
-msgstr ""
+msgstr "Format Numere"
 
-#, fuzzy
 msgctxt "view:ir.model.log:"
 msgid "Date"
 msgstr "Data"
 
-#, fuzzy
 msgctxt "view:ir.model.log:"
 msgid "Hour"
 msgstr "Ora"
 
-#, fuzzy
 msgctxt "view:ir.model.log:"
 msgid "at"
-msgstr "Sâm"
+msgstr "la"
 
 msgctxt "view:ir.module.activate_upgrade.done:"
 msgid "The modules have been upgraded / activated."
-msgstr ""
+msgstr "Modulele au fost actualizate / activate."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Note that this operation may take a few minutes."
-msgstr ""
+msgstr "Rețineți că această operațiune poate dura câteva minute."
 
 msgctxt "view:ir.module.activate_upgrade.start:"
 msgid "Your system will be upgraded."
-msgstr ""
+msgstr "Sistemul dumneavoastră va fi actualizat."
 
 msgctxt "view:ir.module.config.start:"
 msgid "You can now activate additional modules to the system."
-msgstr ""
+msgstr "Acum se pot activa module suplimentare în sistem."
 
 msgctxt "view:ir.module.config_wizard.done:"
 msgid "The configuration is done."
-msgstr ""
+msgstr "Configurarea este făcută."
 
 msgctxt "view:ir.module.config_wizard.first:"
 msgid ""
 "You will be able to configure your installation depending on the modules you"
 " have installed."
 msgstr ""
+"Veți putea să vă configurați instalarea în funcție de modulele pe care le-"
+"ați instalat."
 
 msgctxt "view:ir.module:"
 msgid "Cancel Activation"
-msgstr ""
+msgstr "Anulați activarea"
 
 msgctxt "view:ir.module:"
 msgid "Cancel Deactivation"
-msgstr ""
+msgstr "Anulați dezactivarea"
 
 msgctxt "view:ir.module:"
 msgid "Cancel Upgrade"
-msgstr ""
+msgstr "Anulați actualizarea"
 
 msgctxt "view:ir.module:"
 msgid "Mark for Activation"
-msgstr ""
+msgstr "Marcați pentru activare"
 
 msgctxt "view:ir.module:"
 msgid "Mark for Deactivation (beta)"
-msgstr ""
+msgstr "Marcați pentru dezactivare (beta)"
 
 msgctxt "view:ir.module:"
 msgid "Mark for Upgrade"
-msgstr ""
+msgstr "Marcați pentru actualizare"
 
 msgctxt "view:ir.note:"
 msgid "Date"
 msgstr "Data"
 
 msgctxt "view:ir.note:"
 msgid "Time"
-msgstr ""
+msgstr "Timp"
 
 msgctxt "view:ir.note:"
 msgid "User"
-msgstr ""
+msgstr "Utilizator"
 
+#, fuzzy
 msgctxt "view:ir.rule.group:"
 msgid ""
 "If there is no test defined, the rule is always satisfied if not global."
 msgstr ""
+"Dacă nu există nici un test definit, regula este întotdeauna satisfăcută, "
+"dacă nu este globală."
 
+#, fuzzy
 msgctxt "view:ir.rule.group:"
 msgid "The rule is satisfied if at least one test is True."
-msgstr ""
+msgstr "Regula este îndeplinită dacă cel puțin un test este Adevărat."
 
+#, fuzzy
 msgctxt "view:ir.translation.clean.start:"
 msgid "Clean Translations?"
-msgstr ""
+msgstr "Curățare Traduceri?"
 
 msgctxt "view:ir.translation.clean.succeed:"
 msgid "Translations cleaned successfully."
-msgstr ""
+msgstr "Traducerile au fost curățate cu succes."
 
 msgctxt "view:ir.translation.set.start:"
 msgid "Synchronize Translations?"
-msgstr ""
+msgstr "Sincronizare Traduceri?"
 
 msgctxt "view:ir.translation.set.succeed:"
 msgid "Translations set successfully."
-msgstr ""
+msgstr "Traduceri setate cu succes."
 
-#, fuzzy
 msgctxt "view:ir.ui.menu:"
 msgid "Actions"
-msgstr "Acțiuni"
+msgstr "Acţiuni"
 
 msgctxt "wizard_button:ir.lang.config,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:ir.lang.config,start,load:"
 msgid "Load"
 msgstr ""
 
 msgctxt "wizard_button:ir.model.print_model_graph,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:ir.model.print_model_graph,start,print_:"
 msgid "Print"
-msgstr ""
+msgstr "Tipărire"
 
 msgctxt "wizard_button:ir.module.activate_upgrade,done,next_:"
 msgid "OK"
-msgstr ""
+msgstr "OK"
 
 msgctxt "wizard_button:ir.module.activate_upgrade,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
+#, fuzzy
 msgctxt "wizard_button:ir.module.activate_upgrade,start,upgrade:"
 msgid "Start Upgrade"
-msgstr ""
+msgstr "Start Actualizare"
 
 msgctxt "wizard_button:ir.module.config,start,activate:"
 msgid "Activate"
-msgstr ""
+msgstr "Activare"
 
-#, fuzzy
 msgctxt "wizard_button:ir.module.config,start,end:"
 msgid "Cancel"
 msgstr "Anulare"
 
 msgctxt "wizard_button:ir.module.config_wizard,done,end:"
 msgid "OK"
-msgstr ""
+msgstr "OK"
 
 msgctxt "wizard_button:ir.module.config_wizard,first,action:"
 msgid "OK"
-msgstr ""
+msgstr "OK"
 
 msgctxt "wizard_button:ir.module.config_wizard,first,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:ir.module.config_wizard,other,action:"
 msgid "Next"
-msgstr ""
+msgstr "Următorul"
 
 msgctxt "wizard_button:ir.module.config_wizard,other,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:ir.translation.clean,start,clean:"
 msgid "Clean"
 msgstr ""
 
 msgctxt "wizard_button:ir.translation.clean,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:ir.translation.clean,succeed,end:"
 msgid "OK"
-msgstr ""
+msgstr "OK"
 
 msgctxt "wizard_button:ir.translation.export,result,end:"
 msgid "Close"
-msgstr ""
+msgstr "Închidere"
 
 msgctxt "wizard_button:ir.translation.export,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:ir.translation.export,start,export:"
 msgid "Export"
 msgstr "Export"
 
 msgctxt "wizard_button:ir.translation.set,start,end:"
 msgid "Cancel"
@@ -4182,20 +4233,20 @@
 
 msgctxt "wizard_button:ir.translation.set,start,set_:"
 msgid "Set"
 msgstr ""
 
 msgctxt "wizard_button:ir.translation.set,succeed,end:"
 msgid "OK"
-msgstr ""
+msgstr "OK"
 
 msgctxt "wizard_button:ir.translation.update,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:ir.translation.update,start,update:"
 msgid "Update"
-msgstr ""
+msgstr "Actualizare"
 
 msgctxt "wizard_button:ir.ui.view.show,start,end:"
 msgid "Close"
-msgstr ""
+msgstr "Închidere"
```

### Comparing `trytond-7.0.9/trytond/ir/locale/ru.po` & `trytond-7.2.0/trytond/ir/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -2832,23 +2832,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
 " to its domain."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_edited_at"
@@ -2894,15 +2894,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -3026,15 +3026,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 #, fuzzy
@@ -3046,15 +3048,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
@@ -3108,23 +3110,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
@@ -3215,16 +3217,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/sl.po` & `trytond-7.2.0/trytond/ir/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -2635,25 +2635,31 @@
 msgid "Type"
 msgstr "Vrsta"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "Da"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
+"Število decimalk \"%(digits)s\" polja \"%(field)s\" pri \"%(value)s\" je "
+"preseženo."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
+"The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
+" to its domain."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "Urejeno ob"
 
 msgctxt "model:ir.message,text:msg_edited_by"
 msgid "Edited by"
@@ -2687,19 +2693,22 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (naziv modela)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(field)s (niz znakov)"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
+"The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
+"valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
 "The records could not be deleted because they are used by field "
 "\"%(field)s\" of \"%(model)s\"."
 msgstr ""
 
@@ -2802,35 +2811,41 @@
 "\"%(exception)s\"."
 msgstr "Neveljaven kontekst \"%(context)s\" pri ukrepu \"%(action)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Vrednost je zahtevana za polje \"%(field)s\" na modelu \"%(model)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
-msgstr ""
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
+msgstr "Vrednost je zahtevana za polje \"%(field)s\" na modelu \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "Neveljavna domena pri pravilu \"%(name)s\"."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
+"The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
+"the selection."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
 msgstr "Številčna serija"
 
 msgctxt "model:ir.message,text:msg_sequence_change_sequence_type"
 msgid ""
@@ -2871,25 +2886,31 @@
 
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
+"The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
+"the selection."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
+"The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
+"valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
 msgid "Y"
@@ -2969,19 +2990,20 @@
 
 msgctxt "model:ir.message,text:msg_write_rule_error"
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
-msgstr ""
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
+msgstr "Nimate dovoljenja za brisanje zapisa \"%(record)s\" na modelu \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/tr.po` & `trytond-7.2.0/trytond/ir/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -2738,23 +2738,23 @@
 msgid "Yes"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" exceeds the "
 "digits limit of \"%(digits)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "The value of the field \"%(field)s\" on \"%(model)s\" is not valid according"
 " to its domain."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2795,15 +2795,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2916,15 +2916,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2935,15 +2937,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Missing search function on field \"%s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not in "
 "the selection."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_sequence"
@@ -2992,23 +2994,23 @@
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr ""
 "The time value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" is not "
 "valid."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr ""
@@ -3091,16 +3093,16 @@
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "The value \"%(value)s\" of field \"%(field)s\" on \"%(model)s\" doesn't exist."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/uk.po` & `trytond-7.2.0/trytond/ir/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -2658,23 +2658,23 @@
 msgid "Yes"
 msgstr "Так"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr ""
 "Кількість цифр у значенні \"%(value)s\" для поля \"%(field)s\" у "
 "\"%(model)s\" перевищує ліміт \"%(digits)i\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr ""
 "Значення поля \"%(field)s\" в \"%(model)s\" недійсне відповідно дойого "
 "домену."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
@@ -2723,15 +2723,15 @@
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "Значення \"%(value)s\" для поля \"%(field)s\" в \"%(model)s\" містить деякі "
 "недійсні символи \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2853,15 +2853,17 @@
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Потрібно значення для поля \"%(field)s\" в \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "Потрібно значення для поля \"%(field)s\" в \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "Ресурси, на які потрібно скопіювати цей запис."
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
@@ -2871,15 +2873,15 @@
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "Відсутня функція пошуку для поля \"%(field)s\" в \"%(model)s\"."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "Значення \"%(value)s\" для поля \"%(field)s\" в \"%(model)s\" не є одним із "
 "дозволених параметрів."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2935,25 +2937,25 @@
 msgstr ""
 "Значення поля \"%(field)s\" в \"%(model)s\" задовге (%(size)i > "
 "%(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "Значення поля \"%(field)s\" в \"%(model)s\" задовге (%(size)i > "
 "%(max_size)i)."
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr "Недійсне значення часу \"%(value)s\" поля \"%(field)s\" в \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "M"
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
@@ -3042,16 +3044,16 @@
 msgstr ""
 "Вам заборонено писати в записи \"%(ids)s\" з \"%(model)s\" через принаймні одне з цих правил:\n"
 "%(rules)s"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "Потрібно значення для поля \"%(field)s\" в \"%(model)s\"."
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/ir/locale/zh_CN.po` & `trytond-7.2.0/trytond/ir/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -2631,23 +2631,25 @@
 msgid "Type"
 msgstr "类型"
 
 msgctxt "model:ir.message,text:msg_dict_yes"
 msgid "Yes"
 msgstr "是"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_digits_validation_record"
 msgid ""
 "The number of digits in the value \"%(value)r\" for field \"%(field)s\" in "
-"\"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
+"record \"%(record)s\" of \"%(model)s\" exceeds the limit of \"%(digits)i\"."
 msgstr "模型 \"%(model)s\" ，其字段 \"%(field)s\" 的数字取值 \"%(value)s\" 的位数超出了 \"%(digits)i\" 的限制."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_domain_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not valid according to its domain."
 msgstr "模型 \"%(model)s\" 的记录\"%(record)s\"，其字段 \"%(field)s\" 的取值\"%(value)s\" 对于其域来说，是无效取值."
 
 msgctxt "model:ir.message,text:msg_edited_at"
 msgid "Edited at"
 msgstr "编辑时间"
 
@@ -2683,17 +2685,18 @@
 msgid "%(field)s (model name)"
 msgstr "%(field)s (模型名称)"
 
 msgctxt "model:ir.message,text:msg_field_string"
 msgid "%(field)s (string)"
 msgstr "%(field)s (字符串)"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_forbidden_char_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" contains some invalid chars \"%(chars)s\"."
 msgstr ""
 "模型 \"%(model)s\" 的记录 \"%(record)s\"，其字段 \"%(field)s\" 的取值 \"%(value)s\" "
 "包含一些无效字符 \"%(chars)s\"."
 
 msgctxt "model:ir.message,text:msg_foreign_model_exist"
 msgid ""
@@ -2796,33 +2799,37 @@
 "\"%(exception)s\"."
 msgstr "报告 \"%(report)s\" 中的记录名称定义无效，异常为 \"%(exception)s\"."
 
 msgctxt "model:ir.message,text:msg_required_validation"
 msgid "A value is required for field \"%(field)s\" in \"%(model)s\"."
 msgstr "模型\"%(model)s\"的字段\"%(field)s\"需要有取值."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_required_validation_record"
-msgid "A value is required for field \"%(field)s\" in \"%(record)s\" of \"%(model)s\"."
+msgid ""
+"A value is required for field \"%(field)s\" in record \"%(record)s\" of "
+"\"%(model)s\"."
 msgstr "模型\"%(model)s\"包含记录\"%(record)s\"，此记录包含的字段\"%(field)s\"需要有取值."
 
 msgctxt "model:ir.message,text:msg_resource_copy_help"
 msgid "The resources to which this record must be copied."
 msgstr "必须将此记录复制的资源."
 
 msgctxt "model:ir.message,text:msg_rule_invalid_domain"
 msgid "Invalid domain in rule \"%(name)s\"."
 msgstr "规则\"%(name)s\"的域配置无效."
 
 msgctxt "model:ir.message,text:msg_search_function_missing"
 msgid "Missing search function for field \"%(field)s\" in \"%(model)s\"."
 msgstr "模型 \"%(model)s\" 的字段 \"%(field)s\" 缺少搜索函数."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_selection_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is not one of the allowed options."
 msgstr ""
 "模型 \"%(model)s\" 包含记录 \"%(record)s\"，此记录包含字段 "
 "\"%(field)s\"，这个字段的取值\"%(value)s\" 不在允许的选项范围内."
 
 msgctxt "model:ir.message,text:msg_sequence"
 msgid "Sequence"
@@ -2868,26 +2875,28 @@
 
 msgctxt "model:ir.message,text:msg_size_validation"
 msgid ""
 "The value \"%(value)s\" for field \"%(field)s\" in \"%(model)s\" is too long"
 " (%(size)i > %(max_size)i)."
 msgstr "模型 \"%(model)s\" 中字段 \"%(field)s\" 的值 \"%(value)s\" 太长 (%(size)i > %(max_size)i)。"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_size_validation_record"
 msgid ""
-"The value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
+"The value \"%(value)s\" for field \"%(field)s\" in record \"%(record)s\" of "
 "\"%(model)s\" is too long (%(size)i > %(max_size)i)."
 msgstr ""
 "模型 \"%(model)s\" 的字段 \"%(field)s\" ，其取值 \"%(value)s\" 位数太长(%(size)i > "
 "%(max_size)i)."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_time_format_validation_record"
 msgid ""
-"The time value \"%(value)s\" for field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\" is not valid."
+"The time value \"%(value)s\" for field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\" is not valid."
 msgstr "\"%(model)s\" 包含的记录 \"%(record)s\" 中的字段 \"%(field)s\" 时间取值 \"%(value)s\" 无效。"
 
 msgctxt "model:ir.message,text:msg_timedelta_M"
 msgid "M"
 msgstr "月"
 
 msgctxt "model:ir.message,text:msg_timedelta_Y"
@@ -2964,18 +2973,19 @@
 msgid ""
 "You are not allowed to write to records \"%(ids)s\" of \"%(model)s\" because of at least one of these rules:\n"
 "%(rules)s"
 msgstr ""
 "不允许写入模型 \"%(model)s\" 的记录 \"%(ids)s\" ， 由于下面的规则（至少一条）:\n"
 "%(rules)s"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_write_xml_record"
 msgid ""
-"You are not allowed to modify the field \"%(field)s\" in \"%(record)s\" of "
-"\"%(model)s\"."
+"You are not allowed to modify the field \"%(field)s\" in record "
+"\"%(record)s\" of \"%(model)s\"."
 msgstr "不允许修改 \"%(model)s\" 的 \"%(record)s\" 中的字段 \"%(field)s\"。"
 
 msgctxt "model:ir.message,text:msg_xml_id_syntax_error"
 msgid ""
 "Syntax error for XML id: %(value)r in \"%(field)s\" of \"%(model)s\" "
 "(%(column)s)."
 msgstr "\"%(model)s\"（%(column)s 的 \"%(field)s\"）中的 XML %(value)r 的语法错误。"
```

### Comparing `trytond-7.0.9/trytond/ir/message.py` & `trytond-7.2.0/trytond/ir/message.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/message.xml` & `trytond-7.2.0/trytond/ir/message.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/message.xml` & `trytond-7.2.0/trytond/ir/message.xml`

```diff
@@ -44,14 +44,17 @@
     </record>
     <record model="ir.message" id="msg_edited_at">
       <field name="text">Edited at</field>
     </record>
     <record model="ir.message" id="msg_record_name">
       <field name="text">Record Name</field>
     </record>
+    <record model="ir.message" id="msg_xml_id">
+      <field name="text">XML ID</field>
+    </record>
     <record model="ir.message" id="msg_active">
       <field name="text">Active</field>
     </record>
     <record model="ir.message" id="msg_active_help">
       <field name="text">Uncheck to exclude from future use.</field>
     </record>
     <record model="ir.message" id="msg_dict_schema_name">
@@ -132,15 +135,15 @@
     <record model="ir.message" id="msg_id_positive">
       <field name="text">ID must be positive.</field>
     </record>
     <record model="ir.message" id="msg_singleton">
       <field name="text">Only one singleton can be created.</field>
     </record>
     <record model="ir.message" id="msg_write_xml_record">
-      <field name="text">You are not allowed to modify the field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot;.</field>
+      <field name="text">You are not allowed to modify the field &quot;%(field)s&quot; in record &quot;%(record)s&quot; of &quot;%(model)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_delete_xml_record">
       <field name="text">You are not allowed to delete the record &quot;%(record)s&quot; of &quot;%(model)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_base_config_record">
       <field name="text">This record is part of the base configuration.</field>
     </record>
@@ -156,39 +159,39 @@
     <record model="ir.message" id="msg_reference_syntax_error">
       <field name="text">Syntax error for reference: %(value)r in &quot;%(field)s&quot; of &quot;%(model)s&quot; (%(column)s).</field>
     </record>
     <record model="ir.message" id="msg_xml_id_syntax_error">
       <field name="text">Syntax error for XML id: %(value)r in &quot;%(field)s&quot; of &quot;%(model)s&quot; (%(column)s).</field>
     </record>
     <record model="ir.message" id="msg_domain_validation_record">
-      <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot; is not valid according to its domain.</field>
+      <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in record &quot;%(record)s&quot; of &quot;%(model)s&quot; is not valid according to its domain.</field>
     </record>
     <record model="ir.message" id="msg_required_validation">
       <field name="text">A value is required for field &quot;%(field)s&quot; in &quot;%(model)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_required_validation_record">
-      <field name="text">A value is required for field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot;.</field>
+      <field name="text">A value is required for field &quot;%(field)s&quot; in record &quot;%(record)s&quot; of &quot;%(model)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_size_validation">
       <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in &quot;%(model)s&quot; is too long (%(size)i &gt; %(max_size)i).</field>
     </record>
     <record model="ir.message" id="msg_size_validation_record">
-      <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot; is too long (%(size)i &gt; %(max_size)i).</field>
+      <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in record &quot;%(record)s&quot; of &quot;%(model)s&quot; is too long (%(size)i &gt; %(max_size)i).</field>
     </record>
     <record model="ir.message" id="msg_digits_validation_record">
-      <field name="text">The number of digits in the value &quot;%(value)r&quot; for field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot; exceeds the limit of &quot;%(digits)i&quot;.</field>
+      <field name="text">The number of digits in the value &quot;%(value)r&quot; for field &quot;%(field)s&quot; in record &quot;%(record)s&quot; of &quot;%(model)s&quot; exceeds the limit of &quot;%(digits)i&quot;.</field>
     </record>
     <record model="ir.message" id="msg_forbidden_char_validation_record">
-      <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot; contains some invalid chars &quot;%(chars)s&quot;.</field>
+      <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in record &quot;%(record)s&quot; of &quot;%(model)s&quot; contains some invalid chars &quot;%(chars)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_selection_validation_record">
-      <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot; is not one of the allowed options.</field>
+      <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in record &quot;%(record)s&quot; of &quot;%(model)s&quot; is not one of the allowed options.</field>
     </record>
     <record model="ir.message" id="msg_time_format_validation_record">
-      <field name="text">The time value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in &quot;%(record)s&quot; of &quot;%(model)s&quot; is not valid.</field>
+      <field name="text">The time value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in record &quot;%(record)s&quot; of &quot;%(model)s&quot; is not valid.</field>
     </record>
     <record model="ir.message" id="msg_foreign_model_missing">
       <field name="text">The value &quot;%(value)s&quot; for field &quot;%(field)s&quot; in &quot;%(model)s&quot; does not exist.</field>
     </record>
     <record model="ir.message" id="msg_foreign_model_exist">
       <field name="text">The records could not be deleted because they are used by field &quot;%(field)s&quot; of &quot;%(model)s&quot;.</field>
     </record>
@@ -216,14 +219,20 @@
     <record model="ir.message" id="msg_write_error">
       <field name="text">You are trying to write to records &quot;%(ids)s&quot; of &quot;%(model)s&quot; that don't exist.</field>
     </record>
     <record model="ir.message" id="msg_delete_rule_error">
       <field name="text">You are not allowed to delete records &quot;%(ids)s&quot; of &quot;%(model)s&quot; because of at lease one of those rules:
 %(rules)s</field>
     </record>
+    <record model="ir.message" id="msg_context_datetime">
+      <field name="text">At date/time: %(datetime)s</field>
+    </record>
+    <record model="ir.message" id="msg_context_groups">
+      <field name="text">Within groups: %(groups)s</field>
+    </record>
     <record model="ir.message" id="msg_dict_schema_invalid_domain">
       <field name="text">Invalid domain in schema &quot;%(schema)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_dict_schema_invalid_selection">
       <field name="text">Invalid selection in schema &quot;%(schema)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_dict_schema_invalid_help_selection">
```

### Comparing `trytond-7.0.9/trytond/ir/model.py` & `trytond-7.2.0/trytond/ir/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from sql import Literal, Null
 from sql.aggregate import Max
 from sql.conditionals import Case
 from sql.operators import Equal
 
 from trytond.cache import Cache
+from trytond.config import config
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, EvalEnvironment, Exclude, Index, ModelSingleton,
     ModelSQL, ModelView, Unique, Workflow, fields)
 from trytond.model.exceptions import AccessError, ValidationError
 from trytond.pool import Pool
 from trytond.protocols.jsonrpc import JSONDecoder, JSONEncoder
@@ -27,21 +28,27 @@
 from trytond.tools.string_ import StringMatcher
 from trytond.transaction import Transaction, without_check_access
 from trytond.wizard import Button, StateAction, StateView, Wizard
 
 from .resource import ResourceAccessMixin
 
 logger = logging.getLogger(__name__)
+_request_timeout = config.getint('request', 'timeout', default=0)
 
 
 class ConditionError(ValidationError):
     pass
 
 
-class Model(ModelSQL, ModelView):
+class Model(
+        fields.fmany2one(
+            'module_ref', 'module', 'ir.module,name', "Module",
+            readonly=True, ondelete='CASCADE',
+            help="Module in which this model is defined."),
+        ModelSQL, ModelView):
     "Model"
     __name__ = 'ir.model'
     _order_name = 'model'
     name = fields.Char('Model Description', translate=True, loading='lazy',
         states={
             'readonly': Bool(Eval('module')),
             },
@@ -52,19 +59,17 @@
             },
         depends=['module'])
     info = fields.Text('Information',
         states={
             'readonly': Bool(Eval('module')),
             },
         depends=['module'])
-    module = fields.Char('Module',
-       help="Module in which this model is defined.", readonly=True)
+    module = fields.Char("Module", readonly=True)
     global_search_p = fields.Boolean('Global Search')
-    fields = fields.One2Many('ir.model.field', 'model', 'Fields',
-       required=True)
+    fields = fields.One2Many('ir.model.field', 'model_ref', "Fields")
     _get_names_cache = Cache('ir.model.get_names')
 
     @classmethod
     def __setup__(cls):
         super(Model, cls).__setup__()
         table = cls.__table__()
         cls._sql_constraints += [
@@ -73,15 +78,15 @@
             ]
         cls._order.insert(0, ('model', 'ASC'))
         cls.__rpc__.update({
                 'list_models': RPC(),
                 'list_history': RPC(),
                 'get_notification': RPC(),
                 'get_names': RPC(),
-                'global_search': RPC(),
+                'global_search': RPC(timeout=_request_timeout),
                 })
 
     @classmethod
     def register(cls, model, module_name):
         cursor = Transaction().connection.cursor()
 
         ir_model = cls.__table__()
@@ -215,33 +220,40 @@
         return heapq.nlargest(int(limit), generate())
 
     @classmethod
     def get_name(cls, model):
         return cls.get_names().get(model, model)
 
 
-class ModelField(ModelSQL, ModelView):
+class ModelField(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            required=True, ondelete='CASCADE'),
+        fields.fmany2one(
+            'module_ref', 'module', 'ir.module,name', "Module",
+            readonly=True, ondelete='CASCADE',
+            help="Module in which this field is defined."),
+        ModelSQL, ModelView):
     "Model field"
     __name__ = 'ir.model.field'
     name = fields.Char('Name', required=True,
         states={
             'readonly': Bool(Eval('module')),
             },
         depends=['module'])
     relation = fields.Char('Model Relation',
         states={
             'readonly': Bool(Eval('module')),
             },
         depends=['module'])
-    model = fields.Many2One('ir.model', 'Model', required=True,
-        ondelete='CASCADE',
+    model = fields.Char(
+        "Model", required=True,
         states={
             'readonly': Bool(Eval('module')),
-            },
-        depends=['module'])
+            })
     field_description = fields.Char('Field Description', translate=True,
         loading='lazy',
         states={
             'readonly': Bool(Eval('module')),
             },
         depends=['module'])
     ttype = fields.Char('Field Type',
@@ -250,107 +262,136 @@
             },
         depends=['module'])
     help = fields.Text('Help', translate=True, loading='lazy',
         states={
             'readonly': Bool(Eval('module')),
             },
         depends=['module'])
-    module = fields.Char('Module',
-       help="Module in which this field is defined.")
+    module = fields.Char("Module", readonly=True)
     access = fields.Boolean(
         "Access",
         states={
             'invisible': ~Eval('relation'),
             },
         depends=['relation'],
         help="If checked, the access right on the model of the field "
         "is also tested against the relation of the field.")
 
     _get_name_cache = Cache('ir.model.field.get_name')
 
     @classmethod
     def __setup__(cls):
         super(ModelField, cls).__setup__()
-        cls.__access__.add('model')
+        cls.__access__.add('model_ref')
         table = cls.__table__()
         cls._sql_constraints += [
             ('name_model_uniq', Unique(table, table.name, table.model),
                 'The field name in model must be unique!'),
             ]
         cls._order.insert(0, ('name', 'ASC'))
 
     @classmethod
-    def register(cls, model, module_name, model_id):
+    def __register__(cls, module):
         pool = Pool()
         Model = pool.get('ir.model')
+        transaction = Transaction()
+        cursor = transaction.connection.cursor()
+        table_h = cls.__table_handler__(module)
+        table = cls.__table__()
+        model = Model.__table__()
+
+        # Migration from 7.0: model as char
+        if (table_h.column_exist('model')
+                and table_h.column_is_type('model', 'INTEGER')):
+            table_h.column_rename('model', '_temp_model')
+            table_h.add_column('model', 'VARCHAR')
+            cursor.execute(*table.update(
+                    [table.model], [model.model],
+                    from_=[model],
+                    where=table._temp_model == model.id))
+            table_h.drop_column('_temp_model')
+
+        super().__register__(module)
+
+    @classmethod
+    def register(cls, model, module_name, model_id):
         cursor = Transaction().connection.cursor()
 
         ir_model_field = cls.__table__()
-        ir_model = Model.__table__()
 
-        cursor.execute(*ir_model_field.join(ir_model,
-                condition=ir_model_field.model == ir_model.id
-                ).select(ir_model_field.id.as_('id'),
+        cursor.execute(*ir_model_field
+            .select(
+                ir_model_field.id.as_('id'),
                 ir_model_field.name.as_('name'),
                 ir_model_field.field_description.as_('field_description'),
                 ir_model_field.ttype.as_('ttype'),
                 ir_model_field.relation.as_('relation'),
                 ir_model_field.module.as_('module'),
                 ir_model_field.help.as_('help'),
                 ir_model_field.access.as_('access'),
-                where=ir_model.model == model.__name__))
+                where=ir_model_field.model == model.__name__))
         model_fields = {f['name']: f for f in cursor_dict(cursor)}
 
         for field_name, field in model._fields.items():
             if hasattr(field, 'model_name'):
                 relation = field.model_name
             elif hasattr(field, 'relation_name'):
                 relation = field.relation_name
             else:
                 relation = None
             access = field_name in model.__access__
 
             if field_name not in model_fields:
-                cursor.execute(*ir_model_field.insert(
-                        [ir_model_field.model, ir_model_field.name,
+                cursor.execute(*ir_model_field.insert([
+                            ir_model_field.model,
+                            ir_model_field.name,
                             ir_model_field.field_description,
-                            ir_model_field.ttype, ir_model_field.relation,
-                            ir_model_field.help, ir_model_field.module,
-                            ir_model_field.access],
-                        [[
-                                model_id, field_name,
+                            ir_model_field.ttype,
+                            ir_model_field.relation,
+                            ir_model_field.help,
+                            ir_model_field.module,
+                            ir_model_field.access,
+                            ], [[
+                                model.__name__,
+                                field_name,
                                 field.string,
-                                field._type, relation,
-                                field.help, module_name,
-                                access]]))
+                                field._type,
+                                relation,
+                                field.help,
+                                module_name,
+                                access,
+                                ]]))
             elif (model_fields[field_name]['field_description'] != field.string
                     or model_fields[field_name]['ttype'] != field._type
                     or model_fields[field_name]['relation'] != relation
                     or model_fields[field_name]['help'] != field.help
                     or model_fields[field_name]['access'] != access):
-                cursor.execute(*ir_model_field.update(
-                        [ir_model_field.field_description,
-                            ir_model_field.ttype, ir_model_field.relation,
-                            ir_model_field.help, ir_model_field.access],
-                        [field.string, field._type, relation, field.help,
+                cursor.execute(*ir_model_field.update([
+                            ir_model_field.field_description,
+                            ir_model_field.ttype,
+                            ir_model_field.relation,
+                            ir_model_field.help,
+                            ir_model_field.access,
+                            ], [
+                            field.string,
+                            field._type,
+                            relation,
+                            field.help,
                             access],
                         where=(ir_model_field.id
                             == model_fields[field_name]['id'])))
 
     @classmethod
     def clean(cls):
         pool = Pool()
-        IrModel = pool.get('ir.model')
         transaction = Transaction()
         cursor = transaction.connection.cursor()
-        ir_model = IrModel.__table__()
         ir_model_field = cls.__table__()
-        cursor.execute(*ir_model_field
-            .join(ir_model, condition=ir_model_field.model == ir_model.id)
-            .select(ir_model.model, ir_model_field.name, ir_model_field.id))
+        cursor.execute(*ir_model_field.select(
+                ir_model_field.model, ir_model_field.name, ir_model_field.id))
         for model, field, id_ in cursor:
             Model = pool.get(model)
             if field not in Model._fields:
                 logger.info("remove field: %s.%s", model, field)
                 try:
                     cls.delete([cls(id_)])
                     transaction.commit()
@@ -401,15 +442,14 @@
                 name = field
         return name
 
     @classmethod
     def read(cls, ids, fields_names):
         pool = Pool()
         Translation = pool.get('ir.translation')
-        Model = pool.get('ir.model')
 
         to_delete = []
         if Transaction().context.get('language'):
             if 'field_description' in fields_names \
                     or 'help' in fields_names:
                 if 'model' not in fields_names:
                     fields_names.append('model')
@@ -419,88 +459,95 @@
                     to_delete.append('name')
 
         res = super(ModelField, cls).read(ids, fields_names)
 
         if (Transaction().context.get('language')
                 and ('field_description' in fields_names
                     or 'help' in fields_names)):
-            model_ids = set()
-            for rec in res:
-                if isinstance(rec['model'], (list, tuple)):
-                    model_ids.add(rec['model'][0])
-                else:
-                    model_ids.add(rec['model'])
-            model_ids = list(model_ids)
-            cursor = Transaction().connection.cursor()
-            model = Model.__table__()
-            cursor.execute(*model.select(model.id, model.model,
-                    where=model.id.in_(model_ids)))
-            id2model = dict(cursor)
-
             trans_args = []
             for rec in res:
-                if isinstance(rec['model'], (list, tuple)):
-                    model_id = rec['model'][0]
-                else:
-                    model_id = rec['model']
                 if 'field_description' in fields_names:
-                    trans_args.append((id2model[model_id] + ',' + rec['name'],
-                        'field', Transaction().language, None))
+                    trans_args.append((
+                            rec['model'] + ',' + rec['name'],
+                            'field', Transaction().language, None))
                 if 'help' in fields_names:
-                    trans_args.append((id2model[model_id] + ',' + rec['name'],
+                    trans_args.append((
+                            rec['model'] + ',' + rec['name'],
                             'help', Transaction().language, None))
             Translation.get_sources(trans_args)
             for rec in res:
-                if isinstance(rec['model'], (list, tuple)):
-                    model_id = rec['model'][0]
-                else:
-                    model_id = rec['model']
                 if 'field_description' in fields_names:
                     res_trans = Translation.get_source(
-                            id2model[model_id] + ',' + rec['name'],
+                            rec['model'] + ',' + rec['name'],
                             'field', Transaction().language)
                     if res_trans:
                         rec['field_description'] = res_trans
                 if 'help' in fields_names:
                     res_trans = Translation.get_source(
-                            id2model[model_id] + ',' + rec['name'],
+                            rec['model'] + ',' + rec['name'],
                             'help', Transaction().language)
                     if res_trans:
                         rec['help'] = res_trans
 
         if to_delete:
             for rec in res:
                 for field in to_delete:
                     del rec[field]
         return res
 
 
-class ModelAccess(DeactivableMixin, ModelSQL, ModelView):
+class ModelAccess(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            required=True, ondelete='CASCADE'),
+        DeactivableMixin, ModelSQL, ModelView):
     "Model access"
     __name__ = 'ir.model.access'
-    model = fields.Many2One('ir.model', 'Model', required=True,
-            ondelete="CASCADE")
+    model = fields.Char("Model", required=True)
     group = fields.Many2One('res.group', 'Group',
             ondelete="CASCADE")
     perm_read = fields.Boolean('Read Access')
     perm_write = fields.Boolean('Write Access')
     perm_create = fields.Boolean('Create Access')
     perm_delete = fields.Boolean('Delete Access')
     description = fields.Text('Description')
     _get_access_cache = Cache('ir_model_access.get_access', context=False)
 
     @classmethod
     def __setup__(cls):
         super(ModelAccess, cls).__setup__()
-        cls.__access__.add('model')
+        cls.__access__.add('model_ref')
         cls.__rpc__.update({
                 'get_access': RPC(),
                 })
 
     @classmethod
+    def __register__(cls, module):
+        pool = Pool()
+        Model = pool.get('ir.model')
+        transaction = Transaction()
+        cursor = transaction.connection.cursor()
+        table_h = cls.__table_handler__(module)
+        table = cls.__table__()
+        model = Model.__table__()
+
+        # Migration from 7.0: model as char
+        if (table_h.column_exist('model')
+                and table_h.column_is_type('model', 'INTEGER')):
+            table_h.column_rename('model', '_temp_model')
+            table_h.add_column('model', 'VARCHAR')
+            cursor.execute(*table.update(
+                    [table.model], [model.model],
+                    from_=[model],
+                    where=table._temp_model == model.id))
+            table_h.drop_column('_temp_model')
+
+        super().__register__(module)
+
+    @classmethod
     def check_xml_record(cls, accesses, values):
         pass
 
     @staticmethod
     def default_perm_read():
         return False
 
@@ -513,33 +560,31 @@
         return False
 
     @staticmethod
     def default_perm_delete():
         return False
 
     def get_rec_name(self, name):
-        return self.model.rec_name
+        return self.model_ref.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
-        return [('model',) + tuple(clause[1:])]
+        return [('model_ref.rec_name', *clause[1:])]
 
     @classmethod
     def get_access(cls, models):
         'Return access for models'
         # root user above constraint
         if Transaction().user == 0:
             return defaultdict(lambda: defaultdict(lambda: True))
 
         pool = Pool()
-        Model = pool.get('ir.model')
         User = pool.get('res.user')
         cursor = Transaction().connection.cursor()
         model_access = cls.__table__()
-        ir_model = Model.__table__()
 
         groups = User.get_groups()
 
         access = {}
         for model in models:
             maccess = cls._get_access_cache.get((groups, model), default=-1)
             if maccess == -1:
@@ -576,35 +621,33 @@
                     maccess['write'] = default['write']
                 if Model.delete.__func__ != ModelSQL.delete.__func__:
                     maccess['delete'] = default['delete']
             elif issubclass(Model, ModelSingleton):
                 access[model] = default_singleton
             else:
                 access[model] = default
-        cursor.execute(*model_access.join(ir_model, 'LEFT',
-                condition=model_access.model == ir_model.id
-                ).select(
-                ir_model.model,
+        cursor.execute(*model_access.select(
+                model_access.model,
                 Max(Case(
                         (model_access.perm_read == Literal(True), 1),
                         else_=0)),
                 Max(Case(
                         (model_access.perm_write == Literal(True), 1),
                         else_=0)),
                 Max(Case(
                         (model_access.perm_create == Literal(True), 1),
                         else_=0)),
                 Max(Case(
                         (model_access.perm_delete == Literal(True), 1),
                         else_=0)),
-                where=ir_model.model.in_(all_models)
+                where=model_access.model.in_(all_models)
                 & (model_access.active == Literal(True))
                 & (model_access.group.in_(groups or [-1])
                     | (model_access.group == Null)),
-                group_by=ir_model.model))
+                group_by=model_access.model))
         raw_access = {
             m: {'read': r, 'write': w, 'create': c, 'delete': d}
             for m, r, w, c, d in cursor}
 
         for model in models:
             access[model] = {
                 perm: max(
@@ -624,19 +667,26 @@
         assert mode in ['read', 'write', 'create', 'delete'], \
             'Invalid access mode for security'
         transaction = Transaction()
         if (transaction.user == 0
                 or (raise_exception and not transaction.check_access)):
             return True
 
+        User = pool.get('res.user')
+        Group = pool.get('res.group')
+
         access = cls.get_access([model_name])[model_name][mode]
         if not access and access is not None:
             if raise_exception:
-                raise AccessError(gettext(
-                        'ir.msg_access_rule_error', **Model.__names__()))
+                groups = Group.browse(User.get_groups())
+                raise AccessError(
+                    gettext('ir.msg_access_rule_error', **Model.__names__()),
+                    gettext(
+                        'ir.msg_context_groups',
+                        groups=', '.join(g.rec_name for g in groups)))
             else:
                 return False
         return True
 
     @classmethod
     def check_relation(cls, model_name, field_name, mode='read'):
         'Check access to relation field for model_name and mode'
@@ -693,31 +743,66 @@
     def delete(cls, accesses):
         super(ModelAccess, cls).delete(accesses)
         # Restart the cache
         cls._get_access_cache.clear()
         ModelView._fields_view_get_cache.clear()
 
 
-class ModelFieldAccess(DeactivableMixin, ModelSQL, ModelView):
+class ModelFieldAccess(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            required=True, ondelete='CASCADE'),
+        fields.fmany2one(
+            'field_ref', 'field,model', 'ir.model.field,name,model', "Field",
+            required=True, ondelete='CASCADE',
+            domain=[
+                ('model', '=', Eval('model')),
+                ]),
+        DeactivableMixin, ModelSQL, ModelView):
     "Model Field Access"
     __name__ = 'ir.model.field.access'
-    field = fields.Many2One('ir.model.field', 'Field', required=True,
-            ondelete='CASCADE')
+    model = fields.Char("Model", required=True)
+    field = fields.Char("Field", required=True)
     group = fields.Many2One('res.group', 'Group', ondelete='CASCADE')
     perm_read = fields.Boolean('Read Access')
     perm_write = fields.Boolean('Write Access')
     perm_create = fields.Boolean('Create Access')
     perm_delete = fields.Boolean('Delete Access')
     description = fields.Text('Description')
     _get_access_cache = Cache('ir_model_field_access.check', context=False)
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
-        cls.__access__.add('field')
+        cls.__access__.add('field_ref')
+
+    @classmethod
+    def __register__(cls, module):
+        pool = Pool()
+        Field = pool.get('ir.model.field')
+        transaction = Transaction()
+        cursor = transaction.connection.cursor()
+        table_h = cls.__table_handler__(module)
+        table = cls.__table__()
+        field = Field.__table__()
+
+        # Migration from 7.0: field as char
+        if (table_h.column_exist('field')
+                and table_h.column_is_type('field', 'INTEGER')):
+            table_h.column_rename('field', '_temp_field')
+            table_h.add_column('model', 'VARCHAR')
+            table_h.add_column('field', 'VARCHAR')
+            cursor.execute(*table.update(
+                    [table.model, table.field],
+                    [field.model, field.name],
+                    from_=[field],
+                    where=table._temp_field == field.id))
+            table_h.drop_column('_temp_field')
+
+        super().__register__(module)
 
     @classmethod
     def check_xml_record(cls, field_accesses, values):
         pass
 
     @staticmethod
     def default_perm_read():
@@ -732,35 +817,31 @@
         return True
 
     @staticmethod
     def default_perm_delete():
         return True
 
     def get_rec_name(self, name):
-        return self.field.rec_name
+        return self.field_ref.rec_name
 
     @classmethod
     def search_rec_name(cls, name, clause):
-        return [('field',) + tuple(clause[1:])]
+        return [('field_ref.rec_name', *clause[1:])]
 
     @classmethod
     def get_access(cls, models):
         'Return fields access for models'
         # root user above constraint
         if Transaction().user == 0:
             return defaultdict(lambda: defaultdict(
                     lambda: defaultdict(lambda: True)))
 
         pool = Pool()
-        Model = pool.get('ir.model')
-        ModelField = pool.get('ir.model.field')
         User = pool.get('res.user')
         field_access = cls.__table__()
-        ir_model = Model.__table__()
-        model_field = ModelField.__table__()
 
         groups = User.get_groups()
 
         accesses = {}
         for model in models:
             maccesses = cls._get_access_cache.get((groups, model))
             if maccesses is None:
@@ -768,38 +849,34 @@
             accesses[model] = maccesses
         else:
             return accesses
 
         default = {}
         accesses = dict((m, default) for m in models)
         cursor = Transaction().connection.cursor()
-        cursor.execute(*field_access.join(model_field,
-                condition=field_access.field == model_field.id
-                ).join(ir_model,
-                condition=model_field.model == ir_model.id
-                ).select(
-                ir_model.model,
-                model_field.name,
+        cursor.execute(*field_access.select(
+                field_access.model,
+                field_access.field,
                 Max(Case(
                         (field_access.perm_read == Literal(True), 1),
                         else_=0)),
                 Max(Case(
                         (field_access.perm_write == Literal(True), 1),
                         else_=0)),
                 Max(Case(
                         (field_access.perm_create == Literal(True), 1),
                         else_=0)),
                 Max(Case(
                         (field_access.perm_delete == Literal(True), 1),
                         else_=0)),
-                where=ir_model.model.in_(models)
+                where=field_access.model.in_(models)
                 & (field_access.active == Literal(True))
                 & (field_access.group.in_(groups or [-1])
                     | (field_access.group == Null)),
-                group_by=[ir_model.model, model_field.name]))
+                group_by=[field_access.model, field_access.field]))
         for m, f, r, w, c, d in cursor:
             accesses[m][f] = {'read': r, 'write': w, 'create': c, 'delete': d}
         for model, maccesses in accesses.items():
             cls._get_access_cache.set((groups, model), maccesses)
         return accesses
 
     @classmethod
@@ -815,24 +892,32 @@
         transaction = Transaction()
         if (transaction.user == 0
                 or (raise_exception and not transaction.check_access)):
             if access:
                 return dict((x, True) for x in fields)
             return True
 
+        User = pool.get('res.user')
+        Group = pool.get('res.group')
+
         accesses = dict((f, a[mode])
             for f, a in cls.get_access([model_name])[model_name].items())
         if access:
             return accesses
         for field in fields:
             if not accesses.get(field, True):
                 if raise_exception:
+                    groups = Group.browse(User.get_groups())
                     raise AccessError(
-                        gettext('ir.msg_access_rule_field_error',
-                            **Model.__names__(field)))
+                        gettext(
+                            'ir.msg_access_rule_field_error',
+                            **Model.__names__(field)),
+                        gettext(
+                            'ir.msg_context_groups',
+                            groups=', '.join(g.rec_name for g in groups)))
                 else:
                     return False
         return True
 
     @classmethod
     def write(cls, field_accesses, values, *args):
         super(ModelFieldAccess, cls).write(field_accesses, values, *args)
@@ -852,59 +937,77 @@
     def delete(cls, field_accesses):
         super(ModelFieldAccess, cls).delete(field_accesses)
         # Restart the cache
         cls._get_access_cache.clear()
         ModelView._fields_view_get_cache.clear()
 
 
-class ModelButton(DeactivableMixin, ModelSQL, ModelView):
+class ModelButton(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            required=True, readonly=True, ondelete='CASCADE'),
+        DeactivableMixin, ModelSQL, ModelView):
     "Model Button"
     __name__ = 'ir.model.button'
     name = fields.Char('Name', required=True, readonly=True)
     string = fields.Char("Label", translate=True)
     help = fields.Text("Help", translate=True)
     confirm = fields.Text("Confirm", translate=True,
         help="Text to ask user confirmation when clicking the button.")
-    model = fields.Many2One('ir.model', 'Model', required=True, readonly=True,
-        ondelete='CASCADE')
+    model = fields.Char("Model", required=True, readonly=True)
     rules = fields.One2Many('ir.model.button.rule', 'button', "Rules")
     _rules_cache = Cache('ir.model.button.rules')
     clicks = fields.One2Many('ir.model.button.click', 'button', "Clicks")
     reset_by = fields.Many2Many(
         'ir.model.button-button.reset', 'button_ruled', 'button', "Reset by",
         domain=[
-            ('model', '=', Eval('model', -1)),
+            ('model', '=', Eval('model')),
             ('id', '!=', Eval('id', -1)),
             ],
-        depends=['model', 'id'],
         help="Button that should reset the rules.")
     reset = fields.Many2Many(
         'ir.model.button-button.reset', 'button', 'button_ruled', "Reset",
         domain=[
-            ('model', '=', Eval('model', -1)),
+            ('model', '=', Eval('model')),
             ('id', '!=', Eval('id', -1)),
-            ],
-        depends=['model', 'id'])
+            ])
     _reset_cache = Cache('ir.model.button.reset')
     _view_attributes_cache = Cache(
         'ir.model.button.view_attributes', context=False)
 
     @classmethod
     def __register__(cls, module_name):
-        super().__register__(module_name)
-
+        pool = Pool()
+        Model = pool.get('ir.model')
+        transaction = Transaction()
+        cursor = transaction.connection.cursor()
         table_h = cls.__table_handler__(module_name)
+        table = cls.__table__()
+        model = Model.__table__()
+
+        # Migration from 7.0: model as char
+        if (table_h.column_exist('model')
+                and table_h.column_is_type('model', 'INTEGER')):
+            table_h.column_rename('model', '_temp_model')
+            table_h.add_column('model', 'VARCHAR')
+            cursor.execute(*table.update(
+                    [table.model], [model.model],
+                    from_=[model],
+                    where=table._temp_model == model.id))
+            table_h.drop_column('_temp_model')
+
+        super().__register__(module_name)
 
         # Migration from 6.2: replace unique by exclude
         table_h.drop_constraint('name_model_uniq')
 
     @classmethod
     def __setup__(cls):
         super(ModelButton, cls).__setup__()
-        cls.__access__.add('model')
+        cls.__access__.add('model_ref')
         t = cls.__table__()
         cls._sql_constraints += [
             ('name_model_exclude',
                 Exclude(t, (t.name, Equal), (t.model, Equal),
                     where=(t.active == Literal(True))),
                 'ir.msg_button_name_unique'),
             ]
@@ -948,15 +1051,15 @@
         pool = Pool()
         Rule = pool.get('ir.model.button.rule')
         key = (model, name)
         rule_ids = cls._rules_cache.get(key)
         if rule_ids is not None:
             return Rule.browse(rule_ids)
         buttons = cls.search([
-                ('model.model', '=', model),
+                ('model', '=', model),
                 ('name', '=', name),
                 ])
         if not buttons:
             rules = []
         else:
             button, = buttons
             rules = button.rules
@@ -968,15 +1071,15 @@
     def get_reset(cls, model, name):
         "Return a list of button names to reset"
         key = (model, name)
         reset = cls._reset_cache.get(key)
         if reset is not None:
             return reset
         buttons = cls.search([
-                ('model.model', '=', model),
+                ('model', '=', model),
                 ('name', '=', name),
                 ])
         if not buttons:
             reset = []
         else:
             button, = buttons
             reset = [b.name for b in button.reset]
@@ -987,15 +1090,15 @@
     def get_view_attributes(cls, model, name):
         "Return the view attributes of the named button of the model"
         key = (model, name, Transaction().language)
         attributes = cls._view_attributes_cache.get(key)
         if attributes is not None:
             return attributes
         buttons = cls.search([
-                ('model.model', '=', model),
+                ('model', '=', model),
                 ('name', '=', name),
                 ])
         if not buttons:
             attributes = {}
         else:
             button, = buttons
             attributes = {
@@ -1164,15 +1267,22 @@
         'ir.model.button', "Button Ruled",
         required=True, ondelete='CASCADE')
     button = fields.Many2One(
         'ir.model.button', "Button",
         required=True, ondelete='CASCADE')
 
 
-class ModelData(ModelSQL, ModelView):
+class ModelData(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            required=True, ondelete='CASCADE'),
+        fields.fmany2one(
+            'module_ref', 'module', 'ir.module,name', "Module",
+            required=True, ondelete='CASCADE'),
+        ModelSQL, ModelView):
     "Model data"
     __name__ = 'ir.model.data'
     fs_id = fields.Char('Identifier on File System', required=True,
         help="The id of the record as known on the file system.")
     model = fields.Char('Model', required=True)
     module = fields.Char('Module', required=True)
     db_id = fields.Integer(
```

### Comparing `trytond-7.0.9/trytond/ir/model.xml` & `trytond-7.2.0/trytond/ir/model.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/model.xml` & `trytond-7.2.0/trytond/ir/model.xml`

```diff
@@ -78,15 +78,15 @@
       <field name="view" ref="model_access_view_form"/>
       <field name="act_window" ref="act_model_access_form"/>
     </record>
     <menuitem parent="ir.menu_models" action="act_model_access_form" sequence="30" id="menu_model_access_form"/>
     <record model="ir.action.act_window" id="act_model_access_form_relate_model">
       <field name="name">Access</field>
       <field name="res_model">ir.model.access</field>
-      <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('model', '=', Eval('active_id')), ('model', 'in', Eval('active_ids')))]" pyson="1"/>
+      <field name="domain" eval="[('model_ref.id', 'in', Eval('active_ids', []))]" pyson="1"/>
     </record>
     <record model="ir.action.keyword" id="act_model_access_form_relate_model_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">ir.model,-1</field>
       <field name="action" ref="act_model_access_form_relate_model"/>
     </record>
     <record model="ir.ui.view" id="model_field_access_view_tree">
@@ -113,15 +113,15 @@
       <field name="view" ref="model_field_access_view_form"/>
       <field name="act_window" ref="act_model_field_access_form"/>
     </record>
     <menuitem parent="menu_model_access_form" action="act_model_field_access_form" sequence="10" id="menu_model_field_access_form"/>
     <record model="ir.action.act_window" id="act_model_field_access_form_relate_field">
       <field name="name">Access</field>
       <field name="res_model">ir.model.field.access</field>
-      <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('field', '=', Eval('active_id')), ('field', 'in', Eval('active_ids')))]" pyson="1"/>
+      <field name="domain" eval="[('field_ref.id', 'in', Eval('active_ids'))]" pyson="1"/>
     </record>
     <record model="ir.action.keyword" id="act_modelfield__access_form_relate_field_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">ir.model.field,-1</field>
       <field name="action" ref="act_model_field_access_form_relate_field"/>
     </record>
     <record model="ir.action.report" id="report_model_graph">
@@ -244,17 +244,17 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_model_data_form"/>
     </record>
     <menuitem parent="menu_model_form" action="act_model_data_form" sequence="50" id="menu_model_data_form"/>
     <record model="ir.model.button" id="model_data_sync_button">
+      <field name="model">ir.model.data</field>
       <field name="name">sync</field>
       <field name="string">Sync</field>
-      <field name="model" search="[('model', '=', 'ir.model.data')]"/>
     </record>
     <record model="ir.ui.view" id="model_log_view_form">
       <field name="model">ir.model.log</field>
       <field name="type">form</field>
       <field name="name">model_log_form</field>
     </record>
     <record model="ir.ui.view" id="model_log_view_list">
```

### Comparing `trytond-7.0.9/trytond/ir/module.py` & `trytond-7.2.0/trytond/ir/module.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/module.xml` & `trytond-7.2.0/trytond/ir/module.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/module.xml` & `trytond-7.2.0/trytond/ir/module.xml`

```diff
@@ -28,42 +28,42 @@
     <record model="ir.action.act_window.view" id="act_module_form_view2">
       <field name="sequence" eval="2"/>
       <field name="view" ref="module_view_form"/>
       <field name="act_window" ref="act_module_form"/>
     </record>
     <menuitem parent="menu_modules" action="act_module_form" sequence="10" id="menu_module_form"/>
     <record model="ir.model.button" id="module_activate_button">
+      <field name="model">ir.module</field>
       <field name="name">activate</field>
       <field name="string">Mark for Activation</field>
-      <field name="model" search="[('model', '=', 'ir.module')]"/>
     </record>
     <record model="ir.model.button" id="module_activate_cancel_button">
+      <field name="model">ir.module</field>
       <field name="name">activate_cancel</field>
       <field name="string">Cancel Activation</field>
-      <field name="model" search="[('model', '=', 'ir.module')]"/>
     </record>
     <record model="ir.model.button" id="module_deactivate_button">
+      <field name="model">ir.module</field>
       <field name="name">deactivate</field>
       <field name="string">Mark for Deactivation (beta)</field>
-      <field name="model" search="[('model', '=', 'ir.module')]"/>
     </record>
     <record model="ir.model.button" id="module_deactivate_cancel_button">
+      <field name="model">ir.module</field>
       <field name="name">deactivate_cancel</field>
       <field name="string">Cancel Deactivation</field>
-      <field name="model" search="[('model', '=', 'ir.module')]"/>
     </record>
     <record model="ir.model.button" id="module_upgrade_button">
+      <field name="model">ir.module</field>
       <field name="name">upgrade</field>
       <field name="string">Mark for Upgrade</field>
-      <field name="model" search="[('model', '=', 'ir.module')]"/>
     </record>
     <record model="ir.model.button" id="module_upgrade_cancel_button">
+      <field name="model">ir.module</field>
       <field name="name">upgrade_cancel</field>
       <field name="string">Cancel Upgrade</field>
-      <field name="model" search="[('model', '=', 'ir.module')]"/>
     </record>
     <record model="ir.ui.view" id="module_dependency_view_form">
       <field name="model">ir.module.dependency</field>
       <field name="type">form</field>
       <field name="name">module_dependency_form</field>
     </record>
     <record model="ir.ui.view" id="module_dependency_view_list">
```

### Comparing `trytond-7.0.9/trytond/ir/note.py` & `trytond-7.2.0/trytond/ir/note.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/note.xml` & `trytond-7.2.0/trytond/ir/note.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/queue_.py` & `trytond-7.2.0/trytond/ir/queue_.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from sql.aggregate import Min
 from sql.functions import CurrentTimestamp, Extract
 
 from trytond.config import config
 from trytond.model import Index, ModelSQL, fields
 from trytond.pool import Pool
 from trytond.tools import grouped_slice
-from trytond.transaction import Transaction, inactive_records
+from trytond.transaction import (
+    Transaction, inactive_records, without_check_access)
 
 has_worker = config.getboolean('queue', 'worker', default=False)
 clean_days = config.getint('queue', 'clean_days', default=30)
 batch_size = config.getint('queue', 'batch_size', default=20)
 
 
 class Queue(ModelSQL):
@@ -62,15 +63,15 @@
         return super(Queue, cls).copy(records, default=default)
 
     @classmethod
     def push(cls, name, data, scheduled_at=None, expected_at=None):
         transaction = Transaction()
         database = transaction.database
         cursor = transaction.connection.cursor()
-        with transaction.set_user(0):
+        with without_check_access():
             record, = cls.create([{
                         'name': name,
                         'data': data,
                         'scheduled_at': scheduled_at,
                         'expected_at': expected_at,
                         }])
         if database.has_channel():
@@ -243,18 +244,18 @@
                 }
             return self.__queue.push(
                 name, data,
                 scheduled_at=scheduled_at, expected_at=expected_at)
 
         if isinstance(instances, list):
             if has_worker and queue_batch:
-                if isinstance(queue_batch, int):
-                    count = queue_batch
-                else:
+                if isinstance(queue_batch, bool):
                     count = batch_size
+                else:
+                    count = int(queue_batch)
             else:
                 count = len(instances)
             task_ids = []
             for sub_instances in grouped_slice(instances, count=count):
                 task_ids.append(_push(list(sub_instances)))
             return task_ids
         else:
```

### Comparing `trytond-7.0.9/trytond/ir/resource.py` & `trytond-7.2.0/trytond/ir/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/routes.py` & `trytond-7.2.0/trytond/ir/routes.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/rule.py` & `trytond-7.2.0/trytond/ir/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,47 @@
 from trytond.transaction import Transaction, inactive_records
 
 
 class DomainError(ValidationError):
     pass
 
 
-class RuleGroup(ModelSQL, ModelView):
+def _get_access_models(Model, names=None, model2field=None, path=None):
+    "Return names and model2field"
+    if names is None:
+        names = set()
+    if model2field is None:
+        model2field = defaultdict(list)
+    if Model.__name__ in names:
+        return
+    names.add(Model.__name__)
+    if path:
+        model2field[Model.__name__].append(path)
+    for field_name in Model.__access__:
+        field = getattr(Model, field_name)
+        Target = field.get_target()
+        if path:
+            target_path = path + '.' + field_name
+        else:
+            target_path = field_name
+        _get_access_models(Target, names, model2field, target_path)
+    return names, model2field
+
+
+class RuleGroup(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            required=True, ondelete='CASCADE'),
+        ModelSQL, ModelView):
     "Rule group"
     __name__ = 'ir.rule.group'
     name = fields.Char(
         "Name", translate=True, required=True,
         help="Displayed to users when access error is raised for this rule.")
-    model = fields.Many2One('ir.model', 'Model',
-        required=True, ondelete='CASCADE')
+    model = fields.Char("Model", required=True)
     global_p = fields.Boolean('Global',
         help="Make the rule global \nso every users must follow this rule.")
     default_p = fields.Boolean('Default',
         help="Add this rule to all users by default.")
     rules = fields.One2Many('ir.rule', 'rule_group', 'Tests',
         help="The rule is satisfied if at least one test is True.")
     perm_read = fields.Boolean('Read Access')
@@ -51,14 +76,37 @@
                     | (t.default_p == Literal(False))),
                 'Global and Default are mutually exclusive!'),
             ]
         cls._sql_indexes.update({
                 Index(t, (t.model, Index.Equality())),
                 })
 
+    @classmethod
+    def __register__(cls, module):
+        pool = Pool()
+        Model = pool.get('ir.model')
+        transaction = Transaction()
+        cursor = transaction.connection.cursor()
+        table_h = cls.__table_handler__(module)
+        table = cls.__table__()
+        model = Model.__table__()
+
+        # Migration from 7.0: model as char
+        if (table_h.column_exist('model')
+                and table_h.column_is_type('model', 'INTEGER')):
+            table_h.column_rename('model', '_temp_model')
+            table_h.add_column('model', 'VARCHAR')
+            cursor.execute(*table.update(
+                    [table.model], [model.model],
+                    from_=[model],
+                    where=table._temp_model == model.id))
+            table_h.drop_column('_temp_model')
+
+        super().__register__(module)
+
     @staticmethod
     def default_global_p():
         return True
 
     @staticmethod
     def default_default_p():
         return False
@@ -126,15 +174,15 @@
         cls.check_domain(rules, field_names)
 
     @classmethod
     def check_domain(cls, rules, field_names=None):
         if field_names and 'domain' not in field_names:
             return
         for rule in rules:
-            ctx = cls._get_context(rule.rule_group.model.model)
+            ctx = cls._get_context(rule.rule_group.model)
             try:
                 value = PYSONDecoder(ctx).decode(rule.domain)
             except Exception:
                 raise DomainError(gettext(
                         'ir.msg_rule_invalid_domain', name=rule.rec_name))
             if not isinstance(value, list):
                 raise DomainError(gettext(
@@ -151,99 +199,77 @@
         pool = Pool()
         User = pool.get('res.user')
         return {
             'groups': User.get_groups()
             }
 
     @classmethod
-    def _get_cache_key(cls, model_name):
+    def _get_cache_key(cls, model_names):
         pool = Pool()
         User = pool.get('res.user')
         # _datetime value will be added to the domain
         return (Transaction().context.get('_datetime'), User.get_groups())
 
     @classmethod
     def get(cls, model_name, mode='read'):
         "Return dictionary of non-global and global rules"
         pool = Pool()
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
         RuleGroup_Group = pool.get('ir.rule.group-res.group')
         User = pool.get('res.user')
         rule_table = cls.__table__()
         rule_group = RuleGroup.__table__()
         rule_group_group = RuleGroup_Group.__table__()
-        model = Model.__table__()
         transaction = Transaction()
 
         assert mode in cls.modes
 
         groups = User.get_groups()
 
-        model_names = []
-        model2field = defaultdict(list)
-
-        def update_model_names(Model, path=None):
-            if Model.__name__ in model_names:
-                return
-            model_names.append(Model.__name__)
-            if path:
-                model2field[Model.__name__].append(path)
-            for field_name in Model.__access__:
-                field = getattr(Model, field_name)
-                Target = field.get_target()
-                if path:
-                    target_path = path + '.' + field_name
-                else:
-                    target_path = field_name
-                update_model_names(Target, target_path)
-        update_model_names(pool.get(model_name))
+        model_names, model2field = _get_access_models(pool.get(model_name))
+        model_names = list(model_names)
 
         cursor = transaction.connection.cursor()
         # root user above constraint
         if transaction.user == 0:
             return {}, {}
         cursor.execute(*rule_table.join(rule_group,
                 condition=rule_group.id == rule_table.rule_group
-                ).join(model,
-                condition=rule_group.model == model.id
                 ).join(rule_group_group, 'LEFT',
                 condition=rule_group_group.rule_group == rule_group.id
                 ).select(rule_table.id,
-                where=(model.model.in_(model_names))
+                where=(rule_group.model.in_(model_names))
                 & (getattr(rule_group, 'perm_%s' % mode) == Literal(True))
                 & (rule_group_group.group.in_(groups or [-1])
                     | (rule_group.default_p == Literal(True))
                     | (rule_group.global_p == Literal(True))
                     )))
         ids = [x for x, in cursor]
 
         # Test if there is no rule_group that have no rule
-        cursor.execute(*rule_group.join(model,
-                condition=rule_group.model == model.id
-                ).join(rule_group_group, 'LEFT',
+        cursor.execute(*rule_group.join(rule_group_group, 'LEFT',
                 condition=rule_group_group.rule_group == rule_group.id
                 ).select(rule_group.id,
-                where=(model.model.in_(model_names))
+                where=(rule_group.model.in_(model_names))
                 & ~rule_group.id.in_(rule_table.select(rule_table.rule_group))
                 & rule_group_group.group.in_(groups or [-1])))
         no_rules = cursor.fetchone()
 
         clause = defaultdict(lambda: ['OR'])
         clause_global = defaultdict(lambda: ['OR'])
         # Use root user without context to prevent recursion
         with transaction.set_user(0), transaction.set_context(user=0):
             rules = cls.browse(ids)
         for rule in rules:
             decoder = PYSONDecoder(
-                cls._get_context(rule.rule_group.model.model))
+                cls._get_context(rule.rule_group.model))
             assert rule.domain, ('Rule domain empty,'
                 'check if migration was done')
             dom = decoder.decode(rule.domain)
-            target_model = rule.rule_group.model.model
+            target_model = rule.rule_group.model
             if target_model in model2field:
                 target_dom = ['OR']
                 for field in model2field[target_model]:
                     target_dom.append((field, 'where', dom))
                 dom = target_dom
             if rule.rule_group.global_p:
                 clause_global[rule.rule_group].append(dom)
@@ -254,22 +280,25 @@
             group_id = no_rules[0]
             clause[RuleGroup(group_id)] = []
 
         return clause, clause_global
 
     @classmethod
     def domain_get(cls, model_name, mode='read'):
+        pool = Pool()
         transaction = Transaction()
         # root user above constraint
         if transaction.user == 0 or not transaction.check_access:
             return []
 
         assert mode in cls.modes
 
-        key = (model_name, mode) + cls._get_cache_key(model_name)
+        model_names, _ = _get_access_models(pool.get(model_name))
+
+        key = (model_name, mode) + cls._get_cache_key(model_names)
         domain = cls._domain_get_cache.get(key, False)
         if domain is not False:
             return domain
 
         clause, clause_global = cls.get(model_name, mode=mode)
 
         clause = list(clause.values())
```

### Comparing `trytond-7.0.9/trytond/ir/rule.xml` & `trytond-7.2.0/trytond/ir/rule.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/sequence.py` & `trytond-7.2.0/trytond/ir/sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/sequence.xml` & `trytond-7.2.0/trytond/ir/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/session.py` & `trytond-7.2.0/trytond/ir/session.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/translation.py` & `trytond-7.2.0/trytond/ir/translation.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,22 @@
 class TrytonPOFile(polib.POFile):
 
     def sort(self):
         return super(TrytonPOFile, self).sort(
             key=lambda x: (x.msgctxt, x.msgid))
 
 
-class Translation(ModelSQL, ModelView):
+class Translation(
+        fields.fmany2one(
+            'module_ref', 'module', 'ir.module,name', "Module",
+            readonly=True, ondelete='CASCADE'),
+        fields.fmany2one(
+            'overriding_module_ref', 'overriding_module', 'ir.module,name',
+            "Overriding Module", readonly=True),
+        ModelSQL, ModelView):
     "Translation"
     __name__ = "ir.translation"
 
     name = fields.Char('Field Name', required=True)
     res_id = fields.Integer('Resource ID', required=True)
     lang = fields.Selection('get_language', string='Language')
     type = fields.Selection(TRANSLATION_TYPE, string='Type',
@@ -337,32 +344,32 @@
             else:
                 ttype = 'model'
                 records = Model.browse(ids)
 
             trans_args = []
             for record in records:
                 if ttype in ('field', 'help'):
-                    name = record.model.model + ',' + record.name
+                    name = record.model + ',' + record.name
                 else:
                     name = record.model + ',' + field_name
                 trans_args.append((name, ttype, lang, None))
             cls.get_sources(trans_args)
 
             for record in records:
                 if ttype in ('field', 'help'):
-                    name = record.model.model + ',' + record.name
+                    name = record.model + ',' + record.name
                 else:
                     name = record.model + ',' + field_name
                 translations[record.id] = cls.get_source(name, ttype, lang)
                 if translations[record.id] is None:
                     with Transaction().set_context(language=lang):
                         if ttype in {'field', 'help'}:
                             try:
                                 field = getattr(
-                                    pool.get(record.model.model), record.name)
+                                    pool.get(record.model), record.name)
                             except KeyError:
                                 continue
                             translations[record.id] = ''
                             if ttype == 'field':
                                 value = field.string
                             else:
                                 value = field.help
@@ -454,15 +461,15 @@
             else:
                 ttype = 'model'
                 with Transaction().set_context(language=INTERNAL_LANG):
                     records = Model.browse(ids)
 
             def get_name(record):
                 if ttype in ('field', 'help'):
-                    return record.model.model + ',' + record.name
+                    return record.model + ',' + record.name
                 else:
                     return record.model + ',' + field_name
 
             name2translations = defaultdict(list)
             for translation in cls.search([
                         ('lang', '=', lang),
                         ('type', '=', ttype),
```

### Comparing `trytond-7.0.9/trytond/ir/translation.xml` & `trytond-7.2.0/trytond/ir/translation.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/trigger.py` & `trytond-7.2.0/trytond/ir/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/trigger.xml` & `trytond-7.2.0/trytond/ir/trigger.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/board.rnc` & `trytond-7.2.0/trytond/ir/ui/board.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/board.rng` & `trytond-7.2.0/trytond/ir/ui/board.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/calendar.rnc` & `trytond-7.2.0/trytond/ir/ui/calendar.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/calendar.rng` & `trytond-7.2.0/trytond/ir/ui/calendar.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/form.rnc` & `trytond-7.2.0/trytond/ir/ui/form.rnc`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 attlist.field &= attribute filename { text }?
 attlist.field &= attribute help_field { text }?
 attlist.field &=
   [a:defaultValue = "0"] attribute toolbar { "0" | "1" }?
 attlist.field &= attribute symbol { text }?
 attlist.field &= [a:defaultValue = "1"] attribute grouping { "0" | "1" }?
 attlist.field &= [a:defaultValue = "square"] attribute border { "square" | "circle" | "rounded" }?
+attlist.field &= attribute loading { "lazy" | "eager" }?
 image = element image { attlist.image, empty }
 attlist.image &= attribute name { text }
 attlist.image &= [a:defaultValue = "icon"] attribute type { "icon" | "url" }?
 attlist.image &= attribute url_size { text }?
 attlist.image &= [a:defaultValue = "square"] attribute border { "square" | "circle" | "rounded" }?
 attlist.image &= [ a:defaultValue = "1" ] attribute colspan { text }?
 attlist.image &=
```

### Comparing `trytond-7.0.9/trytond/ir/ui/form.rng` & `trytond-7.2.0/trytond/ir/ui/form.rng`

 * *Files 1% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/ui/form.rng` & `trytond-7.2.0/trytond/ir/ui/form.rng`

```diff
@@ -572,14 +572,25 @@
           <value>square</value>
           <value>circle</value>
           <value>rounded</value>
         </choice>
       </attribute>
     </optional>
   </define>
+  <define name="attlist.field" combine="interleave">
+    <optional>
+      <attribute>
+        <name ns="">loading</name>
+        <choice>
+          <value>lazy</value>
+          <value>eager</value>
+        </choice>
+      </attribute>
+    </optional>
+  </define>
   <define name="image">
     <element>
       <name ns="">image</name>
       <ref name="attlist.image"/>
       <empty/>
     </element>
   </define>
```

### Comparing `trytond-7.0.9/trytond/ir/ui/graph.rnc` & `trytond-7.2.0/trytond/ir/ui/graph.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/graph.rng` & `trytond-7.2.0/trytond/ir/ui/graph.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/icon.py` & `trytond-7.2.0/trytond/ir/ui/icon.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from trytond.cache import Cache
 from trytond.model import ModelSQL, ModelView, fields, sequence_ordered
 from trytond.rpc import RPC
 from trytond.tools import file_open
 from trytond.transaction import Transaction
 
 
-class Icon(sequence_ordered(), ModelSQL, ModelView):
+class Icon(
+        fields.fmany2one(
+            'module_ref', 'module', 'ir.module,name', "Module",
+            readonly=True, required=True, ondelete='CASCADE'),
+        sequence_ordered(), ModelSQL, ModelView):
     'Icon'
     __name__ = 'ir.ui.icon'
 
     name = fields.Char('Name', required=True)
     module = fields.Char('Module', readonly=True, required=True)
     path = fields.Char('SVG Path', readonly=True, required=True)
     icon = fields.Function(fields.Char('Icon', depends=['path']), 'get_icon')
```

### Comparing `trytond-7.0.9/trytond/ir/ui/icon.xml` & `trytond-7.2.0/trytond/ir/ui/icon.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/icons/LICENSE` & `trytond-7.2.0/trytond/ir/ui/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/icons/tryton-settings.svg` & `trytond-7.2.0/trytond/ir/ui/icons/tryton-settings.svg`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/menu.py` & `trytond-7.2.0/trytond/ir/ui/menu.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/menu.xml` & `trytond-7.2.0/trytond/ir/ui/menu.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/tree.rnc` & `trytond-7.2.0/trytond/ir/ui/tree.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/tree.rng` & `trytond-7.2.0/trytond/ir/ui/tree.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/ui.xml` & `trytond-7.2.0/trytond/ir/ui/ui.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/ui/view.py` & `trytond-7.2.0/trytond/ir/ui/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import json
 import os
 
 from lxml import etree
+from sql import Literal, Null
 
 from trytond.cache import Cache, MemoryCache
 from trytond.i18n import gettext
-from trytond.model import Index, ModelSQL, ModelView, fields
+from trytond.model import Index, ModelSQL, ModelView, fields, sequence_ordered
 from trytond.model.exceptions import ValidationError
 from trytond.pool import Pool
 from trytond.pyson import PYSON, Bool, Eval, If, PYSONDecoder
 from trytond.rpc import RPC
 from trytond.tools import file_open
 from trytond.transaction import Transaction
 from trytond.wizard import Button, StateView, Wizard
@@ -19,22 +20,37 @@
 from ..action import DomainError, ViewError
 
 
 class XMLError(ValidationError):
     pass
 
 
-class View(ModelSQL, ModelView):
+class View(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            ondelete='CASCADE'),
+        fields.fmany2one(
+            'field_children', 'field_childs,model',
+            'ir.model.field,name,model',
+            "Children Field",
+            domain=[
+                ('model', '=', Eval('model')),
+                ],
+            states={
+                'invisible': Eval('type') != 'tree',
+                }),
+        fields.fmany2one(
+            'module_ref', 'module', 'ir.module,name', "Module",
+            readonly=True, ondelete='CASCADE'),
+        sequence_ordered('priority', "Priority"), ModelSQL, ModelView):
     "View"
     __name__ = 'ir.ui.view'
-    _rec_name = 'model'
     model = fields.Char('Model', states={
             'required': Eval('type') != 'board',
             })
-    priority = fields.Integer('Priority', required=True)
     type = fields.Selection([
             (None, ''),
             ('tree', 'Tree'),
             ('form', 'Form'),
             ('graph', 'Graph'),
             ('calendar', 'Calendar'),
             ('board', 'Board'),
@@ -50,16 +66,30 @@
     data = fields.Text('Data')
     name = fields.Char('Name', states={
             'invisible': ~(Eval('module') & Eval('name')),
             }, depends=['module'], readonly=True)
     arch = fields.Function(fields.Text('View Architecture', states={
                 'readonly': Bool(Eval('name')),
                 }, depends=['name']), 'get_arch', setter='set_arch')
+    basis = fields.Function(fields.Boolean("Basis"), 'get_basis')
     inherit = fields.Many2One('ir.ui.view', 'Inherited View',
             ondelete='CASCADE')
+    extensions = fields.One2Many(
+        'ir.ui.view', 'inherit', "Extensions",
+        filter=[
+            ('basis', '=', False),
+            ],
+        domain=[
+            ('model', '=', Eval('model')),
+            ('type', '=', None),
+            ],
+        states={
+            'invisible': ~Eval('type'),
+            },
+        order=[('id', None)])
     field_childs = fields.Char('Children Field', states={
             'invisible': Eval('type') != 'tree',
             }, depends=['type'])
     module = fields.Char('Module', states={
             'invisible': ~Eval('module'),
             }, readonly=True)
     domain = fields.Char('Domain', states={
@@ -69,21 +99,22 @@
     _view_get_cache = Cache('ir_ui_view.view_get')
     __module_index = None
 
     @classmethod
     def __setup__(cls):
         super(View, cls).__setup__()
         table = cls.__table__()
+        cls.priority.required = True
 
         cls.__rpc__['view_get'] = RPC(instantiate=0, cache=dict(days=1))
-        cls._order.insert(0, ('priority', 'ASC'))
         cls._buttons.update({
                 'show': {
                     'readonly': Eval('type') != 'form',
-                    'depends': ['type'],
+                    'invisible': ~Eval('basis', False),
+                    'depends': ['type', 'basis'],
                     },
                 })
         cls._sql_indexes.update({
                 Index(table,
                     (table.model, Index.Equality()),
                     (table.inherit, Index.Equality())),
                 Index(
@@ -96,20 +127,54 @@
     def default_priority():
         return 16
 
     @staticmethod
     def default_module():
         return Transaction().context.get('module') or ''
 
+    def get_basis(self, name):
+        return not self.inherit or self.model != self.inherit.model
+
+    @classmethod
+    def domain_basis(cls, domain, tables):
+        table, _ = tables[None]
+        if 'inherit' not in tables:
+            inherit = cls.__table__()
+            tables['inherit'] = {
+                None: (inherit, table.inherit == inherit.id),
+                }
+        else:
+            inherit, _ = tables['inherit'][None]
+        expression = (table.inherit == Null) | (table.model != inherit.model)
+
+        _, operator, value = domain
+        if operator in {'=', '!='}:
+            if (operator == '=') != value:
+                expression = ~expression
+        elif operator in {'in', 'not in'}:
+            if True in value and False not in value:
+                pass
+            elif False in value and True not in value:
+                expression = ~expression
+            else:
+                expression = Literal(True)
+        else:
+            expression = Literal(True)
+        return expression
+
     def get_rec_name(self, name):
         return '%s (%s)' % (
-            self.model,
+            self.model_ref.rec_name,
             self.inherit.rec_name if self.inherit else self.type_string)
 
     @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('model_ref.rec_name', *clause[1:])]
+
+    @classmethod
     @ModelView.button_action('ir.act_view_show')
     def show(cls, views):
         pass
 
     @classmethod
     def get_rng(cls, type_):
         key = (cls.__name__, type_)
@@ -371,18 +436,27 @@
             return {}
 
     start = ShowStateView('ir.ui.view.show.start', [
             Button('Close', 'end', 'tryton-close', default=True),
             ])
 
 
-class ViewTreeWidth(ModelSQL, ModelView):
+class ViewTreeWidth(
+        fields.fmany2one(
+            'model_ref', 'model', 'ir.model,model', "Model",
+            required=True, ondelete='CASCADE'),
+        fields.fmany2one(
+            'field_ref', 'field,model', 'ir.model.field,name,model', "Field",
+            required=True, ondelete='CASCADE',
+            domain=[
+                ('model', '=', Eval('model')),
+                ]),
+        ModelSQL, ModelView):
     "View Tree Width"
     __name__ = 'ir.ui.view_tree_width'
-    _rec_name = 'model'
     model = fields.Char('Model', required=True)
     field = fields.Char('Field', required=True)
     user = fields.Many2One('res.user', 'User', required=True,
         ondelete='CASCADE')
     width = fields.Integer('Width', required=True)
 
     @classmethod
@@ -395,14 +469,29 @@
         cls._sql_indexes.add(
             Index(
                 table,
                 (table.user, Index.Equality()),
                 (table.model, Index.Equality()),
                 (table.field, Index.Equality())))
 
+    def get_rec_name(self, name):
+        return f'{self.field_ref.rec_name} @ {self.model_ref.rec_name}'
+
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        operator = clause[1]
+        if operator.startswith('!') or operator.startswith('not '):
+            bool_op = 'AND'
+        else:
+            bool_op = 'OR'
+        return [bool_op,
+            ('model_ref.rec_name', *clause[1:]),
+            ('field_ref.rec_name', *clause[1:]),
+            ]
+
     @classmethod
     def delete(cls, records):
         ModelView._fields_view_get_cache.clear()
         super(ViewTreeWidth, cls).delete(records)
 
     @classmethod
     def create(cls, vlist):
```

### Comparing `trytond-7.0.9/trytond/ir/ui/view.xml` & `trytond-7.2.0/trytond/ir/ui/view.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/ui/view.xml` & `trytond-7.2.0/trytond/ir/ui/view.xml`

```diff
@@ -11,36 +11,45 @@
       <field name="model">ir.ui.view</field>
       <field name="type">form</field>
       <field name="name">ui_view_form</field>
     </record>
     <record model="ir.ui.view" id="view_view_tree">
       <field name="model">ir.ui.view</field>
       <field name="type">tree</field>
+      <field name="priority" eval="10"/>
       <field name="name">ui_view_list</field>
     </record>
+    <record model="ir.ui.view" id="view_view_list_extension">
+      <field name="model">ir.ui.view</field>
+      <field name="type">tree</field>
+      <field name="priority" eval="20"/>
+      <field name="name">ui_view_list_extension</field>
+    </record>
     <record model="ir.action.act_window" id="act_view_form">
       <field name="name">Views</field>
       <field name="type">ir.action.act_window</field>
       <field name="res_model">ir.ui.view</field>
+      <field name="domain" eval="[('basis', '=', True)]" pyson="1"/>
+      <field name="order" eval="[('model', None)]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_view_form_view1">
       <field name="sequence" eval="1"/>
       <field name="view" ref="view_view_tree"/>
       <field name="act_window" ref="act_view_form"/>
     </record>
     <record model="ir.action.act_window.view" id="act_view_form_view2">
       <field name="sequence" eval="2"/>
       <field name="view" ref="view_view_form"/>
       <field name="act_window" ref="act_view_form"/>
     </record>
     <menuitem parent="menu_ui" action="act_view_form" sequence="10" id="menu_view"/>
     <record model="ir.model.button" id="view_show_button">
+      <field name="model">ir.ui.view</field>
       <field name="name">show</field>
       <field name="string">Show</field>
-      <field name="model" search="[('model', '=', 'ir.ui.view')]"/>
     </record>
     <record model="ir.ui.view" id="view_tree_width_view_form">
       <field name="model">ir.ui.view_tree_width</field>
       <field name="type">form</field>
       <field name="name">ui_view_tree_width_form</field>
     </record>
     <record model="ir.ui.view" id="view_tree_width_view_tree">
```

### Comparing `trytond-7.0.9/trytond/ir/view/action_act_window_domain_form.xml` & `trytond-7.2.0/trytond/ir/view/action_act_window_domain_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/action_act_window_form.xml` & `trytond-7.2.0/trytond/ir/view/action_act_window_form.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/action_act_window_form.xml` & `trytond-7.2.0/trytond/ir/view/action_act_window_form.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <data>
   <xpath expr="//page[@id='general']" position="inside">
-    <label name="res_model"/>
-    <field name="res_model"/>
-    <label name="context_model"/>
-    <field name="context_model"/>
+    <label name="res_model_ref"/>
+    <field name="res_model_ref"/>
+    <label name="context_model_ref"/>
+    <field name="context_model_ref"/>
     <field name="act_window_views" colspan="4" view_ids="ir.act_window_view_view_list2"/>
     <field name="act_window_domains" colspan="4" view_ids="ir.act_window_domain_view_list2"/>
     <label name="domain"/>
     <field name="domain" colspan="3" widget="pyson"/>
     <label name="context_domain"/>
     <field name="context_domain" colspan="3" widget="pyson"/>
     <label name="context"/>
```

### Comparing `trytond-7.0.9/trytond/ir/view/action_form.xml` & `trytond-7.2.0/trytond/ir/view/action_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/action_report_form.xml` & `trytond-7.2.0/trytond/ir/view/action_report_form.xml`

 * *Files 13% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/action_report_form.xml` & `trytond-7.2.0/trytond/ir/view/action_report_form.xml`

```diff
@@ -7,21 +7,22 @@
     <field name="translatable" xexpand="0" width="25"/>
     <label name="single"/>
     <field name="single" xexpand="0" width="25"/>
     <label name="direct_print"/>
     <field name="direct_print" xexpand="0" width="25"/>
   </xpath>
   <xpath expr="//page[@id='general']" position="inside">
-    <label name="model"/>
-    <field name="model"/>
+    <label name="model_ref"/>
+    <field name="model_ref"/>
+    <label name="module_ref"/>
+    <field name="module_ref"/>
     <label name="report_name"/>
     <field name="report_name"/>
     <label name="record_name"/>
     <field name="record_name"/>
-    <newline/>
     <label name="report_content"/>
     <group col="-1" id="report_content">
       <field name="report_content" xexpand="0"/>
       <field name="report_content_html" string="Edit" widget="html" xexpand="0"/>
     </group>
     <label name="report"/>
     <field name="report"/>
```

### Comparing `trytond-7.0.9/trytond/ir/view/attachment_form.xml` & `trytond-7.2.0/trytond/ir/view/attachment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/attachment_list.xml` & `trytond-7.2.0/trytond/ir/view/attachment_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/cron_form.xml` & `trytond-7.2.0/trytond/ir/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/cron_list.xml` & `trytond-7.2.0/trytond/ir/view/cron_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/email_form.xml` & `trytond-7.2.0/trytond/ir/view/email_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/email_template_form.xml` & `trytond-7.2.0/trytond/ir/view/email_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/error_form.xml` & `trytond-7.2.0/trytond/ir/view/error_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/lang_form.xml` & `trytond-7.2.0/trytond/ir/view/lang_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/model_access_form.xml` & `trytond-7.2.0/trytond/ir/view/model_access_form.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/model_access_form.xml` & `trytond-7.2.0/trytond/ir/view/model_access_form.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form col="6">
-  <label name="model"/>
-  <field name="model"/>
+  <label name="model_ref"/>
+  <field name="model_ref"/>
   <label name="group"/>
   <field name="group"/>
   <label name="active"/>
   <field name="active"/>
   <group id="checkboxes" colspan="6">
     <label name="perm_read"/>
     <field name="perm_read"/>
```

### Comparing `trytond-7.0.9/trytond/ir/view/model_button_form.xml` & `trytond-7.2.0/trytond/ir/view/model_field_form.xml`

 * *Files 22% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/model_button_form.xml` & `trytond-7.2.0/trytond/ir/view/model_field_form.xml`

```diff
@@ -1,20 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
-  <label name="model"/>
-  <field name="model"/>
-  <label name="active"/>
-  <field name="active"/>
   <label name="name"/>
   <field name="name"/>
-  <label name="string"/>
-  <field name="string"/>
-  <separator name="help" colspan="4"/>
-  <field name="help" colspan="4"/>
-  <separator name="confirm" colspan="4"/>
-  <field name="confirm" colspan="4"/>
-  <field name="groups" colspan="4"/>
-  <field name="rules" colspan="2"/>
-  <field name="reset_by" colspan="2"/>
+  <label name="model_ref"/>
+  <field name="model_ref"/>
+  <label name="ttype"/>
+  <field name="ttype"/>
+  <label name="relation"/>
+  <field name="relation"/>
+  <label name="field_description"/>
+  <field name="field_description" colspan="3"/>
+  <label name="help" yfill="1"/>
+  <field name="help" colspan="3"/>
+  <label name="access"/>
+  <field name="access"/>
+  <label name="module_ref"/>
+  <field name="module_ref"/>
 </form>
```

### Comparing `trytond-7.0.9/trytond/ir/view/model_button_rule_form.xml` & `trytond-7.2.0/trytond/ir/view/model_button_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/model_data_form.xml` & `trytond-7.2.0/trytond/ir/view/model_data_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/model_data_form.xml` & `trytond-7.2.0/trytond/ir/view/model_data_form.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
   <label name="module"/>
   <field name="module"/>
-  <label name="model"/>
-  <field name="model"/>
+  <label name="model_ref"/>
+  <field name="model_ref"/>
   <label name="fs_id"/>
   <field name="fs_id"/>
   <label name="db_id"/>
   <field name="db_id"/>
   <label name="noupdate"/>
   <field name="noupdate"/>
   <newline/>
```

### Comparing `trytond-7.0.9/trytond/ir/view/model_field_access_form.xml` & `trytond-7.2.0/trytond/ir/view/note_form.xml`

 * *Files 21% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/model_field_access_form.xml` & `trytond-7.2.0/trytond/ir/view/note_form.xml`

```diff
@@ -1,23 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form col="6">
-  <label name="field"/>
-  <field name="field"/>
-  <label name="group"/>
-  <field name="group"/>
-  <label name="active"/>
-  <field name="active"/>
-  <group id="checkboxes" colspan="6">
-    <label name="perm_read"/>
-    <field name="perm_read"/>
-    <label name="perm_write"/>
-    <field name="perm_write"/>
-    <label name="perm_create"/>
-    <field name="perm_create"/>
-    <label name="perm_delete"/>
-    <field name="perm_delete"/>
-  </group>
-  <separator name="description" colspan="6"/>
-  <field name="description" colspan="6"/>
+<form>
+  <label name="resource"/>
+  <field name="resource"/>
+  <label name="unread"/>
+  <field name="unread"/>
+  <label name="last_user"/>
+  <field name="last_user"/>
+  <label name="last_modification"/>
+  <field name="last_modification"/>
+  <label name="copy_to_resources"/>
+  <field name="copy_to_resources" yexpand="0"/>
+  <field name="message" colspan="4"/>
 </form>
```

### Comparing `trytond-7.0.9/trytond/ir/view/model_field_form.xml` & `trytond-7.2.0/trytond/ir/view/ui_view_form.xml`

 * *Files 18% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/model_field_form.xml` & `trytond-7.2.0/trytond/ir/view/ui_view_form.xml`

```diff
@@ -1,21 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
+  <label name="model_ref"/>
+  <field name="model_ref"/>
+  <label name="type"/>
+  <field name="type"/>
+  <label name="inherit"/>
+  <field name="inherit"/>
+  <label name="domain"/>
+  <field name="domain" widget="pyson"/>
+  <label name="priority"/>
+  <field name="priority"/>
+  <label name="field_children"/>
+  <field name="field_children"/>
+  <label name="module_ref"/>
+  <field name="module_ref"/>
   <label name="name"/>
   <field name="name"/>
-  <label name="model"/>
-  <field name="model" readonly="1"/>
-  <label name="ttype"/>
-  <field name="ttype"/>
-  <label name="relation"/>
-  <field name="relation"/>
-  <label name="field_description"/>
-  <field name="field_description" colspan="3"/>
-  <label name="help" yfill="1"/>
-  <field name="help" colspan="3"/>
-  <label name="access"/>
-  <field name="access"/>
-  <label name="module"/>
-  <field name="module"/>
+  <separator name="arch" colspan="4"/>
+  <field name="arch" colspan="4"/>
+  <field name="extensions" colspan="4" view_ids="ir.view_view_list_extension"/>
+  <button name="show" colspan="4"/>
 </form>
```

### Comparing `trytond-7.0.9/trytond/ir/view/model_form.xml` & `trytond-7.2.0/trytond/ir/view/ui_menu_form.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/model_form.xml` & `trytond-7.2.0/trytond/ir/view/ui_menu_form.xml`

```diff
@@ -1,16 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form col="6">
+<form>
   <label name="name"/>
   <field name="name"/>
-  <label name="model"/>
-  <field name="model"/>
-  <label name="module"/>
-  <field name="module"/>
-  <label name="global_search_p"/>
-  <field name="global_search_p"/>
-  <separator name="info" colspan="6"/>
-  <field name="info" colspan="6"/>
-  <field name="fields" colspan="6" readonly="1"/>
+  <label name="active"/>
+  <field name="active"/>
+  <label name="parent"/>
+  <field name="parent"/>
+  <newline/>
+  <label name="icon"/>
+  <field name="icon"/>
+  <label name="sequence"/>
+  <field name="sequence"/>
+  <field name="action_keywords" string="Actions" colspan="4"/>
+  <field name="groups" colspan="4"/>
 </form>
```

### Comparing `trytond-7.0.9/trytond/ir/view/module_activate_upgrade_start_form.xml` & `trytond-7.2.0/trytond/ir/view/module_activate_upgrade_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/module_form.xml` & `trytond-7.2.0/trytond/ir/view/module_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/module_list.xml` & `trytond-7.2.0/trytond/ir/view/module_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/note_form.xml` & `trytond-7.2.0/trytond/ir/view/ui_view_tree_state_form.xml`

 * *Files 25% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/note_form.xml` & `trytond-7.2.0/trytond/ir/view/ui_view_tree_state_form.xml`

```diff
@@ -1,16 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
-  <label name="resource"/>
-  <field name="resource"/>
-  <label name="unread"/>
-  <field name="unread"/>
-  <label name="last_user"/>
-  <field name="last_user"/>
-  <label name="last_modification"/>
-  <field name="last_modification"/>
-  <label name="copy_to_resources"/>
-  <field name="copy_to_resources" yexpand="0"/>
-  <field name="message" colspan="4"/>
+  <label name="model"/>
+  <field name="model"/>
+  <label name="user"/>
+  <field name="user"/>
+  <label name="domain"/>
+  <field name="domain"/>
+  <label name="child_name"/>
+  <field name="child_name"/>
+  <separator name="nodes" colspan="4"/>
+  <field name="nodes" colspan="4"/>
+  <separator name="selected_nodes" colspan="4"/>
+  <field name="selected_nodes" colspan="4"/>
 </form>
```

### Comparing `trytond-7.0.9/trytond/ir/view/note_list.xml` & `trytond-7.2.0/trytond/ir/view/note_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/rule_group_form.xml` & `trytond-7.2.0/trytond/ir/view/rule_group_form.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/rule_group_form.xml` & `trytond-7.2.0/trytond/ir/view/rule_group_form.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form col="6">
-  <label name="model"/>
-  <field name="model"/>
+  <label name="model_ref"/>
+  <field name="model_ref"/>
   <label name="global_p"/>
   <field name="global_p"/>
   <label name="default_p"/>
   <field name="default_p"/>
   <group col="4" colspan="6" id="perm">
     <label name="perm_read"/>
     <field name="perm_read"/>
```

### Comparing `trytond-7.0.9/trytond/ir/view/sequence_form.xml` & `trytond-7.2.0/trytond/ir/view/sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/translation_form.xml` & `trytond-7.2.0/trytond/ir/view/translation_form.xml`

 * *Files 9% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/translation_form.xml` & `trytond-7.2.0/trytond/ir/view/translation_form.xml`

```diff
@@ -8,18 +8,18 @@
   <field name="type"/>
   <label name="res_id"/>
   <field name="res_id"/>
   <label name="fuzzy"/>
   <field name="fuzzy"/>
   <label name="lang"/>
   <field name="lang"/>
-  <label name="module"/>
-  <field name="module"/>
-  <label name="overriding_module"/>
-  <field name="overriding_module"/>
+  <label name="module_ref"/>
+  <field name="module_ref"/>
+  <label name="overriding_module_ref"/>
+  <field name="overriding_module_ref"/>
   <group col="2" colspan="6" yexpand="1" yfill="1" id="src_value">
     <separator name="src"/>
     <separator name="value"/>
     <field name="src"/>
     <field name="value"/>
   </group>
 </form>
```

### Comparing `trytond-7.0.9/trytond/ir/view/trigger_form.xml` & `trytond-7.2.0/trytond/ir/view/trigger_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/ir/view/ui_menu_form.xml` & `trytond-7.2.0/trytond/ir/view/model_field_access_form.xml`

 * *Files 27% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/ui_menu_form.xml` & `trytond-7.2.0/trytond/ir/view/model_field_access_form.xml`

```diff
@@ -1,18 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form>
-  <label name="name"/>
-  <field name="name"/>
+<form col="6">
+  <label name="model_ref"/>
+  <field name="model_ref"/>
+  <label name="field_ref"/>
+  <field name="field_ref"/>
   <label name="active"/>
   <field name="active"/>
-  <label name="parent"/>
-  <field name="parent"/>
-  <newline/>
-  <label name="icon"/>
-  <field name="icon"/>
-  <label name="sequence"/>
-  <field name="sequence"/>
-  <field name="action_keywords" string="Actions" colspan="4"/>
-  <field name="groups" colspan="4"/>
+  <label name="group"/>
+  <field name="group"/>
+  <group id="checkboxes" colspan="6">
+    <label name="perm_read"/>
+    <field name="perm_read"/>
+    <label name="perm_write"/>
+    <field name="perm_write"/>
+    <label name="perm_create"/>
+    <field name="perm_create"/>
+    <label name="perm_delete"/>
+    <field name="perm_delete"/>
+  </group>
+  <separator name="description" colspan="6"/>
+  <field name="description" colspan="6"/>
 </form>
```

### Comparing `trytond-7.0.9/trytond/ir/view/ui_view_form.xml` & `trytond-7.2.0/trytond/ir/view/model_button_form.xml`

 * *Files 20% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/ir/view/ui_view_form.xml` & `trytond-7.2.0/trytond/ir/view/model_button_form.xml`

```diff
@@ -1,24 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
-  <label name="model"/>
-  <field name="model"/>
-  <label name="type"/>
-  <field name="type"/>
-  <label name="inherit"/>
-  <field name="inherit"/>
-  <label name="domain"/>
-  <field name="domain" widget="pyson"/>
-  <label name="priority"/>
-  <field name="priority"/>
-  <label name="field_childs"/>
-  <field name="field_childs"/>
-  <label name="module"/>
-  <field name="module"/>
+  <label name="model_ref"/>
+  <field name="model_ref"/>
+  <label name="active"/>
+  <field name="active"/>
   <label name="name"/>
   <field name="name"/>
-  <separator name="arch" colspan="4"/>
-  <field name="arch" colspan="4"/>
-  <button name="show" colspan="4"/>
+  <label name="string"/>
+  <field name="string"/>
+  <separator name="help" colspan="4"/>
+  <field name="help" colspan="4"/>
+  <separator name="confirm" colspan="4"/>
+  <field name="confirm" colspan="4"/>
+  <field name="groups" colspan="4"/>
+  <field name="rules" colspan="2"/>
+  <field name="reset_by" colspan="2"/>
 </form>
```

### Comparing `trytond-7.0.9/trytond/model/__init__.py` & `trytond-7.2.0/trytond/model/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/active.py` & `trytond-7.2.0/trytond/model/active.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/avatar.py` & `trytond-7.2.0/trytond/model/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/descriptors.py` & `trytond-7.2.0/trytond/model/descriptors.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/dictschema.py` & `trytond-7.2.0/trytond/model/dictschema.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/digits.py` & `trytond-7.2.0/trytond/model/digits.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/exceptions.py` & `trytond-7.2.0/trytond/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/__init__.py` & `trytond-7.2.0/trytond/model/fields/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .char import Char
 from .date import Date, DateTime, Time, TimeDelta, Timestamp
 from .dict import Dict
 from .field import (
     SQL_OPERATORS, Field, context_validate, depends, domain_validate,
     get_eval_fields, on_change_result, states_validate)
 from .float import Float
+from .fmany2one import fmany2one
 from .function import Function, MultiValue
 from .integer import Integer
 from .many2many import Many2Many
 from .many2one import Many2One
 from .multiselection import MultiSelection
 from .numeric import Numeric
 from .one2many import One2Many
@@ -24,8 +25,8 @@
 
 __all__ = [
     depends, SQL_OPERATORS, on_change_result,
     get_eval_fields, states_validate, domain_validate, context_validate, Field,
     Boolean, Integer, Char, Text, FullText, Float, Numeric, Date,
     Timestamp, DateTime, Time, TimeDelta, Binary, Selection, Reference,
     Many2One, One2Many, Many2Many, Function, MultiValue, One2One, Dict,
-    MultiSelection]
+    MultiSelection, fmany2one]
```

### Comparing `trytond-7.0.9/trytond/model/fields/binary.py` & `trytond-7.2.0/trytond/model/fields/binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/boolean.py` & `trytond-7.2.0/trytond/model/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/char.py` & `trytond-7.2.0/trytond/model/fields/char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/date.py` & `trytond-7.2.0/trytond/model/fields/date.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     _sql_type = 'DATE'
     _py_type = datetime.date
 
     def sql_format(self, value):
         if isinstance(value, str):
             value = datetime.date.fromisoformat(value)
         elif isinstance(value, datetime.datetime):
-            if value.time() != datetime.time():
-                raise ValueError("Date field can not have time")
+            raise ValueError("Date field can not have time")
         return super().sql_format(value)
 
     def sql_cast(self, expression, timezone=None):
         if backend.name == 'sqlite':
             return SQLite_Date(expression)
         if timezone:
             expression = AtTimeZone(expression, 'utc')
```

### Comparing `trytond-7.0.9/trytond/model/fields/dict.py` & `trytond-7.2.0/trytond/model/fields/dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/field.py` & `trytond-7.2.0/trytond/model/fields/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -555,23 +555,21 @@
 
     def sortable(self, model):
         return hasattr(model, 'search')
 
 
 class FieldTranslate(Field):
 
-    def _get_translation_join(self, Model, name,
-            translation, model, table, from_, language):
+    def _get_translation_join(
+            self, Model, name, translation, table, from_, language):
         if Model.__name__ == 'ir.model.field':
             pool = Pool()
-            IrModel = pool.get('ir.model')
             ModelData = pool.get('ir.model.data')
             ModelField = pool.get('ir.model.field')
             Translation = pool.get('ir.translation')
-            model = IrModel.__table__()
             model_data = ModelData.__table__()
             model_field = ModelField.__table__()
             msg_trans = Translation.__table__()
             if name == 'field_description':
                 type_ = 'field'
             else:
                 type_ = 'help'
@@ -589,22 +587,20 @@
                     condition=(msg_trans.res_id == model_data.db_id)
                     & (model_data.model == 'ir.message')
                     & (msg_trans.name == 'ir.message,text'))
                 .join(model_field,
                     condition=Concat(
                         Concat(model_data.module, '.'),
                         model_data.fs_id) == getattr(model_field, name))
-                .join(model,
-                    condition=model_field.model == model.id)
                 .select(
                     msg_trans.id.as_('id'),
                     Literal(-1).as_('res_id'),
                     msg_trans.value.as_('value'),
                     Concat(
-                        Concat(model.model, ','),
+                        Concat(model_field.model, ','),
                         model_field.name).as_('name'),
                     msg_trans.lang.as_('lang'),
                     Literal(type_).as_('type'),
                     msg_trans.fuzzy.as_('fuzzy'),
                     ))
         if backend.name == 'postgresql' and _sql_version >= (1, 1, 0):
             query = translation.select(
@@ -624,17 +620,15 @@
                 translation.name.as_('name'),
                 group_by=[translation.res_id, translation.name])
         if Model.__name__ == 'ir.model':
             name_ = Concat(Concat(table.model, ','), name)
             type_ = 'model'
             res_id = -1
         elif Model.__name__ == 'ir.model.field':
-            from_ = from_.join(model, 'LEFT',
-                condition=model.id == table.model)
-            name_ = Concat(Concat(model.model, ','), table.name)
+            name_ = Concat(Concat(table.model, ','), table.name)
             if name == 'field_description':
                 type_ = 'field'
             else:
                 type_ = 'help'
             res_id = -1
         else:
             name_ = '%s,%s' % (Model.__name__, name)
@@ -648,24 +642,22 @@
         return query, from_.join(query, 'LEFT',
             condition=(query.res_id == res_id) & (query.name == name_))
 
     def _get_translation_column(self, Model, name):
         from trytond.ir.lang import get_parent_language
         pool = Pool()
         Translation = pool.get('ir.translation')
-        IrModel = pool.get('ir.model')
 
         table = join = Model.__table__()
-        model = IrModel.__table__()
         language = Transaction().language
         column = None
         while language:
             translation = Translation.__table__()
             translation, join = self._get_translation_join(
-                Model, name, translation, model, table, join, language)
+                Model, name, translation, table, join, language)
             column = Coalesce(NullIf(column, ''), translation.value)
             language = get_parent_language(language)
         return table, join, column
 
     @domain_method
     def convert_domain(self, domain, tables, Model):
         if not self.translate:
@@ -686,26 +678,24 @@
         where = self._domain_add_null(column, operator, value, where)
         return table.id.in_(join.select(model.id, where=where))
 
     def _get_translation_order(self, tables, Model, name):
         from trytond.ir.lang import get_parent_language
         pool = Pool()
         Translation = pool.get('ir.translation')
-        IrModel = pool.get('ir.model')
         table, _ = tables[None]
         join = table
         language = Transaction().language
         column = None
         while language:
             key = name + '.translation-' + language
             if key not in tables:
                 translation = Translation.__table__()
-                model = IrModel.__table__()
                 translation, join = self._get_translation_join(
-                    Model, name, translation, model, table, table, language)
+                    Model, name, translation, table, table, language)
                 if join.left == table:
                     tables[key] = {
                         None: (join.right, join.condition),
                         }
                 else:
                     tables[key] = {
                         None: (join.left.right, join.left.condition),
```

### Comparing `trytond-7.0.9/trytond/model/fields/float.py` & `trytond-7.2.0/trytond/model/fields/float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/function.py` & `trytond-7.2.0/trytond/model/fields/function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/many2many.py` & `trytond-7.2.0/trytond/model/fields/many2many.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from trytond.tools import cached_property, grouped_slice
 from trytond.transaction import Transaction
 
 from .field import (
     Field, context_validate, domain_method, domain_validate, get_eval_fields,
     instanciate_values, instantiate_context, search_order_validate,
     size_validate)
-from .function import Function
 
 
 class Many2Many(Field):
     '''
     Define many2many field (``list``).
     '''
     _type = 'many2many'
@@ -137,17 +136,19 @@
             return res
         for i in ids:
             res[i] = []
 
         Relation = self.get_relation()
         origin_field = Relation._fields[self.origin]
 
-        if (not isinstance(origin_field, Function)
-                or hasattr(Relation, 'order_' + self.field)):
-            order = [(self.origin, None)]
+        if origin_field.sortable(Relation):
+            if origin_field._type == 'reference':
+                order = [(self.origin, None)]
+            else:
+                order = [(self.origin + '.id', None)]
         else:
             order = []
         if self.order is None:
             order += [(self.target, None)]
         else:
             order += self.order
```

### Comparing `trytond-7.0.9/trytond/model/fields/many2one.py` & `trytond-7.2.0/trytond/model/fields/many2one.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,25 +260,24 @@
                 return super(Many2One, self).convert_domain(domain, tables,
                     Model)
             else:
                 target_name = 'rec_name'
         else:
             _, target_name = name.split('.', 1)
         target_domain = [(target_name,) + tuple(domain[1:])]
-        if Target.estimated_count() < _subquery_threshold:
+        rule_domain = Rule.domain_get(Target.__name__, mode='read')
+        if not rule_domain and target_name == 'id':
+            # No need to join with the target table
+            return super().convert_domain(
+                (self.name, operator, value), tables, Model)
+        elif Target.estimated_count() < _subquery_threshold:
             query = Target.search(target_domain, order=[], query=True)
             return column.in_(query)
         else:
-            rule_domain = Rule.domain_get(Target.__name__, mode='read')
-            if rule_domain:
-                target_domain = [target_domain, rule_domain]
-            elif target_name == 'id':
-                # No need to join with the target table
-                return super().convert_domain(
-                    (self.name, operator, value), tables, Model)
+            target_domain = [target_domain, rule_domain]
             target_tables = self._get_target_tables(tables)
             target_table, _ = target_tables[None]
             _, expression = Target.search_domain(
                 target_domain, tables=target_tables)
             return expression
 
     @order_method
```

### Comparing `trytond-7.0.9/trytond/model/fields/multiselection.py` & `trytond-7.2.0/trytond/model/fields/multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/numeric.py` & `trytond-7.2.0/trytond/model/fields/numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/one2many.py` & `trytond-7.2.0/trytond/model/fields/one2many.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from trytond.tools import cached_property, grouped_slice
 from trytond.transaction import Transaction
 
 from .field import (
     Field, context_validate, domain_method, domain_validate, get_eval_fields,
     instanciate_values, instantiate_context, search_order_validate,
     size_validate)
-from .function import Function
 
 _subquery_threshold = config.getint('database', 'subquery_threshold')
 
 
 class One2Many(Field):
     '''
     Define one2many field (``list``).
@@ -143,17 +142,19 @@
         '''
         Target = self.get_target()
         field = Target._fields[self.field]
         res = {}
         for i in ids:
             res[i] = []
 
-        if (not isinstance(field, Function)
-                or hasattr(Target, 'order_' + self.field)):
-            order = [(self.field, None)]
+        if field.sortable(Target):
+            if field._type == 'reference':
+                order = [(self.field, None)]
+            else:
+                order = [(self.field + '.id', None)]
         else:
             order = []
         if self.order:
             order += self.order
         elif Target._order:
             order += Target._order
         targets = []
```

### Comparing `trytond-7.0.9/trytond/model/fields/one2one.py` & `trytond-7.2.0/trytond/model/fields/one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/reference.py` & `trytond-7.2.0/trytond/model/fields/reference.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/selection.py` & `trytond-7.2.0/trytond/model/fields/selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/fields/text.py` & `trytond-7.2.0/trytond/model/fields/text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/match.py` & `trytond-7.2.0/trytond/model/match.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/model.py` & `trytond-7.2.0/trytond/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 
 
 @total_ordering
 class Model(URLMixin, PoolBase, metaclass=ModelMeta):
     """
     Define a model in Tryton.
     """
-    __slots__ = ('_id', '_values', '_init_values', '_removed', '_deleted')
+    __slots__ = (
+        '_id', '_values', '_init_values', '_removed', '_deleted',
+        '__weakref__')
     _rec_name = 'name'
 
     id = fields.Integer(lazy_gettext('ir.msg_ID'), readonly=True)
 
     @classmethod
     def __setup__(cls):
         super(Model, cls).__setup__()
@@ -240,19 +242,23 @@
     @classmethod
     def __names__(cls, field=None, record=None):
         pool = Pool()
         IrModel = pool.get('ir.model')
         IrModelField = pool.get('ir.model.field')
 
         def format_value(value):
+            ffield = getattr(cls, field, None)
             if isinstance(value, Model):
                 try:
                     return value.rec_name
                 except Exception:
                     return str(value.id)
+            elif ffield and ffield._type in {'selection', 'multiselection'}:
+                selection = ffield.get_selection(cls, field, record)
+                return ffield.get_selection_string(selection, value)
             else:
                 return str(value)
 
         names = {
             'model': IrModel.get_name(cls.__name__),
             }
         if field:
```

### Comparing `trytond-7.0.9/trytond/model/modelsingleton.py` & `trytond-7.2.0/trytond/model/modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/modelsql.py` & `trytond-7.2.0/trytond/model/modelsql.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import datetime
 from collections import OrderedDict, defaultdict
 from functools import wraps
 from itertools import chain, groupby, islice, product, repeat
 
 from sql import (
     Asc, Column, Desc, Expression, For, Literal, Null, NullsFirst, NullsLast,
-    Table, Union, With)
+    Table, Union, Window, With)
 from sql.aggregate import Count, Max
 from sql.conditionals import Coalesce
-from sql.functions import CurrentTimestamp, Extract, Substring
-from sql.operators import And, Concat, Equal, Operator, Or
+from sql.functions import CurrentTimestamp, Extract, RowNumber, Substring
+from sql.operators import And, Concat, Equal, Exists, Operator, Or
 
 from trytond import backend
 from trytond.cache import freeze
 from trytond.config import config
 from trytond.exceptions import ConcurrencyException
 from trytond.i18n import gettext
 from trytond.pool import Pool
@@ -283,14 +283,15 @@
         assert cls._table[-9:] != '__history', \
             'Model _table %s cannot end with "__history"' % cls._table
 
         super(ModelSQL, cls).__setup__()
 
         cls._sql_constraints = []
         cls._sql_indexes = set()
+        cls._history_sql_indexes = set()
         if not callable(cls.table_query):
             table = cls.__table__()
             cls._sql_constraints.append(
                 ('id_positive', Check(table, table.id >= 0),
                     'ir.msg_id_positive'))
             rec_name_field = getattr(cls, cls._rec_name, None)
             if (isinstance(rec_name_field, fields.Field)
@@ -303,18 +304,28 @@
         cls._order = [('id', None)]
         if issubclass(cls, ModelView):
             cls.__rpc__.update({
                     'history_revisions': RPC(),
                     })
         if cls._history:
             history_table = cls.__table_history__()
-            cls._sql_indexes.add(
-                Index(
-                    history_table,
-                    (history_table.id, Index.Equality())))
+            cls._history_sql_indexes.update({
+                    Index(
+                        history_table,
+                        (history_table.id, Index.Equality())),
+                    Index(
+                        history_table,
+                        (Coalesce(
+                                history_table.write_date,
+                                history_table.create_date).desc,
+                            Index.Range()),
+                        include=[
+                            Column(history_table, '__id'),
+                            history_table.id]),
+                    })
 
     @classmethod
     def __post_setup__(cls):
         super().__post_setup__()
 
         # Define Range index to optimise with reduce_ids
         for field in cls._fields.values():
@@ -439,15 +450,15 @@
                             backend.TableHandler(ref_model)
                     else:
                         ref = None
                 if field_name in ['create_uid', 'write_uid']:
                     # migration from 3.6
                     table.drop_fk(field_name)
                 elif ref:
-                    table.add_fk(field_name, ref, field.ondelete)
+                    table.add_fk(field_name, ref, on_delete=field.ondelete)
 
             required = field.required
             # Do not set 'NOT NULL' for Binary field as the database column
             # will be left empty if stored in the filestore or filled later by
             # the set method.
             if isinstance(field, fields.Binary):
                 required = False
@@ -501,24 +512,28 @@
                             [Column(h_table, c) for c in columns],
                             sql_table.select(*(Column(sql_table, c)
                                     for c in columns))))
                     cursor.execute(*h_table.update(
                             [h_table.write_date], [None]))
 
     @classmethod
-    def _update_sql_indexes(cls):
+    def _update_sql_indexes(cls, concurrently=False):
         def no_subset(index):
             for j in cls._sql_indexes:
                 if j != index and index < j:
                     return False
             return True
         if not callable(cls.table_query):
             table_h = cls.__table_handler__()
             indexes = filter(no_subset, cls._sql_indexes)
-            table_h.set_indexes(indexes)
+            table_h.set_indexes(indexes, concurrently=concurrently)
+            if cls._history:
+                history_th = cls.__table_handler__(history=True)
+                indexes = filter(no_subset, cls._history_sql_indexes)
+                history_th.set_indexes(indexes, concurrently=concurrently)
 
     @classmethod
     def _update_history_table(cls):
         if cls._history:
             history_table = cls.__table_handler__(history=True)
             for field_name, field in cls._fields.items():
                 if not field.sql_type():
@@ -845,15 +860,15 @@
                         raise_func = cls.__raise_data_error
                     with transaction.new_transaction():
                         for value in values:
                             skip = len(['create_uid', 'create_date'])
                             recomposed = dict(zip(column_names, value[skip:]))
                             raise_func(
                                 exception, recomposed, transaction=transaction)
-                    raise
+                        raise
 
         to_insert = []
         previous_columns = [table.create_uid, table.create_date]
         previous_column_names = []
 
         for values in vlist:
             # Clean values
@@ -1194,15 +1209,19 @@
                             target_ids.append(id_)
             else:
                 add = target_ids.append
             for row in rows:
                 value = row[name]
                 if value is not None:
                     add(value)
-            return Target.read(target_ids, fields)
+            related_read_limit = transaction.context.get('related_read_limit')
+            rows = Target.read(target_ids[:related_read_limit], fields)
+            if related_read_limit is not None:
+                rows += [{'id': i} for i in target_ids[related_read_limit:]]
+            return rows
 
         def add_related(field, rows, targets):
             name = field.name
             key = name + '.'
             if field._type.endswith('2many'):
                 for row in rows:
                     row[key] = values = list()
@@ -1349,15 +1368,15 @@
                             cls.__raise_integrity_error(
                                 exception, values, list(values.keys()),
                                 transaction=transaction)
                         elif isinstance(exception, backend.DatabaseDataError):
                             cls.__raise_data_error(
                                 exception, values, list(values.keys()),
                                 transaction=transaction)
-                    raise
+                        raise
 
             for fname, value in values.items():
                 field = cls._fields[fname]
                 if (getattr(field, 'translate', False)
                         and not hasattr(field, 'set')):
                     Translation.set_ids(
                         '%s,%s' % (cls.__name__, fname), 'model',
@@ -1518,28 +1537,34 @@
             try:
                 cursor.execute(*table.delete(where=red_sql))
             except backend.DatabaseIntegrityError as exception:
                 transaction = Transaction()
                 with Transaction().new_transaction():
                     cls.__raise_integrity_error(
                         exception, {}, transaction=transaction)
-                raise
+                    raise
 
         if has_translation:
             Translation.delete_ids(cls.__name__, 'model', ids)
 
         cls._insert_history(ids, deleted=True)
 
         cls._update_mptt(list(tree_ids.keys()), list(tree_ids.values()))
 
     @classmethod
     def __check_domain_rule(cls, ids, mode):
         pool = Pool()
+        Lang = pool.get('ir.lang')
         Rule = pool.get('ir.rule')
         Model = pool.get('ir.model')
+        try:
+            User = pool.get('res.user')
+            Group = pool.get('res.group')
+        except KeyError:
+            User = Group = None
         table = cls.__table__()
         transaction = Transaction()
         in_max = transaction.database.IN_MAX
         history_clause = None
         limit = None
         if (mode == 'read'
                 and cls._history
@@ -1609,15 +1634,26 @@
 
                     msg = gettext(
                         f'ir.msg_{mode}_rule_error', ids=ids, model=model,
                         rules='\n'.join(r.name for r in rules))
                 else:
                     msg = gettext(
                         f'ir.msg_{mode}_error', ids=ids, model=model)
-                raise AccessError(msg)
+
+                ctx_msg = []
+                lang = Lang.get()
+                if cls._history and transaction.context.get('_datetime'):
+                    ctx_msg.append(gettext('ir.msg_context_datetime',
+                            datetime=lang.strftime(
+                                transaction.context['_datetime'])))
+                if domain and User and Group:
+                    groups = Group.browse(User.get_groups())
+                    ctx_msg.append(gettext('ir.msg_context_groups',
+                            groups=', '.join(g.rec_name for g in groups)))
+                raise AccessError(msg, '\n'.join(ctx_msg))
 
     @classmethod
     def __search_query(cls, domain, count, query, order):
         pool = Pool()
         Rule = pool.get('ir.rule')
 
         rule_domain = Rule.domain_get(cls.__name__, mode='read')
@@ -1792,72 +1828,18 @@
             return select
         cursor.execute(*select)
 
         rows = list(cursor_dict(cursor, transaction.database.IN_MAX))
         cache = transaction.get_cache()
         delete_records = transaction.delete_records[cls.__name__]
 
-        def filter_history(rows):
-            if not (cls._history and transaction.context.get('_datetime')):
-                return rows
-
-            def history_key(row):
-                return row['_datetime'], row['__id']
-
-            ids_history = {}
-            create_dates = {}
-            for row in rows:
-                key = history_key(row)
-                if row['id'] in create_dates:
-                    if row['_datetime'] < create_dates[row['id']]:
-                        create_dates[row['id']] = row['_datetime']
-                else:
-                    create_dates[row['id']] = row['_datetime']
-                if row['id'] in ids_history:
-                    if key < ids_history[row['id']]:
-                        continue
-                ids_history[row['id']] = key
-
-            to_delete = set()
-            history = cls.__table_history__()
-            for sub_ids in grouped_slice([r['id'] for r in rows]):
-                sub_ids = list(sub_ids)
-                where = reduce_ids(history.id, sub_ids)
-                min_date = min(create_dates[r_id] for r_id in sub_ids)
-                cursor.execute(*history.select(
-                        history.id.as_('id'),
-                        history.write_date.as_('write_date'),
-                        (history.create_date == Null).as_('deleted'),
-                        where=where
-                        & (history.write_date != Null)
-                        & (Coalesce(history.write_date, history.create_date)
-                            >= min_date)
-                        & (history.write_date
-                            <= transaction.context['_datetime'])))
-                for h_id, write_date, deleted in cursor:
-                    if h_id in to_delete:
-                        continue
-                    history_date, _ = ids_history[h_id]
-                    if isinstance(history_date, str):
-                        strptime = datetime.datetime.strptime
-                        format_ = '%Y-%m-%d %H:%M:%S.%f'
-                        history_date = strptime(history_date, format_)
-                    if history_date < write_date:
-                        to_delete.add(h_id)
-                    elif history_date == write_date and deleted:
-                        to_delete.add(h_id)
-
-            return filter(lambda r: history_key(r) == ids_history[r['id']]
-                and r['id'] not in to_delete, rows)
-
         # Can not cache the history value if we are not sure to have fetch all
         # the rows for each records
         if (not (cls._history and transaction.context.get('_datetime'))
                 or len(rows) < transaction.database.IN_MAX):
-            rows = list(filter_history(rows))
             keys = None
             for data in islice(rows, 0, cache.size_limit):
                 if data['id'] in delete_records:
                     continue
                 if keys is None:
                     keys = list(data.keys())
                     for k in keys[:]:
@@ -1867,21 +1849,14 @@
                         if not getattr(field, 'datetime_field', None):
                             keys.remove(k)
                             continue
                 for k in keys:
                     del data[k]
                 cache[cls.__name__][data['id']]._update(data)
 
-        if len(rows) >= transaction.database.IN_MAX:
-            columns = cls.__searched_columns(main_table, history=True)
-            cursor.execute(*table.select(*columns,
-                    where=expression, order_by=order_by,
-                    limit=limit, offset=offset))
-            rows = filter_history(list(cursor_dict(cursor)))
-
         return cls.browse([x['id'] for x in rows])
 
     @classmethod
     def search_domain(cls, domain, active_test=None, tables=None):
         '''
         Return SQL tables and expression
         Set active_test to add it.
@@ -1915,17 +1890,64 @@
                 return And((convert(d) for d in (
                             domain[1:] if domain[0] == 'AND' else domain)))
 
         with without_check_access():
             expression = convert(domain)
 
         if cls._history and transaction.context.get('_datetime'):
-            table, _ = tables[None]
-            expression &= (Coalesce(table.write_date, table.create_date)
-                <= transaction.context['_datetime'])
+            database = Transaction().database
+            if database.has_window_functions():
+                table, _ = tables[None]
+                history = cls.__table_history__()
+                last_change = Coalesce(history.write_date, history.create_date)
+                # prefilter the history records for a bit of a speedup
+                selected_h_ids = convert_from(None, tables).select(
+                    table.id, where=expression)
+                most_recent = history.select(
+                    history.create_date, Column(history, '__id'),
+                    RowNumber(
+                        window=Window([history.id],
+                            order_by=[
+                                last_change.desc,
+                                Column(history, '__id').desc])).as_('rank'),
+                    where=((last_change <= transaction.context['_datetime'])
+                        & history.id.in_(selected_h_ids)))
+                # Filter again as the latest records from most_recent might not
+                # match the expression
+                expression &= Exists(most_recent.select(
+                        Literal(1),
+                        where=(
+                            (Column(table, '__id')
+                                == Column(most_recent, '__id'))
+                            & (most_recent.create_date != Null)
+                            & (most_recent.rank == 1))))
+            else:
+                table, _ = tables[None]
+                history_1 = cls.__table_history__()
+                history_2 = cls.__table_history__()
+                last_change = Coalesce(
+                    history_1.write_date, history_1.create_date)
+                latest_change = history_1.select(
+                    history_1.id, Max(last_change).as_('date'),
+                    where=(last_change <= transaction.context['_datetime']),
+                    group_by=[history_1.id])
+                most_recent = history_2.join(
+                    latest_change,
+                    condition=(
+                        (history_2.id == latest_change.id)
+                        & (Coalesce(
+                                history_2.write_date, history_2.create_date)
+                            == latest_change.date))
+                    ).select(
+                        Max(Column(history_2, '__id')).as_('h_id'),
+                        where=(history_2.create_date != Null),
+                        group_by=[history_2.id])
+                expression &= Exists(most_recent.select(
+                        Literal(1),
+                        where=(Column(table, '__id') == most_recent.h_id)))
         return tables, expression
 
     @classmethod
     def _rebuild_path(cls, field_name):
         "Rebuild path for the tree."
         cursor = Transaction().connection.cursor()
         field = cls._fields[field_name]
```

### Comparing `trytond-7.0.9/trytond/model/modelstorage.py` & `trytond-7.2.0/trytond/model/modelstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 __all__ = ['ModelStorage', 'EvalEnvironment']
 _cache_field = config.getint('cache', 'field')
 _cache_count_timeout = config.getint(
     'cache', 'count_timeout', default=60 * 60 * 24)
 _cache_count_clear = config.getint(
     'cache', 'count_clear', default=1000)
+_request_timeout = config.getint('request', 'timeout', default=0)
 
 
 def local_cache(Model, transaction=None):
     if transaction is None:
         transaction = Transaction()
     return LRUDictTransaction(record_cache_size(transaction), Model._record)
 
@@ -114,14 +115,16 @@
     write_uid = fields.Many2One(
         'res.user', lazy_gettext('ir.msg_edited_by'), readonly=True)
     write_date = fields.Timestamp(
         lazy_gettext('ir.msg_edited_at'), readonly=True)
     rec_name = fields.Function(
         fields.Char(lazy_gettext('ir.msg_record_name')), 'get_rec_name',
         searcher='search_rec_name')
+    xml_id = fields.Function(
+        fields.Char(lazy_gettext('ir.msg_xml_id')), 'get_xml_id')
     _count_cache = Cache(
         'modelstorage.count', duration=_cache_count_timeout, context=False)
     _log = None
 
     @classmethod
     def __setup__(cls):
         from .modelview import ModelView
@@ -132,19 +135,23 @@
                         result=lambda r: list(map(int, r))),
                     'read': RPC(),
                     'write': RPC(readonly=False,
                         instantiate=slice(0, None, 2)),
                     'delete': RPC(readonly=False, instantiate=0),
                     'copy': RPC(readonly=False, instantiate=0, unique=False,
                         result=lambda r: list(map(int, r))),
-                    'search': RPC(result=lambda r: list(map(int, r))),
-                    'search_count': RPC(),
-                    'search_read': RPC(),
-                    'resources': RPC(instantiate=0, unique=False),
-                    'export_data_domain': RPC(),
+                    'search': RPC(
+                        result=lambda r: list(map(int, r)),
+                        timeout=_request_timeout),
+                    'search_count': RPC(timeout=_request_timeout),
+                    'search_read': RPC(timeout=_request_timeout),
+                    'resources': RPC(
+                        instantiate=0, unique=False,
+                        timeout=_request_timeout),
+                    'export_data_domain': RPC(timeout=_request_timeout),
                     'export_data': RPC(instantiate=0, unique=False),
                     'import_data': RPC(readonly=False),
                     })
         if cls._log is None:
             cls._log = not cls.__name__.startswith('ir.')
 
     @classmethod
@@ -373,15 +380,23 @@
         pool = Pool()
         Lang = pool.get('ir.lang')
         if default is None:
             default = {}
         else:
             default = default.copy()
 
-        def is_readonly(Model):
+        def is_readonly(field):
+            if field.readonly:
+                return True
+            if hasattr(field, 'get_relation'):
+                Model = field.get_relation()
+            elif hasattr(field, 'get_target'):
+                Model = field.get_target()
+            else:
+                return False
             return (not issubclass(Model, ModelStorage)
                 or callable(getattr(Model, 'table_query', None)))
 
         def get_default(name):
             prefix = name + '.'
             return {name[len(prefix):]: value
                 for name, value in default.items()
@@ -415,22 +430,22 @@
                 elif ftype in ('many2one', 'one2one'):
                     try:
                         data[field_name] = data[field_name] and \
                             data[field_name][0]
                     except Exception:
                         pass
                 elif ftype in ('one2many',):
-                    if is_readonly(field.get_target()):
+                    if is_readonly(field):
                         del data[field_name]
                     elif data[field_name]:
                         data[field_name] = [(
                                 'copy', data[field_name],
                                 get_default(field_name))]
                 elif ftype == 'many2many':
-                    if is_readonly(pool.get(field.relation_name)):
+                    if is_readonly(field):
                         del data[field_name]
                     elif data[field_name]:
                         data[field_name] = [('add', data[field_name])]
                 elif ftype == 'binary':
                     # Copy only file_id
                     if (field.file_id
                             and origin.get(field.file_id)
@@ -669,14 +684,29 @@
         '''
         rec_name = cls._rec_name
         if rec_name not in cls._fields:
             return []
         return [(rec_name,) + tuple(clause[1:])]
 
     @classmethod
+    def get_xml_id(cls, records, name):
+        pool = Pool()
+        ModelData = pool.get('ir.model.data')
+
+        ids = dict.fromkeys(map(int, records))
+        with without_check_access():
+            for sub_records in grouped_slice(records):
+                for record in ModelData.search([
+                            ('model', '=', cls.__name__),
+                            ('db_id', 'in', [r.id for r in sub_records]),
+                            ]):
+                    ids[record.db_id] = f'{record.module}.{record.fs_id}'
+        return ids
+
+    @classmethod
     def search_global(cls, text):
         '''
         Yield tuples (record, name, icon) for text
         '''
         for record in cls.search([
                     ('rec_name', 'ilike', likify(text)),
                     ]):
@@ -692,25 +722,24 @@
         _local_cache = local_cache(cls, transaction)
         transaction_cache = transaction.get_cache()
         return [cls(x, _ids=ids,
                 _local_cache=_local_cache,
                 _transaction_cache=transaction_cache,
                 _transaction=transaction) for x in ids]
 
-    @staticmethod
-    def __export_row(record, fields_names):
+    def __export_row(self, fields_names):
         pool = Pool()
         lines = []
         data = ['' for x in range(len(fields_names))]
         done = []
         for fpos in range(len(fields_names)):
             fields_tree = fields_names[fpos]
             if not fields_tree:
                 continue
-            value = record
+            value = self
             i = 0
             while i < len(fields_tree):
                 if not isinstance(value, ModelStorage):
                     break
                 field_name = fields_tree[i]
                 descriptor = None
                 if '.' in field_name:
@@ -731,16 +760,16 @@
                     first = True
                     child_fields_names = [(x[:i + 1] == fields_tree[:i + 1]
                             and x[i + 1:]) or [] for x in fields_names]
                     if child_fields_names in done:
                         break
                     done.append(child_fields_names)
                     for child_record in value:
-                        child_lines = ModelStorage.__export_row(child_record,
-                                child_fields_names)
+                        child_lines = child_record.__export_row(
+                            child_fields_names)
                         if first:
                             if child_lines:
                                 for child_fpos in range(len(fields_names)):
                                     if child_fields_names[child_fpos]:
                                         data[child_fpos] = (
                                             child_lines[0][child_fpos])
                             lines += child_lines[1:]
@@ -787,15 +816,15 @@
     @classmethod
     def export_data(cls, records, fields_names, header=False):
         fields_names = [x.split('/') for x in fields_names]
         data = []
         if header:
             data.append(cls._convert_field_names(fields_names))
         for record in records:
-            data += cls.__export_row(record, fields_names)
+            data += record.__export_row(fields_names)
         return data
 
     @classmethod
     def export_data_domain(
             cls, domain, fields_names, offset=0, limit=None, order=None,
             header=False):
         records = cls.search(domain, limit=limit, offset=offset, order=order)
@@ -853,17 +882,15 @@
                 elif len(res2) > 1:
                     raise ImportDataError(
                         gettext('ir.msg_too_many_relations_found',
                             value=word,
                             column=column,
                             **Relation.__names__()))
                 else:
-                    res.extend(res2)
-            if len(res):
-                res = [('add', [x.id for x in res])]
+                    res.append(res2[0].id)
             return res
 
         def get_one2one(relation, value, column):
             return ('add', get_many2one(relation, value, column))
 
         @lru_cache(maxsize=1000)
         def get_reference(value, field, klass, column):
@@ -926,18 +953,18 @@
                     raise ImportDataError(
                         gettext('ir.msg_xml_id_syntax_error',
                             value=word,
                             column=column,
                             **klass.__names__(field))) from e
                 res_ids.append(db_id)
             if ftype == 'many2many' and res_ids:
-                return [('add', res_ids)]
+                return res_ids
             elif ftype == 'reference' and res_ids:
                 return '%s,%s' % (relation, str(res_ids[0]))
-            return res_ids and res_ids[0] or False
+            return res_ids[0]
 
         def dispatch(create, write, row, Relation=cls):
             id_ = row.pop('id', None)
             if id_:
                 write.append([Relation(id_)])
                 write.append(row)
             else:
@@ -973,15 +1000,15 @@
                 elif value:
                     return Decimal(value)
 
             def convert_date(value):
                 if isinstance(value, datetime.date):
                     return value
                 elif value:
-                    return datetime.datetime.strptime(value, '%Y-%m-%d').date()
+                    return datetime.date.fromisoformat(value)
 
             def convert_datetime(value):
                 if isinstance(value, datetime.datetime):
                     return value
                 elif value:
                     return datetime.datetime.strptime(
                         value, '%Y-%m-%d %H:%M:%S')
@@ -1018,28 +1045,32 @@
 
         def process_lines(data, prefix, fields_def, position=0, klass=cls):
             line = data[position]
             row = {}
             translate = {}
             todo = set()
             prefix_len = len(prefix)
+            many2many = set()
             # Import normal fields_names
             for i, field in enumerate(fields_names):
                 if i >= len(line):
                     raise Exception('ImportError',
                         'Please check that all your lines have %d cols.'
                         % len(fields_names))
                 is_prefix_len = (len(field) == (prefix_len + 1))
                 value = line[i]
                 column = '/'.join(field)
                 if is_prefix_len and field[-1].endswith(':id'):
                     field_name = field[-1][:-3]
                     ftype = fields_def[field_name]['type']
-                    row[field[0][:-3]] = get_by_id(
-                        value, ftype, field_name, klass, column)
+                    res = get_by_id(value, ftype, field_name, klass, column)
+                    if ftype == 'many2many':
+                        res = [('add', res)] if res else []
+                        many2many.add(field_name)
+                    row[field[0][:-3]] = res
                 elif is_prefix_len and ':lang=' in field[-1]:
                     field_name, lang = field[-1].split(':lang=')
                     translate.setdefault(lang, {})[field_name] = value or False
                 elif is_prefix_len and prefix == field[:-1]:
                     field_name = field[-1]
                     this_field_def = fields_def[field_name]
                     field_type = this_field_def['type']
@@ -1049,27 +1080,39 @@
                             res = int(value)
                         except ValueError:
                             res = get_many2one(klass.__name__, value, column)
                     elif field_type == 'many2one':
                         res = get_many2one(
                             this_field_def['relation'], value, column)
                     elif field_type == 'many2many':
+                        many2many.add(field_name)
                         res = get_many2many(
                             this_field_def['relation'], value, column)
+                        res = [('add', res)] if res else []
                     elif field_type == 'one2one':
                         res = get_one2one(
                             this_field_def['relation'], value, column)
                     elif field_type == 'reference':
                         res = get_reference(value, field_name, klass, column)
                     else:
                         res = convert(
                             value, field_type, field_name, klass, column)
-                    row[field[-1]] = res
+                    row[field_name] = res
                 elif prefix == field[0:prefix_len]:
                     todo.add(field[prefix_len])
+
+            if 'id' in row:
+                record = klass(row['id'])
+                for field_name in many2many:
+                    row[field_name].insert(
+                        0, ('remove',
+                            [x.id for x in getattr(record, field_name)]))
+            else:
+                record = None
+
             # Import one2many fields
             nbrmax = 1
             for field in todo:
                 Relation = pool.get(fields_def[field]['relation'])
                 newfd = Relation.fields_get()
                 newrow, max2, _ = process_lines(
                     data, prefix + [field], newfd, position, klass=Relation)
@@ -1094,14 +1137,21 @@
                     nbrmax = max(nbrmax, i)
                 row[field] = []
                 create = [v for v in create if any(v.values())]
                 if create:
                     row[field].append(('create', create))
                 if write:
                     row[field].append(('write',) + tuple(write))
+                if record:
+                    written = set(map(int, sum(write[0:None:2], [])))
+                    delete = [
+                        r.id for r in getattr(record, field)
+                        if r.id not in written]
+                    row[field].append(('delete', delete))
+
             if prefix_len == 0:
                 for i in range(max(nbrmax, 1)):
                     data.pop(0)
             return (row, nbrmax, translate)
 
         ModelData = pool.get('ir.model.data')
 
@@ -1289,20 +1339,18 @@
             return relations
 
         def validate_relation_domain(field, records, Relation, domain):
             relations = relation_domain(field, records)
             if relations:
                 for sub_relations in grouped_slice(relations):
                     sub_relations = set(sub_relations)
-                    # Use root user to skip access rules
-                    with Transaction().set_user(0):
-                        finds = Relation.search(['AND',
-                                [('id', 'in', [r.id for r in sub_relations])],
-                                domain,
-                                ])
+                    finds = Relation.search(['AND',
+                            [('id', 'in', [r.id for r in sub_relations])],
+                            domain,
+                            ])
                     invalid_relations = sub_relations - set(finds)
                     if Relation == cls and field._type not in {
                             'many2one', 'one2many', 'many2many', 'one2one',
                             'reference'}:
                         invalid_records = invalid_relations
                     elif field._type.endswith('2many'):
                         invalid_records = [
@@ -1432,18 +1480,20 @@
                             digits = digit_record.get_digits()
                         else:
                             digits = None
                     if (value is None
                             or not digits
                             or any(d is None for d in digits)):
                         return
-                    if (round(value, digits[1]) != value
-                            or (isinstance(value, Decimal)
-                                and value.as_tuple().exponent < -digits[1])):
-                        raise_error(value)
+                    if isinstance(value, Decimal):
+                        if value.as_tuple().exponent < -digits[1]:
+                            raise_error(value)
+                    else:
+                        if round(value, digits[1]) != value:
+                            raise_error(value)
                 # validate digits
                 if getattr(field, 'digits', None):
                     if is_pyson(field.digits):
                         pyson_digits = PYSONEncoder().encode(field.digits)
                         for record in records:
                             digits = _record_eval_pyson(
                                 record, pyson_digits, encoded=True)
@@ -1823,16 +1873,14 @@
                             continue
                         fvalue = instantiate(field, data[fname], data)
                     if id_ == self.id and fname == name:
                         value = fvalue
                     if fname not in self._local_cache[id_]:
                         self._local_cache[id_][fname] = fvalue
                     if (field._type in no_local_cache
-                            or field.context
-                            or getattr(field, 'datetime_field', None)
                             or (isinstance(field, fields.Function)
                                 and (not transaction.readonly
                                     or field.getter_with_context))):
                         to_delete.add(fname)
                 self._cache[id_]._update(
                     **{k: v for k, v in data.items() if k not in to_delete})
         return value
@@ -1959,17 +2007,21 @@
                 with Transaction().set_current_transaction(transaction), \
                         transaction.set_user(user), \
                         transaction.reset_context(), \
                         transaction.set_context(context), \
                         without_check_access():
                     if to_create:
                         news = cls.create([save_values[r] for r in to_create])
+                        new_ids = []
                         for record, new in zip(to_create, news):
                             record._ids.remove(record.id)
                             record._id = new.id
+                            # Group all records that are alone
+                            if not record._ids:
+                                record._ids = new_ids
                             record._ids.append(record.id)
                     if to_write:
                         cls.write(*sum(
                                 (([r], save_values[r]) for r in to_write), ()))
             except Exception:
                 for record in to_create + to_write:
                     record._values = values[record]
```

### Comparing `trytond-7.0.9/trytond/model/modelview.py` & `trytond-7.2.0/trytond/model/modelview.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,31 @@
         if value:
             self.value.update(value)
 
     def result(self):
         return self.value
 
 
+def set_visible(node, fields, loading='eager'):
+    "Set loading to visible fields"
+    if node.tag == 'group':
+        if node.attrib.get('expandable', '1') == '1':
+            for child in node:
+                set_visible(child, fields, loading)
+    elif node.tag == 'notebook':
+        if len(node) > 0:
+            set_visible(node[0], fields, loading)
+    elif node.tag == 'field':
+        if node.attrib['name'] in fields:
+            node.attrib['loading'] = 'eager'
+    else:
+        for child in node:
+            set_visible(child, fields, loading)
+
+
 def on_change(func):
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         result = func(self, *args, **kwargs)
         assert result is None, func
         return self
     wrapper.on_change = True
@@ -439,19 +456,22 @@
                         element.tag = 'label'
                         colspan = element.attrib.get('colspan')
                         element.attrib.clear()
                         element.attrib['id'] = 'hidden %s-%s' % (name, i)
                         if colspan is not None:
                             element.attrib['colspan'] = colspan
 
-        # Remove empty pages
         if type == 'form':
             for page in tree.xpath('//page[not(descendant::*)]'):
                 page.getparent().remove(page)
 
+            set_visible(tree,
+                {fname for fname, field in cls._fields.items()
+                    if field._type in {'one2many', 'many2many'}})
+
         if type == 'tree':
             user = Transaction().user
             if Transaction().context.get('view_tree_width'):
                 ViewTreeWidth = pool.get('ir.ui.view_tree_width')
                 viewtreewidths = ViewTreeWidth.search([
                     ('model', '=', cls.__name__),
                     ('user', '=', user),
@@ -503,14 +523,16 @@
                     fields_def[depend] = {'name': depend}
                     field_names.append(depend)
 
         arch = etree.tostring(
             tree, encoding='utf-8', pretty_print=False).decode('utf-8')
         # Do not call fields_def without fields as it returns all fields
         if fields_def:
+            # Prevent clients calling fields_view_get to get 'id' definition
+            fields_def.setdefault('id', {'name': 'id'})
             fields2 = cls.fields_get(list(fields_def.keys()), level=level)
         else:
             fields2 = {}
         for field in fields_def:
             if field in fields2:
                 fields2[field].update(fields_def[field])
         return arch, fields2
@@ -862,14 +884,15 @@
             elif field._type in ['one2many', 'many2many']:
                 targets = value
                 if fname in init_values:
                     init_targets = init_values._get(fname)
                 elif isinstance(field, fields.Function):
                     init_targets = []
                 else:
+                    assert hasattr(init_record, fname), (init_record, fname)
                     init_targets = getattr(init_record, fname, [])
                 value = collections.defaultdict(list)
                 previous = [t.id for t in init_targets if t.id]
                 for i, target in enumerate(targets):
                     if (field._type == 'one2many'
                             and field.field
                             and target._values):
```

### Comparing `trytond-7.0.9/trytond/model/multivalue.py` & `trytond-7.2.0/trytond/model/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/order.py` & `trytond-7.2.0/trytond/model/order.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/symbol.py` & `trytond-7.2.0/trytond/model/symbol.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/tree.py` & `trytond-7.2.0/trytond/model/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/union.py` & `trytond-7.2.0/trytond/model/union.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/model/workflow.py` & `trytond-7.2.0/trytond/model/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/modules/__init__.py` & `trytond-7.2.0/trytond/modules/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import configparser
 import itertools
 import logging
 import os
+import pkgutil
 from collections import defaultdict
 from glob import iglob
 
 from sql import Table
 from sql.functions import CurrentTimestamp
 
 import trytond.convert as convert
@@ -18,15 +19,14 @@
 from trytond.transaction import Transaction
 
 logger = logging.getLogger(__name__)
 
 ir_module = Table('ir_module')
 ir_model_data = Table('ir_model_data')
 
-OPJ = os.path.join
 MODULES_PATH = os.path.abspath(os.path.dirname(__file__))
 
 MODULES = []
 
 
 def get_module_info(name):
     "Return the content of the tryton.cfg"
@@ -128,15 +128,15 @@
     for language, files in lang2filenames.items():
         filenames = [f[base_path_position:] for f in files]
         logger.info('%s:loading %s', module, ','.join(filenames))
         Translation = pool.get('ir.translation')
         Translation.translation_import(language, module, files)
 
 
-def load_module_graph(graph, pool, update=None, lang=None):
+def load_module_graph(graph, pool, update=None, lang=None, indexes=True):
     # Prevent to import backend when importing module
     from trytond.cache import Cache
     from trytond.ir.lang import get_parent_language
 
     if lang is None:
         lang = [config.get('database', 'language')]
     if update is None:
@@ -165,14 +165,17 @@
         for node in graph:
             module = node.name
             if module not in MODULES:
                 continue
             logger.info(module)
             classes = pool.fill(module, modules)
             if update:
+                # Clear all caches to prevent _record with wrong schema to
+                # linger
+                transaction.cache.clear()
                 pool.setup(classes)
             package_state = module2state.get(module, 'not activated')
             if (is_module_to_install(module, update)
                     or (update
                         and package_state in ('to activate', 'to upgrade'))):
                 if package_state not in ('to activate', 'to upgrade'):
                     if package_state == 'activated':
@@ -195,15 +198,16 @@
                 tryton_parser = convert.TrytondXmlHandler(
                     pool, module, package_state, modules, lang)
 
                 for filename in node.info.get('xml', []):
                     filename = filename.replace('/', os.sep)
                     logger.info('%s:loading %s', module, filename)
                     # Feed the parser with xml content:
-                    with tools.file_open(OPJ(module, filename), 'rb') as fp:
+                    with tools.file_open(
+                            os.path.join(module, filename), 'rb') as fp:
                         tryton_parser.parse_xmlstream(fp)
 
                 modules_todo.append((module, list(tryton_parser.to_delete)))
 
                 load_translations(pool, node, lang)
 
                 if package_state == 'to remove':
@@ -218,50 +222,52 @@
                     cursor.execute(*ir_module.insert(
                             [ir_module.create_uid, ir_module.create_date,
                                 ir_module.name, ir_module.state],
                             [[0, CurrentTimestamp(), module, 'activated'],
                                 ]))
                 module2state[module] = 'activated'
 
-            # Rollback cache changes to prevent dead lock on ir.cache table
-            Cache.rollback(transaction)
-            transaction.commit()
-            # Clear the cache so that the transaction has an empty cache
-            # from now on. The cache is not empty because the rollback might
-            # have filled it with old data from before the transaction
-            # started.
-            Cache.clear_all()
-            # Clear transaction cache to update default_factory
-            transaction.cache.clear()
-
         if not update:
             pool.setup()
         else:
+            # As the caches are cleared at the end of the process there's
+            # no need to do it here.
+            # It may deadlock on the ir_cache SELECT if the table schema has
+            # been modified
+            Cache._reset.clear()
+            transaction.commit()
             # Remove unknown models and fields
             Model = pool.get('ir.model')
             Model.clean()
             ModelField = pool.get('ir.model.field')
             ModelField.clean()
-            transaction.commit()
 
         pool.setup_mixin()
 
-        if update:
+        def create_indexes(concurrently):
             for model_name in models_with_indexes:
                 model = pool.get(model_name)
                 if model._sql_indexes:
-                    logger.info('index:create %s', model_name)
-                    model._update_sql_indexes()
-            transaction.commit()
+                    logger.info('index:update %s', model_name)
+                    model._update_sql_indexes(concurrently=concurrently)
+
+        if update:
+            if indexes:
+                create_indexes(concurrently=False)
+            else:
+                logger.info('index:skipping indexes creation')
             for model_name in models_to_update_history:
                 model = pool.get(model_name)
                 if model._history:
                     logger.info('history:update %s', model.__name__)
                     model._update_history_table()
             transaction.commit()
+        elif indexes:
+            with transaction.new_transaction(autocommit=True):
+                create_indexes(concurrently=True)
 
         # Vacuum :
         while modules_todo:
             (module, to_delete) = modules_todo.pop()
             convert.post_import(pool, module, to_delete)
 
         if update:
@@ -269,22 +275,15 @@
             Cache.clear_all()
             Cache.refresh_pool(transaction)
     logger.info('all modules loaded')
 
 
 def get_modules(with_test=False):
     modules = {'ir', 'res'}
-    if os.path.exists(MODULES_PATH) and os.path.isdir(MODULES_PATH):
-        for file in os.listdir(MODULES_PATH):
-            if file.startswith('.'):
-                continue
-            if file == '__pycache__':
-                continue
-            if os.path.isdir(OPJ(MODULES_PATH, file)):
-                modules.add(file)
+    modules.update((m.name for m in pkgutil.iter_modules([MODULES_PATH])))
     for ep in tools.entry_points().select(group=MODULES_GROUP):
         modules.add(ep.name)
     if with_test:
         modules.add('tests')
     return modules
 
 
@@ -312,15 +311,16 @@
         # Some modules register nothing in the Pool
         if hasattr(module, 'register'):
             module.register()
         MODULES.append(module_name)
 
 
 def load_modules(
-        database_name, pool, update=None, lang=None, activatedeps=False):
+        database_name, pool, update=None, lang=None, indexes=True,
+        activatedeps=False):
     # Do not import backend when importing module
     res = True
     if update:
         update = update[:]
     else:
         update = []
 
@@ -345,15 +345,15 @@
                 try:
                     graph = create_graph(modules)
                 except MissingDependenciesException as e:
                     if not activatedeps:
                         raise
                     update += e.missings
 
-            load_module_graph(graph, pool, update, lang)
+            load_module_graph(graph, pool, update, lang, indexes)
 
             Configuration = pool.get('ir.configuration')
             Configuration(1).check()
 
             if update:
                 cursor.execute(*ir_module.select(ir_module.name,
                         where=(ir_module.state == 'to remove')))
@@ -372,16 +372,14 @@
                 cursor.execute(*ir_module.update([ir_module.state],
                         ['not activated'],
                         where=(ir_module.state == 'to remove')))
                 transaction.connection.commit()
 
                 Module = pool.get('ir.module')
                 Module.update_list()
-        # Need to commit to unlock SQLite database
-        transaction.commit()
 
     if not Transaction().connection:
         with Transaction().start(database_name, 0):
             _load_modules(update)
     else:
         with Transaction().new_transaction(), \
                 Transaction().set_user(0), \
```

### Comparing `trytond-7.0.9/trytond/pool.py` & `trytond-7.2.0/trytond/pool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import builtins
 import logging
 from collections import OrderedDict, defaultdict
-from threading import RLock
+from threading import RLock, local
+from weakref import WeakSet
 
 from trytond.modules import load_modules, register_classes
 from trytond.transaction import Transaction
 
 __all__ = ['Pool', 'PoolMeta', 'PoolBase', 'isregisteredby']
 
 logger = logging.getLogger(__name__)
@@ -38,64 +39,65 @@
 
     @classmethod
     def __register__(cls, module_name):
         pass
 
 
 class Pool(object):
+    __slots__ = ('database_name', '_modules', '_pool', '__weakref__')
 
     classes = {
         'model': defaultdict(OrderedDict),
         'wizard': defaultdict(OrderedDict),
         'report': defaultdict(OrderedDict),
     }
     classes_mixin = defaultdict(list)
     _started = False
     _lock = RLock()
-    _locks = {}
-    _pool = {}
+    _local = local()
+    _pools = defaultdict(lambda: defaultdict(dict))
+    _pool_modules = defaultdict(list)
+    _pool_instances = WeakSet()
     test = False
-    _instances = {}
-    _modules = None
 
     def __new__(cls, database_name=None):
         if database_name is None:
             database_name = Transaction().database.name
-        result = cls._instances.get(database_name)
-        if result:
-            return result
-        lock = cls._locks.get(database_name)
-        if not lock:
+        instances = cls._local.__dict__.setdefault('instances', {})
+        if (instance := instances.get(database_name)) is None:
+            instances[database_name] = instance = super().__new__(cls)
+        if instance not in cls._pool_instances:
             with cls._lock:
-                lock = cls._locks.setdefault(database_name, RLock())
-        with lock:
-            return cls._instances.setdefault(database_name,
-                super(Pool, cls).__new__(cls))
+                instance._pool = cls._pools[database_name]
+                instance._modules = cls._pool_modules[database_name]
+                cls._pool_instances.add(instance)
+        return instance
 
     def __init__(self, database_name=None):
         if database_name is None:
             database_name = Transaction().database.name
         self.database_name = database_name
 
     @staticmethod
     def register(*classes, **kwargs):
         '''
         Register a list of classes
         '''
-        module = kwargs['module']
-        type_ = kwargs['type_']
-        depends = set(kwargs.get('depends', []))
-        assert type_ in {'model', 'report', 'wizard'}, (
-            f"{type_} is not a valid type_")
-        for cls in classes:
-            mpool = Pool.classes[type_][module]
-            assert cls not in mpool, f"{cls} is already registered"
-            assert issubclass(cls.__class__, PoolMeta), (
-                f"{cls} is missing metaclass {PoolMeta}")
-            mpool[cls] = depends
+        with Pool._lock:
+            module = kwargs['module']
+            type_ = kwargs['type_']
+            depends = set(kwargs.get('depends', []))
+            assert type_ in {'model', 'report', 'wizard'}, (
+                f"{type_} is not a valid type_")
+            for cls in classes:
+                mpool = Pool.classes[type_][module]
+                assert cls not in mpool, f"{cls} is already registered"
+                assert issubclass(cls.__class__, PoolMeta), (
+                    f"{cls} is missing metaclass {PoolMeta}")
+                mpool[cls] = depends
 
     @staticmethod
     def register_mixin(mixin, classinfo, module):
         Pool.classes_mixin[module].append((classinfo, mixin))
 
     @classmethod
     def start(cls):
@@ -110,88 +112,62 @@
 
     @classmethod
     def stop(cls, database_name):
         '''
         Stop the Pool
         '''
         with cls._lock:
-            if database_name in cls._instances:
-                del cls._instances[database_name]
-            lock = cls._locks.get(database_name)
-            if not lock:
-                return
-            with lock:
-                if database_name in cls._pool:
-                    del cls._pool[database_name]
+            cls._pools.pop(database_name, None)
+            cls._pool_instances.clear()
 
     @classmethod
     def database_list(cls):
         '''
         :return: database list
         '''
         with cls._lock:
-            databases = []
-            for database in cls._pool.keys():
-                if cls._locks.get(database):
-                    if cls._locks[database].acquire(False):
-                        databases.append(database)
-                        cls._locks[database].release()
-            return databases
+            return list(cls._pools.keys())
 
-    @property
-    def lock(self):
-        '''
-        Return the database lock for the pool.
-        '''
-        return self._locks[self.database_name]
-
-    def init(self, update=None, lang=None, activatedeps=False):
+    def init(self, update=None, lang=None, activatedeps=False, indexes=True):
         '''
         Init pool
         Set update to proceed to update
         lang is a list of language code to be updated
+        indexes is a boolean specifying if the indexes should be created
         '''
         with self._lock:
             if not self._started:
                 self.start()
-        with self._locks[self.database_name]:
-            # Don't reset pool if already init and not to update
-            if not update and self._pool.get(self.database_name):
-                return
             logger.info('init pool for "%s"', self.database_name)
-            self._pool.setdefault(self.database_name, {})
+            # Clear before loading modules
+            self._pool = defaultdict(dict)
             self._modules = []
-            # Clean the _pool before loading modules
-            for type in self.classes.keys():
-                self._pool[self.database_name][type] = {}
-            try:
-                restart = not load_modules(
-                    self.database_name, self, update=update, lang=lang,
-                    activatedeps=activatedeps)
-            except Exception:
-                del self._pool[self.database_name]
-                self._modules = None
-                raise
+            restart = not load_modules(
+                self.database_name, self, update=update, lang=lang,
+                activatedeps=activatedeps, indexes=indexes)
+            self._pools[self.database_name] = self._pool
+            self._pool_modules[self.database_name] = self._modules
+            self._pool_instances.clear()
             if restart:
                 self.init()
 
     def get(self, name, type='model'):
         '''
         Get an object from the pool
 
         :param name: the object name
         :param type: the type
         :return: the instance
         '''
         if type == '*':
             for type in self.classes.keys():
-                if name in self._pool[self.database_name][type]:
+                if name in self._pool[type]:
                     break
         try:
-            return self._pool[self.database_name][type][name]
+            return self._pool[type][name]
         except KeyError:
             if type == 'report':
                 from trytond.report import Report
 
                 # Keyword argument 'type' conflicts with builtin function
                 cls = builtins.type(name, (Report,), {'__slots__': ()})
                 cls.__setup__()
@@ -201,25 +177,24 @@
                 return self.get(name, type=type)
             raise
 
     def add(self, cls, type='model'):
         '''
         Add a classe to the pool
         '''
-        with self._locks[self.database_name]:
-            self._pool[self.database_name][type][cls.__name__] = cls
+        self._pool[type][cls.__name__] = cls
 
     def iterobject(self, type='model'):
         '''
         Return an iterator over object name, object
 
         :param type: the type
         :return: an iterator
         '''
-        return self._pool[self.database_name][type].items()
+        return self._pool[type].items()
 
     def fill(self, module, modules):
         '''
         Fill the pool with the registered class from the module for the
         activated modules.
         Return a list of classes for each type in a dictionary.
         '''
@@ -242,17 +217,16 @@
         self._modules.append(module)
         return classes
 
     def setup(self, classes=None):
         logger.info('setup pool for "%s"', self.database_name)
         if classes is None:
             classes = {}
-            for type_ in self._pool[self.database_name]:
-                classes[type_] = list(
-                    self._pool[self.database_name][type_].values())
+            for type_ in self._pool:
+                classes[type_] = list(self._pool[type_].values())
         for type_, lst in classes.items():
             for cls in lst:
                 cls.__setup__()
             for cls in lst:
                 cls.__post_setup__()
 
     def setup_mixin(self, type=None, name=None):
@@ -272,16 +246,18 @@
                         if (not issubclass(cls, parent)
                                 or issubclass(cls, mixin)):
                             continue
                         cls = builtins.type(
                             cls.__name__, (mixin, cls), {'__slots__': ()})
                         self.add(cls, type=type_)
 
-    def refresh(self, modules):
-        if self._modules and set(self._modules) != modules:
-            self.stop(self.database_name)
+    @classmethod
+    def refresh(cls, database_name, modules):
+        if (cls._pool_modules[database_name]
+                and set(cls._pool_modules[database_name]) != set(modules)):
+            cls.stop(database_name)
 
 
 def isregisteredby(obj, module, type_='model'):
     pool = Pool()
     classes = pool.classes[type_]
     return any(issubclass(obj, cls) for cls in classes[module])
```

### Comparing `trytond-7.0.9/trytond/protocols/dispatcher.py` & `trytond-7.2.0/trytond/protocols/dispatcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 
 @app.route('/<string:database_name>/', methods=['POST'])
 def rpc(request, database_name):
     methods = {
         'common.db.login': login,
         'common.db.logout': logout,
+        'common.db.reset_password': reset_password,
         'system.listMethods': list_method,
         'system.methodHelp': help_method,
         'system.methodSignature': lambda *a: 'signatures not supported',
         }
     return methods.get(request.rpc_method, _dispatch)(
         request, database_name, *request.rpc_params)
 
@@ -68,14 +69,32 @@
 def logout(request, database_name):
     auth = request.authorization
     security.logout(
         database_name, auth.get('userid'), auth.get('session'),
         context={'_request': request.context})
 
 
+def reset_password(request, database_name, user, language=None):
+    authentications = config.get(
+        'session', 'authentications', default='password').split(',')
+    if not any('password' in m.split('+') for m in authentications):
+        abort(HTTPStatus.FORBIDDEN)
+    context = {
+        'language': language,
+        '_request': request.context,
+        }
+    try:
+        security.reset_password(database_name, user, context=context)
+    except backend.DatabaseOperationalError:
+        logger.error('fail to connect to %s', database_name, exc_info=True)
+        abort(HTTPStatus.NOT_FOUND)
+    except RateLimitException:
+        abort(HTTPStatus.TOO_MANY_REQUESTS)
+
+
 @app.route('/', methods=['POST'])
 def root(request, *args):
     methods = {
         'common.server.version': lambda *a: __version__,
         'common.db.list': db_list,
         'common.authentication.services': authentication_services,
         }
@@ -180,15 +199,16 @@
     retry = config.getint('database', 'retry')
     count = 0
     transaction_extras = {}
     while True:
         if count:
             time.sleep(0.02 * (retry - count))
         with Transaction().start(
-                pool.database_name, user, readonly=rpc.readonly,
+                pool.database_name, user,
+                readonly=rpc.readonly, timeout=rpc.timeout,
                 **transaction_extras) as transaction:
             try:
                 c_args, c_kwargs, transaction.context, transaction.timestamp \
                     = rpc.convert(obj, *args, **kwargs)
                 transaction.context['_request'] = request.context
                 meth = rpc.decorate(getattr(obj, method))
                 if (rpc.instantiate is None
@@ -203,14 +223,17 @@
                         result = [rpc.result(meth(i, *c_args, **c_kwargs))
                             for i in inst]
             except TransactionError as e:
                 transaction.rollback()
                 transaction.tasks.clear()
                 e.fix(transaction_extras)
                 continue
+            except backend.DatabaseTimeoutError:
+                logger.warning(log_message, *log_args, exc_info=True)
+                abort(HTTPStatus.REQUEST_TIMEOUT)
             except backend.DatabaseOperationalError:
                 if count < retry and not rpc.readonly:
                     transaction.rollback()
                     transaction.tasks.clear()
                     count += 1
                     logger.debug("Retry: %i", count)
                     continue
```

### Comparing `trytond-7.0.9/trytond/protocols/jsonrpc.py` & `trytond-7.2.0/trytond/protocols/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/protocols/wrappers.py` & `trytond-7.2.0/trytond/protocols/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from http import HTTPStatus
 except ImportError:
     from http import client as HTTPStatus
 
 from werkzeug import exceptions
 from werkzeug.datastructures import Authorization
 from werkzeug.exceptions import abort
-from werkzeug.utils import redirect
+from werkzeug.utils import redirect, send_file
 from werkzeug.wrappers import Request as _Request
 from werkzeug.wrappers import Response
 
 from trytond import backend, security
 from trytond.config import config
 from trytond.exceptions import RateLimitException, UserError, UserWarning
 from trytond.pool import Pool
@@ -30,14 +30,15 @@
     'HTTPStatus',
     'Request',
     'Response',
     'abort',
     'allow_null_origin',
     'exceptions',
     'redirect',
+    'send_file',
     'set_max_request_size',
     'user_application',
     'with_pool',
     'with_transaction',
     ]
 
 logger = logging.getLogger(__name__)
@@ -58,25 +59,29 @@
             if auth:
                 args.append("%s@%s" % (
                         auth.get('userid', auth.username), self.remote_addr))
             else:
                 args.append(self.remote_addr)
             args.append("'%s'" % url)
             args.append("[%s]" % self.method)
-            args.append("%s" % (self.rpc_method or ''))
+            if self.view_args:
+                args.append("%s" % (self.rpc_method or ''))
         except Exception:
             args.append("(invalid WSGI environ)")
         return "<%s %s>" % (
             self.__class__.__name__, " ".join(filter(None, args)))
 
     @property
     def decoded_data(self):
         if self.content_encoding == 'gzip':
-            zipfile = gzip.GzipFile(fileobj=BytesIO(self.data), mode='rb')
-            return zipfile.read()
+            if self.user_id:
+                zipfile = gzip.GzipFile(fileobj=BytesIO(self.data), mode='rb')
+                return zipfile.read()
+            else:
+                abort(HTTPStatus.UNSUPPORTED_MEDIA_TYPE)
         else:
             return self.data
 
     @property
     def parsed_data(self):
         return self.data
 
@@ -102,16 +107,15 @@
                 return parse_authorization_header(header)
             else:
                 return parse_session(authorization.token)
         return authorization
 
     @cached_property
     def user_id(self):
-        if not self.view_args:
-            return None
+        assert self.view_args is not None
         database_name = self.view_args.get('database_name')
         if not database_name:
             return None
         auth = self.authorization
         if not auth:
             return None
         context = {'_request': self.context}
@@ -189,31 +193,44 @@
     @wraps(func)
     def wrapper(request, database_name, *args, **kwargs):
         database_list = Pool.database_list()
         pool = Pool(database_name)
         if database_name not in database_list:
             with Transaction().start(database_name, 0, readonly=True):
                 pool.init()
+
+        log_message = '%s in %i ms'
+
+        def duration():
+            return (time.monotonic() - started) * 1000
+        started = time.monotonic()
+
         try:
-            return func(request, pool, *args, **kwargs)
+            result = func(request, pool, *args, **kwargs)
         except exceptions.HTTPException:
-            logger.debug('%s', request, exc_info=True)
+            logger.info(
+                log_message, request, duration(),
+                exc_info=logger.isEnabledFor(logging.DEBUG))
             raise
         except (UserError, UserWarning) as e:
-            logger.debug('%s', request, exc_info=True)
+            logger.info(
+                log_message, request, duration(),
+                exc_info=logger.isEnabledFor(logging.DEBUG))
             if request.rpc_method:
                 raise
             else:
                 abort(HTTPStatus.BAD_REQUEST, e)
         except Exception as e:
-            logger.error('%s', request, exc_info=True)
+            logger.exception(log_message, request, duration())
             if request.rpc_method:
                 raise
             else:
                 abort(HTTPStatus.INTERNAL_SERVER_ERROR, e)
+        logger.info(log_message, request, duration())
+        return result
     return wrapper
 
 
 def with_transaction(readonly=None, user=0, context=None):
     from trytond.worker import run_task
 
     def decorator(func):
@@ -251,14 +268,15 @@
                         e.fix(transaction_extras)
                         continue
                     except backend.DatabaseOperationalError:
                         if count < retry and not readonly_:
                             transaction.rollback()
                             transaction.tasks.clear()
                             count += 1
+                            logger.debug("Retry: %i", count)
                             continue
                         raise
                     # Need to commit to unlock SQLite database
                     transaction.commit()
                 while transaction.tasks:
                     task_id = transaction.tasks.pop()
                     run_task(pool, task_id)
```

### Comparing `trytond-7.0.9/trytond/protocols/xmlrpc.py` & `trytond-7.2.0/trytond/protocols/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/pyson.py` & `trytond-7.2.0/trytond/pyson.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from decimal import Decimal
 from functools import reduce
 
 from dateutil.relativedelta import relativedelta
 
 
 class PYSON(object):
+    _operator = None
+    _binary_operator = None
 
     def pyson(self):
         raise NotImplementedError
 
     def types(self):
         raise NotImplementedError
 
@@ -77,16 +79,25 @@
     def in_(self, obj):
         return In(self, obj)
 
     def contains(self, k):
         return In(k, self)
 
     def __repr__(self):
-        klass = self.__class__.__name__
-        return '%s(%s)' % (klass, ', '.join(map(repr, self.__repr_params__)))
+        params = self.__repr_params__
+        if self._operator and isinstance(params[0], PYSON):
+            return '%s.%s(%s)' % (
+                repr(params[0]), self._operator,
+                ', '.join(map(repr, params[1:])))
+        elif self._binary_operator and isinstance(params[0], PYSON):
+            return '(%s %s %s)' % (
+                repr(params[0]), self._binary_operator, repr(params[1]))
+        else:
+            klass = self.__class__.__name__
+            return '%s(%s)' % (klass, ', '.join(map(repr, params)))
 
     @property
     def __repr_params__(self):
         return NotImplementedError
 
 
 class PYSONEncoder(json.JSONEncoder):
@@ -133,15 +144,18 @@
     def __init__(self, v, d=''):
         super(Eval, self).__init__()
         self._value = v
         self._default = d
 
     @property
     def __repr_params__(self):
-        return self._value, self._default
+        params = (self._value,)
+        if self._default != '':
+            params += (self._default,)
+        return params
 
     def pyson(self):
         return {
             '__class__': 'Eval',
             'v': self._value,
             'd': self._default,
             }
@@ -179,14 +193,25 @@
         if isinstance(v, PYSON):
             if v.types() != {bool}:
                 v = Bool(v)
         elif not isinstance(v, bool):
             v = bool(v)
         self._value = v
 
+    def __repr__(self):
+        if (isinstance(self._value, Equal)
+                and isinstance(self._value._statement1, PYSON)):
+            return '(%s != %s)' % (
+                repr(self._value._statement1),
+                repr(self._value._statement2))
+        elif isinstance(self._value, PYSON):
+            return '~%s' % repr(self._value)
+        else:
+            return super().__repr__()
+
     @property
     def __repr_params__(self):
         return (self._value,)
 
     def pyson(self):
         return {
             '__class__': 'Not',
@@ -194,15 +219,15 @@
             }
 
     def types(self):
         return {bool}
 
     @staticmethod
     def eval(dct, context):
-        return not dct['v']
+        return not Bool(dct['v']).eval(dct, context)
 
 
 class Bool(PYSON):
 
     def __init__(self, v):
         super(Bool, self).__init__()
         self._value = v
@@ -222,14 +247,16 @@
 
     @staticmethod
     def eval(dct, context):
         return bool(dct['v'])
 
 
 class And(PYSON):
+    _pyson_class = 'And'
+    _binary_operator = '&'
 
     def __init__(self, *statements, **kwargs):
         super(And, self).__init__()
         statements = list(statements) + kwargs.get('s', [])
         for i, statement in enumerate(list(statements)):
             if isinstance(statement, PYSON):
                 if statement.types() != {bool}:
@@ -254,26 +281,28 @@
 
     @staticmethod
     def eval(dct, context):
         return bool(reduce(lambda x, y: x and y, dct['s']))
 
 
 class Or(And):
+    _binary_operator = '|'
 
     def pyson(self):
         res = super(Or, self).pyson()
         res['__class__'] = 'Or'
         return res
 
     @staticmethod
     def eval(dct, context):
         return bool(reduce(lambda x, y: x or y, dct['s']))
 
 
 class Equal(PYSON):
+    _binary_operator = '=='
 
     def __init__(self, s1, s2):
         statement1, statement2 = s1, s2
         super(Equal, self).__init__()
         if isinstance(statement1, PYSON):
             types1 = statement1.types()
         else:
@@ -329,14 +358,18 @@
         elif not isinstance(equal, bool):
             equal = bool(equal)
         self._statement1 = statement1
         self._statement2 = statement2
         self._equal = equal
 
     @property
+    def _binary_operator(self):
+        return '>=' if self._equal else '>'
+
+    @property
     def __repr_params__(self):
         return (self._statement1, self._statement2, self._equal)
 
     def pyson(self):
         return {
             '__class__': 'Greater',
             's1': self._statement1,
@@ -374,14 +407,18 @@
             return dct['s1'] >= dct['s2']
         else:
             return dct['s1'] > dct['s2']
 
 
 class Less(Greater):
 
+    @property
+    def _binary_operator(self):
+        return '<=' if self._equal else '<'
+
     def pyson(self):
         res = super(Less, self).pyson()
         res['__class__'] = 'Less'
         return res
 
     @staticmethod
     def eval(dct, context):
@@ -436,14 +473,15 @@
         if dct['c']:
             return dct['t']
         else:
             return dct['e']
 
 
 class Get(PYSON):
+    _operator = 'get'
 
     def __init__(self, v, k, d=''):
         obj, key, default = v, k, d
         super(Get, self).__init__()
         if isinstance(obj, PYSON):
             assert obj.types() == {dict}, 'obj must be a dict'
         else:
@@ -454,15 +492,18 @@
         else:
             assert isinstance(key, str), 'key must be a string'
         self._key = key
         self._default = default
 
     @property
     def __repr_params__(self):
-        return (self._obj, self._key, self._default)
+        params = (self._obj, self._key)
+        if self._default != '':
+            params += (self._default,)
+        return params
 
     def pyson(self):
         return {
             '__class__': 'Get',
             'v': self._obj,
             'k': self._key,
             'd': self._default,
@@ -476,14 +517,15 @@
 
     @staticmethod
     def eval(dct, context):
         return dct['v'].get(dct['k'], dct['d'])
 
 
 class In(PYSON):
+    _operator = 'in_'
 
     def __init__(self, k, v):
         key, obj = k, v
         super(In, self).__init__()
         if isinstance(key, PYSON):
             assert key.types().issubset({str, int}), \
                 'key must be a string or an integer or a long'
@@ -504,14 +546,22 @@
                 if isinstance(key, PYSON):
                     assert key.types() == {str}, 'key must be a string'
                 else:
                     assert isinstance(key, str), 'key must be a string'
         self._key = key
         self._obj = obj
 
+    def __repr__(self):
+        params = self.__repr_params__
+        if isinstance(params[1], PYSON):
+            return '%s.contains(%s)' % (
+                repr(params[1]), ', '.join(map(repr, params[:1] + params[2:])))
+        else:
+            return super().__repr__()
+
     @property
     def __repr_params__(self):
         return (self._key, self._obj)
 
     def pyson(self):
         return {
             '__class__': 'In',
```

### Comparing `trytond-7.0.9/trytond/report/report.py` & `trytond-7.2.0/trytond/report/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 import os
 import subprocess
 import tempfile
 import time
 import unicodedata
 import warnings
 import zipfile
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
+from email.message import EmailMessage
 from io import BytesIO
 from itertools import groupby
 
 import dateutil.tz
 
 try:
     import html2text
@@ -543,28 +542,35 @@
             report_name = report.report_name
             report_id = report.id
         else:
             report_name = report
         Report_ = pool.get(report_name, type='report')
     converter = None
     title = None
-    msg = MIMEMultipart('alternative')
+    msg = EmailMessage()
     msg.add_header('Content-Language', ', '.join(l.code for l in languages))
-    for language in languages:
+    for alternative, language in enumerate(languages):
         with Transaction().set_context(
                 language=language.code, with_rec_name=False):
             ext, content, _, title = Report_.execute(
                 [record.id], {
                     'action_id': report_id,
                     'language': language,
                     })
+        if ext == 'txt':
+            ext = 'plain'
         if ext == 'html' and html2text:
             if not converter:
                 converter = html2text.HTML2Text()
-            part = MIMEText(
-                converter.handle(content), 'plain', _charset='utf-8')
-            part.add_header('Content-Language', language.code)
-            msg.attach(part)
-        part = MIMEText(content, ext, _charset='utf-8')
-        part.add_header('Content-Language', language.code)
-        msg.attach(part)
+            content_text = converter.handle(content)
+            msg.add_alternative(content_text, subtype='plain', params={
+                    'Content-Language': language.code,
+                    })
+        if alternative or msg.is_multipart():
+            msg.add_alternative(content, subtype=ext, params={
+                    'Content-Language': language.code,
+                    })
+        else:
+            msg.set_content(content, subtype=ext, params={
+                    'Content-Language': language.code,
+                    })
     return msg, title
```

### Comparing `trytond-7.0.9/trytond/res/__init__.py` & `trytond-7.2.0/trytond/res/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/res/email_reset_password.html` & `trytond-7.2.0/trytond/res/email_reset_password.html`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,25 @@
         <title>Reset Password</title>
     </head>
     <body>
         <div style="display: block; text-align: center">
             <div>
                 <h1>Reset Password</h1>
                 <p i18n:msg="login,password,host,database,http_host,database">
-                The password for your account, <strong>${record.login}</strong>, has been reset.<br/>
-                You must set a new one from the user's preferences.<br/>
+                Hello,
+                we have received a request to reset the password for the account associated with <strong>${record.login}</strong>. No changes have been made to your account yet.<br/>
                 You can connect with this temporary password <strong>${record.password_reset}</strong> to<br/>
                 <a href="tryton://${host}/${database}">tryton://${host}/${database}</a><br/>
-                <a href="${http_host}/#${database}">${http_host}/#${database}</a>
+                <a href="${http_host}/#${database}">${http_host}/#${database}</a><br/>
+                You must set a new one from the user's preferences.<br/>
                 </p>
             </div>
-            <hr style="margin-top: 20px; border-style: solid none none; border-color: #EEE"></hr>
+            <hr style="margin-top: 20px; border-style: solid none none; border-color: #EEE"/>
             <div style="font-size: 80%; color: #777">
                 <p i18n:msg="datetime,expire_delay">
                 The password will expire in <time datetime="${record.password_reset_expire.isoformat()}">${format_timedelta(expire_delay)}</time>.
                 </p>
+                <p>If you didn't make this request, you can safely ignore this email.</p>
             </div>
         </div>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
 ************ RReesseett PPaasssswwoorrdd ************
-The password for your account, $${{rreeccoorrdd..llooggiinn}}, has been reset.
-You must set a new one from the user's preferences.
+Hello, we have received a request to reset the password for the account
+associated with $${{rreeccoorrdd..llooggiinn}}. No changes have been made to your account yet.
 You can connect with this temporary password $${{rreeccoorrdd..ppaasssswwoorrdd__rreesseett}} to
 _t_r_y_t_o_n_:_/_/_$_{_h_o_s_t_}_/_$_{_d_a_t_a_b_a_s_e_}
 _$_{_h_t_t_p___h_o_s_t_}_/_#_$_{_d_a_t_a_b_a_s_e_}
+You must set a new one from the user's preferences.
 ===============================================================================
 The password will expire in ${format_timedelta(expire_delay)}.
+If you didn't make this request, you can safely ignore this email.
```

### Comparing `trytond-7.0.9/trytond/res/group.py` & `trytond-7.2.0/trytond/res/group.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/res/group.xml` & `trytond-7.2.0/trytond/res/group.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/res/group.xml` & `trytond-7.2.0/trytond/res/group.xml`

```diff
@@ -29,22 +29,22 @@
     <record model="ir.action.act_window.view" id="act_group_form_view2">
       <field name="sequence" eval="2"/>
       <field name="view" ref="group_view_form"/>
       <field name="act_window" ref="act_group_form"/>
     </record>
     <menuitem parent="res.menu_res" action="act_group_form" sequence="20" id="menu_group_form"/>
     <record model="ir.model.access" id="access_group">
-      <field name="model" search="[('model', '=', 'res.group')]"/>
+      <field name="model">res.group</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_group_admin">
-      <field name="model" search="[('model', '=', 'res.group')]"/>
+      <field name="model">res.group</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond-7.0.9/trytond/res/ir.py` & `trytond-7.2.0/trytond/res/ir.py`

 * *Files 6% similar despite different names*

```diff
@@ -216,17 +216,17 @@
     def _get_context(cls, model_name):
         context = super()._get_context(model_name)
         if model_name in {'res.user.warning', 'res.user.application'}:
             context['user_id'] = Transaction().user
         return context
 
     @classmethod
-    def _get_cache_key(cls, model_name):
-        key = super()._get_cache_key(model_name)
-        if model_name in {'res.user.warning', 'res.user.application'}:
+    def _get_cache_key(cls, model_names):
+        key = super()._get_cache_key(model_names)
+        if model_names & {'res.user.warning', 'res.user.application'}:
             key = (*key, Transaction().user)
         return key
 
 
 class SequenceType(metaclass=PoolMeta):
     __name__ = 'ir.sequence.type'
     groups = fields.Many2Many('ir.sequence.type-res.group', 'sequence_type',
```

### Comparing `trytond-7.0.9/trytond/res/ir.xml` & `trytond-7.2.0/trytond/res/ir.xml`

 * *Files 22% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/res/ir.xml` & `trytond-7.2.0/trytond/res/ir.xml`

```diff
@@ -1,252 +1,252 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data>
     <record model="ir.model.access" id="access_ir_sequence_type">
-      <field name="model" search="[('model', '=', 'ir.sequence.type')]"/>
+      <field name="model">ir.sequence.type</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_sequence_type_admin">
-      <field name="model" search="[('model', '=', 'ir.sequence.type')]"/>
+      <field name="model">ir.sequence.type</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_icon">
-      <field name="model" search="[('model', '=', 'ir.ui.icon')]"/>
+      <field name="model">ir.ui.icon</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_icon_admin">
-      <field name="model" search="[('model', '=', 'ir.ui.icon')]"/>
+      <field name="model">ir.ui.icon</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_menu">
-      <field name="model" search="[('model', '=', 'ir.ui.menu')]"/>
+      <field name="model">ir.ui.menu</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_menu_admin">
-      <field name="model" search="[('model', '=', 'ir.ui.menu')]"/>
+      <field name="model">ir.ui.menu</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_menu_favorite">
-      <field name="model" search="[('model', '=', 'ir.ui.menu.favorite')]"/>
+      <field name="model">ir.ui.menu.favorite</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_menu_favorite_admin">
-      <field name="model" search="[('model', '=', 'ir.ui.menu.favorite')]"/>
+      <field name="model">ir.ui.menu.favorite</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_view">
-      <field name="model" search="[('model', '=', 'ir.ui.view')]"/>
+      <field name="model">ir.ui.view</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_view_admin">
-      <field name="model" search="[('model', '=', 'ir.ui.view')]"/>
+      <field name="model">ir.ui.view</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_action">
-      <field name="model" search="[('model', '=', 'ir.action')]"/>
+      <field name="model">ir.action</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_action_admin">
-      <field name="model" search="[('model', '=', 'ir.action')]"/>
+      <field name="model">ir.action</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_model">
-      <field name="model" search="[('model', '=', 'ir.model')]"/>
+      <field name="model">ir.model</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_model_admin">
-      <field name="model" search="[('model', '=', 'ir.model')]"/>
+      <field name="model">ir.model</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_model_data">
-      <field name="model" search="[('model', '=', 'ir.model.data')]"/>
+      <field name="model">ir.model.data</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_model_log">
-      <field name="model" search="[('model', '=', 'ir.model.log')]"/>
+      <field name="model">ir.model.log</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_cron">
-      <field name="model" search="[('model', '=', 'ir.cron')]"/>
+      <field name="model">ir.cron</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_cron_admin">
-      <field name="model" search="[('model', '=', 'ir.cron')]"/>
+      <field name="model">ir.cron</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_queue">
-      <field name="model" search="[('model', '=', 'ir.queue')]"/>
+      <field name="model">ir.queue</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_queue_admin">
-      <field name="model" search="[('model', '=', 'ir.queue')]"/>
+      <field name="model">ir.queue</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_lang">
-      <field name="model" search="[('model', '=', 'ir.lang')]"/>
+      <field name="model">ir.lang</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_lang_admin">
-      <field name="model" search="[('model', '=', 'ir.lang')]"/>
+      <field name="model">ir.lang</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_translation">
-      <field name="model" search="[('model', '=', 'ir.translation')]"/>
+      <field name="model">ir.translation</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_translation_admin">
-      <field name="model" search="[('model', '=', 'ir.translation')]"/>
+      <field name="model">ir.translation</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_rule_group">
-      <field name="model" search="[('model', '=', 'ir.rule.group')]"/>
+      <field name="model">ir.rule.group</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_rule_group_admin">
-      <field name="model" search="[('model', '=', 'ir.rule.group')]"/>
+      <field name="model">ir.rule.group</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_module">
-      <field name="model" search="[('model', '=', 'ir.module')]"/>
+      <field name="model">ir.module</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_module_admin">
-      <field name="model" search="[('model', '=', 'ir.module')]"/>
+      <field name="model">ir.module</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_trigger">
-      <field name="model" search="[('model', '=', 'ir.trigger')]"/>
+      <field name="model">ir.trigger</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_trigger_admin">
-      <field name="model" search="[('model', '=', 'ir.trigger')]"/>
+      <field name="model">ir.trigger</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_menu">
       <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.ui.menu')]"/>
+      <field name="model">ir.ui.menu</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_menu1">
       <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_menu"/>
     </record>
     <record model="ir.rule" id="rule_menu2">
       <field name="domain" eval="[('groups', '=', None)]" pyson="1"/>
       <field name="rule_group" ref="rule_group_menu"/>
     </record>
     <record model="ir.rule.group" id="rule_group_action">
       <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.action')]"/>
+      <field name="model">ir.action</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_action1">
       <field name="domain" eval="[('groups', 'in', Eval('groups', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_action"/>
     </record>
     <record model="ir.rule" id="rule_action2">
@@ -312,76 +312,76 @@
     <record model="ir.ui.view" id="sequence_type_view_form">
       <field name="model">ir.sequence.type</field>
       <field name="inherit" ref="ir.sequence_type_view_form"/>
       <field name="name">sequence_type_form</field>
     </record>
     <record model="ir.rule.group" id="rule_group_sequence">
       <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.sequence')]"/>
+      <field name="model">ir.sequence</field>
       <field name="global_p" eval="True"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_sequence">
       <field name="domain" eval="[('sequence_type.groups', 'in', Eval('groups', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sequence"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sequence_strict">
       <field name="name">User in groups</field>
-      <field name="model" search="[('model', '=', 'ir.sequence.strict')]"/>
+      <field name="model">ir.sequence.strict</field>
       <field name="global_p" eval="True"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_sequence_strict">
       <field name="domain" eval="[('sequence_type.groups', 'in', Eval('groups', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sequence_strict"/>
     </record>
     <record model="ir.cron" id="cron_trigger_time">
       <field name="method">ir.trigger|trigger_time</field>
       <field name="interval_number" eval="5"/>
       <field name="interval_type">minutes</field>
     </record>
     <record model="ir.model.access" id="rule_default_view_tree_state">
-      <field name="model" search="[('model', '=', 'ir.ui.view_tree_state')]"/>
+      <field name="model">ir.ui.view_tree_state</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="rule_group_view_tree_state">
-      <field name="model" search="[('model', '=', 'ir.ui.view_tree_state')]"/>
+      <field name="model">ir.ui.view_tree_state</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_view_search">
-      <field name="model" search="[('model', '=', 'ir.ui.view_search')]"/>
+      <field name="model">ir.ui.view_search</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_ui_view_search_admin">
-      <field name="model" search="[('model', '=', 'ir.ui.view_search')]"/>
+      <field name="model">ir.ui.view_search</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_message">
-      <field name="model" search="[('model', '=', 'ir.message')]"/>
+      <field name="model">ir.message</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_message_group_admin">
-      <field name="model" search="[('model', '=', 'ir.message')]"/>
+      <field name="model">ir.message</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="export_view_form">
@@ -391,52 +391,52 @@
     </record>
     <record model="ir.ui.view" id="export_view_list">
       <field name="model">ir.export</field>
       <field name="inherit" ref="ir.export_view_tree"/>
       <field name="name">export_list</field>
     </record>
     <record model="ir.model.access" id="access_ir_export">
-      <field name="model" search="[('model', '=', 'ir.export')]"/>
+      <field name="model">ir.export</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_export_admin">
-      <field name="model" search="[('model', '=', 'ir.export')]"/>
+      <field name="model">ir.export</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_email_template">
-      <field name="model" search="[('model', '=', 'ir.email.template')]"/>
+      <field name="model">ir.email.template</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_email_template_admin">
-      <field name="model" search="[('model', '=', 'ir.email.template')]"/>
+      <field name="model">ir.email.template</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_ir_error">
-      <field name="model" search="[('model', '=', 'ir.error')]"/>
+      <field name="model">ir.error</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_ir_error_admin">
-      <field name="model" search="[('model', '=', 'ir.error')]"/>
+      <field name="model">ir.error</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond-7.0.9/trytond/res/locale/bg.po` & `trytond-7.2.0/trytond/res/locale/bg.po`

 * *Files 2% similar despite different names*

```diff
@@ -510,28 +510,33 @@
 msgid "Login Attempt"
 msgstr ""
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Потребителско предупреждение"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset Password"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+#, fuzzy
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Reset Password"
+
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/res/locale/ca.po` & `trytond-7.2.0/trytond/res/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -483,33 +483,39 @@
 msgid "Login Attempt"
 msgstr "Intent d'inici de sessió"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Alerta usuari"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Restableix la contrasenya"
-
+#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "La contrasenya del teu compte, [1:%(login)s], s'ha resetablert.[2:]\n"
 "                Heu d'establir una nova contraseña des de les preferències del usuari.[3:]\n"
 "                Podeu conectar amb aquesta contraseña temporal [4:%(password)s] a [5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
 "                [8:%(host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Restableix la contrasenya"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "La contrasenya caducarà el [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Cancel·lada"
```

### Comparing `trytond-7.0.9/trytond/res/locale/cs.po` & `trytond-7.2.0/trytond/res/locale/cs.po`

 * *Files 0% similar despite different names*

```diff
@@ -511,28 +511,33 @@
 msgid "Login Attempt"
 msgstr ""
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset Password"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+#, fuzzy
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Reset Password"
+
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/res/locale/de.po` & `trytond-7.2.0/trytond/res/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -484,33 +484,39 @@
 msgid "Login Attempt"
 msgstr "Login Versuch"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Benutzer Warnung"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Passwort zurücksetzen"
-
+#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "Das Passwort für Ihr Konto, [1:%(login)s], wurde zurückgesetzt.[2:]\n"
 "                Sie müssen ein neues über die Benutzereinstellungen vergeben.[3:]\n"
 "                Sie können sich mit diesem temporären Passwort [4:%(password)s] verbinden mit[5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
 "                [8:%(http_host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Passwort zurücksetzen"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Das Passwort wird in [1:%(datetime)s] ablaufen."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Annulliert"
```

### Comparing `trytond-7.0.9/trytond/res/locale/es.po` & `trytond-7.2.0/trytond/res/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -484,33 +484,39 @@
 msgid "Login Attempt"
 msgstr "Intento de inicio de sesión"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Aviso usuario"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Restablecer contraseña"
-
+#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "La contraseña para su cuenta, [1:%(login)s], se ha reseteado.[2:]\n"
 "                Debe establecer una nueva desde las preferencias de usuario.[3:]\n"
 "                Puede conectar con esta contraseña temporal [4:%(password)s] a [5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
 "                [8:%(host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Restablecer contraseña"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "La contraseña caducará en [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Cancelado"
```

### Comparing `trytond-7.0.9/trytond/res/locale/es_419.po` & `trytond-7.2.0/trytond/res/locale/es_419.po`

 * *Files 4% similar despite different names*

```diff
@@ -492,24 +492,29 @@
 msgstr ""
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
 msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "selection:res.user.application,state:"
```

### Comparing `trytond-7.0.9/trytond/res/locale/et.po` & `trytond-7.2.0/trytond/res/locale/et.po`

 * *Files 2% similar despite different names*

```diff
@@ -498,26 +498,31 @@
 msgstr "Sisselogimiskatse"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Kasutaja hoiatus"
 
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Salasõna lähtestamine"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Salasõna lähtestamine"
+
 #, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Salasõna aegub"
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
```

### Comparing `trytond-7.0.9/trytond/res/locale/fa.po` & `trytond-7.2.0/trytond/res/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -500,26 +500,31 @@
 msgstr "تلاش برای ورود"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "هشدار کاربر"
 
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "بازنشانی کلمه عبور"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "بازنشانی کلمه عبور"
+
 #, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "کلمه عبور شما منقضی میشود در"
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
```

### Comparing `trytond-7.0.9/trytond/res/locale/fi.po` & `trytond-7.2.0/trytond/res/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -508,28 +508,33 @@
 msgid "Login Attempt"
 msgstr ""
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset Password"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+#, fuzzy
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Reset Password"
+
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/res/locale/fr.po` & `trytond-7.2.0/trytond/res/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -486,30 +486,38 @@
 msgstr "Tentative d'identification"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Avertissement utilisateur"
 
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Réinitialisation de mot de passe"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
+"Bonjour,\n"
+"                nous avons reçu une demande de réinitialisation du mot de passe du compte associé à [1:%(login)s]. Aucune modification n'a encore été apportée à votre compte.[2:]\n"
+"                Vous pouvez vous connecter avec ce mot de passe temporaire [3:%(password)s] à[4:]\n"
+"                [5:tryton://%(hôte)s/%(base de données)s][6:]\n"
+"                [7:%(http_host)s/#%(base de données)s][8:]\n"
+"                Vous devez en définir un nouveau à partir des préférences de l'utilisateur.[9:]"
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
-"Le mot de passe de votre compte, [1:%(login)s], a été réinitialisé.[2:]\n"
-"                Vous devez en définir un nouveau dans les préférences de l'utilisateur.[3:]\n"
-"                Vous pouvez vous connecter avec ce mot de passe temporaire [4:%(password)s] à [5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Si vous n'avez pas fait cette demande, vous pouvez ignorer cet e-mail en "
+"toute sécurité."
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Réinitialisation de mot de passe"
 
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Le mot de passe expirera dans [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
```

### Comparing `trytond-7.0.9/trytond/res/locale/hu.po` & `trytond-7.2.0/trytond/res/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -488,33 +488,38 @@
 msgid "Login Attempt"
 msgstr "Bejelentkezés kísérlet"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Felhasználó figyelmeztetés"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Jelszó visszaállítása"
-
 #, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "A [1:%(login)s] nevű felhasználójának a jelszavát visszaállítottuk.[2:]\n"
 "                Adjon meg egy újat a Felhasználói beállítások ablakban.[3:]\n"
 "                Most a [4:%(password)s] ideiglenes jelszóval tud bejelentkezni a következő rendszerbe[5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
 "                [8:%(host)s/#%(database)s]"
 
+msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Jelszó visszaállítása"
+
 #, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Az ideiglenes jelszó az [1:%(datetime)s UTC] időpontig érvényes."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
```

### Comparing `trytond-7.0.9/trytond/res/locale/id.po` & `trytond-7.2.0/trytond/res/locale/id.po`

 * *Files 4% similar despite different names*

```diff
@@ -491,27 +491,32 @@
 msgstr ""
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Atur Ulang Kata Sandi"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Atur Ulang Kata Sandi"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Kata sandi akan kedaluwarsa dalam [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Dibatalkan"
```

### Comparing `trytond-7.0.9/trytond/res/locale/it.po` & `trytond-7.2.0/trytond/res/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -496,28 +496,33 @@
 msgid "Login Attempt"
 msgstr "Tentativo di Login"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Gruppi Utente"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset Password"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+#, fuzzy
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Reset Password"
+
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Annullato"
```

### Comparing `trytond-7.0.9/trytond/res/locale/lo.po` & `trytond-7.2.0/trytond/res/locale/lo.po`

 * *Files 2% similar despite different names*

```diff
@@ -509,28 +509,33 @@
 msgid "Login Attempt"
 msgstr "ການພະຍາຍາມເຂົ້າສູ່ລະບົບ"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "ຄຳເຕືອນຜູ້ໃຊ້ງານ"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset Password"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+#, fuzzy
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Reset Password"
+
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "ຍົກເລີກແລ້ວ"
```

### Comparing `trytond-7.0.9/trytond/res/locale/lt.po` & `trytond-7.2.0/trytond/res/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -497,26 +497,31 @@
 msgstr "Bandymas prisijungti"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Perspėjimai naudotojui"
 
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Atstatyti slaptažodį"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Atstatyti slaptažodį"
+
 #, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Slaptažodžio galiojimas baigsis"
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
```

### Comparing `trytond-7.0.9/trytond/res/locale/nl.po` & `trytond-7.2.0/trytond/res/locale/nl.po`

 * *Files 2% similar despite different names*

```diff
@@ -485,33 +485,39 @@
 msgid "Login Attempt"
 msgstr "Inlogpoging"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Gebruikerswaarschuwing"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset wachtwoord"
-
+#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "Het wachtwoord voor uw account, [1:%(login)s], is opnieuw ingesteld.[2:]\n"
 "                U moet er een nieuw aanmaken in de gebruikers voorkeuren[3:]\n"
 "               U kunt verbinding maken met dit tijdelijke wachtwoord [4:%(password)s] op[5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
 "                [8:%(host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Reset wachtwoord"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Het wachtwoord verloopt op [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Geannuleerd"
```

### Comparing `trytond-7.0.9/trytond/res/locale/pl.po` & `trytond-7.2.0/trytond/res/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -486,33 +486,38 @@
 msgid "Login Attempt"
 msgstr "Próba logowania"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Ostrzeżenie użytkownika"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Zresetuj hasło"
-
 #, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "Hasło do twojego konta, [1:%(login)s], zostało zresetowane.[2:]\n"
 "                Musisz ustawić nowe hasło w preferencjach użytkownika.[3:]\n"
 "                Możesz połączyć się używając tymczasowego hasła [4:%(password)s] do [5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
 "                [8:%(host)s/#%(database)s]"
 
+msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Zresetuj hasło"
+
 #, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Hasło wygaśnie o [1:%(datetime)s UTC]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
```

### Comparing `trytond-7.0.9/trytond/res/locale/pt.po` & `trytond-7.2.0/trytond/res/locale/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -500,26 +500,31 @@
 msgstr "Tentativa de Entrar"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Alerta de Usuário"
 
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Redefinir senha"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Redefinir senha"
+
 #, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "A senha irá expirar em"
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
```

### Comparing `trytond-7.0.9/trytond/res/locale/ro.po` & `trytond-7.2.0/trytond/res/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -482,33 +482,39 @@
 msgid "Login Attempt"
 msgstr "Încercare de conectare"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Avertisment utilizator"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Resetare parola"
-
+#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "Parolă pentru contul dvs, [1:%(login)s], a fost resetat.[2:]\n"
 "Trebuie să setaţi o parolă noua de la preferinţele al utilizatorului.[3:]\n"
 "Vă puteţi autentifica cu aceasta parolă temporară: [4:%(password)s] până la [5:]\n"
 "[6:tryton://%(host)s/%(database)s][7:]\n"
 "[8:%(host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Resetare parola"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Parola va expira in [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Anulat"
```

### Comparing `trytond-7.0.9/trytond/res/locale/ru.po` & `trytond-7.2.0/trytond/res/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -510,28 +510,33 @@
 msgid "Login Attempt"
 msgstr "Попытка входа"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Внимание Пользователь"
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset Password"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+#, fuzzy
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Reset Password"
+
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/res/locale/sl.po` & `trytond-7.2.0/trytond/res/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -480,33 +480,39 @@
 msgid "Login Attempt"
 msgstr "Poskus prijave"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Uporabniško opozorilo"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Ponastavitev gesla"
-
+#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "Geslo za vaš uporabniški račun, [1:%(login)s], je bilo ponastavljeno.[2:]\n"
 "                V uporabniških nastavitvah si morate nastaviti novo geslo.[3:]\n"
 "                Povežete se lahko s tem začasnim geslom [4:%(password)s] to[5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
 "                [8:%(http_host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Ponastavitev gesla"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Geslo poteče v [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Preklicano"
```

### Comparing `trytond-7.0.9/trytond/res/locale/tr.po` & `trytond-7.2.0/trytond/res/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -508,28 +508,33 @@
 msgid "Login Attempt"
 msgstr ""
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Reset Password"
+msgid ""
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
+msgstr ""
 
 msgctxt "report:res.user.email_reset_password:"
-msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+msgid "If you didn't make this request, you can safely ignore this email."
 msgstr ""
 
+#, fuzzy
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Reset Password"
+
 msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr ""
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr ""
```

### Comparing `trytond-7.0.9/trytond/res/locale/uk.po` & `trytond-7.2.0/trytond/res/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -485,33 +485,39 @@
 msgid "Login Attempt"
 msgstr "Спроба входу"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "Попередження користувача"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "Скинути пароль"
-
+#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "Пароль вашого облікового запису, [1:%(login)s], було скинуто.[2:]\n"
 "    Ви повинні встановити новий пароль у налаштуваннях користувача.[3:]\n"
 "    Ви можете підключитися за допомогою тимчасового паролю [4:%(password)s] до[5:]\n"
 "    [6:tryton://%(host)s/%(database)s][7:]\n"
 "    [8:%(http_host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "Скинути пароль"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "Термін дії пароля закінчиться [1:%(datetime)s]."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "Скасовано"
```

### Comparing `trytond-7.0.9/trytond/res/locale/zh_CN.po` & `trytond-7.2.0/trytond/res/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -480,33 +480,39 @@
 msgid "Login Attempt"
 msgstr "登录次数"
 
 msgctxt "model:res.user.warning,name:"
 msgid "User Warning"
 msgstr "用户警告"
 
-msgctxt "report:res.user.email_reset_password:"
-msgid "Reset Password"
-msgstr "重置密码"
-
+#, fuzzy
 msgctxt "report:res.user.email_reset_password:"
 msgid ""
-"The password for your account, [1:%(login)s], has been reset.[2:]\n"
-"                You must set a new one from the user's preferences.[3:]\n"
-"                You can connect with this temporary password [4:%(password)s] to[5:]\n"
-"                [6:tryton://%(host)s/%(database)s][7:]\n"
-"                [8:%(http_host)s/#%(database)s]"
+"Hello,\n"
+"                we have received a request to reset the password for the account associated with [1:%(login)s]. No changes have been made to your account yet.[2:]\n"
+"                You can connect with this temporary password [3:%(password)s] to[4:]\n"
+"                [5:tryton://%(host)s/%(database)s][6:]\n"
+"                [7:%(http_host)s/#%(database)s][8:]\n"
+"                You must set a new one from the user's preferences.[9:]"
 msgstr ""
 "你的账户 [1:%(login)s] 的密码已经重置.[2:]\n"
 "                你必须使用用户偏好功能设置一个新的密码.[3:]\n"
 "                你可以使用临时密码 [4:%(password)s] 连接到[5:]\n"
 "                [6:tryton://%(host)s/%(database)s][7:]\n"
 "                [8:%(host)s/#%(database)s]"
 
 msgctxt "report:res.user.email_reset_password:"
+msgid "If you didn't make this request, you can safely ignore this email."
+msgstr ""
+
+msgctxt "report:res.user.email_reset_password:"
+msgid "Reset Password"
+msgstr "重置密码"
+
+msgctxt "report:res.user.email_reset_password:"
 msgid "The password will expire in [1:%(datetime)s]."
 msgstr "密码将在 [1:%(datetime)s ] 过期."
 
 msgctxt "selection:res.user.application,state:"
 msgid "Cancelled"
 msgstr "已取消"
```

### Comparing `trytond-7.0.9/trytond/res/message.xml` & `trytond-7.2.0/trytond/res/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/res/routes.py` & `trytond-7.2.0/trytond/res/routes.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/res/user.py` & `trytond-7.2.0/trytond/res/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 try:
     import secrets
 except ImportError:
     secrets = None
 import ipaddress
 import warnings
 from ast import literal_eval
-from email.header import Header
 from functools import wraps
 from itertools import groupby
 from operator import attrgetter
 
 from passlib.context import CryptContext
 from sql import Literal, Null
 from sql.aggregate import Count
@@ -42,25 +41,25 @@
 
 from trytond.cache import Cache
 from trytond.config import config
 from trytond.exceptions import LoginException, RateLimitException, UserError
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, ModelSQL, ModelView, Unique, Workflow,
-    avatar_mixin, fields)
+    avatar_mixin, dualmethod, fields)
 from trytond.model.exceptions import ValidationError
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, PYSONEncoder
 from trytond.report import Report, get_email
 from trytond.rpc import RPC
-from trytond.sendmail import sendmail_transactional
+from trytond.sendmail import send_message_transactional
 from trytond.tools import grouped_slice
 from trytond.tools.email_ import (
     EmailNotValidError, normalize_email, set_from_header, validate_email)
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 from trytond.url import host, http_host
 from trytond.wizard import Button, StateTransition, StateView, Wizard
 
 logger = logging.getLogger(__name__)
 _has_password = 'password' in re.split('[,+]', config.get(
     'session', 'authentications', default='password'))
 
@@ -92,16 +91,16 @@
     for user in users:
         if not user.email:
             logger.info("Missing address for '%s' to send email", user.login)
             continue
         msg, title = email_func(user)
         set_from_header(msg, from_cfg, from_ or from_cfg)
         msg['To'] = user.email
-        msg['Subject'] = Header(title, 'utf-8')
-        sendmail_transactional(from_cfg, [user.email], msg)
+        msg['Subject'] = title
+        send_message_transactional(msg)
 
 
 class PasswordError(UserError):
     pass
 
 
 class DeleteError(UserError):
@@ -258,14 +257,16 @@
         if Transaction().user and value:
             cls.validate_password(value, users)
 
         to_write = []
         for user in users:
             to_write.extend([[user], {
                         'password_hash': cls.hash_password(value),
+                        'password_reset': None,
+                        'password_reset_expire': None,
                         }])
         cls.write(*to_write)
 
     @classmethod
     def validate_password(cls, password, users):
         password_b = password
         if isinstance(password, str):
@@ -289,24 +290,23 @@
                     (getattr(user, 'name', ''), 'res.msg_password_name'),
                     (getattr(user, 'login', ''), 'res.msg_password_login'),
                     (getattr(user, 'email', ''), 'res.msg_password_email'),
                     ]:
                 if test and password.lower() == test.lower():
                     raise PasswordError(gettext(message))
 
-    @classmethod
+    @dualmethod
     @ModelView.button
     def reset_password(cls, users, length=8, from_=None):
         length = max(length, config.getint('password', 'length', default=0))
         for user in users:
             user.password_reset = gen_password(length=length)
             user.password_reset_expire = (
                 datetime.datetime.now() + datetime.timedelta(
                     seconds=config.getint('password', 'reset_timeout')))
-            user.password = None
         cls.save(users)
         _send_email(from_, users, cls.get_email_reset_password)
 
     def get_email_reset_password(self):
         return get_email(
             'res.user.email_reset_password', self, self.languages)
 
@@ -325,15 +325,15 @@
     @staticmethod
     def get_sessions(users, name):
         Session = Pool().get('ir.session')
         now = datetime.datetime.now()
         timeout = datetime.timedelta(
             seconds=config.getint('session', 'max_age'))
         result = dict((u.id, 0) for u in users)
-        with Transaction().set_user(0):
+        with without_check_access():
             for sub_ids in grouped_slice(users):
                 sessions = Session.search([
                         ('create_uid', 'in', sub_ids),
                         ], order=[('create_uid', 'ASC')])
 
                 def filter_(session):
                     timestamp = session.write_date or session.create_date
@@ -749,21 +749,21 @@
         user_id, password_hash, password_reset = cls._get_login(login)
         if user_id and password_hash:
             password = parameters['password']
             valid, new_hash = cls.check_password(password, password_hash)
             if valid:
                 if new_hash:
                     logger.info("Update password hash for %s", user_id)
-                    with Transaction().new_transaction() as transaction:
-                        with transaction.set_user(0):
+                    with Transaction().new_transaction():
+                        with without_check_access():
                             cls.write([cls(user_id)], {
                                     'password_hash': new_hash,
                                     })
                 return user_id
-        elif user_id and password_reset:
+        if user_id and password_reset:
             if password_reset == parameters['password']:
                 return user_id
 
     @classmethod
     def hash_password(cls, password):
         '''Hash given password in the form
         <hash_method>$<password>$<salt>...'''
@@ -1074,14 +1074,15 @@
 
     @classmethod
     def format(cls, name, records):
         key = '|'.join(map(str, records)).encode('utf-8')
         return '%s.%s' % (hashlib.md5(key).hexdigest(), name)
 
     @classmethod
+    @without_check_access
     def check(cls, warning_name):
         transaction = Transaction()
         user = transaction.user
         context = transaction.context
         if not user or context.get('_skip_warnings'):
             return False
         key = (user, warning_name)
```

### Comparing `trytond-7.0.9/trytond/res/user.xml` & `trytond-7.2.0/trytond/res/user.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond-7.0.9/trytond/res/user.xml` & `trytond-7.2.0/trytond/res/user.xml`

```diff
@@ -43,33 +43,33 @@
     <record model="ir.action.act_window.view" id="act_user_form_view2">
       <field name="sequence" eval="2"/>
       <field name="view" ref="user_view_form"/>
       <field name="act_window" ref="act_user_form"/>
     </record>
     <menuitem parent="res.menu_res" action="act_user_form" sequence="10" id="menu_user_form"/>
     <record model="ir.model.access" id="access_user">
-      <field name="model" search="[('model', '=', 'res.user')]"/>
+      <field name="model">res.user</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_user_admin">
-      <field name="model" search="[('model', '=', 'res.user')]"/>
+      <field name="model">res.user</field>
       <field name="group" ref="group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="user_reset_password_button">
+      <field name="model">res.user</field>
       <field name="name">reset_password</field>
       <field name="string">Reset Password</field>
       <field name="help">Send by email a new temporary password to the user</field>
-      <field name="model" search="[('model', '=', 'res.user')]"/>
     </record>
     <record model="ir.ui.view" id="user_config_start_view_form">
       <field name="model">res.user.config.start</field>
       <field name="type">form</field>
       <field name="name">user_config_start_form</field>
     </record>
     <record model="ir.action.wizard" id="act_user_config">
@@ -88,15 +88,15 @@
     <record model="ir.ui.view" id="user_warning_view_tree">
       <field name="model">res.user.warning</field>
       <field name="type">tree</field>
       <field name="name">user_warning_tree</field>
     </record>
     <record model="ir.rule.group" id="rule_group_user_warning">
       <field name="name">Own warning</field>
-      <field name="model" search="[('model', '=', 'res.user.warning')]"/>
+      <field name="model">res.user.warning</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_user_warning1">
       <field name="domain" eval="[('user', '=', Eval('user_id', -1))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_user_warning"/>
     </record>
     <record model="ir.ui.view" id="user_application_view_form">
@@ -107,25 +107,25 @@
     <record model="ir.ui.view" id="user_application_view_list">
       <field name="model">res.user.application</field>
       <field name="type">tree</field>
       <field name="name">user_application_list</field>
     </record>
     <record model="ir.rule.group" id="rule_group_user_application">
       <field name="name">Own user application</field>
-      <field name="model" search="[('model', '=', 'res.user.application')]"/>
+      <field name="model">res.user.application</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_user_application1">
       <field name="domain" eval="[('user', '=', Eval('user_id', -1))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_user_application"/>
     </record>
     <record model="ir.rule.group" id="rule_group_user_application_admin">
       <field name="name">Any user application</field>
-      <field name="model" search="[('model', '=', 'res.user.application')]"/>
+      <field name="model">res.user.application</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_user_application_admin1">
       <field name="domain" eval="[]" pyson="1"/>
       <field name="rule_group" ref="rule_group_user_application_admin"/>
     </record>
@@ -137,18 +137,18 @@
       <field name="name">Reset Password</field>
       <field name="model">res.user</field>
       <field name="report_name">res.user.email_reset_password</field>
       <field name="report">res/email_reset_password.html</field>
       <field name="template_extension">html</field>
     </record>
     <record model="ir.model.button" id="user_application_validate_button">
+      <field name="model">res.user.application</field>
       <field name="name">validate_</field>
       <field name="string">Validate</field>
-      <field name="model" search="[('model', '=', 'res.user.application')]"/>
     </record>
     <record model="ir.model.button" id="user_application_cancel_button">
+      <field name="model">res.user.application</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'res.user.application')]"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond-7.0.9/trytond/res/view/group_form.xml` & `trytond-7.2.0/trytond/res/view/group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/res/view/user_application_form.xml` & `trytond-7.2.0/trytond/res/view/user_application_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/res/view/user_config_start_form.xml` & `trytond-7.2.0/trytond/res/view/user_config_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/res/view/user_form.xml` & `trytond-7.2.0/trytond/res/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/res/view/user_form_preferences.xml` & `trytond-7.2.0/trytond/res/view/user_form_preferences.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/rpc.py` & `trytond-7.2.0/trytond/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,33 +17,35 @@
     check_access: If access right must be checked
     fresh_session: If a fresh session is required
     unique: Check instances are unique
     '''
 
     __slots__ = (
         'readonly', 'instantiate', 'decorator', 'result',
-        'check_access', 'fresh_session', 'unique', 'cache')
+        'check_access', 'fresh_session', 'unique', 'cache', 'timeout')
 
     def __init__(
             self, readonly=True, instantiate=None, decorator=None, result=None,
-            check_access=True, fresh_session=False, unique=True, cache=None):
+            check_access=True, fresh_session=False, unique=True, cache=None,
+            timeout=None):
         self.readonly = readonly
         self.instantiate = instantiate
         self.decorator = decorator
         if result is None:
             def result(r):
                 return r
         self.result = result
         self.check_access = check_access
         self.fresh_session = fresh_session
         self.unique = unique
         if cache:
             if not isinstance(cache, RPCCache):
                 cache = RPCCache(**cache)
         self.cache = cache
+        self.timeout = timeout
 
     def convert(self, obj, *args, **kwargs):
         args = list(args)
         kwargs = kwargs.copy()
         if 'context' in kwargs:
             context = kwargs.pop('context')
             if not isinstance(context, dict):
```

### Comparing `trytond-7.0.9/trytond/security.py` & `trytond-7.2.0/trytond/security.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+import datetime as dt
 import logging
+import random
+import time
 
 from trytond import backend
 from trytond.config import config
 from trytond.exceptions import LoginException, RateLimitException
 from trytond.pool import Pool
 from trytond.transaction import Transaction
 
@@ -72,14 +75,44 @@
         logger.info("logout for '%s' from '%s' on database '%s'",
             name, _get_remote_addr(context), dbname)
     else:
         logger.error("logout failed for '%s' from '%s' on database '%s'",
             user, _get_remote_addr(context), dbname)
 
 
+def reset_password(dbname, user, context=None):
+    now = dt.datetime.now()
+    # Prevent guessing code execution path
+    time.sleep(random.random())
+    for count in range(config.getint('database', 'retry'), -1, -1):
+        with Transaction().start(dbname, 0, context=context):
+            pool = _get_pool(dbname)
+            User = pool.get('res.user')
+            try:
+                users = User.search([
+                        ('login', '=', user),
+                        ])
+                if not users:
+                    logger.info("Reset password for unknown user: %s", user)
+                    break
+                else:
+                    user, = users
+                if user.password_reset and user.password_reset_expire > now:
+                    logger.info(
+                        "Password reset already exists for user: %s", user)
+                else:
+                    user.reset_password()
+                    logger.info("Password reset for user: %s", user)
+                break
+            except backend.DatabaseOperationalError:
+                if count:
+                    continue
+                raise
+
+
 def check(dbname, user, session, context=None):
     for count in range(config.getint('database', 'retry'), -1, -1):
         with Transaction().start(dbname, user, context=context) as transaction:
             pool = _get_pool(dbname)
             Session = pool.get('ir.session')
             try:
                 find = Session.check(user, session)
```

### Comparing `trytond-7.0.9/trytond/sendmail.py` & `trytond-7.2.0/trytond/sendmail.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,68 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import logging
 import smtplib
 import ssl
 import time
-from email.message import Message
-from email.mime.text import MIMEText
+from email.message import EmailMessage, Message
 from email.utils import formatdate
 from urllib.parse import parse_qs, unquote_plus
 
 from trytond.config import config, parse_uri
 from trytond.transaction import Transaction
 
-__all__ = ['sendmail_transactional', 'sendmail', 'SMTPDataManager']
+__all__ = [
+    'sendmail_transactional', 'sendmail',
+    'send_message_transactional', 'send_message',
+    'SMTPDataManager']
 logger = logging.getLogger(__name__)
 retry = config.getint('email', 'retry', default=5)
 
 
 def sendmail_transactional(
         from_addr, to_addrs, msg, transaction=None, datamanager=None,
         strict=False):
+    send_message_transactional(
+        msg, from_addr, to_addrs, transaction, datamanager, strict)
+
+
+def send_message_transactional(
+        msg, from_addr=None, to_addrs=None, transaction=None, datamanager=None,
+        strict=False):
     if transaction is None:
         transaction = Transaction()
     assert isinstance(transaction, Transaction), transaction
     if datamanager is None:
         datamanager = SMTPDataManager(strict=strict)
     datamanager = transaction.join(datamanager)
     datamanager.put(from_addr, to_addrs, msg)
 
 
 def sendmail(from_addr, to_addrs, msg, server=None, strict=False):
+    return send_message(msg, from_addr, to_addrs, server, strict)
+
+
+def send_message(
+        msg, from_addr=None, to_addrs=None, server=None, strict=False):
     if server is None:
         server = get_smtp_server(strict=strict)
         if not server:
             return
         quit = True
     else:
         assert server.uri
         quit = False
     if 'Date' not in msg:
         msg['Date'] = formatdate()
     for count in range(retry, -1, -1):
         if count != retry:
             time.sleep(0.02 * (retry - count))
         try:
-            senderrs = server.sendmail(from_addr, to_addrs, msg.as_string())
+            senderrs = server.send_message(msg, from_addr, to_addrs)
         except smtplib.SMTPServerDisconnected:
             if count:
                 server = get_smtp_server(strict=strict)
                 if server:
                     continue
             if strict:
                 raise
@@ -74,20 +88,20 @@
         server.quit()
     else:
         return server
 
 
 def send_test_email(to_addrs, server=None):
     from_ = config.get('email', 'from')
-    msg = MIMEText('Success!\nYour email settings work correctly.')
+    msg = EmailMessage()
+    msg.set_content('Success!\nYour email settings work correctly.')
     msg['From'] = from_
     msg['To'] = to_addrs
     msg['Subject'] = 'Tryton test email'
-    sendmail(
-        config.get('email', 'from'), to_addrs, msg, server=server, strict=True)
+    send_message(msg, server=server, strict=True)
 
 
 def get_smtp_server(uri=None, strict=False):
     if uri is None:
         uri = config.get('email', 'uri')
     ini_uri = uri
     uri = parse_uri(uri)
@@ -149,16 +163,16 @@
     def tpc_vote(self, trans):
         if self._server is None:
             self._server = get_smtp_server(self.uri, strict=self.strict)
 
     def tpc_finish(self, trans):
         if self._server is not None:
             for from_addr, to_addrs, msg in self.queue:
-                new_server = sendmail(
-                    from_addr, to_addrs, msg, server=self._server)
+                new_server = send_message(
+                    msg, from_addr, to_addrs, server=self._server)
                 if new_server:
                     self._server = new_server
             self._server.quit()
             self._finish()
 
     def tpc_abort(self, trans):
         if self._server:
```

### Comparing `trytond-7.0.9/trytond/status.py` & `trytond-7.2.0/trytond/status.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/__init__.py` & `trytond-7.2.0/trytond/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/access.py` & `trytond-7.2.0/trytond/tests/access.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/copy_.py` & `trytond-7.2.0/trytond/tests/copy_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/export_data.py` & `trytond-7.2.0/trytond/tests/export_data.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_binary.py` & `trytond-7.2.0/trytond/tests/field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_boolean.py` & `trytond-7.2.0/trytond/tests/field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_char.py` & `trytond-7.2.0/trytond/tests/field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_context.py` & `trytond-7.2.0/trytond/tests/field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_date.py` & `trytond-7.2.0/trytond/tests/field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_datetime.py` & `trytond-7.2.0/trytond/tests/field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_dict.py` & `trytond-7.2.0/trytond/tests/field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_float.py` & `trytond-7.2.0/trytond/tests/field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_function.py` & `trytond-7.2.0/trytond/tests/field_function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_integer.py` & `trytond-7.2.0/trytond/tests/field_integer.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_many2many.py` & `trytond-7.2.0/trytond/tests/field_many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_many2one.py` & `trytond-7.2.0/trytond/tests/field_many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_multiselection.py` & `trytond-7.2.0/trytond/tests/field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_numeric.py` & `trytond-7.2.0/trytond/tests/field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_one2many.py` & `trytond-7.2.0/trytond/tests/field_one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_one2one.py` & `trytond-7.2.0/trytond/tests/field_one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_reference.py` & `trytond-7.2.0/trytond/tests/field_reference.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_selection.py` & `trytond-7.2.0/trytond/tests/field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_text.py` & `trytond-7.2.0/trytond/tests/field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_time.py` & `trytond-7.2.0/trytond/tests/field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/field_timedelta.py` & `trytond-7.2.0/trytond/tests/field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/history.py` & `trytond-7.2.0/trytond/tests/history.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/import_data.py` & `trytond-7.2.0/trytond/tests/import_data.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/import_data.xml` & `trytond-7.2.0/trytond/tests/import_data.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/message.xml` & `trytond-7.2.0/trytond/tests/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/mixin.py` & `trytond-7.2.0/trytond/tests/mixin.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/model.py` & `trytond-7.2.0/trytond/tests/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 from trytond.pyson import Eval
 
 
 class Model(ModelSQL):
     'Model'
     __name__ = 'test.model'
     name = fields.Char('Name')
+    selection = fields.Selection([
+            ('foo', "Foo"),
+            ('bar', "Bar"),
+            (None, ""),
+            ], "Selection")
+    multiselection = fields.MultiSelection([
+            ('foo', "Foo"),
+            ('bar', "Bar"),
+            ], "MultiSelection")
 
 
 class ModelParent(Model):
     "Model Parent"
     __name__ = 'test.model_parent'
     name = fields.Char("Name")
     children = fields.One2Many('test.model_child', 'parent', "Children")
```

### Comparing `trytond-7.0.9/trytond/tests/model_log.py` & `trytond-7.2.0/trytond/tests/model_log.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/modelsql.py` & `trytond-7.2.0/trytond/tests/modelsql.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,36 @@
     "ModelSQL to test read with ID in context"
     __name__ = 'test.modelsql.read.context_id'
     name = fields.Char("Name", context={
             'test': Eval('id'),
             })
 
 
+class ModelSQLReadLimit(ModelSQL):
+    "ModelSQL to test related limit"
+    __name__ = 'test.modelsql.read.limit'
+    name = fields.Char("Name")
+    targets = fields.One2Many(
+        'test.modelsql.read.limit.target', 'parent', "Targets")
+    sum_targets = fields.Function(
+        fields.Integer("Sum of Targets"), 'on_change_with_sum_targets')
+
+    @fields.depends('targets')
+    def on_change_with_sum_targets(self, name=None):
+        return sum(t.integer for t in self.targets)
+
+
+class ModelSQLReadLimitTarget(ModelSQL):
+    "ModelSQL to test related limit"
+    __name__ = 'test.modelsql.read.limit.target'
+    name = fields.Char("Name")
+    integer = fields.Integer("Integer")
+    parent = fields.Many2One('test.modelsql.read.limit', "Parent")
+
+
 class ModelSQLRequiredField(ModelSQL):
     'model with a required field'
     __name__ = 'test.modelsql'
 
     integer = fields.Integer(string="integer", required=True)
     desc = fields.Char(string="desc", required=True)
 
@@ -253,14 +275,16 @@
 
 
 def register(module):
     Pool.register(
         ModelSQLRead,
         ModelSQLReadTarget,
         ModelSQLReadContextID,
+        ModelSQLReadLimit,
+        ModelSQLReadLimitTarget,
         ModelSQLRequiredField,
         ModelSQLTimestamp,
         ModelSQLCreate,
         ModelSQLWrite,
         ModelSQLDelete,
         ModelSQLFieldSet,
         ModelSQLOne2Many,
```

### Comparing `trytond-7.0.9/trytond/tests/modelstorage.py` & `trytond-7.2.0/trytond/tests/modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/modelview.py` & `trytond-7.2.0/trytond/tests/modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/modelview.xml` & `trytond-7.2.0/trytond/tests/modelview.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/mptt.py` & `trytond-7.2.0/trytond/tests/mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/multivalue.py` & `trytond-7.2.0/trytond/tests/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/path.py` & `trytond-7.2.0/trytond/tests/path.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/resource.py` & `trytond-7.2.0/trytond/tests/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/rule.py` & `trytond-7.2.0/trytond/tests/rule.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/sequence.xml` & `trytond-7.2.0/trytond/tests/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_access.py` & `trytond-7.2.0/trytond/tests/test_access.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,21 +17,14 @@
     @classmethod
     def setUpClass(cls):
         activate_module('tests')
 
     model_name = model_access_name = 'test.access'
 
     @property
-    def model(self):
-        pool = Pool()
-        Model = pool.get('ir.model')
-        model, = Model.search([('model', '=', self.model_access_name)])
-        return model
-
-    @property
     def group(self):
         pool = Pool()
         Group = pool.get('res.group')
         group, = Group.search([('users', '=', Transaction().user)])
         return group
 
     def _assert(self, record):
@@ -53,140 +46,140 @@
     def test_access_without_group(self):
         "Test access without group"
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': None,
                     self._perm: True,
                     }])
 
         self._assert(record)
 
     @with_transaction(context=_context)
     def test_no_access_without_group(self):
         "Test no access without group"
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': None,
                     self._perm: False,
                     }])
 
         self._assert_raises(record)
 
     @with_transaction(context=_context)
     def test_one_access_with_groups(self):
         "Test one access with groups"
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': None,
                     self._perm: False,
                     }])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: True,
                     }])
 
         self._assert(record)
 
     @with_transaction(context=_context)
     def test_one_access_without_group(self):
         "Test one access without group"
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': None,
                     self._perm: True,
                     }])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: False,
                     }])
 
         self._assert(record)
 
     @with_transaction(context=_context)
     def test_all_access_with_groups(self):
         "Test all access with groups"
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': None,
                     self._perm: True,
                     }])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: True,
                     }])
 
         self._assert(record)
 
     @with_transaction(context=_context)
     def test_no_access_with_groups(self):
         "Test no access with groups"
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': None,
                     self._perm: False,
                     }])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: False,
                     }])
 
         self._assert_raises(record)
 
     @with_transaction(context=_context)
     def test_one_access_with_group(self):
         "Test one access with group"
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: True,
                     }])
 
         self._assert(record)
 
     @with_transaction(context=_context)
     def test_no_access_with_group(self):
         "Test no access with group"
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: False,
                     }])
 
         self._assert_raises(record)
 
     @with_transaction(context=_context)
@@ -195,20 +188,20 @@
         pool = Pool()
         Group = pool.get('res.group')
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: True,
                     }])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': group.id,
                     self._perm: True,
                     }])
 
         self._assert(record)
 
     @with_transaction(context=_context)
@@ -217,20 +210,20 @@
         pool = Pool()
         Group = pool.get('res.group')
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: False,
                     }])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': group.id,
                     self._perm: True,
                     }])
 
         self._assert_raises(record)
 
     @with_transaction(context=_context)
@@ -239,20 +232,20 @@
         pool = Pool()
         Group = pool.get('res.group')
         ModelAccess = pool.get('ir.model.access')
         TestAccess = pool.get(self.model_name)
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: True,
                     }])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': group.id,
                     self._perm: False,
                     }])
 
         self._assert(record)
 
     @with_transaction(context=_context)
@@ -264,20 +257,20 @@
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         Group.write([self.group], {
                 'parent': group.id,
                 })
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': self.group.id,
                     self._perm: False,
                     }])
         ModelAccess.create([{
-                    'model': self.model.id,
+                    'model': self.model_name,
                     'group': group.id,
                     self._perm: True,
                     }])
 
         self._assert(record)
 
 
@@ -310,20 +303,18 @@
         TestAccess.search([('reference.value', '=', 42, 'test.access.relate')])
 
     @with_transaction(context=_context)
     def test_access_relate(self):
         "Test access on search relate"
         pool = Pool()
         TestAccess = pool.get(self.model_name)
-        Model = pool.get('ir.model')
         ModelAccess = pool.get('ir.model.access')
         record, = TestAccess.create([{}])
-        model, = Model.search([('model', '=', 'test.access.relate')])
         ModelAccess.create([{
-                    'model': model.id,
+                    'model': 'test.access.relate',
                     'perm_read': True,
                     }])
 
         TestAccess.read([record.id], ['relate.value'])
         TestAccess.search([('relate.value', '=', 42)])
         TestAccess.search([('reference.value', '=', 42, 'test.access.relate')])
         TestAccess.search([('dict_.key', '=', 42)])
@@ -331,20 +322,18 @@
         TestAccess.search([], order=[('dict_.key', 'ASC')])
 
     @with_transaction(context=_context)
     def test_no_access_relate(self):
         "Test no access on search relate"
         pool = Pool()
         TestAccess = pool.get(self.model_name)
-        Model = pool.get('ir.model')
         ModelAccess = pool.get('ir.model.access')
         record, = TestAccess.create([{}])
-        model, = Model.search([('model', '=', 'test.access.relate')])
         ModelAccess.create([{
-                    'model': model.id,
+                    'model': 'test.access.relate',
                     'perm_read': False,
                     }])
 
         with self.assertRaises(AccessError):
             TestAccess.read([record.id], ['relate.value'])
         with self.assertRaises(AccessError):
             TestAccess.search([('relate.value', '=', 42)])
@@ -422,31 +411,14 @@
 class _ModelFieldAccessTestCase(unittest.TestCase):
     _perm = None
 
     @classmethod
     def setUpClass(cls):
         activate_module('tests')
 
-    def _field(self, name):
-        pool = Pool()
-        Field = pool.get('ir.model.field')
-        field1, = Field.search([
-                ('model.model', '=', 'test.access'),
-                ('name', '=', name),
-                ])
-        return field1
-
-    @property
-    def field1(self):
-        return self._field('field1')
-
-    @property
-    def field2(self):
-        return self._field('field2')
-
     @property
     def group(self):
         pool = Pool()
         Group = pool.get('res.group')
         group, = Group.search([('users', '=', Transaction().user)])
         return group
 
@@ -476,15 +448,16 @@
     def test_access_without_group(self):
         "Test access without group"
         pool = Pool()
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -492,15 +465,16 @@
     def test_no_access_without_group(self):
         "Test no access without group"
         pool = Pool()
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: False,
                     }])
 
         self._assert_raises1(record)
         self._assert2(record)
 
@@ -508,20 +482,22 @@
     def test_one_access_with_groups(self):
         "Test one access with groups"
         pool = Pool()
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: False,
                     }])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -529,20 +505,22 @@
     def test_one_access_without_group(self):
         "Test one access without group"
         pool = Pool()
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: False,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -550,20 +528,22 @@
     def test_all_access_with_groups(self):
         "Test all access with groups"
         pool = Pool()
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -571,20 +551,22 @@
     def test_no_access_with_groups(self):
         "Test no access with groups"
         pool = Pool()
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: False,
                     }])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: False,
                     }])
 
         self._assert_raises1(record)
         self._assert2(record)
 
@@ -592,15 +574,16 @@
     def test_one_access_with_group(self):
         "Test one access with group"
         pool = Pool()
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -608,15 +591,16 @@
     def test_no_access_with_group(self):
         "Test no access with group"
         pool = Pool()
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: False,
                     }])
 
         self._assert_raises1(record)
         self._assert2(record)
 
@@ -626,20 +610,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': group.id,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -649,20 +635,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: False,
                     }])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': group.id,
                     self._perm: True,
                     }])
 
         self._assert_raises1(record)
         self._assert2(record)
 
@@ -672,20 +660,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': group.id,
                     self._perm: False,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -698,20 +688,22 @@
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         Group.write([self.group], {
                 'parent': group.id,
                 })
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: False,
                     }])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': group.id,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -721,20 +713,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field2.id,
+                    'model': 'test.access',
+                    'field': 'field2',
                     'group': None,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -744,20 +738,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: False,
                     }])
         FieldAccess.create([{
-                    'field': self.field2.id,
+                    'model': 'test.access',
+                    'field': 'field2',
                     'group': None,
                     self._perm: False,
                     }])
 
         self._assert_raises1(record)
         self._assert_raises2(record)
 
@@ -767,20 +763,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': None,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field2.id,
+                    'model': 'test.access',
+                    'field': 'field2',
                     'group': None,
                     self._perm: False,
                     }])
 
         self._assert1(record)
         self._assert_raises2(record)
 
@@ -790,20 +788,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field2.id,
+                    'model': 'test.access',
+                    'field': 'field2',
                     'group': None,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -813,20 +813,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field2.id,
+                    'model': 'test.access',
+                    'field': 'field2',
                     'group': self.group.id,
                     self._perm: True,
                     }])
 
         self._assert1(record)
         self._assert2(record)
 
@@ -836,20 +838,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: False,
                     }])
         FieldAccess.create([{
-                    'field': self.field2.id,
+                    'model': 'test.access',
+                    'field': 'field2',
                     'group': self.group.id,
                     self._perm: False,
                     }])
 
         self._assert_raises1(record)
         self._assert_raises2(record)
 
@@ -859,20 +863,22 @@
         pool = Pool()
         Group = pool.get('res.group')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.access')
         record, = TestAccess.create([{}])
         group, = Group.create([{'name': 'Test'}])
         FieldAccess.create([{
-                    'field': self.field1.id,
+                    'model': 'test.access',
+                    'field': 'field1',
                     'group': self.group.id,
                     self._perm: True,
                     }])
         FieldAccess.create([{
-                    'field': self.field2.id,
+                    'model': 'test.access',
+                    'field': 'field2',
                     'group': None,
                     self._perm: False,
                     }])
 
         self._assert1(record)
         self._assert_raises2(record)
 
@@ -918,44 +924,36 @@
         TestAccess.search([('reference.value', '=', 42, 'test.access.relate')])
 
     @with_transaction(context=_context)
     def test_access_search_relate(self):
         "Test access on search relate"
         pool = Pool()
         TestAccess = pool.get('test.access')
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
-        field, = Field.search([
-                ('model.model', '=', 'test.access.relate'),
-                ('name', '=', 'value'),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': 'test.access.relate',
+                    'field': 'value',
                     'perm_read': True,
                     }])
 
         TestAccess.search([('relate.value', '=', 42)])
         TestAccess.search([('reference.value', '=', 42, 'test.access.relate')])
         TestAccess.search([
                 ('reference.parent.value', '=', 42, 'test.access.relate')])
         TestAccess.search([], order=[('relate.value', 'ASC')])
 
     @with_transaction(context=_context)
     def test_no_access_search_relate(self):
         "Test access on search relate"
         pool = Pool()
         TestAccess = pool.get('test.access')
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
-        field, = Field.search([
-                ('model.model', '=', 'test.access.relate'),
-                ('name', '=', 'value'),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': 'test.access.relate',
+                    'field': 'value',
                     'perm_read': False,
                     }])
 
         with self.assertRaises(AccessError):
             TestAccess.search([('relate.value', '=', 42)])
         with self.assertRaises(AccessError):
             TestAccess.search(
@@ -967,40 +965,32 @@
             TestAccess.search([], order=[('relate.value', 'ASC')])
 
     @with_transaction(context=_context)
     def test_access_search_relate_parent_field(self):
         "Test access on search relate with a parent field"
         pool = Pool()
         TestAccess = pool.get('test.access')
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
-        field, = Field.search([
-                ('model.model', '=', 'test.access.relate'),
-                ('name', '=', 'parent'),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': 'test.access.relate',
+                    'field': 'parent',
                     'perm_read': True,
                     }])
 
         TestAccess.search([('relate', 'child_of', 42, 'parent')])
 
     @with_transaction(context=_context)
     def test_no_access_search_relate_parent_field(self):
         "Test no access on search relate with a parent field"
         pool = Pool()
         TestAccess = pool.get('test.access')
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
-        field, = Field.search([
-                ('model.model', '=', 'test.access.relate'),
-                ('name', '=', 'parent'),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': 'test.access.relate',
+                    'field': 'parent',
                     'perm_read': False,
                     }])
 
         with self.assertRaises(AccessError):
             TestAccess.search([('relate', 'child_of', 42, 'parent')])
 
 
@@ -1045,26 +1035,19 @@
         action = Action(name="Test", res_model='test.access')
         action.save()
         menu = Menu(name="Test", action=action)
         menu.save()
 
         if access is not None:
             ModelAccess.create([{
-                        'model': self.model.id,
+                        'model': 'test.access',
                         'perm_read': access,
                         }])
         return menu
 
-    @property
-    def model(self):
-        pool = Pool()
-        Model = pool.get('ir.model')
-        model, = Model.search([('model', '=', 'test.access')])
-        return model
-
     @with_transaction(context=_context)
     def test_access_empty(self):
         "Search menu without model access"
         pool = Pool()
         Menu = pool.get('ir.ui.menu')
 
         menu = self.create_menu()
```

### Comparing `trytond-7.0.9/trytond/tests/test_backend.py` & `trytond-7.2.0/trytond/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_bus.py` & `trytond-7.2.0/trytond/tests/test_bus.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_cache.py` & `trytond-7.2.0/trytond/tests/test_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     'test.cache.ignored.local', context_ignored_keys={'ignored'})
 cache_ignored_global_context = MemoryCache('test.cache.ignored.global')
 
 
 class CacheTestCase(unittest.TestCase):
     "Test Cache"
 
+    @classmethod
+    def setUpClass(cls):
+        activate_module('tests')
+
     def testFreeze(self):
         "Test freeze"
         self.assertEqual(freeze([1, 2, 3]), (1, 2, 3))
         self.assertEqual(freeze({
                     'list': [1, 2, 3],
                     }),
             frozenset([('list', (1, 2, 3))]))
```

### Comparing `trytond-7.0.9/trytond/tests/test_copy.py` & `trytond-7.2.0/trytond/tests/test_copy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import unittest
+from unittest.mock import patch
 
 from trytond.model import fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool
 from trytond.tests.test_tryton import activate_module, with_transaction
 from trytond.transaction import Transaction
 
@@ -89,14 +90,30 @@
             self.assertEqual(len(one2many.one2many),
                 len(one2many_copy.one2many))
             self.assertNotEqual(one2many.one2many, one2many_copy.one2many)
             self.assertEqual([x.name for x in one2many.one2many],
                 [x.name for x in one2many_copy.one2many])
 
     @with_transaction()
+    def test_one2many_readonly(self):
+        "Test copy one2many readonly"
+        pool = Pool()
+        Model = pool.get('test.copy.one2many')
+        Target = pool.get('test.copy.one2many.target')
+
+        record = Model(name="Test")
+        record.one2many = [Target(name="Target")]
+        record.save()
+
+        with patch.object(Model.one2many, 'readonly', True):
+            copy, = Model.copy([record])
+
+            self.assertEqual(copy.one2many, ())
+
+    @with_transaction()
     def test_one2many_default(self):
         "Test copy one2many with default"
         pool = Pool()
         One2many = pool.get('test.copy.one2many')
         Target = pool.get('test.copy.one2many.target')
 
         record = One2many(name="Test")
@@ -154,14 +171,30 @@
             self.assertEqual(len(many2many.many2many),
                 len(many2many_copy.many2many))
             self.assertEqual(many2many.many2many, many2many_copy.many2many)
             self.assertEqual([x.name for x in many2many.many2many],
                 [x.name for x in many2many_copy.many2many])
 
     @with_transaction()
+    def test_many2many_readonly(self):
+        "test copy many2many readonly"
+        pool = Pool()
+        Model = pool.get('test.copy.many2many')
+        Target = pool.get('test.copy.many2many.target')
+
+        record = Model(name="Test")
+        record.many2many = [Target(name="Target")]
+        record.save()
+
+        with patch.object(Model.many2many, 'readonly', True):
+            copy, = Model.copy([record])
+
+            self.assertEqual(copy.many2many, ())
+
+    @with_transaction()
     def test_many2many_default(self):
         "Test copy many2many with default"
         pool = Pool()
         Many2many = pool.get('test.copy.many2many')
         Target = pool.get('test.copy.many2many.target')
 
         record = Many2many(name="Test")
@@ -199,99 +232,83 @@
         self.assertEqual(record_copy.file_id, record.file_id)
         self.assertEqual(record_copy.binary_id, record.binary_id)
 
     @with_transaction(context={'_check_access': True})
     def test_no_acccess_copy_with_custom_value(self):
         "Test copying field with no access and custom value"
         pool = Pool()
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.copy.access')
 
         record, = TestAccess.create([{'name': 'foo'}])
 
-        field, = Field.search([
-                ('model.model', '=', 'test.copy.access'),
-                ('name', '=', 'name'),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': 'test.copy.access',
+                    'field': 'name',
                     'group': None,
                     'perm_read': True,
                     'perm_write': False,
                     }])
 
         with self.assertRaises(AccessError):
             new_record, = TestAccess.copy([record])
 
     @with_transaction(context={'_check_access': True})
     def test_no_acccess_copy_with_default(self):
         "Test copying field with no access but default value"
         pool = Pool()
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.copy.access')
 
-        field, = Field.search([
-                ('model.model', '=', 'test.copy.access'),
-                ('name', '=', 'name'),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': 'test.copy.access',
+                    'field': 'name',
                     'group': None,
                     'perm_read': True,
                     'perm_write': False,
                     }])
 
         record, = TestAccess.create([{}])
         self.assertEqual(record.name, "Default")
         new_record, = TestAccess.copy([record])
         self.assertEqual(new_record.name, "Default")
 
     @with_transaction(context={'_check_access': True})
     def test_no_acccess_copy_with_defaults(self):
         "Test copying field with no access and defaults"
         pool = Pool()
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.copy.access')
 
         record, = TestAccess.create([{}])
 
-        field, = Field.search([
-                ('model.model', '=', 'test.copy.access'),
-                ('name', '=', 'name'),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': 'test.copy.access',
+                    'field': 'name',
                     'group': None,
                     'perm_read': True,
                     'perm_write': False,
                     }])
 
         with self.assertRaises(AccessError):
             new_record, = TestAccess.copy(
                 [record], default={'name': 'nondefault'})
 
     @with_transaction(context={'_check_access': True})
     def test_copy_with_no_read_access(self):
         "Test copying field with no read access"
         pool = Pool()
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
         TestAccess = pool.get('test.copy.access')
 
         record, = TestAccess.create([{}])
 
-        field, = Field.search([
-                ('model.model', '=', 'test.copy.access'),
-                ('name', '=', 'name'),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': 'test.copy.access',
+                    'field': 'name',
                     'group': None,
                     'perm_read': False,
                     'perm_write': False,
                     }])
 
         new_record, = TestAccess.copy([record])
         self.assertNotEqual(new_record.id, record.id)
```

### Comparing `trytond-7.0.9/trytond/tests/test_exportdata.py` & `trytond-7.2.0/trytond/tests/test_exportdata.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_binary.py` & `trytond-7.2.0/trytond/tests/test_field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_boolean.py` & `trytond-7.2.0/trytond/tests/test_field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_char.py` & `trytond-7.2.0/trytond/tests/test_field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_context.py` & `trytond-7.2.0/trytond/tests/test_field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_date.py` & `trytond-7.2.0/trytond/tests/test_field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_datetime.py` & `trytond-7.2.0/trytond/tests/test_field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_depends.py` & `trytond-7.2.0/trytond/tests/test_field_depends.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_dict.py` & `trytond-7.2.0/trytond/tests/test_field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_float.py` & `trytond-7.2.0/trytond/tests/test_field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_function.py` & `trytond-7.2.0/trytond/tests/test_field_function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_integer.py` & `trytond-7.2.0/trytond/tests/test_field_integer.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     def test_create_with_domain_invalid(self):
         "Test create integer with domain invalid"
         Integer = Pool().get('test.integer_domain')
 
         with self.assertRaisesRegex(
                 DomainValidationError,
                 'The value "10" for field "Integer" '
-                'in ".*" of "Integer Domain"'):
+                'in record ".*" of "Integer Domain"'):
             Integer.create([{
                         'integer': 10,
                         }])
 
     @with_transaction()
     def test_search_equals(self):
         "Test search integer equals"
```

### Comparing `trytond-7.0.9/trytond/tests/test_field_many2many.py` & `trytond-7.2.0/trytond/tests/test_field_many2many.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,15 @@
         "Test create many2many with invalid domain"
         pool = Pool()
         Many2Many = pool.get('test.many2many_domain')
 
         with self.assertRaisesRegex(
                 DomainValidationError,
                 'The value ".*,.*" for field "Targets" '
-                'in ".*" of "Many2Many Domain"'):
+                'in record ".*" of "Many2Many Domain"'):
             Many2Many.create([{
                         'targets': [
                             ('create', [{'value': 10}, {'value': None}]),
                             ],
                         }])
 
     @with_transaction()
```

### Comparing `trytond-7.0.9/trytond/tests/test_field_many2one.py` & `trytond-7.2.0/trytond/tests/test_field_many2one.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         Target = pool.get('test.many2one_target')
         Many2One = pool.get('test.many2one_domainvalidation')
         target, = Target.create([{'value': 1}])
 
         with self.assertRaisesRegex(
                 DomainValidationError,
                 'The value "%s" for field "many2one" '
-                'in ".*" of "Many2One Domain Validation"' % target.rec_name):
+                'in record ".*" of "Many2One Domain Validation"' %
+                target.rec_name):
             Many2One.create([{
                         'many2one': target.id,
                         }])
 
     @with_transaction()
     def test_create_with_domain_inactive(self):
         "Test create many2one with domain and inactive target"
```

### Comparing `trytond-7.0.9/trytond/tests/test_field_multiselection.py` & `trytond-7.2.0/trytond/tests/test_field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_numeric.py` & `trytond-7.2.0/trytond/tests/test_field_numeric.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,24 @@
         with self.assertRaises(DigitsValidationError):
             Numeric.create([{
                         'digits': 10,
                         'numeric': Decimal('1.11111111111'),
                         }])
 
     @with_transaction()
+    def test_create_huge_digits_valid(self):
+        "Test create a huge number with valid digits"
+        Numeric = Pool().get('test.numeric_digits')
+
+        Numeric.create([{
+                    'digits': 2,
+                    'numeric': Decimal('10e25'),
+                    }])
+
+    @with_transaction()
     def test_create_trailing_zero_digits_invalid(self):
         "Test create numeric with invalid trailing zero digits"
         Numeric = Pool().get('test.numeric_digits')
 
         with self.assertRaises(DigitsValidationError):
             Numeric.create([{
                     'digits': 1,
```

### Comparing `trytond-7.0.9/trytond/tests/test_field_one2many.py` & `trytond-7.2.0/trytond/tests/test_field_one2many.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,15 +571,15 @@
         "Test create one2many with invalid domain"
         pool = Pool()
         One2Many = pool.get('test.one2many_domain')
 
         with self.assertRaisesRegex(
                 DomainValidationError,
                 'The value ".*,.*" for field "Targets" '
-                'in ".*" of "One2Many Domain"'):
+                'in record ".*" of "One2Many Domain"'):
             One2Many.create([{
                         'targets': [
                             ('create', [{'value': 10}, {'value': None}]),
                             ],
                         }])
 
     @with_transaction()
```

### Comparing `trytond-7.0.9/trytond/tests/test_field_one2one.py` & `trytond-7.2.0/trytond/tests/test_field_one2one.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         target, = Target.create([{
                     'name': "invalid domain",
                     }])
 
         with self.assertRaisesRegex(
                 DomainValidationError,
                 'The value "%s" for field "One2One" '
-                'in ".*" of "One2One"' % target.rec_name):
+                'in record ".*" of "One2One"' % target.rec_name):
             One2One.create([{
                         'one2one': target.id,
                         }])
 
     @with_transaction()
     def test_search_equals(self):
         "Test search one2one equals"
```

### Comparing `trytond-7.0.9/trytond/tests/test_field_reference.py` & `trytond-7.2.0/trytond/tests/test_field_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -481,15 +481,16 @@
         target = Target(value=1)
         target.save()
 
         reference = Reference(reference=target)
         with self.assertRaisesRegex(
                 DomainValidationError,
                 'The value "%s" for field "Reference" '
-                'in ".*" of "Reference Domain Validation"' % target.rec_name):
+                'in record ".*" of "Reference Domain Validation"' %
+                target.rec_name):
             reference.save()
 
     @with_transaction()
     def test_no_domain(self):
         "Test reference with no domain"
         pool = Pool()
         Reference = pool.get('test.reference_domainvalidation')
```

### Comparing `trytond-7.0.9/trytond/tests/test_field_selection.py` & `trytond-7.2.0/trytond/tests/test_field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_text.py` & `trytond-7.2.0/trytond/tests/test_field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_time.py` & `trytond-7.2.0/trytond/tests/test_field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_field_timedelta.py` & `trytond-7.2.0/trytond/tests/test_field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_filestore.py` & `trytond-7.2.0/trytond/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_history.py` & `trytond-7.2.0/trytond/tests/test_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 import unittest
+from unittest.mock import patch
 
 from trytond import backend
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool
 from trytond.tests.test_tryton import activate_module, with_transaction
 from trytond.transaction import Transaction
 
@@ -246,14 +247,70 @@
         transaction.commit()
 
         History.restore_history([history_id], first)
         history = History(history_id)
         self.assertEqual(history.value, 2)
 
     @with_transaction()
+    def test_search_historical_records_no_window_functions(self):
+        database = Transaction().database
+        with patch.object(database, 'has_window_functions') as has_wf:
+            has_wf.return_value = False
+            self._test_search_historical_records()
+
+    @with_transaction()
+    def test_search_historical_records(self):
+        self._test_search_historical_records()
+
+    def _test_search_historical_records(self):
+        pool = Pool()
+        History = pool.get('test.history')
+        transaction = Transaction()
+
+        first = History(value=1)
+        first.save()
+        first_stamp = first.create_date
+        # Commit so that further call are at a different timestamp
+        transaction.commit()
+
+        second = History(value=1)
+        first.value = 2
+        History.save([first, second])
+        second_stamp = second.create_date
+        transaction.commit()
+
+        third = History(value=1)
+        second.value = 2
+        History.delete([first])
+        History.save([second, third])
+        third_stamp = third.create_date
+        transaction.commit()
+
+        third.value = 2
+        History.delete([second])
+        third.save()
+        transaction.commit()
+
+        for test_name, timestamp, expected_1, expected_2 in [
+                ('min', datetime.datetime.min, [], []),
+                ('first', first_stamp, [first], []),
+                ('second', second_stamp, [second], [first]),
+                ('third', third_stamp, [third], [second]),
+                ('max', datetime.datetime.max, [], [third]),
+                ('no history', None, [], [third]),
+                ]:
+            with Transaction().set_context(_datetime=timestamp):
+                with self.subTest(f"{test_name} ('value', '=', 1)"):
+                    records = History.search([('value', '=', 1)])
+                    self.assertEqual(records, expected_1)
+                with self.subTest(f"{test_name} ('value', '=', 2)"):
+                    records = History.search([('value', '=', 2)])
+                    self.assertEqual(records, expected_2)
+
+    @with_transaction()
     def test_ordered_search(self):
         'Test ordered search of history models'
         pool = Pool()
         History = pool.get('test.history')
         transaction = Transaction()
         order = [('value', 'ASC')]
```

### Comparing `trytond-7.0.9/trytond/tests/test_i18n.py` & `trytond-7.2.0/trytond/tests/test_i18n.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import unittest
+from unittest.mock import patch
 
 from trytond.i18n import gettext, lazy_gettext
 from trytond.pool import Pool
 from trytond.tests.test_tryton import activate_module, with_transaction
 from trytond.tools.string_ import LazyString
 
 
@@ -78,30 +79,24 @@
         message = gettext('tests.msg_test', lang.code)
 
         self.assertEqual(message, 'Message')
 
     @with_transaction()
     def test_gettest_wrong_id_format(self):
         "gettext returns the id if it has wrong format"
-        Pool().test = False
-        try:
+        with patch('trytond.pool.Pool.test', False):
             message = gettext("Wrong Format")
-        finally:
-            Pool().test = True
 
         self.assertEqual(message, "Wrong Format")
 
     @with_transaction()
     def test_gettext_wrong_id(self):
         "gettext returns the id if it does not exist"
-        Pool().test = False
-        try:
+        with patch('trytond.pool.Pool.test', False):
             message = gettext('tests.not_exist')
-        finally:
-            Pool().test = True
 
         self.assertEqual(message, 'tests.not_exist')
 
     def test_gettext_without_transaction(self):
         "gettext return the id if there is no transaction"
         message = gettext('test.msg_test')
```

### Comparing `trytond-7.0.9/trytond/tests/test_importdata.py` & `trytond-7.2.0/trytond/tests/test_importdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -565,24 +565,61 @@
         count = Char.import_data(['id', 'name'], [[record.rec_name, "bar"]])
 
         record, = Char.search([])
         self.assertEqual(count, 1)
         self.assertEqual(record.name, "bar")
 
     @with_transaction()
+    def test_update_many2many(self):
+        "Test update many2many"
+        pool = Pool()
+        Many2many = pool.get('test.import_data.many2many')
+        Target = pool.get('test.import_data.many2many.target')
+
+        record = Many2many(many2many=[{'name': "Foo"}])
+        record.save()
+        target = Target(name="Bar")
+        target.save()
+
+        count = Many2many.import_data(
+            ['id', 'many2many'],
+            [[record.id, "Bar"]])
+
+        self.assertEqual(count, 1)
+        self.assertEqual([m.name for m in record.many2many], ["Bar"])
+
+    @with_transaction()
+    def test_update_many2many_id(self):
+        "Test update many2many with id"
+        pool = Pool()
+        Many2many = pool.get('test.import_data.many2many')
+
+        record = Many2many(many2many=[{'name': "Foo"}])
+        record.save()
+
+        count = Many2many.import_data(
+            ['id', 'many2many:id'],
+            [[record.id, 'tests.import_data_many2many_target_test1']])
+
+        self.assertEqual(count, 1)
+        self.assertEqual([m.name for m in record.many2many], ["Test 1"])
+
+    @with_transaction()
     def test_update_one2many(self):
         "Test update one2many"
         pool = Pool()
         One2many = pool.get('test.import_data.one2many')
         Target = pool.get('test.import_data.one2many.target')
-        record = One2many(name="test", one2many=[Target(name="foo")])
+        record = One2many(name="test", one2many=[
+                Target(name="foo"), Target(name="test")])
         record.save()
-        target, = record.one2many
+        target, _ = record.one2many
 
         count = One2many.import_data(
             ['id', 'one2many/id', 'one2many/name'],
             [[record.id, target.id, "bar"],
                 ['', '', "baz"]])
 
         self.assertEqual(count, 1)
         self.assertEqual(len(record.one2many), 2)
         self.assertEqual([t.name for t in record.one2many], ["bar", "baz"])
+        self.assertFalse(Target.search([('name', '=', "test")]))
```

### Comparing `trytond-7.0.9/trytond/tests/test_ir.py` & `trytond-7.2.0/trytond/tests/test_ir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
+import shutil
 import unittest
 from decimal import Decimal
 from unittest.mock import ANY, Mock, patch
 
 try:
     import zoneinfo
 except ImportError:
     zoneinfo = None
+try:
+    import pydot
+except ImportError:
+    pydot = None
 
 from dateutil.relativedelta import relativedelta
 
-from trytond.config import config
 from trytond.ir.exceptions import SequenceAffixError
 from trytond.ir.lang import _replace
 from trytond.pool import Pool
 from trytond.pyson import Eval, If, PYSONEncoder
 from trytond.tools import timezone
 from trytond.transaction import Transaction
 
@@ -57,42 +61,42 @@
     def test_model_field_search_description(self):
         "Test searching on description of model field"
         pool = Pool()
         ModelField = pool.get('ir.model.field')
 
         field, = ModelField.search([
                 ('field_description', '=', "Name"),
-                ('model.model', '=', 'ir.lang'),
+                ('model', '=', 'ir.lang'),
                 ('module', '=', 'ir'),
                 ])
         self.assertEqual(field.field_description, "Name")
 
     @with_transaction()
     def test_model_field_search_order_description(self):
         "Test searching and ordering on description of model field"
         pool = Pool()
         ModelField = pool.get('ir.model.field')
 
         fields = ModelField.search([
                 ('field_description', 'in', ["Name", "Code"]),
-                ('model.model', '=', 'ir.lang'),
+                ('model', '=', 'ir.lang'),
                 ('module', '=', 'ir'),
                 ])
         self.assertEqual(
             [f.field_description for f in fields], ["Code", "Name"])
 
     @with_transaction()
     def test_model_field_lazy(self):
         "Test searching on lazy string of model field"
         pool = Pool()
         ModelField = pool.get('ir.model.field')
 
         field, = ModelField.search([
                 ('field_description', '=', "ID"),
-                ('model.model', '=', 'ir.lang'),
+                ('model', '=', 'ir.lang'),
                 ('module', '=', 'ir'),
                 ])
         self.assertEqual(field.field_description, "ID")
 
     @with_transaction()
     def test_sequence_substitutions(self):
         'Test Sequence Substitutions'
@@ -330,15 +334,17 @@
             model='res.user',
             report_name='tests.email_send',
             report_content=b'report',
             template_extension='txt',
             )
         report.save()
 
-        with patch('trytond.ir.email_.sendmail_transactional') as sendmail:
+        with patch(
+                'trytond.ir.email_.send_message_transactional'
+                ) as send_message:
             email = Email.send(
                 to='"John Doe" <john@example.com>, Jane <jane@example.com>',
                 cc='User <user@example.com>',
                 bcc='me@example.com',
                 subject="Email subject",
                 body='<p>Hello</p>',
                 files=[('file.txt', b'data')],
@@ -350,19 +356,18 @@
                     ])
 
         addresses = [
             'john@example.com',
             'jane@example.com',
             'user@example.com',
             'me@example.com']
-        sendmail.assert_called_once_with(
-            config.get('email', 'from'), addresses, ANY, strict=True)
+        send_message.assert_called_once_with(ANY, strict=True)
         self.assertEqual(
             email.recipients,
-            '"John Doe" <john@example.com>, Jane <jane@example.com>')
+            'John Doe <john@example.com>, Jane <jane@example.com>')
         self.assertEqual(email.recipients_secondary, 'User <user@example.com>')
         self.assertEqual(email.recipients_hidden, 'me@example.com')
         self.assertEqual(
             [a.address for a in email.addresses],
             addresses)
         self.assertEqual(email.subject, "Email subject")
         self.assertEqual(email.body, '<p>Hello</p>')
@@ -383,15 +388,15 @@
         User = pool.get('res.user')
 
         admin = User(1)
         admin.email = 'admin@example.com'
         admin.save()
         model, = IrModel.search([('model', '=', 'res.user')])
         field, = IrModelField.search([
-                ('model', '=', model.id),
+                ('model', '=', 'res.user'),
                 ('name', '=', 'id'),
                 ])
 
         template = Template(
             model=model,
             name="Test",
             recipients=field,
@@ -418,15 +423,15 @@
         User = pool.get('res.user')
 
         admin = User(1)
         admin.email = 'admin@example.com'
         admin.save()
         model, = IrModel.search([('model', '=', 'res.user')])
         field, = IrModelField.search([
-                ('model', '=', model.id),
+                ('model', '=', 'res.user'),
                 ('name', '=', 'id'),
                 ])
 
         values = Template.get_default(User.__name__, admin.id)
 
         self.assertEqual(
             values, {
@@ -444,15 +449,15 @@
         User = pool.get('res.user')
 
         admin = User(1)
         admin.email = 'admin@example.com'
         admin.save()
         model, = IrModel.search([('model', '=', 'res.user')])
         field, = IrModelField.search([
-                ('model', '=', model.id),
+                ('model', '=', 'res.user'),
                 ('name', '=', 'id'),
                 ])
 
         template = Template(
             model=model,
             name="Test",
             recipients_pyson=PYSONEncoder().encode(
@@ -547,9 +552,27 @@
     @with_transaction()
     def test_get_timezone(self):
         "Test get_timezone"
         cron = self._get_cron()
 
         self.assertIsInstance(cron.get_timezone('timezone'), str)
 
+    @unittest.skipUnless(
+            pydot and shutil.which('dot'), "pydot is needed to generate graph")
+    @with_transaction()
+    def test_workflow_graph(self):
+        "Test workflow graph"
+        pool = Pool()
+        Model = pool.get('ir.model')
+        ModelWorkflowGraph = pool.get('ir.model.workflow_graph', type='report')
+
+        model, = Model.search([('model', '=', 'ir.error')])
+
+        oext, content, print_, filename = (
+                ModelWorkflowGraph.execute([model.id], {}))
+        self.assertEqual(oext, 'png')
+        self.assertTrue(content)
+        self.assertFalse(print_)
+        self.assertEqual(filename, "Workflow Graph")
+
 
 del ModuleTestCase
```

### Comparing `trytond-7.0.9/trytond/tests/test_mixins.py` & `trytond-7.2.0/trytond/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_model.py` & `trytond-7.2.0/trytond/tests/test_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -201,14 +201,42 @@
 
         self.assertEqual(
             names, {
                 'model': "Model", 'field': "Name",
                 'record': record.id, 'value': "Test"})
 
     @with_transaction()
+    def test_names_value_selection(self):
+        "test __names__ with selection value"
+        pool = Pool()
+        Model = pool.get('test.model')
+
+        record = Model(selection='foo')
+        names = Model.__names__(field='selection', record=record)
+
+        self.assertEqual(
+            names, {
+                'model': "Model", 'field': "Selection",
+                'record': record.id, 'value': "Foo"})
+
+    @with_transaction()
+    def test_names_value_multiselection(self):
+        "test __names__ with multiselection value"
+        pool = Pool()
+        Model = pool.get('test.model')
+
+        record = Model(multiselection=['foo', 'bar'])
+        names = Model.__names__(field='multiselection', record=record)
+
+        self.assertEqual(
+            names, {
+                'model': "Model", 'field': "MultiSelection",
+                'record': record.id, 'value': "Foo, Bar"})
+
+    @with_transaction()
     def test_names_value_list(self):
         "Test __names__ with value as list"
         pool = Pool()
         Model = pool.get('test.model_parent')
         Child = pool.get('test.model_child')
 
         record = Model(
@@ -236,23 +264,19 @@
                 'record': record.id, 'value': 'None'})
 
     @with_transaction()
     def test_fields_get_no_write_access(self):
         "Test field is readonly when no write access on it"
         pool = Pool()
         Model = pool.get('test.model')
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
 
-        field, = Field.search([
-                ('name', '=', 'name'),
-                ('model.model', '=', Model.__name__),
-                ])
         FieldAccess.create([{
-                    'field': field.id,
+                    'model': Model.__name__,
+                    'field': 'name',
                     'perm_write': False,
                     }])
 
         definition = Model.fields_get(['name'])
 
         self.assertTrue(definition['name']['readonly'])
```

### Comparing `trytond-7.0.9/trytond/tests/test_model_index.py` & `trytond-7.2.0/trytond/tests/test_model_index.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_model_log.py` & `trytond-7.2.0/trytond/tests/test_model_log.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_model_match.py` & `trytond-7.2.0/trytond/tests/test_model_match.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_modelsingleton.py` & `trytond-7.2.0/trytond/tests/test_modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_modelsql.py` & `trytond-7.2.0/trytond/tests/test_modelsql.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,80 @@
                             'parent.': {
                                 'id': record.id,
                                 'name': "Record",
                                 },
                             }],
                     }])
 
+    @with_transaction()
+    def test_read_limit(self):
+        "Test that we limit the number or related records read"
+        pool = Pool()
+        Model = pool.get('test.modelsql.read')
+
+        model, = Model.create([{
+                    'name': 'Record',
+                    'targets': [
+                        ('create', [{'name': str(i)} for i in range(10)]),
+                        ]
+                    }])
+
+        values, = Model.read([model.id], ['targets.name'])
+        self.assertTrue(all('id' in t and 'name' in t
+                for t in values['targets.']))
+
+        with Transaction().set_context(related_read_limit=4):
+            values, = Model.read([model.id], ['targets.name'])
+            self.assertTrue(all('id' in t and 'name' in t
+                    for t in values['targets.'][:4]))
+            self.assertTrue(all('id' in t and len(t) == 1
+                    for t in values['targets.'][4:]))
+
+    @with_transaction()
+    def test_read_limit_only_limit_related(self):
+        "Test that we don't limit reading records with related_read_limit"
+        pool = Pool()
+        Model = pool.get('test.modelsql.read')
+
+        records = Model.create([
+                {
+                    'name': f'Record {i}',
+                    'targets': [
+                        ('create', [{'name': str(i)} for i in range(10)]),
+                        ]
+                    } for i in range(10)])
+        with Transaction().set_context(related_read_limit=4):
+            values = Model.read(
+                [r.id for r in records], ['name', 'targets.name'])
+            self.assertTrue(all('id' in v and 'name' in v for v in values))
+            self.assertTrue(all(len(v['targets.']) == 10 for v in values))
+
+    @with_transaction()
+    def test_read_limit_caching(self):
+        "Test that limiting the related records read plays nice with caching"
+        pool = Pool()
+        Model = pool.get('test.modelsql.read.limit')
+
+        records = Model.create([
+                {
+                    'name': f'Record {i}',
+                    'targets': [
+                        ('create', [{'name': str(j), 'integer': j}
+                                for j in range(1, i + 1)]),
+                        ],
+                    } for i in range(10)])
+
+        with Transaction().set_context(read_limit=4):
+            values = Model.read(
+                [r.id for r in records],
+                ['name', 'targets.name', 'sum_targets'])
+            computed = {r['name']: r['sum_targets'] for r in values}
+            expected = {f'Record {i}': i * (i + 1) // 2 for i in range(10)}
+            self.assertEqual(computed, expected)
+
     @unittest.skipIf(backend.name == 'sqlite',
         'SQLite not concerned because tryton don\'t set "NOT NULL"'
         'constraint: "ALTER TABLE" don\'t support NOT NULL constraint'
         'without default value')
     @with_transaction()
     def test_required_field_missing(self):
         'Test error message when a required field is missing'
```

### Comparing `trytond-7.0.9/trytond/tests/test_modelstorage.py` & `trytond-7.2.0/trytond/tests/test_modelstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -830,40 +830,36 @@
         self.assertEqual(env.get('_parent_many2one').get('char'), "Test")
 
     @with_transaction()
     def test_model_save_skip_check_access(self):
         "Test model save skips check access"
         pool = Pool()
         Model = pool.get('test.modelstorage')
-        IrModel = pool.get('ir.model')
         IrModelAccess = pool.get('ir.model.access')
 
-        model, = IrModel.search([('model', '=', Model.__name__)])
         IrModelAccess.create([{
-                    'model': model.id,
+                    'model': Model.__name__,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     }])
         with check_access():
             record = Model(name="Test")
             record.save()
 
     @with_transaction()
     def test_model_getattr_skip_check_access(self):
         "Test model getattr skips check access"
         pool = Pool()
         Model = pool.get('test.modelstorage')
-        IrModel = pool.get('ir.model')
         IrModelAccess = pool.get('ir.model.access')
 
-        model, = IrModel.search([('model', '=', Model.__name__)])
         IrModelAccess.create([{
-                    'model': model.id,
+                    'model': Model.__name__,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     }])
         record, = Model.create([{'name': "Test"}])
```

### Comparing `trytond-7.0.9/trytond/tests/test_modelview.py` & `trytond-7.2.0/trytond/tests/test_modelview.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,191 @@
 import unittest
 from unittest.mock import patch
 
 from lxml import etree
 
 from trytond.model.exceptions import (
     AccessButtonError, AccessError, ButtonActionException)
+from trytond.model.modelview import set_visible
 from trytond.pool import Pool
 from trytond.pyson import Eval, PYSONDecoder, PYSONEncoder
 from trytond.tests.test_tryton import activate_module, with_transaction
 
 
 class ModelView(unittest.TestCase):
     "Test ModelView"
 
     @classmethod
     def setUpClass(cls):
         activate_module('tests')
 
+    def test_set_visible(self):
+        "Test loading of visible x2m fields in group"
+
+        GROUP_XML = """
+        <form>
+            <group>
+                <field name="OK"/>
+            </group>
+            <group expandable="1">
+                <field name="OK"/>
+                <group expandable="0">
+                    <field name="KO"/>
+                </group>
+            </group>
+            <group expandable="0">
+                <field name="KO"/>
+                <group>
+                    <field name="KO"/>
+                </group>
+            </group>
+            <group>
+                <group>
+                    <field name="OK"/>
+                </group>
+                <group expandable="1">
+                    <field name="OK"/>
+                </group>
+                <group expandable="0">
+                    <field name="KO"/>
+                </group>
+            </group>
+         </form>
+        """
+        group_tree = etree.fromstring(GROUP_XML)
+        set_visible(group_tree, {'OK', 'KO'})
+        self.assertEqual(
+            ['OK', 'OK', 'OK', 'OK'],
+            [n.attrib['name']
+                for n in group_tree.xpath("//field[@loading='eager']")])
+
+    def test_mark_visible_x2m_notebook(self):
+        "Test marking visible x2m fields in notebook"
+
+        NOTEBOOK_XML = """
+        <form>
+            <notebook>
+                <page>
+                    <field name="OK"/>
+                    <field name="OK"/>
+                    <notebook>
+                        <page>
+                            <field name="OK"/>
+                            <notebook>
+                                <page>
+                                    <field name="OK"/>
+                                    <field name="OK"/>
+                                </page>
+                                <page>
+                                    <field name="KO"/>
+                                </page>
+                            </notebook>
+                        </page>
+                        <page>
+                            <field name="KO"/>
+                        </page>
+                    </notebook>
+                </page>
+                <page>
+                    <field name="KO"/>
+                    <notebook>
+                        <page>
+                            <field name="KO"/>
+                        </page>
+                        <page>
+                            <field name="KO"/>
+                        </page>
+                    </notebook>
+                </page>
+            </notebook>
+         </form>
+        """
+        nb_tree = etree.fromstring(NOTEBOOK_XML)
+        set_visible(nb_tree, {'OK', 'KO'})
+        self.assertEqual(
+            ['OK', 'OK', 'OK', 'OK', 'OK'],
+            [n.attrib['name']
+                for n in nb_tree.xpath("//field[@loading='eager']")])
+
+    def test_mark_visible_x2m_notebook_group(self):
+        "Test marking visible x2m fields in notebook and groups"
+
+        NBGROUP_XML = """
+        <form>
+            <notebook>
+                <page>
+                    <group>
+                        <field name="OK"/>
+                    </group>
+                    <group expandable="0">
+                        <field name="KO"/>
+                    </group>
+                    <group expandable="1">
+                        <field name="OK"/>
+                    </group>
+                </page>
+                <page>
+                    <group>
+                        <field name="KO"/>
+                    </group>
+                    <group expandable="0">
+                        <field name="KO"/>
+                    </group>
+                    <group expandable="1">
+                        <field name="KO"/>
+                    </group>
+                </page>
+            </notebook>
+            <group expandable="0">
+                <notebook>
+                    <page>
+                        <field name="KO"/>
+                    </page>
+                    <page>
+                        <field name="KO"/>
+                    </page>
+                </notebook>
+            </group>
+            <group expandable="1">
+                <notebook>
+                    <page>
+                        <field name="OK"/>
+                    </page>
+                    <page>
+                        <field name="KO"/>
+                    </page>
+                </notebook>
+            </group>
+            <group>
+                <notebook>
+                    <page>
+                        <field name="OK"/>
+                    </page>
+                    <page>
+                        <field name="KO"/>
+                    </page>
+                </notebook>
+            </group>
+         </form>
+        """
+        ng_tree = etree.fromstring(NBGROUP_XML)
+        set_visible(ng_tree, {'OK', 'KO'})
+        self.assertEqual(
+            ['OK', 'OK', 'OK', 'OK'],
+            [n.attrib['name']
+                for n in ng_tree.xpath("//field[@loading='eager']")])
+
     @with_transaction()
     def test_changed_values(self):
         "Test ModelView._changed_values"
         pool = Pool()
         Model = pool.get('test.modelview.changed_values')
         Target = pool.get('test.modelview.changed_values.target')
 
-        record = Model()
+        record = Model(targets=[], m2m_targets=[], m2m_function=[])
 
         self.assertEqual(record._changed_values, {})
 
         record.name = 'foo'
         record.target = Target(1)
         record.ref_target = Target(2)
         record.targets = [Target(name='bar')]
@@ -94,15 +251,15 @@
         self.assertEqual(record._changed_values, {
                 'targets': {
                     'update': [{'id': 1, 'name': 'bar'}],
                     },
                 })
 
         # no initial value
-        record = Model()
+        record = Model(targets=[], m2m_targets=[], m2m_function=[])
         record._values = record._record()
         target = Target(id=1)
         record._values['targets'] = [target]
         target.name = 'foo'
         self.assertEqual(record._changed_values, {
                 'targets': {
                     'add': [(0, {'id': 1, 'name': 'foo'})],
@@ -204,15 +361,15 @@
     @with_transaction()
     def test_changed_values_reverse_field(self):
         "Test _changed_values with reverse field set"
         pool = Pool()
         Model = pool.get('test.modelview.changed_values')
         Target = pool.get('test.modelview.changed_values.target')
 
-        record = Model(id=1)
+        record = Model(id=1, targets=[], m2m_targets=[], m2m_function=[])
         record.name = "Record"
         target = Target()
         target.name = "Target"
         record.targets = [target]
 
         self.assertEqual(record._changed_values, {
                 'name': "Record",
@@ -222,31 +379,30 @@
                 })
 
     @with_transaction(context={'_check_access': True})
     def test_button_access(self):
         'Test Button Access'
         pool = Pool()
         TestModel = pool.get('test.modelview.button')
-        Model = pool.get('ir.model')
         Button = pool.get('ir.model.button')
         ModelAccess = pool.get('ir.model.access')
         Group = pool.get('res.group')
 
-        model, = Model.search([('model', '=', 'test.modelview.button')])
         admin, = Group.search([('name', '=', 'Administration')])
         test = TestModel()
 
-        button = Button(name='test', model=model)
+        button = Button(model=TestModel.__name__, name='test')
         button.save()
 
         # Without model/button access
         TestModel.test([test])
 
         # Without read access
-        access = ModelAccess(model=model, group=None, perm_read=False)
+        access = ModelAccess(
+            model=TestModel.__name__, group=None, perm_read=False)
         access.save()
         with self.assertRaises(AccessError):
             TestModel.test([test])
 
         # Without write access
         access.perm_read = True
         access.perm_write = False
@@ -286,22 +442,20 @@
         self.assertEqual(len(clicks), 0)
 
     @with_transaction(context={'_check_access': True})
     def test_button_rule_not_passed(self):
         "Test not passed Button Rule"
         pool = Pool()
         TestModel = pool.get('test.modelview.button')
-        Model = pool.get('ir.model')
         Button = pool.get('ir.model.button')
         ButtonRule = pool.get('ir.model.button.rule')
         ButtonClick = pool.get('ir.model.button.click')
 
-        model, = Model.search([('model', '=', 'test.modelview.button')])
         rule = ButtonRule(number_user=2)
-        button = Button(name='test', model=model, rules=[rule])
+        button = Button(model=TestModel.__name__, name='test', rules=[rule])
         button.save()
 
         record = TestModel(id=-1)
         with patch.object(TestModel, 'test_non_decorated') as button_func:
             TestModel.test([record])
             button_func.assert_called_with([])
 
@@ -314,22 +468,20 @@
         self.assertEqual(click.user.id, 1)
 
     @with_transaction(context={'_check_access': True})
     def test_button_rule_passed(self):
         "Test passed Button Rule"
         pool = Pool()
         TestModel = pool.get('test.modelview.button')
-        Model = pool.get('ir.model')
         Button = pool.get('ir.model.button')
         ButtonRule = pool.get('ir.model.button.rule')
         ButtonClick = pool.get('ir.model.button.click')
 
-        model, = Model.search([('model', '=', 'test.modelview.button')])
         rule = ButtonRule(number_user=1)
-        button = Button(name='test', model=model, rules=[rule])
+        button = Button(model=TestModel.__name__, name='test', rules=[rule])
         button.save()
 
         record = TestModel(id=-1)
         with patch.object(TestModel, 'test_non_decorated') as button_func:
             TestModel.test([record])
             button_func.assert_called_with([record])
 
@@ -471,19 +623,18 @@
         self.assertIsInstance(int(link.attrib['id']), int)
 
     @with_transaction()
     def test_link_without_read_access(self):
         "Test link in view without read access"
         pool = Pool()
         TestModel = pool.get('test.modelview.link')
-        Model = pool.get('ir.model')
         ModelAccess = pool.get('ir.model.access')
 
-        model, = Model.search([('model', '=', 'test.modelview.link.target')])
-        access = ModelAccess(model=model, group=None, perm_read=False)
+        access = ModelAccess(
+            model='test.modelview.link.target', group=None, perm_read=False)
         access.save()
 
         arch = TestModel.fields_view_get()['arch']
         parser = etree.XMLParser()
         tree = etree.fromstring(arch, parser=parser)
         links = tree.xpath('//link')
         labels = tree.xpath('//label')
@@ -493,20 +644,19 @@
 
     @unittest.skipUnless(hasattr(etree, 'RelaxNG'), "etree is missing RelaxNG")
     @with_transaction()
     def test_link_label_valid_view(self):
         "Test that replacing link by label results in a valid view"
         pool = Pool()
         TestModel = pool.get('test.modelview.link')
-        Model = pool.get('ir.model')
         ModelAccess = pool.get('ir.model.access')
         UIView = pool.get('ir.ui.view')
 
-        model, = Model.search([('model', '=', 'test.modelview.link.target')])
-        access = ModelAccess(model=model, group=None, perm_read=False)
+        access = ModelAccess(
+            model='test.modelview.link.target', group=None, perm_read=False)
         access.save()
 
         arch = TestModel.fields_view_get()['arch']
         parser = etree.XMLParser()
         tree = etree.fromstring(arch, parser=parser)
         validator = etree.RelaxNG(etree=UIView.get_rng('form'))
 
@@ -593,40 +743,36 @@
         self.assertNotIn('active', fields)
 
     @with_transaction(context={'_check_access': True})
     def test_circular_depends_removed(self):
         "Testing circular depends are removed when user has no access"
         pool = Pool()
         CircularDepends = pool.get('test.modelview.circular_depends')
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
 
-        foo_field, = Field.search([
-                ('model.model', '=', 'test.modelview.circular_depends'),
-                ('name', '=', 'foo'),
-                ])
         FieldAccess.create([{
-            'field': foo_field.id,
-            'group': None,
-            'perm_read': False,
-            }])
+                    'model': CircularDepends.__name__,
+                    'field': 'foo',
+                    'group': None,
+                    'perm_read': False,
+                    }])
 
         fields = CircularDepends.fields_view_get(view_type='form')['fields']
 
         self.assertEqual(fields, {})
 
     @with_transaction()
     def test_depends_depends(self):
         "Test depends of depends are included"
         pool = Pool()
         DependsDepends = pool.get('test.modelview.depends_depends')
 
         fields = DependsDepends.fields_view_get(view_type='form')['fields']
 
-        self.assertEqual(fields.keys(), {'foo', 'bar', 'baz'})
+        self.assertEqual(fields.keys(), {'id', 'foo', 'bar', 'baz'})
 
     @with_transaction(context={'_check_access': True})
     def test_button_depends_access(self):
         "Testing buttons are not removed when dependant fields are accesible"
         pool = Pool()
         Button = pool.get('test.modelview.button_depends')
 
@@ -638,26 +784,22 @@
         self.assertEqual(len(buttons), 1)
 
     @with_transaction(context={'_check_access': True})
     def test_button_depends_no_access(self):
         "Testing buttons are removed when dependant fields are not accesible"
         pool = Pool()
         Button = pool.get('test.modelview.button_depends')
-        Field = pool.get('ir.model.field')
         FieldAccess = pool.get('ir.model.field.access')
 
-        field, = Field.search([
-                ('model.model', '=', Button.__name__),
-                ('name', '=', 'value'),
-                ])
         FieldAccess.create([{
-            'field': field.id,
-            'group': None,
-            'perm_read': False,
-            }])
+                    'model': Button.__name__,
+                    'field': 'value',
+                    'group': None,
+                    'perm_read': False,
+                    }])
 
         arch = Button.fields_view_get(view_type='form')['arch']
         parser = etree.XMLParser()
         tree = etree.fromstring(arch, parser=parser)
         buttons = tree.xpath('//button')
 
         self.assertEqual(len(buttons), 0)
```

### Comparing `trytond-7.0.9/trytond/tests/test_mptt.py` & `trytond-7.2.0/trytond/tests/test_mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_multivalue.py` & `trytond-7.2.0/trytond/tests/test_multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_order.py` & `trytond-7.2.0/trytond/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_path.py` & `trytond-7.2.0/trytond/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_protocols.py` & `trytond-7.2.0/trytond/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_pyson.py` & `trytond-7.2.0/trytond/tests/test_pyson.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,35 @@
         self.assertFalse(pyson.PYSONDecoder().decode(eval))
 
         eval = pyson.PYSONEncoder().encode(pyson.Not(False))
         self.assertTrue(pyson.PYSONDecoder().decode(eval))
 
         self.assertEqual(repr(pyson.Not(True)), 'Not(True)')
 
+        self.assertEqual(
+            repr(~pyson.Eval('foo', False)), "~Eval('foo', False)")
+
+        self.assertEqual(
+            repr(pyson.Eval('foo') != 'bar'),
+            "(Eval('foo') != 'bar')")
+
+        eval_ = pyson.PYSONEncoder().encode(pyson.Not({}))
+        self.assertTrue(pyson.PYSONDecoder().decode(eval_))
+
+        eval_ = pyson.PYSONEncoder().encode(pyson.Not({
+                    'a': 1,
+                    }))
+        self.assertFalse(pyson.PYSONDecoder().decode(eval_))
+
+        eval_ = pyson.PYSONEncoder().encode(pyson.Not([]))
+        self.assertTrue(pyson.PYSONDecoder().decode(eval_))
+
+        eval_ = pyson.PYSONEncoder().encode(pyson.Not(['a']))
+        self.assertFalse(pyson.PYSONDecoder().decode(eval_))
+
     def test_Bool(self):
         'Test pyson.Bool'
         self.assertEqual(pyson.Bool('test').pyson(), {
             '__class__': 'Bool',
             'v': 'test',
             })
 
@@ -143,14 +164,18 @@
 
         eval = pyson.PYSONEncoder().encode(pyson.And(False, False, True))
         self.assertFalse(pyson.PYSONDecoder().decode(eval))
 
         self.assertEqual(repr(pyson.And(False, True, True)),
             'And(False, True, True)')
 
+        self.assertEqual(
+            repr(pyson.Eval('foo', True) & pyson.Eval('bar', False)),
+            "(Eval('foo', True) & Eval('bar', False))")
+
     def test_Or(self):
         'Test pyson.Or'
         self.assertEqual(pyson.Or(True, False).pyson(), {
             '__class__': 'Or',
             's': [True, False],
             })
 
@@ -186,14 +211,18 @@
 
         eval = pyson.PYSONEncoder().encode(pyson.Or(False, False, True))
         self.assertTrue(pyson.PYSONDecoder().decode(eval))
 
         self.assertEqual(repr(pyson.Or(False, True, True)),
             'Or(False, True, True)')
 
+        self.assertEqual(
+            repr(pyson.Eval('foo', True) | pyson.Eval('bar', False)),
+            "(Eval('foo', True) | Eval('bar', False))")
+
     def test_Equal(self):
         'Test pyson.Equal'
         self.assertEqual(pyson.Equal('test', 'test').pyson(), {
             '__class__': 'Equal',
             's1': 'test',
             's2': 'test',
             })
@@ -208,14 +237,18 @@
 
         eval = pyson.PYSONEncoder().encode(pyson.Equal('foo', 'bar'))
         self.assertFalse(pyson.PYSONDecoder().decode(eval))
 
         self.assertEqual(repr(pyson.Equal('foo', 'bar')),
             "Equal('foo', 'bar')")
 
+        self.assertEqual(
+            repr(pyson.Eval('foo') == 'bar'),
+            "(Eval('foo') == 'bar')")
+
     def test_Greater(self):
         'Test pyson.Greater'
         self.assertEqual(pyson.Greater(1, 0).pyson(), {
             '__class__': 'Greater',
             's1': 1,
             's2': 0,
             'e': False,
@@ -318,14 +351,22 @@
                 datetime.timedelta(4, 2)))
         self.assertTrue(pyson.PYSONDecoder().decode(eval))
 
         eval = pyson.PYSONEncoder().encode(
             pyson.Greater(pyson.Eval('i', 0), 0))
         self.assertTrue(pyson.PYSONDecoder({'i': 1}).decode(eval))
 
+        self.assertEqual(
+            repr(pyson.Eval('i', 0) > 0),
+            "(Eval('i', 0) > 0)")
+
+        self.assertEqual(
+            repr(pyson.Eval('i', 0) >= 0),
+            "(Eval('i', 0) >= 0)")
+
     def test_Less(self):
         'Test pyson.Less'
         self.assertEqual(pyson.Less(0, 1).pyson(), {
             '__class__': 'Less',
             's1': 0,
             's2': 1,
             'e': False,
@@ -397,14 +438,22 @@
                 pyson.Date(2020, 1, 1), True))
         self.assertTrue(pyson.PYSONDecoder().decode(eval))
 
         eval = pyson.PYSONEncoder().encode(pyson.Less(
                 pyson.DateTime(2020, 1, 1, 0, 0, 0, 0), 90000))
         self.assertFalse(pyson.PYSONDecoder().decode(eval))
 
+        self.assertEqual(
+            repr(pyson.Eval('i', 0) > 0),
+            "(Eval('i', 0) > 0)")
+
+        self.assertEqual(
+            repr(pyson.Eval('i', 0) >= 0),
+            "(Eval('i', 0) >= 0)")
+
     def test_If(self):
         'Test pyson.If'
         self.assertEqual(pyson.If(True, 'foo', 'bar').pyson(), {
             '__class__': 'If',
             'c': True,
             't': 'foo',
             'e': 'bar',
@@ -454,14 +503,18 @@
         eval = pyson.PYSONEncoder().encode(pyson.Get(
             {}, 'foo', 'default'))
         self.assertEqual(pyson.PYSONDecoder().decode(eval), 'default')
 
         self.assertEqual(repr(pyson.Get({'foo': 'bar'}, 'foo', 'default')),
             "Get({'foo': 'bar'}, 'foo', 'default')")
 
+        self.assertEqual(
+            repr(pyson.Eval('foo', {}).get('bar')),
+            "Eval('foo', {}).get('bar')")
+
     def test_In(self):
         'Test pyson.In'
         self.assertEqual(pyson.In('foo', {'foo': 'bar'}).pyson(), {
             '__class__': 'In',
             'k': 'foo',
             'v': {'foo': 'bar'},
             })
@@ -513,14 +566,18 @@
         eval = pyson.PYSONEncoder().encode(
             pyson.In('test', pyson.Eval('foo', [])))
         self.assertFalse(pyson.PYSONDecoder({'foo': None}).decode(eval))
 
         self.assertEqual(repr(pyson.In('foo', ['foo', 'bar'])),
             "In('foo', ['foo', 'bar'])")
 
+        self.assertEqual(
+            repr(pyson.Eval('foo').in_(['foo', 'bar'])),
+            "Eval('foo').in_(['foo', 'bar'])")
+
     def test_Date(self):
         'Test pyson.Date'
         self.assertEqual(pyson.Date(2010, 1, 12, -1, 12, -7).pyson(), {
             '__class__': 'Date',
             'y': 2010,
             'M': 1,
             'd': 12,
@@ -821,15 +878,15 @@
             pyson.Get(pyson.Eval('context', {}), 'company', -1)])
         self.assertEqual(pyson.PYSONDecoder({'context': {'company': 1}}
             ).decode(eval), ['id', '!=', 1])
         self.assertEqual(pyson.PYSONDecoder({'context': {}}
             ).decode(eval), ['id', '=', -1])
 
         self.assertEqual(repr(expr),
-            "If(Not(In('company', Eval('context', {}))), '=', '!=')")
+            "If(~Eval('context', {}).contains('company'), '=', '!=')")
 
     def test_noeval(self):
         decoder = pyson.PYSONDecoder(noeval=True)
         encoder = pyson.PYSONEncoder()
 
         for instance in [
                 pyson.Eval('test', 0),
```

### Comparing `trytond-7.0.9/trytond/tests/test_report.py` & `trytond-7.2.0/trytond/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_res.py` & `trytond-7.2.0/trytond/tests/test_res.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_resource.py` & `trytond-7.2.0/trytond/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_routes.py` & `trytond-7.2.0/trytond/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_rpc.py` & `trytond-7.2.0/trytond/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_rule.py` & `trytond-7.2.0/trytond/tests/test_rule.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,20 +27,18 @@
 
     @with_transaction(context=_context)
     def test_perm_create_with_rule(self):
         "Test create with rule"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': True,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -52,20 +50,18 @@
 
     @with_transaction(context=_context)
     def test_perm_create_with_rule_fail(self):
         "Test create with rule fail"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': True,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -78,20 +74,18 @@
 
     @with_transaction(context=_context)
     def test_perm_create_with_default_rule_fail(self):
         "Test create with default rule fail"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': False,
                     'default_p': True,
                     'perm_read': False,
                     'perm_create': True,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
@@ -115,20 +109,18 @@
 
     @with_transaction(context=_context)
     def test_perm_write_with_rule(self):
         "Test write with rule"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': True,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -141,20 +133,18 @@
 
     @with_transaction(context=_context)
     def test_perm_write_with_rule_fail_before(self):
         "Test write with rule fail before"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': True,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -168,20 +158,18 @@
 
     @with_transaction(context=_context)
     def test_perm_write_with_rule_fail_after(self):
         "Test write with rule fail after"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': True,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -205,20 +193,18 @@
 
     @with_transaction(context=_context)
     def test_perm_delete_with_rule(self):
         "Test delete with rule"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': True,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -231,20 +217,18 @@
 
     @with_transaction(context=_context)
     def test_perm_delete_with_rule_fail(self):
         "Test delete with rule fail"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': True,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -268,20 +252,18 @@
 
     @with_transaction(context=_context)
     def test_perm_read_with_rule(self):
         "Test read with rule"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': True,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -294,20 +276,18 @@
 
     @with_transaction(context=_context)
     def test_perm_read_with_rule_fail(self):
         "Test read with rule fail"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': True,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -321,20 +301,18 @@
 
     @with_transaction(context=_context)
     def test_perm_read_with_rule_no_sql_type_fail(self):
         "Test read with rule fail and without SQL type"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': True,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -358,20 +336,18 @@
 
     @with_transaction(context=_context)
     def test_search_with_rule(self):
         "Test search with rule"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': True,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -384,20 +360,18 @@
 
     @with_transaction(context=_context)
     def test_search_with_rule_match(self):
         "Test search with rule match"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': True,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -420,20 +394,18 @@
 
     @with_transaction(context=_context)
     def test_write_field_rule_True(self):
         "Test _write field when there's a rule - True"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': True,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -447,20 +419,18 @@
 
     @with_transaction(context=_context)
     def test_write_field_rule_False(self):
         "Test _write field when there's a rule - False"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': True,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -475,20 +445,18 @@
     @with_transaction(context=_context)
     def test_write_field_relation_rule_True(self):
         "Test _write field when there's a rule with a relation - True"
         pool = Pool()
         TestRule = pool.get('test.rule')
         TestRuleRelation = pool.get('test.rule.relation')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': True,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -504,20 +472,18 @@
     @with_transaction(context=_context)
     def test_write_field_relation_rule_False(self):
         "Test _write field when there's a rule with a relation - False"
         pool = Pool()
         TestRule = pool.get('test.rule')
         TestRuleRelation = pool.get('test.rule.relation')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': True,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -542,20 +508,18 @@
 
     @with_transaction(context=_context)
     def test_delete_field_rule_True(self):
         "Test _delete field when there's a rule - True"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': True,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -569,20 +533,18 @@
 
     @with_transaction(context=_context)
     def test_delete_field_rule_False(self):
         "Test _delete field when there's a rule - False"
         pool = Pool()
         TestRule = pool.get('test.rule')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': True,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -597,20 +559,18 @@
     @with_transaction(context=_context)
     def test_delete_field_relation_rule_True(self):
         "Test _delete field when there's a rule with a relation - True"
         pool = Pool()
         TestRule = pool.get('test.rule')
         TestRuleRelation = pool.get('test.rule.relation')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': True,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -626,20 +586,18 @@
     @with_transaction(context=_context)
     def test_delete_field_relation_rule_False(self):
         "Test _delete field when there's a rule with a relation - False"
         pool = Pool()
         TestRule = pool.get('test.rule')
         TestRuleRelation = pool.get('test.rule.relation')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': False,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': True,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -655,20 +613,18 @@
     @with_transaction(context=_context)
     def test_model_with_rule(self):
         "Test model with rule"
         pool = Pool()
         TestRule = pool.get('test.rule')
         TestRuleModel = pool.get('test.rule.model')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': True,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
@@ -683,20 +639,18 @@
     @with_transaction(context=_context)
     def test_model_with_rule_fail(self):
         "Test model with rule fail"
         pool = Pool()
         TestRule = pool.get('test.rule')
         TestRuleModel = pool.get('test.rule.model')
         RuleGroup = pool.get('ir.rule.group')
-        Model = pool.get('ir.model')
 
-        model, = Model.search([('model', '=', 'test.rule')])
         rule_group, = RuleGroup.create([{
                     'name': "Field different from foo",
-                    'model': model.id,
+                    'model': TestRule.__name__,
                     'global_p': True,
                     'perm_read': True,
                     'perm_create': False,
                     'perm_write': False,
                     'perm_delete': False,
                     'rules': [('create', [{
                                     'domain': json.dumps(
```

### Comparing `trytond-7.0.9/trytond/tests/test_sendmail.py` & `trytond-7.2.0/trytond/tests/test_sendmail.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
     def test_sendmail(self):
         'Test sendmail'
         message = MagicMock()
         server = Mock()
         sendmail(
             'tryton@example.com', 'foo@example.com', message, server=server)
-        server.sendmail.assert_called_with(
-            'tryton@example.com', 'foo@example.com', message.as_string())
+        server.send_message.assert_called_with(
+            message, 'tryton@example.com', 'foo@example.com')
         server.quit.assert_not_called()
 
     def test_get_smtp_server(self):
         'Test get_smtp_server'
         with patch.object(smtplib, 'SMTP') as SMTP:
             SMTP.return_value = server = Mock()
             self.assertEqual(get_smtp_server('smtp://localhost:25'), server)
@@ -93,22 +93,22 @@
         msg1 = MagicMock(Message)
         msg2 = MagicMock(Message)
         datamanager.put('foo@example.com', 'bar@example.com', msg1)
         datamanager.put('bar@example.com', 'foo@example.com', msg2)
 
         transaction.commit()
 
-        server.sendmail.assert_has_calls([
-                call('foo@example.com', 'bar@example.com', msg1.as_string()),
-                call('bar@example.com', 'foo@example.com', msg2.as_string()),
+        server.send_message.assert_has_calls([
+                call(msg1, 'foo@example.com', 'bar@example.com'),
+                call(msg2, 'bar@example.com', 'foo@example.com'),
                 ])
         server.quit.assert_called_once_with()
         self.assertFalse(datamanager.queue)
 
         server.reset_mock()
 
         datamanager.put(
             'foo@example.com', 'bar@example.com', MagicMock(Message))
         transaction.rollback()
 
-        server.sendmail.assert_not_called()
+        server.send_message.assert_not_called()
         self.assertFalse(datamanager.queue)
```

### Comparing `trytond-7.0.9/trytond/tests/test_sequence.py` & `trytond-7.2.0/trytond/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_tools.py` & `trytond-7.2.0/trytond/tests/test_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import unittest
 from io import BytesIO
 
 import sql
 import sql.operators
 
 from trytond.tools import (
-    decimal_, escape_wildcard, file_open, firstline, grouped_slice,
-    is_full_text, is_instance_method, likify, lstrip_wildcard,
+    cached_property, decimal_, escape_wildcard, file_open, firstline,
+    grouped_slice, is_full_text, is_instance_method, likify, lstrip_wildcard,
     pairwise_longest, reduce_domain, reduce_ids, remove_forbidden_chars,
     rstrip_wildcard, slugify, sortable_values, strip_wildcard, timezone,
     unescape_wildcard)
 from trytond.tools.domain_inversion import (
     canonicalize, concat, domain_inversion, eval_domain,
     extract_reference_models, localize_domain, merge, parse,
     prepare_reference_domain, simplify, sort, unique_value)
@@ -279,15 +279,15 @@
         "Test slugify"
         self.assertEqual(slugify('unicode ♥ is ☢'), 'unicode-is')
 
     def test_slugify_hyphenate(self):
         "Test hyphenate in slugify"
         self.assertEqual(slugify('foo bar', hyphenate='_'), 'foo_bar')
 
-    def test_sortable_values(self):
+    def test_sortable_values_couple(self):
         def key(values):
             return values
 
         values = [
             (('a', 1), ('b', None)),
             (('a', 1), ('b', 3)),
             (('a', 1), ('b', 2)),
@@ -298,14 +298,33 @@
         self.assertEqual(
             sorted(values, key=sortable_values(key)), [
                 (('a', 1), ('b', 2)),
                 (('a', 1), ('b', 3)),
                 (('a', 1), ('b', None)),
                 ])
 
+    def test_sortable_values_single(self):
+        def key(values):
+            return values
+
+        values = [
+            (1, None),
+            (1, 3),
+            (1, 2),
+            ]
+
+        with self.assertRaises(TypeError):
+            sorted(values, key=key)
+        self.assertEqual(
+            sorted(values, key=sortable_values(key)), [
+                (1, 2),
+                (1, 3),
+                (1, None),
+                ])
+
     def test_firstline(self):
         "Test firstline"
         for text, result in [
                 ("", ""),
                 ("first line\nsecond line", "first line"),
                 ("\nsecond line", "second line"),
                 ("\n\nthird line", "third line"),
@@ -1214,10 +1233,62 @@
     def test_generate_png(self):
         "Test generate PNG"
         image = qrcode.generate_png("Tryton")
         self.assertIsInstance(image, BytesIO)
         self.assertIsNotNone(image.getvalue())
 
 
+class CachedProperty:
+    _count = 0
+
+    def get_count(self):
+        self._count += 1
+        return self._count
+
+    cached_count = cached_property(get_count)
+
+
+class CachedPropertySlots:
+    __slots__ = ('_count', '__weakref__')
+
+    def __init__(self):
+        self._count = 0
+
+    def get_count(self):
+        self._count += 1
+        return self._count
+
+    cached_count = cached_property(get_count)
+
+
+class CachedPropertyTestCase(unittest.TestCase):
+    "Test cached_property"
+
+    def test_cached_property_clear(self):
+        "Test clear cached property"
+        item = CachedProperty()
+
+        self.assertEqual(item.cached_count, 1)
+        del item.cached_count
+        self.assertEqual(item.cached_count, 2)
+
+    def test_cached_property_with_slots(self):
+        "Test cached property with slots"
+        item = CachedPropertySlots()
+
+        self.assertEqual(item.cached_count, 1)
+        self.assertEqual(item.cached_count, 1)
+        self.assertEqual(item.get_count(), 2)
+        self.assertEqual(item.cached_count, 1)
+
+    def test_cached_property_with_slots_clear(self):
+        "Test clear cached property with slots"
+        item = CachedPropertySlots()
+
+        self.assertEqual(item.cached_count, 1)
+        del item.cached_count
+        self.assertEqual(item.cached_count, 2)
+
+
 def load_tests(loader, tests, pattern):
     tests.addTest(doctest.DocTestSuite(decimal_))
     return tests
```

### Comparing `trytond-7.0.9/trytond/tests/test_tree.py` & `trytond-7.2.0/trytond/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_trigger.py` & `trytond-7.2.0/trytond/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_tryton.py` & `trytond-7.2.0/trytond/tests/test_tryton.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import hashlib
 import inspect
 import json
 import multiprocessing
 import operator
 import os
 import pathlib
+import re
 import subprocess
 import sys
 import time
 import unittest
 import unittest.mock
 from configparser import ConfigParser
 from fnmatch import fnmatchcase
@@ -673,30 +674,30 @@
                         })
 
     @with_transaction()
     def test_model_access(self):
         'Test missing default model access'
         pool = Pool()
         Access = pool.get('ir.model.access')
-        no_groups = {a.model.model for a in Access.search([
+        no_groups = {a.model for a in Access.search([
                     ('group', '=', None),
                     ])}
 
         def has_access(Model, models):
             if Model.__name__ in models:
                 return True
             for field_name in Model.__access__:
                 Target = Model._fields[field_name].get_target()
                 if has_access(Target, models):
                     return True
         for mname, Model in pool.iterobject():
             if has_access(Model, no_groups):
                 no_groups.add(mname)
 
-        with_groups = {a.model.model for a in Access.search([
+        with_groups = {a.model for a in Access.search([
                     ('group', '!=', None),
                     ])}
 
         self.assertGreaterEqual(no_groups, with_groups,
             msg='Model "%(models)s" are missing a default access' % {
                 'models': list(with_groups - no_groups),
                 })
@@ -1093,27 +1094,49 @@
 
 
 def doctest_teardown(test):
     unittest.mock.patch.stopall()
     return drop_db()
 
 
-doctest_checker = doctest.OutputChecker()
+STRIP_DECIMAL = doctest.register_optionflag('STRIP_DECIMAL')
+
+
+class OutputChecker(doctest.OutputChecker):
+
+    def check_output(self, want, got, optionflags):
+        if optionflags & STRIP_DECIMAL:
+            want = self._strip_decimal(want)
+            got = self._strip_decimal(got)
+        return super().check_output(want, got, optionflags)
+
+    def _strip_decimal(self, value):
+        return re.sub(
+            r"Decimal\s*\('(\d*\.\d*?)0+'\)", r"Decimal('\1')", value)
+
+
+doctest_checker = OutputChecker()
 
 
 def load_doc_tests(name, path, loader, tests, pattern):
     def shouldIncludeScenario(path):
         return (
             loader.testNamePatterns is None
             or any(
                 fnmatchcase(path, pattern)
                 for pattern in loader.testNamePatterns))
     directory = os.path.dirname(path)
     # TODO: replace by glob root_dir in Python 3.10
     cwd = os.getcwd()
+    optionflags = (
+        doctest.REPORT_ONLY_FIRST_FAILURE
+        | doctest.ELLIPSIS
+        | doctest.IGNORE_EXCEPTION_DETAIL)
+    if backend.name == 'sqlite':
+        optionflags |= STRIP_DECIMAL
     try:
         os.chdir(directory)
         for scenario in filter(
                 shouldIncludeScenario, glob.glob('*.rst')):
             config = pathlib.Path(scenario).with_suffix('.json')
             if os.path.exists(config):
                 with config.open() as fp:
@@ -1121,15 +1144,15 @@
             else:
                 configs = [{}]
             for globs in configs:
                 tests.addTests(doctest.DocFileSuite(
                         scenario, package=name, globs=globs,
                         tearDown=doctest_teardown, encoding='utf-8',
                         checker=doctest_checker,
-                        optionflags=doctest.REPORT_ONLY_FIRST_FAILURE))
+                        optionflags=optionflags))
     finally:
         os.chdir(cwd)
     return tests
 
 
 class TestSuite(unittest.TestSuite):
     def run(self, *args, **kwargs):
```

### Comparing `trytond-7.0.9/trytond/tests/test_union.py` & `trytond-7.2.0/trytond/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_user.py` & `trytond-7.2.0/trytond/tests/test_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of this
 # repository contains the full copyright notices and license terms.
 import datetime
 import os
 import unittest
 from contextlib import contextmanager
-from unittest.mock import ANY, Mock, patch
+from unittest.mock import Mock, patch
 
 from trytond.config import config
 from trytond.pool import Pool
 from trytond.res import user as user_module
 from trytond.res.user import PasswordError
 from trytond.tests.test_tryton import activate_module, with_transaction
 from trytond.transaction import Transaction
@@ -147,67 +147,49 @@
         User = pool.get('res.user')
         user_table = User.__table__()
         transaction = Transaction()
         cursor = transaction.connection.cursor()
 
         user = self.create_user('user', '12345', email='user@example.com')
 
-        with patch.object(user_module, 'sendmail_transactional') as sendmail:
+        with patch.object(
+                user_module, 'send_message_transactional') as send_message:
             User.reset_password([user], length=8)
-            sendmail.assert_called_once_with(FROM, ['user@example.com'], ANY)
+            send_message.assert_called_once()
 
         cursor.execute(*user_table.select(
                 user_table.password_hash,
                 where=user_table.id == user.id))
         password_hash, = cursor.fetchone()
 
         self.assertEqual(len(user.password_reset), 8)
         self.assertTrue(user.password_reset_expire)
-        self.assertIsNone(password_hash)
+        self.check_user('user', '12345')
         self.check_user('user', user.password_reset)
 
     @with_transaction()
     def test_reset_password_expired(self):
         "Test reset password not working when expired"
         pool = Pool()
         User = pool.get('res.user')
 
         user = User(login='user', email='user@example.com')
         user.save()
 
-        with patch.object(user_module, 'sendmail_transactional'):
+        with patch.object(user_module, 'send_message_transactional'):
             User.reset_password([user], length=8)
 
         user.password_reset_expire = (
             datetime.datetime.now() - datetime.timedelta(10))
         user.save()
         self.assertFalse(User.get_login('user', {
                     'password': user.password_reset,
                     }))
 
     @with_transaction()
-    def test_reset_password_with_password(self):
-        "Test reset password not working when password is set"
-        pool = Pool()
-        User = pool.get('res.user')
-
-        user = User(login='user', email='user@example.com')
-        user.save()
-
-        with patch.object(user_module, 'sendmail_transactional'):
-            User.reset_password([user], length=8)
-
-        user.password = '12345'
-        user.save()
-        self.check_user('user', '12345')
-        self.assertFalse(User.get_login('user', {
-                    'password': user.password_reset,
-                    }))
-
-    @with_transaction()
     def test_authentications(self):
         "Test authentications"
         pool = Pool()
         User = pool.get('res.user')
 
         user = User(login='user')
         user.save()
```

### Comparing `trytond-7.0.9/trytond/tests/test_wizard.py` & `trytond-7.2.0/trytond/tests/test_wizard.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,19 +109,17 @@
         self.assertEqual(len(result['actions']), 1)
 
     @with_transaction()
     def test_execute_without_access(self):
         "Execute wizard without model access"
         pool = Pool()
         Wizard = pool.get('test.test_wizard', type='wizard')
-        Model = pool.get('ir.model')
         ModelAccess = pool.get('ir.model.access')
-        model, = Model.search([('model', '=', 'test.access')])
         ModelAccess.create([{
-                    'model': model.id,
+                    'model': 'test.access',
                     'perm_write': False,
                     }])
 
         session_id, start_state, end_state = Wizard.create()
 
         with self.assertRaises(AccessError):
             with Transaction().set_context(active_model='test.access'):
```

### Comparing `trytond-7.0.9/trytond/tests/test_workflow.py` & `trytond-7.2.0/trytond/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/test_wsgi.py` & `trytond-7.2.0/trytond/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/tools.py` & `trytond-7.2.0/trytond/tests/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+
+import unittest
+
 from proteus import Model, Wizard
 from proteus import config as pconfig
 
 from .test_tryton import backup_db_cache, drop_create, restore_db_cache
 
 __all__ = ['activate_modules', 'set_user']
 
@@ -26,18 +29,24 @@
     Wizard('ir.module.activate_upgrade').execute('upgrade')
 
     backup_db_cache(cache_name)
     return cfg
 
 
 def _get_config():
-    cfg = pconfig.set_trytond()
-    cfg.pool.test = True
-    return cfg
+    return pconfig.set_trytond()
 
 
 def set_user(user, config=None):
     if not config:
         config = pconfig.get_config()
     User = Model.get('res.user', config=config)
     config.user = int(user)
     config._context = User.get_preferences(True, {})
+
+
+_dummy_test_case = unittest.TestCase()
+_dummy_test_case.maxDiff = None
+
+
+def __getattr__(name):
+    return getattr(_dummy_test_case, name)
```

### Comparing `trytond-7.0.9/trytond/tests/tree.py` & `trytond-7.2.0/trytond/tests/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/trigger.py` & `trytond-7.2.0/trytond/tests/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/wizard.py` & `trytond-7.2.0/trytond/tests/wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/wizard.xml` & `trytond-7.2.0/trytond/tests/wizard.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tests/workflow.py` & `trytond-7.2.0/trytond/tests/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/barcode.py` & `trytond-7.2.0/trytond/tools/barcode.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/decimal_.py` & `trytond-7.2.0/trytond/tools/decimal_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/domain_inversion.py` & `trytond-7.2.0/trytond/tools/domain_inversion.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/email_.py` & `trytond-7.2.0/trytond/tools/email_.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-from email.utils import parseaddr
+from email.header import Header
+from email.utils import formataddr, parseaddr
 
 from trytond.pool import Pool
 
 __all__ = [
     'set_from_header', 'validate_email', 'normalize_email',
     'convert_ascii_email', 'EmailNotValidError']
 
@@ -25,14 +26,18 @@
             message['From'] = sender
             message['On-Behalf-Of'] = from_
             message['Reply-To'] = from_
     else:
         message['From'] = from_
 
 
+def has_rcpt(msg):
+    return any((msg['To'], msg['Cc'], msg['Bcc']))
+
+
 try:
     from dns.exception import DNSException
     from email_validator import EmailNotValidError, caching_resolver
     from email_validator import validate_email as _validate_email
 
     try:
         resolver = caching_resolver()
@@ -76,7 +81,13 @@
         return email
 
     def convert_ascii_email(email):
         return email
 
     class EmailNotValidError(Exception):
         pass
+
+
+def format_address(email, name=None):
+    if name:
+        name = str(Header(name, 'utf-8'))
+    return formataddr((name, convert_ascii_email(email)))
```

### Comparing `trytond-7.0.9/trytond/tools/immutabledict.py` & `trytond-7.2.0/trytond/tools/immutabledict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/logging.py` & `trytond-7.2.0/trytond/tools/logging.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/misc.py` & `trytond-7.2.0/trytond/tools/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import io
 import os
 import re
 import types
 import unicodedata
 import warnings
 from array import array
-from collections.abc import Sized
+from collections.abc import Iterable, Sized
 from functools import wraps
-from itertools import islice, tee, zip_longest
+from itertools import chain, islice, tee, zip_longest
 
 from sql import Literal
 from sql.conditionals import Case
 from sql.operators import Or
 
 from trytond.const import MODULES_GROUP, OPERATORS
 
@@ -282,20 +282,22 @@
         value = str(value)
     value = unicodedata.normalize('NFKD', value)
     value = str(_slugify_strip_re.sub('', value).strip())
     return _slugify_hyphenate_re.sub(hyphenate, value)
 
 
 def sortable_values(func):
-    "Decorator that makes list of couple values sortable"
+    "Decorator that makes list of values sortable"
     @wraps(func)
     def wrapper(*args, **kwargs):
         result = list(func(*args, **kwargs))
-        for i, (name, value) in enumerate(list(result)):
-            result[i] = (name, value is None, value)
+        for i, value in enumerate(list(result)):
+            if not isinstance(value, Iterable):
+                value = [value]
+            result[i] = tuple(chain((k is None, k) for k in value))
         return result
     return wrapper
 
 
 def sql_pairing(x, y):
     """Return SQL expression to pair x and y
     Pairing function from http://szudzik.com/ElegantPairing.pdf"""
```

### Comparing `trytond-7.0.9/trytond/tools/qrcode.py` & `trytond-7.2.0/trytond/tools/qrcode.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/singleton.py` & `trytond-7.2.0/trytond/tools/singleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/string_.py` & `trytond-7.2.0/trytond/tools/string_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tools/timezone.py` & `trytond-7.2.0/trytond/tools/timezone.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/transaction.py` & `trytond-7.2.0/trytond/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                     Pool().get(name)._record),
                 default_factory_with_key=True))
         # Keep last used cache references to allow to pre-fill them
         self._cache_deque.append(cache)
         return cache
 
     def start(self, database_name, user, readonly=False, context=None,
-            close=False, autocommit=False, **extras):
+            close=False, autocommit=False, timeout=None, **extras):
         '''
         Start transaction
         '''
         try:
             from trytond import backend
             assert self.user is None
             assert self.database is None
@@ -193,15 +193,15 @@
             self._datamanagers = []
 
             count = 0
             while True:
                 if count:
                     time.sleep(0.002 * (_retry - count))
                 self.connection = database.get_connection(readonly=readonly,
-                    autocommit=autocommit)
+                    autocommit=autocommit, statement_timeout=timeout)
                 try:
                     lock_tables = extras.get('_lock_tables', [])
                     for table in lock_tables:
                         self.database.lock(self.connection, table)
                     self._locked_tables = set(lock_tables)
                 except backend.DatabaseOperationalError:
                     if count < _retry:
@@ -234,16 +234,17 @@
                         # Transaction must be commited to send notifications
                         if commit and (not self.readonly
                                 or self.database.has_channel()):
                             self.commit()
                         else:
                             self.rollback()
                     finally:
-                        self.database.put_connection(
-                            self.connection, self.close)
+                        if self.connection:
+                            self.database.put_connection(
+                                self.connection, self.close)
                 finally:
                     self.database = None
                     self.readonly = False
                     self.connection = None
                     self.close = None
                     self.user = None
                     self.context = None
@@ -353,15 +354,16 @@
         from trytond.cache import Cache
         for cache in self.cache.values():
             cache.clear()
         for datamanager in self._datamanagers:
             datamanager.tpc_abort(self)
         Cache.rollback(self)
         self._clear_log_records()
-        self.connection.rollback()
+        if self.connection:
+            self.connection.rollback()
 
     def join(self, datamanager):
         try:
             idx = self._datamanagers.index(datamanager)
             return self._datamanagers[idx]
         except ValueError:
             self._datamanagers.append(datamanager)
```

### Comparing `trytond-7.0.9/trytond/tryton.rnc` & `trytond-7.2.0/trytond/tryton.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/tryton.rng` & `trytond-7.2.0/trytond/tryton.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/url.py` & `trytond-7.2.0/trytond/url.py`

 * *Files identical despite different names*

### Comparing `trytond-7.0.9/trytond/wizard/wizard.py` & `trytond-7.2.0/trytond/wizard/wizard.py`

 * *Files 6% similar despite different names*

```diff
@@ -247,40 +247,51 @@
 
     @classmethod
     def check_access(cls):
         pool = Pool()
         ModelAccess = pool.get('ir.model.access')
         ActionWizard = pool.get('ir.action.wizard')
         User = pool.get('res.user')
+        Group = pool.get('res.group')
         context = Transaction().context
 
         if Transaction().user == 0:
             return
 
         with check_access():
             model = context.get('active_model')
             if model:
                 Model = pool.get(model)
             if model and model != 'ir.ui.menu':
                 ModelAccess.check(model, 'read')
             models = ActionWizard.get_models(
                 cls.__name__, action_id=context.get('action_id'))
             if model and models and model not in models:
-                raise AccessError(gettext(
+                groups = Group.browse(User.get_groups())
+                raise AccessError(
+                    gettext(
                         'ir.msg_access_wizard_model_error',
                         wizard=cls.__name__,
-                        model=model))
+                        model=model),
+                    gettext(
+                        'ir.msg_context_groups',
+                        groups=', '.join(g.rec_name for g in groups)))
             groups = set(User.get_groups())
             wizard_groups = ActionWizard.get_groups(cls.__name__,
                 action_id=context.get('action_id'))
             if wizard_groups:
                 if not groups & wizard_groups:
-                    raise AccessError(gettext(
+                    groups = Group.browse(User.get_groups())
+                    raise AccessError(
+                        gettext(
                             'ir.msg_access_wizard_error',
-                            name=cls.__name__))
+                            name=cls.__name__),
+                        gettext(
+                            'ir.msg_context_groups',
+                            groups=', '.join(g.rec_name for g in groups)))
             elif model and model != 'ir.ui.menu':
                 if (not callable(getattr(Model, 'table_query', None))
                         or Model.write.__func__ != ModelSQL.write.__func__):
                     ModelAccess.check(model, 'write')
 
             if model:
                 ids = context.get('active_ids') or []
```

### Comparing `trytond-7.0.9/trytond/worker.py` & `trytond-7.2.0/trytond/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime as dt
 import logging
 import random
 import selectors
 import signal
+import sys
 import time
-from multiprocessing import Pool as MPool
+from concurrent import futures
 from multiprocessing import cpu_count
 
 from sql import Flavor
 
 from trytond import backend
 from trytond.config import config
 from trytond.exceptions import UserError, UserWarning
@@ -19,65 +20,83 @@
 from trytond.transaction import Transaction, TransactionError
 
 __all__ = ['work']
 logger = logging.getLogger(__name__)
 
 
 class Queue(object):
-    def __init__(self, database_name, mpool):
+    def __init__(self, database_name, executor):
         self.database = backend.Database(database_name).connect()
         self.connection = self.database.get_connection(autocommit=True)
-        self.mpool = mpool
+        self.executor = executor
 
     def pull(self, name=None):
         database_list = Pool.database_list()
         pool = Pool(self.database.name)
         if self.database.name not in database_list:
             with Transaction().start(self.database.name, 0, readonly=True):
                 pool.init()
         Queue = pool.get('ir.queue')
         return Queue.pull(self.database, self.connection, name=name)
 
     def run(self, task_id):
-        return self.mpool.apply_async(run_task, (self.database.name, task_id))
+        return self.executor.submit(run_task, self.database.name, task_id)
 
 
 class TaskList(list):
     def filter(self):
         for t in list(self):
-            if t.ready():
+            if not t.running():
                 self.remove(t)
         return self
 
 
+def _noop():
+    pass
+
+
 def work(options):
     Flavor.set(backend.Database.flavor)
     if not config.getboolean('queue', 'worker', default=False):
         return
     try:
         processes = options.processes or cpu_count()
     except NotImplementedError:
         processes = 1
     logger.info("start %d workers", processes)
-    mpool = MPool(
-        processes, initializer, (options.database_names,),
-        options.maxtasksperchild)
-    queues = [Queue(name, mpool) for name in options.database_names]
-
-    tasks = TaskList()
-    selector = selectors.DefaultSelector()
-    for queue in queues:
-        selector.register(queue.connection, selectors.EVENT_READ)
-    try:
+    executor_options = dict(
+        max_workers=processes,
+        mp_context=None,
+        initializer=initializer,
+        initargs=(options.database_names,),
+        max_tasks_per_child=options.maxtasksperchild,
+        )
+    if sys.version_info < (3, 11):
+        del executor_options["max_tasks_per_child"]
+
+    with \
+            futures.ProcessPoolExecutor(**executor_options) as executor, \
+            selectors.DefaultSelector() as selector:
+        queues = [Queue(name, executor) for name in options.database_names]
+        tasks = TaskList()
+
+        for queue in queues:
+            selector.register(queue.connection, selectors.EVENT_READ)
+
         while True:
             timeout = options.timeout
             # Add some randomness to avoid concurrent pulling
             time.sleep(0.1 * random.random())
             while len(tasks.filter()) >= processes:
-                time.sleep(0.1)
+                futures.wait(tasks, return_when=futures.FIRST_COMPLETED)
+
+            # Probe process pool is still operative
+            # before pulling a new task
+            executor.submit(_noop).result()
+
             for queue in queues:
                 try:
                     task_id, next_ = queue.pull(options.name)
                 except backend.DatabaseOperationalError:
                     break
                 if next_ is not None:
                     timeout = min(next_, timeout)
@@ -86,18 +105,14 @@
                     break
             else:
                 for key, _ in selector.select(timeout=timeout):
                     connection = key.fileobj
                     connection.poll()
                     while connection.notifies:
                         connection.notifies.pop(0)
-    except KeyboardInterrupt:
-        mpool.close()
-    finally:
-        selector.close()
 
 
 def initializer(database_names, worker=True):
     if worker:
         signal.signal(signal.SIGINT, signal.SIG_IGN)
     pools = []
     database_list = Pool.database_list()
```

### Comparing `trytond-7.0.9/trytond/wsgi.py` & `trytond-7.2.0/trytond/wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 except ImportError:
     from werkzeug.contrib.fixers import ProxyFix as NumProxyFix
 try:
     from werkzeug.middleware.shared_data import SharedDataMiddleware
 except ImportError:
     from werkzeug.wsgi import SharedDataMiddleware
 
+from trytond import backend
 from trytond.config import config
 from trytond.protocols.jsonrpc import JSONProtocol
 from trytond.protocols.wrappers import (
     HTTPStatus, Request, Response, abort, exceptions)
 from trytond.protocols.xmlrpc import XMLProtocol
 from trytond.status import processing
 from trytond.tools import resolve, safe_join
@@ -107,14 +108,18 @@
             max_request_size = getattr(endpoint, 'max_request_size', None)
             self.check_request_size(request, max_request_size)
             return endpoint(request, **request.view_args)
         except exceptions.HTTPException as e:
             logger.debug(
                 "Exception when processing %s", request, exc_info=True)
             return e
+        except backend.DatabaseOperationalError as e:
+            logger.debug(
+                "Exception when processing %s", request, exc_info=True)
+            return exceptions.ServiceUnavailable(description=str(e))
         except Exception as e:
             logger.debug(
                 "Exception when processing %s", request, exc_info=True)
             tb_s = ''.join(traceback.format_exception(*sys.exc_info()))
             for path in sys.path:
                 tb_s = tb_s.replace(path, '')
             e.__format_traceback__ = tb_s
```

### Comparing `trytond-7.0.9/trytond.egg-info/PKG-INFO` & `trytond-7.2.0/trytond.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 7.0.9
+Version: 7.2.0
 Summary: Tryton server
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/latest/server/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -60,14 +60,15 @@
 Requires-Dist: python-sql>=1.3
 Requires-Dist: werkzeug>=0.12
 Requires-Dist: passlib>=1.7.0
 Requires-Dist: pytz; python_version < "3.9"
 Requires-Dist: backports.entry-points-selectable; python_version < "3.10"
 Provides-Extra: test
 Requires-Dist: pillow; extra == "test"
+Requires-Dist: pydot; extra == "test"
 Provides-Extra: postgresql
 Requires-Dist: psycopg2>=2.7.0; extra == "postgresql"
 Provides-Extra: graphviz
 Requires-Dist: pydot; extra == "graphviz"
 Provides-Extra: levenshtein
 Requires-Dist: python-Levenshtein; extra == "levenshtein"
 Provides-Extra: bcrypt
```

### Comparing `trytond-7.0.9/trytond.egg-info/SOURCES.txt` & `trytond-7.2.0/trytond.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,15 @@
 trytond/ir/view/ui_menu_favorite_form.xml
 trytond/ir/view/ui_menu_favorite_list.xml
 trytond/ir/view/ui_menu_form.xml
 trytond/ir/view/ui_menu_list.xml
 trytond/ir/view/ui_menu_tree.xml
 trytond/ir/view/ui_view_form.xml
 trytond/ir/view/ui_view_list.xml
+trytond/ir/view/ui_view_list_extension.xml
 trytond/ir/view/ui_view_search_form.xml
 trytond/ir/view/ui_view_search_list.xml
 trytond/ir/view/ui_view_tree_optional_form.xml
 trytond/ir/view/ui_view_tree_optional_list.xml
 trytond/ir/view/ui_view_tree_state_form.xml
 trytond/ir/view/ui_view_tree_state_list.xml
 trytond/ir/view/ui_view_tree_width_form.xml
@@ -360,14 +361,15 @@
 trytond/model/fields/binary.py
 trytond/model/fields/boolean.py
 trytond/model/fields/char.py
 trytond/model/fields/date.py
 trytond/model/fields/dict.py
 trytond/model/fields/field.py
 trytond/model/fields/float.py
+trytond/model/fields/fmany2one.py
 trytond/model/fields/function.py
 trytond/model/fields/integer.py
 trytond/model/fields/many2many.py
 trytond/model/fields/many2one.py
 trytond/model/fields/multiselection.py
 trytond/model/fields/numeric.py
 trytond/model/fields/one2many.py
```

### Comparing `trytond-7.0.9/trytond.egg-info/requires.txt` & `trytond-7.2.0/trytond.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -50,10 +50,11 @@
 
 [qrcode]
 qrcode[pil]
 webcolors
 
 [test]
 pillow
+pydot
 
 [weasyprint]
 weasyprint
```

