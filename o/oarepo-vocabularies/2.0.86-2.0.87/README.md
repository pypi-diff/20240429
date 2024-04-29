# Comparing `tmp/oarepo_vocabularies-2.0.86.tar.gz` & `tmp/oarepo_vocabularies-2.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo_vocabularies-2.0.86.tar", last modified: Mon Apr 22 15:50:00 2024, max compression
+gzip compressed data, was "oarepo_vocabularies-2.0.87.tar", last modified: Mon Apr 29 13:35:28 2024, max compression
```

## Comparing `oarepo_vocabularies-2.0.86.tar` & `oarepo_vocabularies-2.0.87.tar`

### file list

```diff
@@ -1,249 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.961995 oarepo_vocabularies-2.0.86/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-22 15:50:00.961995 oarepo_vocabularies-2.0.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.913995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.917995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/ext_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.917995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/hacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.917995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/models/ui.json
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.917995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.917995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.921995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/jsonschemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/systemfields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.921995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.921995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/records/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.921995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/vocabulary_type/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/vocabulary_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/vocabulary_type/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/vocabulary_type/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.925995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.925995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/components/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/components/scanning_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.925995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/custom_fields/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/type_ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/ui_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.901995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.901995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.901995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.901995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.925995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.925995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.901995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.925995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.905995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.929995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.929995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.905995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.929995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.905995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.929995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.933995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.933995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.933995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/components/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/components/deposit.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/components/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.933995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/vocabulary_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/vocabulary_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/vocabulary_type/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.937995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/ITaxonomyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/IVocabularyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/VocabularyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/VocabularyItem.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.905995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.937995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.937995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.905995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.909995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.905995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.941995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.941995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.941995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.941995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.945995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.945995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.945995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.945995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.945995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.949995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.949995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.949995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.949995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.949995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.953995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.953995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.953995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.953995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.953995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.953995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.909995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.953995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.957995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.909995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.909995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.957995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.957995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/tree-field.variables
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.909995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.957995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.957995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.909995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.957995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.909995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.957995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/webpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.961995 oarepo_vocabularies-2.0.86/oarepo_vocabularies/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/views/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies/views/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:50:00.961995 oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-22 15:50:00.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-04-22 15:50:00.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:50:00.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-22 15:50:00.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-22 15:50:00.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-22 15:50:00.000000 oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-22 15:50:00.961995 oarepo_vocabularies-2.0.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:41:26.000000 oarepo_vocabularies-2.0.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.420331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.424331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/ext_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.424331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/hacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.424331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.424331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/systemfields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/records/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.432331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.432331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/scanning_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.432331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/custom_fields/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/type_ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/ui_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.432331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.440331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.440331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.440331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/deposit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.440331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.444331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/ITaxonomyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/IVocabularyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/VocabularyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/VocabularyItem.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.448331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.448331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.448331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.448331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.452331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.452331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.452331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.452331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.456331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.456331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.456331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.460331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/tree-field.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/setup.py
```

### Comparing `oarepo_vocabularies-2.0.86/LICENSE` & `oarepo_vocabularies-2.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/MANIFEST.in` & `oarepo_vocabularies-2.0.87/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/PKG-INFO` & `oarepo_vocabularies-2.0.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.86
+Version: 2.0.87
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-vocabularies
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
```

### Comparing `oarepo_vocabularies-2.0.86/README.md` & `oarepo_vocabularies-2.0.87/README.md`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/components.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/components.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/ext.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/resources/resource.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/authorities/service.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/service.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/config.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ext.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/fixtures.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/hacks.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/hacks.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/models/ui.json` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/models/ui.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/proxies.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/proxies.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/api.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/records/systemfields.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/systemfields.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/config.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/records/ui.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/ui.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/vocabulary_type/config.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/resources/vocabulary_type/resource.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/cache.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     hierarchy = marshmallow.fields.Nested(
         DepositI18nHierarchySchema(), data_key="hierarchy"
     )
     props = marshmallow.fields.Dict(
         keys=marshmallow.fields.String(), values=marshmallow.fields.String()
     )
     tags = marshmallow.fields.List(marshmallow.fields.String())
