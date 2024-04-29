# Comparing `tmp/django_quotes-0.5.0.tar.gz` & `tmp/django_quotes-0.5.1.tar.gz`

## Comparing `django_quotes-0.5.0.tar` & `django_quotes-0.5.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/__init__.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/admin.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/apps.py
--rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/py.typed
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/receivers.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/rules.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/signals.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/tasks.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/urls.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/utils.py
--rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/views.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/api/__init__.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/api/serializers.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/api/views.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/management/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/management/commands/__init__.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/management/commands/makemarkov.py
--rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0004_quote_pub_date.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0005_alter_groupmarkovmodel_created_and_more.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0006_alter_source_description_rendered.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0008_auto_20240404_1952.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model_squashed_0012_remove_sourcemarkovmodel_source_and_more.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0013_remove_quote_quote_rendered_and_more.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/0014_alter_source_text_model_alter_sourcegroup_text_model.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/static/.gitkeep
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/base.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/base.html
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_create.html
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_delete.html
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_detail.html
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_list.html
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/group_update.html
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_create.html
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_delete.html
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_detail.html
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_list.html
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_update.html
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_create.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_delete.html
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_detail.html
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_list.html
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 django_quotes-0.5.0/src/django_quotes/templates/quotes/source_update.html
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/api_router.py
--rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/django_settings.py
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_api.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_docs.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_management.py
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_models.py
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_signals.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_tasks.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_utils.py
--rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/test_views.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/urls.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/factories/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 django_quotes-0.5.0/tests/factories/users.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 django_quotes-0.5.0/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 django_quotes-0.5.0/LICENSE
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 django_quotes-0.5.0/README.md
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 django_quotes-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 django_quotes-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/__init__.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/admin.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/apps.py
+-rw-r--r--   0        0        0    26431 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/py.typed
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/receivers.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/rules.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/signals.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/tasks.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/urls.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/utils.py
+-rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/views.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/api/__init__.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/api/serializers.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/api/views.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/management/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/management/commands/__init__.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/management/commands/makemarkov.py
+-rw-r--r--   0        0        0    13189 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0004_quote_pub_date.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0005_alter_groupmarkovmodel_created_and_more.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0006_alter_source_description_rendered.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0008_auto_20240404_1952.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model_squashed_0012_remove_sourcemarkovmodel_source_and_more.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0013_remove_quote_quote_rendered_and_more.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/0014_alter_source_text_model_alter_sourcegroup_text_model.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/static/.gitkeep
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/base.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/base.html
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/group_create.html
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/group_delete.html
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/group_detail.html
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/group_list.html
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/group_update.html
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_create.html
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_delete.html
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_detail.html
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_list.html
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_update.html
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/source_create.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/source_delete.html
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/source_detail.html
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/source_list.html
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 django_quotes-0.5.1/src/django_quotes/templates/quotes/source_update.html
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/api_router.py
+-rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/django_settings.py
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/test_api.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/test_docs.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/test_management.py
+-rw-r--r--   0        0        0    14267 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/test_models.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/test_signals.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/test_tasks.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/test_utils.py
+-rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/test_views.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/urls.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/factories/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 django_quotes-0.5.1/tests/factories/users.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 django_quotes-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 django_quotes-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 django_quotes-0.5.1/README.md
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 django_quotes-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 django_quotes-0.5.1/PKG-INFO
```

### Comparing `django_quotes-0.5.0/src/django_quotes/admin.py` & `django_quotes-0.5.1/src/django_quotes/admin.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/apps.py` & `django_quotes-0.5.1/src/django_quotes/apps.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/models.py` & `django_quotes-0.5.1/src/django_quotes/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 # All rights reserved.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 from __future__ import annotations
 
 import random
+from collections.abc import AsyncIterable, Iterable
 from typing import TYPE_CHECKING, Any
 
-import markovify
 import rules
 from asgiref.sync import async_to_sync
 
 if TYPE_CHECKING:
     from django.db.models.manager import RelatedManager
 from django.conf import settings
 from django.db import models
 from django.db.models import Count
+from django.db.models.query import QuerySet
 from django.utils import timezone
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from loguru import logger
 from markdown import markdown
 from rules.contrib.models import RulesModelBase, RulesModelMixin
 