+    icon = marshmallow.fields.String()
 
 
 class VocabularyCache:
     cache: Dict[str, Dict[str, VocabularyCacheItem]]
     """Language => vocabulary type => last modified + items"""
     lru_terms_cache = TTLCache(maxsize=10000, ttl=3600)
 
@@ -61,26 +62,25 @@
             return
 
         locale = get_locale()
 
         language = locale.language
 
         with self.language_cache(language) as cached_language:
-
             if not self._check_modified(cached_language, vocabulary_types):
                 return
 
             by_vocabulary_type = {}
             max_modified = {}
             for item, dumped_item in self._serialize_items(
                 locale, self._prefetch_vocabularies(vocabulary_types)
             ):
-                by_vocabulary_type.setdefault(item["type"], {})[
-                    item["id"]
-                ] = dumped_item
+                by_vocabulary_type.setdefault(item["type"], {})[item["id"]] = (
+                    dumped_item
+                )
                 if item["type"] not in max_modified:
                     max_modified[item["type"]] = datetime.fromtimestamp(0, timezone.utc)
 
                 modified = datetime.fromisoformat(item["updated"])
                 if max_modified[item["type"]] < modified:
                     max_modified[item["type"]] = modified
 
@@ -192,15 +192,14 @@
                 ][it]
 
     def _split_cached_uncached(self, language, ids):
         cached = {}
         uncached = []
         uncached_small = defaultdict(list)
         with self.language_cache(language) as cached_language:
-
             for vocab_id in ids:
                 term = self.lru_terms_cache.get((language, vocab_id))
                 if term:
                     cached[vocab_id] = term
                 else:
                     if vocab_id[0] in cached_language:
                         uncached_small[vocab_id[0]].append(vocab_id[1])
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/components/hierarchy.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/config.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/custom_fields/hierarchy.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/custom_fields/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/facets.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/facets.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/permissions.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/schema.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/search.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/search.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/service.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/service.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/services/ui_schema.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743589743589743%*

 * *Differences: {"'Icon'": "'Ikona'",*

 * * "'URL for the icon describing the vocabulary item.'": "'URL pro ikonu popisující položku "*

 * *                                                       "slovníku.'"}*

```diff
@@ -12,28 +12,30 @@
     "Export": "Exportovat",
     "Feature": "Preferovat",
     "Find more records with this vocabulary term": "Naj\u00edt dal\u0161\u00ed z\u00e1znamy s touto slovn\u00edkovou polo\u017ekou",
     "Hierarchy": "Hierarchie",
     "Hierarchy title": "N\u00e1zev",
     "ICO": "I\u010cO",
     "ID": "ID",
+    "Icon": "Ikona",
     "Item will be displayed on top of form input options": "Polo\u017eka bude ve formul\u00e1\u0159ov\u00fdch pol\u00edch zobrazena p\u0159ed ostatn\u00edmi",
     "Items Count": "Po\u010det polo\u017eek",
     "Links": "Odkazy",
     "Missing title": "Chyb\u00ed n\u00e1zev",
     "Name": "N\u00e1zev",
     "New child item": "Nov\u00e1 pod\u0159\u00edzen\u00e1 polo\u017eka",
     "Newest": "Nejnov\u011bj\u0161\u00ed",
     "No results found.": "Nebyly nalezeny \u017e\u00e1dn\u00e9 v\u00fdsledky.",
     "Oldest": "Nejstar\u0161\u00ed",
     "PID type": "Typ identifik\u00e1toru",
     "Remove field": "Odebrat pole",
     "Table with available vocabularies": "Tabulka s dostupn\u00fdmi slovn\u00edky",
     "Tags": "\u0160t\u00edtky",
     "Title": "N\u00e1zev",
+    "URL for the icon describing the vocabulary item.": "URL pro ikonu popisuj\u00edc\u00ed polo\u017eku slovn\u00edku.",
     "Updated": "Aktualizov\u00e1no",
     "Vocabularies": "Slovn\u00edky",
     "Vocabulary": "Slovn\u00edk",
     "Vocabulary Code": "K\u00f3d slovn\u00edku",
     "Vocabulary Detail": "Detail polo\u017eky",
     "Vocabulary hierarchy": "Hierarchie slovn\u00edkov\u00fdch polo\u017eek",
     "Vocabulary search": "Hled\u00e1n\u00ed ve slovn\u00edku",
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: \n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.10.3\n"
 
 msgid "(internal)"
 msgstr "(interní)"
 
 msgid "API"
 msgstr "API"
 
@@ -60,14 +60,17 @@
 
 msgid "ICO"
 msgstr "IČO"
 
 msgid "ID"
 msgstr "ID"
 
+msgid "Icon"
+msgstr "Ikona"
+
 msgid "Item will be displayed on top of form input options"
 msgstr "Položka bude ve formulářových polích zobrazena před ostatními"
 
 msgid "Items Count"
 msgstr "Počet položek"
 
 msgid "Links"
@@ -102,14 +105,17 @@
 
 msgid "Tags"
 msgstr "Štítky"
 
 msgid "Title"
 msgstr "Název"
 
+msgid "URL for the icon describing the vocabulary item."
+msgstr "URL pro ikonu popisující položku slovníku."
+
 msgid "Updated"
 msgstr "Aktualizováno"
 
 msgid "Vocabularies"
 msgstr "Slovníky"
 
 msgid "Vocabulary"
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -310,7 +310,13 @@
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:4
 msgid "Missing title"
 msgstr "Chybí název"
 
 msgid "ID"
 msgstr "ID"
+
+msgid "Icon"
+msgstr "Ikona"
+
+msgid "URL for the icon describing the vocabulary item."
+msgstr "URL pro ikonu popisující položku slovníku."
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: \n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.10.3\n"
 
 msgid "(internal)"
 msgstr "(internal)"
 
 msgid "API"
 msgstr "API"
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -311,14 +311,23 @@
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:4
 msgid "Missing title"
 msgstr ""
 
 msgid "ID"
 msgstr ""
 
+msgid "Icon"
+msgstr ""
+
+msgid "URL for the icon describing the vocabulary item. "
+msgstr ""
+
+msgid "URL for the icon describing the vocabulary item."
+msgstr ""
+
 #~ msgid "Export"
 #~ msgstr "Export"
 
 #~ msgid "API"
 #~ msgstr "API"
 
 #~ msgid "Links"
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/translations/messages.pot` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/messages.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,47 +4,47 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-03-18 20:52+0100\n"
+"POT-Creation-Date: 2024-04-23 09:45+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.10.3\n"
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/services/search.py:78
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/services/search.py:139
 msgid "Best match"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/services/search.py:82
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/services/search.py:143
 msgid "Title"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/services/search.py:86
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/services/search.py:147
 msgid "Newest"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/services/search.py:90
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/services/search.py:151
 msgid "Oldest"
 msgstr ""
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/translations/jinjax_messages.jinja:1
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:21
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:27
 #: oarepo_vocabularies/translations/jinjax_messages.jinja:1
 msgid "Created"
 msgstr ""
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/translations/jinjax_messages.jinja:2
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:22
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:28
 #: oarepo_vocabularies/translations/jinjax_messages.jinja:2
 msgid "Updated"
 msgstr ""
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/utils.py:8
 msgid "Vocabulary hierarchy"
 msgstr ""
@@ -61,14 +61,16 @@
 msgid "Add the title..."
 msgstr ""
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/utils.py:18
 msgid "Add the title of the hierarchy"
 msgstr ""
 
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja:9
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja:9
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja:11
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/VocabularyItem.jinja:9
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html:20
 msgid "Find more records with this vocabulary term"
 msgstr ""
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja:3
@@ -107,66 +109,66 @@
 msgid "PID type"
 msgstr ""
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja:26
 msgid "(internal)"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:4
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:5
 msgid "Missing title"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:6
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:12
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html:2
 msgid "vocabulary.vocabulary"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:11
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:17
 msgid "vocabulary.nonpreferredLabels_en"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:15
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:21
 msgid "vocabulary.nonpreferredLabels_cs"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:25
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:31
 msgid "vocabulary.hint_cs"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:28
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:34
 msgid "vocabulary.hint_en"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:35
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja:41
 msgid "vocabulary.tags"
 msgstr ""
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja:3
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html:3
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html:19
 msgid "Vocabulary search"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:5
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:4
 msgid "Edit"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:8
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:7
 msgid "New child item"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:14
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:13
 msgid "Export"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:60
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:59
 msgid "API"
 msgstr ""
 