-from django_markov.models import MarkovTextModel
+from django_markov.models import MarkovCombineError, MarkovEmptyError, MarkovTextModel
 from django_markov.text_models import POSifiedText
 from django_quotes.rules import (  # is_character_owner,; is_group_owner_and_authenticated,
     is_owner,
     is_owner_or_public,
 )
 from django_quotes.signals import quote_random_retrieved
 from django_quotes.utils import generate_unique_slug_for_model
@@ -403,41 +404,47 @@
 
     def update_markov_model(self) -> None:
         """
         Sync wrapper around `aupdate_markov_model`.
         """
         async_to_sync(self.aupdate_markov_model)()
 
-    async def aadd_new_quote_to_model(self, quote_to_add: Quote) -> None:
+    async def aadd_new_quote_to_model(self, quote_to_add: Quote | Iterable[Quote] | AsyncIterable[Quote]) -> None:
         """Allows adding a new quote to the source's (and group's) text model without parsing the whole corpus.
         Note that deleting or editing a quote will still require a full re-ingest of the corpus to remove old data.
 
         Args:
-            quote_to_add (Quote): A quote to add to the source text model.
+            quote_to_add (Quote | Iterable[Quote] | AsyncIterable[Quote]): A Quote instance, or an iterable of Quote
+                instances to add to the source text model.
         """
         if self.allow_markov and await self.quote_set.acount() > 10 and self.text_model is not None:  # noqa: PLR2004
             if not self.text_model.data:
                 await self.aupdate_markov_model()
                 await self.group.aupdate_markov_model()
             else:
                 if self.group.text_model is None:  # no cov
                     self.group.text_model = await MarkovTextModel.objects.acreate()
-                source_model = POSifiedText.from_json(self.text_model.data)
-                group_model = POSifiedText.from_json(self.group.text_model.data)
-                quote_model = POSifiedText(quote_to_add.quote)
+                if isinstance(quote_to_add, AsyncIterable | QuerySet):
+                    corpus_entries = [quote.quote async for quote in quote_to_add]
+                elif isinstance(quote_to_add, Iterable):
+                    corpus_entries = [quote.quote for quote in quote_to_add]
+                else:
+                    corpus_entries = [quote_to_add.quote]
                 try:
-                    combined_source_model = markovify.combine([source_model, quote_model])
-                    combined_group_model = markovify.combine([group_model, quote_model])
-                except ValueError as ve:
+                    await self.text_model.aadd_new_corpus_data_to_model(corpus_entries=corpus_entries)
+                    await self.group.text_model.aadd_new_corpus_data_to_model(corpus_entries=corpus_entries)
+                except ValueError as ve:  # no cov
                     msg = f"Unable to combine models: {ve}"
                     raise QuoteCorpusError(msg) from ve