-#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:60
+#: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja:59
 msgid "Links"
 msgstr ""
 
 #: /home/dusanst/Projects/oarepo-vocabularies/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html:3
 msgid "created.label"
 msgstr ""
 
@@ -261,14 +263,20 @@
 
 msgid "Tags"
 msgstr ""
 
 msgid "Enter one or more tags."
 msgstr ""
 
+msgid "Icon"
+msgstr ""
+
+msgid "URL for the icon describing the vocabulary item."
+msgstr ""
+
 msgid "Add another language"
 msgstr ""
 
 msgid "Name"
 msgstr ""
 
 msgid "required"
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/config.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/ext.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/components/deposit.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/deposit.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/config.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/resource.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/vocabulary_type/config.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/VocabularyItem.jinja` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/VocabularyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 {% block record_sidebar %}
 <oarepo_vocabularies_ui.VocabulariesSidebar metadata={metadata} ui={ui} url_prefix={url_prefix} record={record} extra_context={extra_context}></oarepo_vocabularies_ui.VocabulariesSidebar>
 {% endblock record_sidebar %}
 
 {% block page_body %}
   {{ super() }}
-  <div class="ui center aligned container">
+  <div class="ui center aligned container rel-mb-2">
     {% block vocabulary_descendants %}
       {% set search_app_config = extra_context["search_app_config"] %}
         {%- include "oarepo_vocabularies_ui/descendants.html" -%}
     {% endblock vocabulary_descendants %}
   </div>
 {% endblock page_body %}
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 {#def metadata, ui, record, d #}
 
 <div class="vocabularies-main">
-<h1 class="rel-mb-1 rel-mt-1 ui header" >{{metadata.title.capitalize() if metadata.title else _("Missing title")}}</h1>
-<dl class="ui very basic table">
-  <dt>{{ _('vocabulary.vocabulary') }}</dt>
-  <dd>
-    <a href="/vocabularies/{{metadata.type}}">{{ _("vocabulary." + metadata.type) }}</a>
-  </dd>
-  {% for l in (metadata.nonpreferredLabels or []) %} {% if l.en %}
-  <dt>{{_("vocabulary.nonpreferredLabels_en")}}</dt>
-  <dd>{{l.en}}</dd>
-  {% endif %} {% endfor %} {% for l in (metadata.nonpreferredLabels or []) %} {% if
-  l.cs %}
-  <dt>{{_("vocabulary.nonpreferredLabels_cs")}}</dt>
-  <dd>{{l.cs}}</dd>
-  {% endif %} {% endfor %} {% for prop, val in (metadata.props or {}).items() %}
-  <dt>{{_("vocabulary." + prop)}}</dt>
-  <dd>{{val}}</dd>
-  {% endfor %}
-  <Field label={_('Created')}>{{metadata.created}}</Field>
-  <Field label={_('Updated')}>{{metadata.updated}}</Field>
-  {% if 'hint' in metadata
-  and metadata.hint.cs %}
-  <dt>{{_("vocabulary.hint_cs")}}</dt>
-  <dd>{{metadata.hint.cs}}</dd>
-  {% endif %} {% if 'hint' in metadata and metadata.hint.en %}
-  <dt>{{_("vocabulary.hint_en")}}</dt>
-  <dd>{{metadata.hint.en}}</dd>
-  {% endif %} {% if metadata.relatedURI %} {% for t in metadata.relatedURI.items() %}
-  <dt>{{_("vocabulary.relatedURI_" + t.0)}}</dt>
-  <dd>{{t.1}}</dd>
-  {% endfor %} {% endif %}
-  {% if 'tags' in metadata and metadata.tags | length > 0 %}
-  <dt>{{_("vocabulary.tags")}}</dt>
-  <dd>
-  {% for t in metadata.tags %}
-  <span class="ui tag label {% if t =='featured' -%}red{%- endif %}">{{t}}</span>
-  {% endfor %}
-  </dd>
-  {% endif %}
-</dl>
-<div class="ui center aligned container">
-  
-</div>
+  <div class="flex align-items-center rel-mt-1">
+    {% if record.icon %}
+      <img class="ui image rel-mr-1" src={{record.icon}}>
+    {% endif %}
+    <h1 class="ui header display-inline mt-0" >{{metadata.title.capitalize() if metadata.title else _("Missing title")}}</h1>
+  </div>
+  <dl class="ui very basic table">
+    <dt>{{ _('vocabulary.vocabulary') }}</dt>
+    <dd>
+      <a href="/vocabularies/{{metadata.type}}">{{ _("vocabulary." + metadata.type) }}</a>
+    </dd>
+    {% for l in (metadata.nonpreferredLabels or []) %} {% if l.en %}
+    <dt>{{_("vocabulary.nonpreferredLabels_en")}}</dt>
+    <dd>{{l.en}}</dd>
+    {% endif %} {% endfor %} {% for l in (metadata.nonpreferredLabels or []) %} {% if
+    l.cs %}
+    <dt>{{_("vocabulary.nonpreferredLabels_cs")}}</dt>
+    <dd>{{l.cs}}</dd>
+    {% endif %} {% endfor %} {% for prop, val in (metadata.props or {}).items() %}
+    <dt>{{_("vocabulary." + prop)}}</dt>
+    <dd>{{val}}</dd>
+    {% endfor %}
+    <Field label={_('Created')}>{{metadata.created}}</Field>
+    <Field label={_('Updated')}>{{metadata.updated}}</Field>
+    {% if 'hint' in metadata
+    and metadata.hint.cs %}
+    <dt>{{_("vocabulary.hint_cs")}}</dt>
+    <dd>{{metadata.hint.cs}}</dd>
+    {% endif %} {% if 'hint' in metadata and metadata.hint.en %}
+    <dt>{{_("vocabulary.hint_en")}}</dt>
+    <dd>{{metadata.hint.en}}</dd>
+    {% endif %} {% if metadata.relatedURI %} {% for t in metadata.relatedURI.items() %}
+    <dt>{{_("vocabulary.relatedURI_" + t.0)}}</dt>
+    <dd><a href={{t.1}}>{{t.1}}</a></dd>
+    {% endfor %} {% endif %}
+    {% if 'tags' in metadata and metadata.tags | length > 0 %}
+    <dt>{{_("vocabulary.tags")}}</dt>
+    <dd>
+    {% for t in metadata.tags %}
+    <span class="ui tag label {% if t =='featured' -%}red{%- endif %}">{{t}}</span>
+    {% endfor %}
+    </dd>
+    {% endif %}
+  </dl>
+  <div class="ui center aligned container">
+    
+  </div>
 
-{% set custom_field_name="VOCABULARIES_CF_UI." + record.type %}
-<div class="ui vocabulary_cf">
-<ICustomFields custom_fields={custom_field_name} d={d} />
-</div>
+  {% set custom_field_name="VOCABULARIES_CF_UI." + record.type %}
+  <div class="ui vocabulary_cf">
+  <ICustomFields custom_fields={custom_field_name} d={d} />
+  </div>
 </div>
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
 {#def metadata, ui, record, d #}
+{% if record.icon %} [{{record.icon}}]{% endif %}
 ************ {{{{mmeettaaddaattaa..ttiittllee..ccaappiittaalliizzee(()) iiff mmeettaaddaattaa..ttiittllee eellssee __((""MMiissssiinngg
 ttiittllee""))}}}} ************
 {% set custom_field_name="VOCABULARIES_CF_UI." + record.type %}
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {#def record, extra_context #}
 <div class="rel-mt-2">
-
 {%- if extra_context.permissions.can_edit %}
   <SidebarLink href={record.links.ui_links["edit"]} icon="edit">{{ _('Edit')}}</SidebarLink>
   {%if extra_context.vocabularyProps["hierarchical"] == True%}
     <SidebarLink icon="plus" href={ record.links.ui_links["create"] ~ '?h-parent=' ~ record['id'] }>
       {{_('New child item')}}
     </SidebarLink>
   {%endif%}
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,23 @@
 import * as Yup from "yup";
 import {
     i18next
 } from "@translations/oarepo_vocabularies_ui/i18next";
-import _uniqWith from "lodash/uniqWith";
-
-const checkDuplicateLanguage = (array) => {
-    const uniqueArray = _uniqWith(
-        array,
-        (itemA, itemB) => itemA.language === itemB.language
-    );
-    return uniqueArray.length === array.length;
-};
+import {
+    invalidUrlMessage
+} from "@js/oarepo_ui";
 
 export const VocabularyFormSchema = Yup.object().shape({
     _title: Yup.array().of(
         Yup.object().shape({
             lang: Yup.string().required(i18next.t("required")),
             name: Yup.string().required(i18next.t("required")),
         })
     ),
+    icon: Yup.string().url(invalidUrlMessage),
     props: Yup.object()
         .shape({
             ICO: Yup.string()
                 .length(8, ({
                         length
                     }) =>
                     i18next.t("invalidLengthError", {
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
       text:
         titlesArray.length === 1 ? (
           <span>{text}</span>
         ) : (
           <Breadcrumb icon="left angle" sections={sections} />
         ),
       name: text,
+      icon: undefined,
     };
   });
 
 export const processVocabularyItems = (
   options,
   showLeafsOnly,
   filterFunction
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx`

 * *Files 16% similar despite different names*

```diff
@@ -31,13 +31,22 @@
       <MultiInput
         fieldPath="tags"
         label={i18next.t("Tags")}
         icon="tags"
         placeholder={i18next.t("Enter one or more tags.")}
         required={false}
       />
+      <TextField
+        fieldPath="icon"
+        label={
+          <FieldLabel htmlFor="icon" icon="pencil" label={i18next.t("Icon")} />
+        }
+        placeholder={i18next.t(
+          "URL for the icon describing the vocabulary item."
+        )}
+      />
       {hasPropFields && (
         <PropFieldsComponent vocabularyProps={vocabularyProps} />
       )}
     </Grid.Column>
   );
 };
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import {
   array2object,
   object2array,
   LanguageSelectField,
   ArrayFieldItem,
 } from "@js/oarepo_ui";
 import { i18next } from "@translations/oarepo_vocabularies_ui/i18next";
+import _isEmpty from "lodash/isEmpty";
 
 export const VocabularyMultilingualInputField = ({
   fieldPath,
   label,
   labelIcon,
   required,
   emptyNewInput,
@@ -29,15 +30,15 @@
   }, [fieldPath]);
 
   const { setFieldValue, values } = useFormikContext();
   useEffect(() => {
     if (!getIn(values, placeholderFieldPath)) {
       setFieldValue(
         placeholderFieldPath,
-        getIn(values, fieldPath)
+        !_isEmpty(getIn(values, fieldPath))
           ? object2array(getIn(values, fieldPath, ""), "lang", "name")
           : object2array(newItemInitialValue, "lang", "name")
       );
       return;
     }
     setFieldValue(
       fieldPath,
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/theme/webpack.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/utils.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/ui/views.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/views.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/views/api.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/api.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies/views/app.py` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/app.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/PKG-INFO` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.86
+Version: 2.0.87
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-vocabularies
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
```

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/SOURCES.txt` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/oarepo_vocabularies.egg-info/entry_points.txt` & `oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.86/setup.cfg` & `oarepo_vocabularies-2.0.87/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-vocabularies
-version = 2.0.86
+version = 2.0.87
 description = Support for custom fields and hierarchy on Invenio vocabularies
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