-                self.text_model.data = combined_source_model.to_json()  # type: ignore
-                self.group.text_model.data = combined_group_model.to_json()  # type: ignore
-                await self.text_model.asave()
-                await self.group.text_model.asave()
+                except MarkovCombineError as mce:
+                    msg = f"Unable to add data to model: {mce}"
+                    raise QuoteCorpusError(msg) from mce
+                except MarkovEmptyError as mee:
+                    msg = f"Cannot add a quote with no text to model: {mee}"
+                    raise QuoteCorpusError(msg) from mee
 
     def add_new_quote_to_model(self, quote_to_add: Quote) -> None:
         """Sync wrapper for `aadd_new_quote_to_model`.
         Allows adding a new quote to the source's text model without parsing the whole corpus.
         Note that deleting or editing a quote will still require a full re-ingest of the corpus to remove old data.
 
         Args:
```

### Comparing `django_quotes-0.5.0/src/django_quotes/receivers.py` & `django_quotes-0.5.1/src/django_quotes/receivers.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/rules.py` & `django_quotes-0.5.1/src/django_quotes/rules.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/signals.py` & `django_quotes-0.5.1/src/django_quotes/signals.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/tasks.py` & `django_quotes-0.5.1/src/django_quotes/tasks.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/urls.py` & `django_quotes-0.5.1/src/django_quotes/urls.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/utils.py` & `django_quotes-0.5.1/src/django_quotes/utils.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/views.py` & `django_quotes-0.5.1/src/django_quotes/views.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/api/serializers.py` & `django_quotes-0.5.1/src/django_quotes/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/api/views.py` & `django_quotes-0.5.1/src/django_quotes/api/views.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/management/commands/makemarkov.py` & `django_quotes-0.5.1/src/django_quotes/management/commands/makemarkov.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0001_squashed_0005_alter_groupmarkovmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0003_alter_source_slug_alter_sourcegroup_slug.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0004_quote_pub_date.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0004_quote_pub_date.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0005_alter_groupmarkovmodel_created_and_more.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0005_alter_groupmarkovmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0006_alter_source_description_rendered.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0006_alter_source_description_rendered.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0007_source_text_model_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0008_auto_20240404_1952.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0008_auto_20240404_1952.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model_squashed_0012_remove_sourcemarkovmodel_source_and_more.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0009_alter_source_text_model_alter_sourcegroup_text_model_squashed_0012_remove_sourcemarkovmodel_source_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0010_alter_source_text_model_alter_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0011_alter_source_text_model_alter_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0012_remove_sourcemarkovmodel_source_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0013_remove_quote_quote_rendered_and_more.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0013_remove_quote_quote_rendered_and_more.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/migrations/0014_alter_source_text_model_alter_sourcegroup_text_model.py` & `django_quotes-0.5.1/src/django_quotes/migrations/0014_alter_source_text_model_alter_sourcegroup_text_model.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_create.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/group_create.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_delete.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/group_delete.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_detail.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/group_detail.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_list.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/group_list.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/group_update.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/group_update.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_create.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_create.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_delete.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_delete.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_detail.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_detail.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_list.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_list.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/quote_update.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/quote_update.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_create.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/source_create.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_delete.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/source_delete.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_detail.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/source_detail.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_list.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/source_list.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/src/django_quotes/templates/quotes/source_update.html` & `django_quotes-0.5.1/src/django_quotes/templates/quotes/source_update.html`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/api_router.py` & `django_quotes-0.5.1/tests/api_router.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/django_settings.py` & `django_quotes-0.5.1/tests/django_settings.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/test_api.py` & `django_quotes-0.5.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/test_management.py` & `django_quotes-0.5.1/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/test_models.py` & `django_quotes-0.5.1/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -303,7 +303,59 @@
     old_group_modify = property_group.text_model.modified
     new_quote = other_source.quote_set.first()
     source.add_new_quote_to_model(new_quote)
     source.text_model.refresh_from_db()
     property_group.text_model.refresh_from_db()
     assert source.text_model.modified > old_source_modify
     assert property_group.text_model.modified > old_group_modify
+
+
+def test_add_empty_quote_list_fails(property_group):
+    source = (
+        property_group.source_set.select_related("text_model", "group", "group__text_model")
+        .prefetch_related("quote_set")
+        .filter(allow_markov=True)
+        .first()
+    )
+    source.update_markov_model()
+    with pytest.raises(QuoteCorpusError):
+        source.add_new_quote_to_model(quote_to_add=[])
+
+
+def test_add_empty_quote_queryset_fails(property_group):
+    source = (
+        property_group.source_set.select_related("text_model", "group", "group__text_model")
+        .prefetch_related("quote_set")
+        .filter(allow_markov=True)
+        .first()
+    )
+    source.update_markov_model()
+    quotes = Quote.objects.none()
+    with pytest.raises(QuoteCorpusError):
+        source.add_new_quote_to_model(quote_to_add=quotes)
+
+
+@pytest.mark.asyncio
+async def test_add_empty_async_quote_queryset_fails(property_group):
+    source = await (
+        property_group.source_set.select_related("text_model", "group", "group__text_model")
+        .prefetch_related("quote_set")
+        .filter(allow_markov=True)
+        .afirst()
+    )
+    await source.aupdate_markov_model()
+    quotes = Quote.objects.none()
+    with pytest.raises(QuoteCorpusError):
+        await source.aadd_new_quote_to_model(quote_to_add=quotes)
+
+
+def test_add_blank_quote_fails(property_group):
+    source = (
+        property_group.source_set.select_related("text_model", "group", "group__text_model")
+        .prefetch_related("quote_set")
+        .filter(allow_markov=True)
+        .first()
+    )
+    source.update_markov_model()
+    quote = Quote.objects.create(quote="", source=source, owner=source.owner)
+    with pytest.raises(QuoteCorpusError):
+        source.add_new_quote_to_model(quote)
```

### Comparing `django_quotes-0.5.0/tests/test_signals.py` & `django_quotes-0.5.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/test_tasks.py` & `django_quotes-0.5.1/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/test_utils.py` & `django_quotes-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/test_views.py` & `django_quotes-0.5.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/urls.py` & `django_quotes-0.5.1/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/tests/factories/users.py` & `django_quotes-0.5.1/tests/factories/users.py`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/.gitignore` & `django_quotes-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/LICENSE` & `django_quotes-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_quotes-0.5.0/README.md` & `django_quotes-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django Quotes
 
 A simple reusable [Django](https://www.djangoproject.com) app that allows you to collect quotes from arbitrary groups of characters, and then serve random quotes or Markov-chain generated sentences based upon them. Includes a Bootstrap compatible set of templates an optional REST API.
 
-![PyPI](https://img.shields.io/pypi/v/django-quotes)
+[![PyPI](https://img.shields.io/pypi/v/django-quotes)](https://pypi.org/project/django-quotes/)
 [![Black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/andrlik/django-quotes/blob/main/.pre-commit-config.yaml)
 [![License](https://img.shields.io/github/license/andrlik/django-quotes)](https://github.com/andrlik/django-quotes/blob/main/LICENSE)
 [![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/rye/main/artwork/badge.json)](https://rye-up.com)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
```

### Comparing `django_quotes-0.5.0/pyproject.toml` & `django_quotes-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "django-quotes"
-version = "0.5.0"
+version = "0.5.1"
 description = """A reusable Django app to collect quotes for use in random retrieval or generation of sentences using \
     Markov Chains."""
 authors = [{ name = "Daniel Andrlik", email = "daniel@andrlik.org" }]
 dependencies = [
-    "django-markov>=0.2.2",
+    "django-markov>=0.3.0",
     "rules>=3.1",
     "Markdown>=3.3.6",
     "python-slugify>=6.1.1",
     "djangorestframework>=3.13.1",
     "django-cors-headers>=3.11.0",
     "drf-spectacular>=0.24.2",
     "django-crispy-forms>=1.14.0",
@@ -246,15 +246,15 @@
 reportIncompatibleMethodOverride = false
 
 [tool.django-stubs]
 django_settings_module = "tests.django_settings"
 
 
 [tool.bumpversion]
-current_version = "0.5.0"
+current_version = "0.5.1"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

### Comparing `django_quotes-0.5.0/PKG-INFO` & `django_quotes-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-quotes
-Version: 0.5.0
+Version: 0.5.1
 Summary: A reusable Django app to collect quotes for use in random retrieval or generation of sentences using Markov Chains.
 Project-URL: Repository, https://github.com/andrlik/django-quotes
 Project-URL: Homepage, https://github.com/andrlik/django-quotes
 Project-URL: Documentation, https://andrlik.github.io/django-quotes/
 Author-email: Daniel Andrlik <daniel@andrlik.org>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: coreapi>=2.3.3
 Requires-Dist: coreschema>=0.0.4
 Requires-Dist: crispy-bootstrap4>=2024.1
 Requires-Dist: django-cors-headers>=3.11.0
 Requires-Dist: django-crispy-forms>=1.14.0
 Requires-Dist: django-easy-logging>=0.70
-Requires-Dist: django-markov>=0.2.2
+Requires-Dist: django-markov>=0.3.0
 Requires-Dist: djangorestframework>=3.13.1
 Requires-Dist: docutils
 Requires-Dist: drf-spectacular>=0.24.2
 Requires-Dist: itypes>=1.2.0
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: markdown>=3.3.6
 Requires-Dist: python-slugify>=6.1.1
@@ -45,15 +45,15 @@
 Requires-Dist: pytest-sugar; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Django Quotes
 
 A simple reusable [Django](https://www.djangoproject.com) app that allows you to collect quotes from arbitrary groups of characters, and then serve random quotes or Markov-chain generated sentences based upon them. Includes a Bootstrap compatible set of templates an optional REST API.
 
-![PyPI](https://img.shields.io/pypi/v/django-quotes)
+[![PyPI](https://img.shields.io/pypi/v/django-quotes)](https://pypi.org/project/django-quotes/)
 [![Black code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/andrlik/django-quotes/blob/main/.pre-commit-config.yaml)
 [![License](https://img.shields.io/github/license/andrlik/django-quotes)](https://github.com/andrlik/django-quotes/blob/main/LICENSE)
 [![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/rye/main/artwork/badge.json)](https://rye-up.com)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
```

