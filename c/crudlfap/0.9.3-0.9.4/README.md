# Comparing `tmp/crudlfap-0.9.3.tar.gz` & `tmp/crudlfap-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crudlfap-0.9.3.tar", last modified: Sun May  9 08:29:38 2021, max compression
+gzip compressed data, was "crudlfap-0.9.4.tar", last modified: Mon Nov  1 22:25:49 2021, max compression
```

## Comparing `crudlfap-0.9.3.tar` & `crudlfap-0.9.4.tar`

### file list

```diff
@@ -1,120 +1,125 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.781485 crudlfap-0.9.3/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2021-05-09 07:03:48.000000 crudlfap-0.9.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       77 2021-05-09 07:03:48.000000 crudlfap-0.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4017 2021-05-09 08:29:38.781485 crudlfap-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2599 2021-05-09 07:03:48.000000 crudlfap-0.9.3/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2021-05-09 08:29:38.781485 crudlfap-0.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1469 2021-05-09 08:29:38.000000 crudlfap-0.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.768152 crudlfap-0.9.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.771485 crudlfap-0.9.3/src/crudlfap/
--rw-rw-rw-   0 root         (0) root         (0)      249 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/crudlfap.py
--rw-rw-rw-   0 root         (0) root         (0)     2923 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/factory.py
--rw-rw-rw-   0 root         (0) root         (0)    25537 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.768152 crudlfap-0.9.3/src/crudlfap/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.768152 crudlfap-0.9.3/src/crudlfap/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.771485 crudlfap-0.9.3/src/crudlfap/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     1423 2021-05-09 08:29:36.000000 crudlfap-0.9.3/src/crudlfap/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1927 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.771485 crudlfap-0.9.3/src/crudlfap/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.771485 crudlfap-0.9.3/src/crudlfap/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/management/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.774819 crudlfap-0.9.3/src/crudlfap/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      597 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/crud.py
--rw-rw-rw-   0 root         (0) root         (0)     3050 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     5064 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/form.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/lock.py
--rw-rw-rw-   0 root         (0) root         (0)      964 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/menu.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3789 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/modelform.py
--rw-rw-rw-   0 root         (0) root         (0)     5956 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/object.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/objectform.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/objects.py
--rw-rw-rw-   0 root         (0) root         (0)      723 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/objectsform.py
--rw-rw-rw-   0 root         (0) root         (0)     1353 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5425 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/table.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/mixins/template.py
--rw-rw-rw-   0 root         (0) root         (0)     3300 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2505 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/registry.py
--rw-rw-rw-   0 root         (0) root         (0)     9970 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/route.py
--rw-rw-rw-   0 root         (0) root         (0)    12537 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/router.py
--rw-rw-rw-   0 root         (0) root         (0)     9549 2021-05-09 08:00:37.000000 crudlfap-0.9.3/src/crudlfap/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/shortcuts.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.774819 crudlfap-0.9.3/src/crudlfap/static/
--rw-rw-rw-   0 root         (0) root         (0)  1098882 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/static/swagger-ui-bundle.js
--rw-rw-rw-   0 root         (0) root         (0)   336841 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/static/swagger-ui-standalone-preset.js
--rw-rw-rw-   0 root         (0) root         (0)   143410 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/static/swagger-ui.css
--rw-rw-rw-   0 root         (0) root         (0)     1381 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/test_conf.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/test_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/test_route.py
--rw-rw-rw-   0 root         (0) root         (0)     3310 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/test_router.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.774819 crudlfap-0.9.3/src/crudlfap/views/
--rw-rw-rw-   0 root         (0) root         (0)      315 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/views/api.py
--rw-rw-rw-   0 root         (0) root         (0)     4643 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap/views/generic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.771485 crudlfap-0.9.3/src/crudlfap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4017 2021-05-09 08:29:38.000000 crudlfap-0.9.3/src/crudlfap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3028 2021-05-09 08:29:38.000000 crudlfap-0.9.3/src/crudlfap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-09 08:29:38.000000 crudlfap-0.9.3/src/crudlfap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      176 2021-05-09 08:29:38.000000 crudlfap-0.9.3/src/crudlfap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       77 2021-05-09 08:29:38.000000 crudlfap-0.9.3/src/crudlfap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_auth/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_auth/backends.py
--rw-rw-rw-   0 root         (0) root         (0)     2784 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_auth/crudlfap.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_auth/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.768152 crudlfap-0.9.3/src/crudlfap_auth/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.768152 crudlfap-0.9.3/src/crudlfap_auth/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_auth/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      657 2021-05-09 08:29:36.000000 crudlfap-0.9.3/src/crudlfap_auth/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1089 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_auth/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_auth/models.py
--rw-rw-rw-   0 root         (0) root         (0)     8040 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_auth/test_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_auth/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_example/artist/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/artist/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      166 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/artist/crudlfap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_example/artist/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      627 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/artist/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/artist/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/artist/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/artist/test_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_example/blog/
--rw-rw-rw-   0 root         (0) root         (0)     2176 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/blog/crudlfap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_example/blog/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      950 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/blog/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/blog/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/blog/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4253 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/blog/test_security.py
--rwxrwxrwx   0 root         (0) root         (0)      121 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/manage.py
--rw-rw-rw-   0 root         (0) root         (0)      814 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_example/song/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/song/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/song/crudlfap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_example/song/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1047 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/song/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/song/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/song/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/song/test_security.py
--rw-rw-rw-   0 root         (0) root         (0)     2005 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_example/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.778152 crudlfap-0.9.3/src/crudlfap_registration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_registration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_registration/crudlfap.py
--rw-rw-rw-   0 root         (0) root         (0)     2266 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_registration/html.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_registration/test_registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.781485 crudlfap-0.9.3/src/crudlfap_sites/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_sites/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_sites/crudlfap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-09 08:29:38.781485 crudlfap-0.9.3/src/crudlfap_sites/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      971 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_sites/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_sites/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1205 2021-05-09 07:03:48.000000 crudlfap-0.9.3/src/crudlfap_sites/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.822173 crudlfap-0.9.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2021-11-01 22:20:27.000000 crudlfap-0.9.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       83 2021-11-01 22:20:27.000000 crudlfap-0.9.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3476 2021-11-01 22:25:49.822173 crudlfap-0.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2021-11-01 22:20:27.000000 crudlfap-0.9.4/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2021-11-01 22:25:49.822173 crudlfap-0.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2021-11-01 22:25:48.000000 crudlfap-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.795507 crudlfap-0.9.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.798840 crudlfap-0.9.4/src/crudlfap/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/crudlfap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    31379 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.795507 crudlfap-0.9.4/src/crudlfap/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.795507 crudlfap-0.9.4/src/crudlfap/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.802173 crudlfap-0.9.4/src/crudlfap/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     1423 2021-11-01 22:25:46.000000 crudlfap-0.9.4/src/crudlfap/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.802173 crudlfap-0.9.4/src/crudlfap/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.802173 crudlfap-0.9.4/src/crudlfap/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/management/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.805507 crudlfap-0.9.4/src/crudlfap/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      597 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7731 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/crud.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)      964 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/menu.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3542 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/modelform.py
+-rw-rw-rw-   0 root         (0) root         (0)     5956 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/object.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/objectform.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)      723 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/objectsform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4667 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2661 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/mixins/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     3300 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2505 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     9970 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/route.py
+-rw-rw-rw-   0 root         (0) root         (0)    14568 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     9549 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/shortcuts.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.812173 crudlfap-0.9.4/src/crudlfap/static/
+-rw-rw-rw-   0 root         (0) root         (0)  1098882 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/static/swagger-ui-bundle.js
+-rw-rw-rw-   0 root         (0) root         (0)   336841 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/static/swagger-ui-standalone-preset.js
+-rw-rw-rw-   0 root         (0) root         (0)   143410 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/static/swagger-ui.css
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/test_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/test_route.py
+-rw-rw-rw-   0 root         (0) root         (0)     3310 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/test_router.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.812173 crudlfap-0.9.4/src/crudlfap/views/
+-rw-rw-rw-   0 root         (0) root         (0)      315 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/views/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5529 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap/views/generic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.802173 crudlfap-0.9.4/src/crudlfap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3476 2021-11-01 22:25:49.000000 crudlfap-0.9.4/src/crudlfap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3253 2021-11-01 22:25:49.000000 crudlfap-0.9.4/src/crudlfap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-01 22:25:49.000000 crudlfap-0.9.4/src/crudlfap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      178 2021-11-01 22:25:49.000000 crudlfap-0.9.4/src/crudlfap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2021-11-01 22:25:49.000000 crudlfap-0.9.4/src/crudlfap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.815507 crudlfap-0.9.4/src/crudlfap_auth/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_auth/backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_auth/crudlfap.py
+-rw-rw-rw-   0 root         (0) root         (0)     3994 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_auth/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.795507 crudlfap-0.9.4/src/crudlfap_auth/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.795507 crudlfap-0.9.4/src/crudlfap_auth/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.815507 crudlfap-0.9.4/src/crudlfap_auth/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      657 2021-11-01 22:25:46.000000 crudlfap-0.9.4/src/crudlfap_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_auth/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_auth/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     8040 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_auth/test_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_auth/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.815507 crudlfap-0.9.4/src/crudlfap_example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.815507 crudlfap-0.9.4/src/crudlfap_example/artist/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/artist/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      166 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/artist/crudlfap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.815507 crudlfap-0.9.4/src/crudlfap_example/artist/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      627 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/artist/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/artist/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/artist/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/artist/test_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.815507 crudlfap-0.9.4/src/crudlfap_example/blog/
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/blog/crudlfap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.818840 crudlfap-0.9.4/src/crudlfap_example/blog/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      950 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/blog/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/blog/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/blog/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4253 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/blog/test_security.py
+-rwxrwxrwx   0 root         (0) root         (0)      121 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/manage.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.818840 crudlfap-0.9.4/src/crudlfap_example/song/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/song/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/song/crudlfap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.818840 crudlfap-0.9.4/src/crudlfap_example/song/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/song/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/song/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/song/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/song/test_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_example/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.818840 crudlfap-0.9.4/src/crudlfap_registration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_registration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_registration/crudlfap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_registration/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.795507 crudlfap-0.9.4/src/crudlfap_registration/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.818840 crudlfap-0.9.4/src/crudlfap_registration/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      275 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_registration/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_registration/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      826 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_registration/test_registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.818840 crudlfap-0.9.4/src/crudlfap_sites/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_sites/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_sites/crudlfap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-01 22:25:49.822173 crudlfap-0.9.4/src/crudlfap_sites/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      971 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_sites/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_sites/migrations/0002_alter_site_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_sites/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2021-11-01 22:20:28.000000 crudlfap-0.9.4/src/crudlfap_sites/models.py
```

### Comparing `crudlfap-0.9.3/LICENSE` & `crudlfap-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/PKG-INFO` & `crudlfap-0.9.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,15 @@
 Metadata-Version: 2.1
 Name: crudlfap
-Version: 0.9.3
+Version: 0.9.4
 Summary: Rich frontend for generic views with Django
 Home-page: https://yourlabs.io/oss/crudlfap
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: BSD
-Description: .. image:: https://img.shields.io/readthedocs/crudlfap.svg
-           :target: https://crudlfap.readthedocs.io
-        .. image:: https://yourlabs.io/oss/crudlfap/badges/master/build.svg
-           :target: https://circleci.com/gh/yourlabs/crudlfap
-        .. image:: https://img.shields.io/codecov/c/github/yourlabs/crudlfap/master.svg
-           :target: https://codecov.io/gh/yourlabs/crudlfap
-        .. image:: https://img.shields.io/npm/v/crudlfap.svg
-           :target: https://www.npmjs.com/package/crudlfap
-        .. image:: https://img.shields.io/pypi/v/crudlfap.svg
-           :target: https://pypi.python.org/pypi/crudlfap
-        
-        Welcome to CRUDLFA+ for Django 3.0: because Django is FUN !
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        CRUDLFA+ stands for Create Read Update Delete List Form Autocomplete and more.
-        
-        This plugin for Django makes a rich user interface from Django models, built
-        with Material Components Web Ryzom Components, offering optionnal databinding
-        with channels support.
-        
-        Demo:
-        
-        - last release: https://demo.crudlfap.ci.yourlabs.io/
-        - current master (might be down/broken etc): https://master.crudlfap.ci.yourlabs.io/
-        
-        Try
-        ===
-        
-        This should start the example project from ``src/crudlfap_example`` where each
-        documented example lives::
-        
-            # This installs the repo in ./src/crudlfap and in your python user packages, i run this from ~
-            pip install --user -e git+https://github.com/yourlabs/crudlfap.git#egg=crudlfap[example]
-            cd src/crudlfap
-        
-            ./manage.py migrate
-            ./manage.py createsuperuser
-            ./manage.py runserver
-        
-        Features
-        ========
-        
-        - DRY into ModelRouter for all views of a Model,
-        - extensive CRUD views, actions, etc
-        - Rich frontend interface out of the box, MDC/Ryzom/Unpoly
-        
-        Resources
-        =========
-        
-        - `Documentation
-          <http://oss.yourlabs.me/crudlfap/>`_
-        - `ChatRoom graciously hosted by
-          <https://www.yourlabs.chat>`_ by `YourLabs Business Service
-          <https://www.yourlabs.biz>`_ on `Mattermost
-          <https://mattermost.com/>`_
-        - `Mailing list graciously hosted
-          <http://groups.google.com/group/yourlabs>`_ by `Google
-          <http://groups.google.com>`_
-        - For **Security** issues, please contact yourlabs-security@googlegroups.com
-        - `Git graciously hosted
-          <https://yourlabs.io/oss/crudlfap/>`_ by `YourLabs Business Service
-          <https://www.yourlabs.biz>`_ with `GitLab
-          <https://www.gitlab.org>`_
-        - `Package graciously hosted
-          <http://pypi.python.org/pypi/crudlfap/>`_ by `PyPi
-          <http://pypi.python.org/pypi>`_,
-        - `Continuous integration graciously hosted
-          <https://yourlabs.io/oss/crudlfap/pipelines>`_ by YourLabs Business Service
-        - Browser test graciously hosted by `SauceLabs
-          <https://saucelabs.com>`_
 Keywords: django crud
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -88,7 +18,80 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 Provides-Extra: project
+License-File: LICENSE
+
+.. image:: https://img.shields.io/readthedocs/crudlfap.svg
+   :target: https://crudlfap.readthedocs.io
+.. image:: https://yourlabs.io/oss/crudlfap/badges/master/build.svg
+   :target: https://circleci.com/gh/yourlabs/crudlfap
+.. image:: https://img.shields.io/codecov/c/github/yourlabs/crudlfap/master.svg
+   :target: https://codecov.io/gh/yourlabs/crudlfap
+.. image:: https://img.shields.io/npm/v/crudlfap.svg
+   :target: https://www.npmjs.com/package/crudlfap
+.. image:: https://img.shields.io/pypi/v/crudlfap.svg
+   :target: https://pypi.python.org/pypi/crudlfap
+
+Welcome to CRUDLFA+ for Django 3.0: because Django is FUN !
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+CRUDLFA+ stands for Create Read Update Delete List Form Autocomplete and more.
+
+This plugin for Django makes a rich user interface from Django models, built
+with Material Components Web Ryzom Components, offering optionnal databinding
+with channels support.
+
+Demo:
+
+- last release: https://demo.crudlfap.ci.yourlabs.io/
+- current master (might be down/broken etc): https://master.crudlfap.ci.yourlabs.io/
+
+Try
+===
+
+This should start the example project from ``src/crudlfap_example`` where each
+documented example lives::
+
+    # This installs the repo in ./src/crudlfap and in your python user packages, i run this from ~
+    pip install --user -e git+https://github.com/yourlabs/crudlfap.git#egg=crudlfap[example]
+    cd src/crudlfap
+
+    ./manage.py migrate
+    ./manage.py createsuperuser
+    ./manage.py runserver
+
+Features
+========
+
+- DRY into ModelRouter for all views of a Model,
+- extensive CRUD views, actions, etc
+- Rich frontend interface out of the box, MDC/Ryzom/Unpoly
+
+Resources
+=========
+
+- `Documentation
+  <http://oss.yourlabs.me/crudlfap/>`_
+- `ChatRoom graciously hosted by
+  <https://www.yourlabs.chat>`_ by `YourLabs Business Service
+  <https://www.yourlabs.biz>`_ on `Mattermost
+  <https://mattermost.com/>`_
+- `Mailing list graciously hosted
+  <http://groups.google.com/group/yourlabs>`_ by `Google
+  <http://groups.google.com>`_
+- For **Security** issues, please contact yourlabs-security@googlegroups.com
+- `Git graciously hosted
+  <https://yourlabs.io/oss/crudlfap/>`_ by `YourLabs Business Service
+  <https://www.yourlabs.biz>`_ with `GitLab
+  <https://www.gitlab.org>`_
+- `Package graciously hosted
+  <http://pypi.python.org/pypi/crudlfap/>`_ by `PyPi
+  <http://pypi.python.org/pypi>`_,
+- `Continuous integration graciously hosted
+  <https://yourlabs.io/oss/crudlfap/pipelines>`_ by YourLabs Business Service
+- Browser test graciously hosted by `SauceLabs
+  <https://saucelabs.com>`_
+
```

### Comparing `crudlfap-0.9.3/README.rst` & `crudlfap-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/setup.py` & `crudlfap-0.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 setup(
     name='crudlfap',
     setup_requires='setupmeta',
-    version='0.9.3',
+    version='0.9.4',
     description='Rich frontend for generic views with Django',
     author='James Pic',
     author_email='jamespic@gmail.com',
     url='https://yourlabs.io/oss/crudlfap',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     keywords='django crud',
     install_requires=[
-        'ryzom>=0.6,<0.7',
+        'ryzom>=0.6.5,<0.7',
         'django>=3.1,<3.2',
         'django-tables2',
         'django-filter',
         'timeago',
         'lookupy-unmanaged',
         'libsass',
     ],
```

### Comparing `crudlfap-0.9.3/src/crudlfap/conf.py` & `crudlfap-0.9.4/src/crudlfap/conf.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/crudlfap.py` & `crudlfap-0.9.4/src/crudlfap/crudlfap.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/factory.py` & `crudlfap-0.9.4/src/crudlfap/factory.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/html.py` & `crudlfap-0.9.4/src/crudlfap/html.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,95 @@
 from django.conf import settings
 from django.contrib.sites.models import Site
+from django.contrib import messages
 from django.urls import reverse
 from django.utils.translation import ugettext as _
 from ryzom_django_mdc.html import *  # noqa
 
 
+UNPOLY_TARGET_ALL = '#main, .mdc-top-app-bar__title, #drawer .mdc-list'
+
+
 class A(A):
     attrs = dict(
-        up_target='#main, .mdc-top-app-bar__title, #drawer .mdc-list',
+        up_target=UNPOLY_TARGET_ALL,
         # up_transition='cross-fade',
     )
 
 
 class Form(Form):
     attrs = dict(
         up_target=A.attrs['up-target'],
         method='post',
     )
 
 
 class Container(Div):
-    style = {
-        'display': 'flex',
-        'flex-direction': 'column',
-        'align-items': 'center',
-        'max-width': '960px',
-        'width': '96vw',
-        'margin': 'auto',
-    }
+    sass = '''
+    .Container
+        display: flex
+        flex-direction: column
+        align-items: center
+        max-width: 960px
+        width: 96vw
+        margin: auto
+
+    .up-modal .Container
+        width: 86vw
+
+    @media screen and (max-width: 500px)
+        .up-modal .up-modal-content
+            padding: 10px
+    '''
 
 
 class FormContainer(Container):
     sass = '''
     .FormContainer
         max-width: 580px
         .mdc-text-field, .mdc-form-field, .mdc-select, form
             width: 100%
+            max-width: 90vw
     '''
 
 
 class PageMenu(Div):
     attrs = dict(cls='mdc-elevation--z2', style='margin-bottom: 10px')
 
+    def __init__(self, *args, _next=None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._next = _next
+
     def to_html(self, *content, **context):
         if 'page-menu' not in context:
             return super().to_html(*content, **context)
 
         content = list(content)
         menu = context['page-menu']
 
         for v in menu:
             if v.urlname == context['view'].urlname:
                 continue
 
+            href = v.url
+            if self._next:
+                if '?' not in href:
+                    href += '?'
+                href += '&_next=' + self._next
             button = A(
                 MDCTextButton(
                     v.label.capitalize(),
                     icon=getattr(v, 'icon', None),
                     tag='span',
                     style={
                         'margin': '10px',
                         'color': getattr(v, 'color', 'inherit'),
                     },
                 ),
-                href=v.url,
+                href=href,
                 style='text-decoration: none',
             )
             if getattr(v, 'controller', None) == 'modal':
                 button.attrs.up_modal = '.main-inner'
                 del button.attrs['up-target']
 
             content.append(button)
@@ -80,57 +102,213 @@
         )
 
 
 class Main(Main):
     pass
 
 
+class ModalClose(Component):
+    '''
+    Close the modal when inserted by Unpoly.
+
+    This should be the default behaviour of Unpoly, as documented, and is the
+    case with modals that do not redirect on the same page, but for modals with
+    a form with a ?_next= redirection then surprisingly unpoly does update the
+    body but does not close the modal by default.
+
+    This tag registers a compiler that calls up.modal.close() when it
+    sees itself, given that unpoly does not execute scripts in
+    response that it loads. As such, this tag MUST be in the initial body, but
+    outside the elements that you will load in modal.
+
+    Remove this hack when we figure the problem in unpoly.
+
+    Equivalent of::
+
+        Script(
+            'up.compiler(".closemodal", function() { up.modal.close(); })',
+            cls='closemodal',
+        ),
+    '''
+    attrs = dict(cls='closemodal')
+
+    def py2js():
+        up.compiler('.closemodal', lambda: up.modal.close())
+
+
+class Message(MDCSnackBar):
+    icons = dict(
+        debug='check_circle',
+        info='check_circle',
+        success='check_circle',
+        warning='warning',
+        error='error',
+    )
+    colors = dict(
+        debug='green',
+        info='yellow',
+        success='green',
+        warning='orange',
+        error='red',
+    )
+    style = '''
+        padding-left: 16px;
+        display: flex;
+        flex-direction: row;
+        align-items: center
+    '''
+
+    def py2js(self):
+        return  # we will use up.compiler
+
+
+class Messages(Div):
+    def to_html(self, *content, **context):
+        msgs = messages.get_messages(context['view'].request)
+        if not msgs:
+            return ''
+
+        return Div(*[
+            Message(message)
+            for message in msgs
+        ]).to_html(*content, **context)
+
+
 class Body(Body):
     style = 'margin: 0'
 
     def __init__(self, *content, **attrs):
         self.drawer = mdcDrawer(id='drawer')
         self.bar = mdcTopAppBar()
+        self.main_inner = Div(
+            Messages(),
+            *content,
+            cls='main-inner',
+        )
         self.main = Main(
-            Div(
-                *content,
-                cls='main-inner',
-            ),
+            self.main_inner,
+            ModalClose(),
             cls='main mdc-drawer-app-content',
             id='main',
         )
         self.debug = settings.DEBUG
         super().__init__(
+            Spinner(),
             self.bar,
             Div(
                 self.drawer,
                 self.main,
                 cls='mdc-top-app-bar--fixed-adjust',
             ),
         )
 
     def py2js(self):
-        up.compiler('[data-mdc-auto-init]', lambda: mdc.autoInit())
+        up.compiler(
+            '[data-mdc-auto-init]',
+            lambda el: mdc.autoInit(el.parentElement)
+        )
         if self.debug:
             up.log.enable()
 
 
+class Spinner(Div):
+    sass = '''
+    .Spinner
+        position: fixed
+        float: right
+        z-index: 20000
+        cursor: pointer
+
+        right: -24px
+        top: 3px
+        @media only screen and (max-width: 600px)
+          top: -32px
+          top: 0
+
+        .lds-dual-ring
+          display: inline-block
+          width: 80px
+          height: 80px
+
+        .lds-dual-ring:after
+          content: " "
+          display: block
+          width: 28px
+          height: 28px
+          margin: 8px
+          border-radius: 50%
+          border: 6px solid #fff
+          border-color: var(--mdc-theme-primary) white var(--mdc-theme-primary) white
+          animation: lds-dual-ring 1.2s linear infinite
+
+        @keyframes lds-dual-ring
+          0%
+            transform: rotate(0deg)
+
+          100%
+            transform: rotate(360deg)
+    '''  # noqa
+
+    def py2js(self):
+        up.proxy.config.slowDelay = 25
+        up.compiler('.Spinner', lambda element: [
+            up.on('up:proxy:slow', lambda: up.element.show(element)),
+            up.on('up:proxy:recover', lambda: up.element.hide(element)),
+        ])
+
+    def __init__(self):
+        super().__init__(Div(cls='lds-dual-ring'), style='display:none')
+
+
+def poll():
+    def poll_setup(element):
+        if not element.getAttribute('id'):
+            console.error('[poll] *REQUIRES* an id attribute!')
+            return
+        interval = parseInt(element.getAttribute('poll') or 5000)
+
+        def poll():
+            if not document.hidden:
+                up.reload(element)
+        poll = setInterval(poll, interval)
+
+        def clear():
+            clearInterval(poll)
+        return clear
+    up.compiler('[poll]', poll_setup)
+
+
+def snack(self):
+    def open_snack(elem):
+        sb = new.mdc.snackbar.MDCSnackbar(elem)
+        sb.open()
+    up.compiler('[data-mdc-auto-init=MDCSnackbar]', open_snack)
+
+
 class App(Html):
     body_class = Body
     scripts = [
-        'https://unpkg.com/unpoly@0.62.1/dist/unpoly.js',
+        'https://unpkg.com/unpoly@1.0.0/dist/unpoly.js',
+        poll,
+        snack,
+        # 'https://unpkg.com/unpoly@2.0.0-rc9/unpoly.min.js',
+        # 'https://unpkg.com/unpoly@2.0.0-rc9/unpoly-migrate.js',
     ]
     stylesheets = [
-        'https://unpkg.com/unpoly@0.62.1/dist/unpoly.min.css',
+        'https://unpkg.com/unpoly@1.0.0/dist/unpoly.css',
+        # 'https://unpkg.com/unpoly@2.0.0-rc9/unpoly.min.css',
     ]
+    sass = '''
+    .up-modal .up-modal-viewport
+        padding-left: 0
+        padding-right: 0
+        padding-top: 10px
+    '''
 
     def to_html(self, *content, **context):
-        self.head.content.append(
-            Style('.up-modal-content { padding-top: 0; padding-bottom: 0; }')
-        )
         if title := getattr(context['view'], 'title', None):
             self.head.content.append(Title(title))
         return super().to_html(*content, **context)
 
 
 class NarrowCard(Div):
     style = {
@@ -157,21 +335,32 @@
             back = A(
                 MDCButton(
                     _('Back'),
                     tag='span',
                 ),
                 href=next_,
             )
+
+        _next = view.request.GET.get(
+            '_next',
+            view.request.POST.get('_next', ''),
+        )
+        if _next:
+            _next = Input(type='hidden', name='_next', value=_next)
+
         return super().to_html(
             H3(view.title),
             Form(
                 form,
                 CSRFInput(view.request),
+                _next,
                 back,
                 MDCButtonRaised(getattr(view, 'title_submit', _('Submit'))),
+                method='post',
+                action=view.request.path_info,
             ),
         )
 
 
 @template('crudlfap/api.html', Html)
 class Swagger(Div):
     def py2js(self):
@@ -201,54 +390,65 @@
                 id='swagger-ui',
                 schema_url=registry.views['schema'].url,
             ),
             **context
         )
 
 
-@template('crudlfap/home.html', App)
+@template('crudlfap/home.html', App, Container)
 class Home(Div):
     def to_html(self, **context):
         site = Site.objects.get_current()
         return super().to_html(
             H1('Welcome to ' + site.name),
+            MDCButtonRaised(
+                'Login to continue',
+                href=reverse('login'),
+                up_target=UNPOLY_TARGET_ALL,
+                tag='a',
+            ),
+            Div('Then, navigate with the menu button at the north west'),
             **context
         )
 
 
 @template('registration/logged_out.html', App, NarrowCard)
 class LoggedOut(Div):
     def to_html(self, **context):
-        from .site import site
         return super().to_html(
             H1(_('Log out')),
             P(_('Thanks for spending some quality time with the Web site today.')),  # noqa
             A(
                 _('Log in again'),
-                href=site.views['login'].url,
+                href=reverse('login'),
             ),
             **context,
         )
 
 
-@template('crudlfap/detail.html', App, NarrowCard)
+@template('crudlfap/detail.html', App)
 class ObjectDetail(Div):
-    def to_html(self, **context):
+    def to_html(self, *content, **context):
         table = MDCDataTable()
         table.thead.attrs.style.display = 'none'
         table.table.attrs.style.width = '100%'
         table.attrs.data_mdc_auto_init = False
 
         for field in context['view'].display_fields:
             table.tbody.addchild(MDCDataTableTr(
                 MDCDataTableTh(field['field'].verbose_name.capitalize()),
                 MDCDataTableTd(field['value']),
             ))
 
-        return super().to_html(table, **context)
+        return super().to_html(
+            PageMenu(),
+            *content,
+            NarrowCard(table),
+            **context
+        )
 
     def context(self, *content, **context):
         context['page-menu'] = context['view'].router.get_menu(
             'object',
             context['view'].request,
             object=context['view'].object,
         )
@@ -286,21 +486,22 @@
             elif not this.previousElementSibling.querySelector(':checked'):
                 this.style.display = 'none'
 
 
 @template('crudlfap/list.html', App)
 class ObjectList(Div):
     def context(self, *content, **context):
-        context['page-menu'] = context['view'].router.get_menu(
-            'model',
-            context['view'].request,
-        )
+        if 'page-menu' not in context:
+            context['page-menu'] = context['view'].router.get_menu(
+                'model',
+                context['view'].request,
+            )
         return super().context(*content, **context)
 
-    def to_html(self, **context):
+    def to_html(self, *content, **context):
         checkbox = None
         context['listactions'] = context['view'].router.get_menu(
             'list_action',
             context['view'].request,
         )
 
         if context['listactions']:
@@ -331,16 +532,17 @@
 
         if context['listactions']:
             table.addchild(self.listactions_component(**context))
 
         table.addchild(self.pagination_component(**context))
 
         return super().to_html(
+            *content,
             self.drawer_component(**context) or '',
-            PageMenu(),
+            PageMenu(_next=context['view'].request.path),
             Div(
                 self.search_component(**context) or '',
                 table,
                 cls='mdc-drawer__content',
                 style='overflow-y: unset',
             ),
             **context,
@@ -704,25 +906,34 @@
             tag='section',
         )]
         return super().to_html(**context)
 
     def nav():
         window.drawer.open = not window.drawer.open
 
+    def close():
+        if window.visualViewport.width < 800:
+            window.drawer.open = False
+
     def py2js(self):
-        window.addEventListener('DOMContentLoaded', self.setup)
+        up.compiler('#drawer, #app-bar, #main', self.setup)
 
     def setup():
-        window.drawer = mdc.drawer.MDCDrawer.attachTo(
-            document.getElementById('drawer'))
-        topAppBar = mdc.topAppBar.MDCTopAppBar.attachTo(
-            document.getElementById('app-bar'))
-        topAppBar.setScrollTarget(document.getElementById('main'))
+        drawer = document.getElementById('drawer')
+        app_bar = document.getElementById('app-bar')
+        main = document.getElementById('main')
+
+        window.drawer = mdc.drawer.MDCDrawer.attachTo(drawer)
+        topAppBar = mdc.topAppBar.MDCTopAppBar.attachTo(app_bar)
+        topAppBar.setScrollTarget(main)
         topAppBar.listen('MDCTopAppBar:nav', self.nav)
 
+        for link in drawer.querySelectorAll('a'):
+            link.addEventListener('click', self.close)
+
 
 class mdcDrawer(Aside):
     menu_hooks = []
 
     def __init__(self, *content, **attrs):
         super().__init__(
             Div(
@@ -740,37 +951,43 @@
 
         menu_content = []
         if request.user.is_authenticated:
             menu_content.append(MDCListItem(str(request.user.email)))
         for view in site.get_menu('main', request):
             icon = getattr(view, 'icon', None)
             title = getattr(view, 'title', '')
+            attrs = dict()
+            if getattr(view, 'unpoly', True):
+                attrs['up_target'] = UNPOLY_TARGET_ALL
 
             menu_content.append(
-                A(
-                    MDCListItem(title.capitalize(), icon=icon),
+                MDCListItem(
+                    title.capitalize(), icon=icon,
                     href=view.url,
                     style='text-decoration: none',
-                )
+                    tag='a',
+                    **attrs,
+                ),
             )
         for hook in self.menu_hooks:
             menu_content = hook(request, menu_content)
 
         content = menu_content
 
         if request.session.get('become_user', None):
-            content.append(Li(
+            content.append(
                 A(
                     ' '.join([
                         str(_('Back to your account')),
                         request.session['become_user_realname'],
                     ]),
                     href=reverse('crudlfap:su'),
+                    up_target=UNPOLY_TARGET_ALL,
                 )
-            ))
+            )
 
         return super().to_html(MDCList(*content))
 
 
 class mdcAppContent(Div):
     def __init__(self, *content):
         super().__init__(
```

### Comparing `crudlfap-0.9.3/src/crudlfap/locale/fr/LC_MESSAGES/django.mo` & `crudlfap-0.9.4/src/crudlfap/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/locale/fr/LC_MESSAGES/django.po` & `crudlfap-0.9.4/src/crudlfap/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/__init__.py` & `crudlfap-0.9.4/src/crudlfap/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/crud.py` & `crudlfap-0.9.4/src/crudlfap/mixins/crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 """CRUD :eMixins that can be used in Actions or Views."""
 import copy
+import json
 
 from django import forms
+from django import http
 from django.contrib.admin.models import ADDITION, CHANGE, DELETION, LogEntry
 from django.contrib.contenttypes.models import ContentType
 
 from crudlfap import html
 
 
 class CreateMixin:
     style = 'success'
     icon = 'add'
     default_template_name = 'crudlfap/create.html'
     template_name_suffixes = ['create', 'form']
     controller = 'modal'
-    action = 'click->modal#open'
     color = 'green'
     log_action_flag = ADDITION
     menus = ['model']
     permission_shortcode = 'add'
 
     def form_valid(self):
         self.object = self.form.save()
         return super().form_valid()
 
-    '''
-    def form_valid_json(self):
-        detail = self.router.get('detail', None)
-        url = None
-        if detail:
-            detail = detail.clone(request=self.request, object=self.object)
-            if detail.has_perm():
-                url = detail.url()
-        return http.JsonResponse({
-            'url': url,
-            'data': data,
-            'status': 'created',
-        }, status=201)
-    '''
-
 
 class ActionMixin:
     def has_perm(self):
         """
         Call has_perm_object or return True.
 
         When called without an object, return True if router agrees.
@@ -84,60 +70,106 @@
         if hasattr(self, 'object_list'):
             self.result = copy.copy(self.object_list).delete()
         else:
             self.result = self.object.delete()
         return super().form_valid()
 
     def get_success_url(self):
-        return self.router['list'].reverse()
+        return self.request.GET.get(
+            '_next',
+            self.request.POST.get(
+                '_next',
+                self.router['list'].reverse()
+            ),
+        )
 
 
 class DetailMixin:
     fa_icon = 'search-plus'
     icon = 'search'
     default_template_name = 'crudlfap/detail.html'
     color = 'blue'
     menus_display = ['object', 'object_detail']
 
     @classmethod
     def get_urlpath(cls):
         """Identify the object by slug or pk in the pattern."""
         return r'<{}>'.format(cls.urlfield)
 
+    def get_JSONField_display(self, name):  # noqa
+        value = getattr(self.object, name, "")
+        formated = json.dumps(value, indent=4)
+        return f'<pre>{formated}</pre>'
+
     def get_title(self):
         return str(self.object)
 
+    def get_visible_fields(self):
+        return [
+            f.name for f in self.model._meta.fields
+            if self.fields == '__all__' or f.name not in self.exclude
+        ]
+
     def get_display_fields(self):
+        """Table field rendering"""
         self.display_fields = [
             {
                 'field': self.model._meta.get_field(field),
                 'value': self.get_field_display(field),
                 'name': field,
             }
-            for field in (
-                [f.name for f in self.model._meta.fields]
-                if self.fields == '__all__'
-                else self.fields
-            ) if field not in self.exclude
+            for field in self.visible_fields
         ]
 
     def get_field_display(self, name):
         value_getter = '_'.join(['get', name, 'display'])
         if hasattr(self.object, value_getter):
             return getattr(self.object, value_getter)()
+        if hasattr(self, value_getter):
+            return getattr(self, value_getter)()
+        type_getter = '_'.join([
+            'get',
+            type(self.model._meta.get_field(name)).__name__,
+            'display',
+        ])
+        if hasattr(self, type_getter):
+            return getattr(self, type_getter)(name)
         value = getattr(self.object, name)
         if hasattr(value, 'get_absolute_url'):
             return html.A(
                 str(value),
                 href=value.get_absolute_url(),
             ).render()
         return value
 
+    def get_json_fields(self):
+        return self.visible_fields
+
+    def get_FIELD_json(self, obj, field):
+        value = getattr(obj, field)
+        if self.router and type(value) in self.router.registry:
+            value = self.router.registry[type(value)].serialize(obj)
+        elif value and not isinstance(value, (str, int, float, bool)):
+            value = str(value)
+        return value
+
+    def serialize(self):
+        if self.router:
+            return self.router.serialize(self.object, self.json_fields)
+        return {
+            field: getattr(
+                self,
+                f'get_{field}_json',
+                'get_FIELD_json',
+            )(self.object, field)
+            for field in self.json_fields
+        }
+
     def json_get(self, request, *args, **kwargs):
-        return {field['name']: field['value'] for field in self.display_fields}
+        return http.JsonResponse(self.serialize())
 
 
 class HistoryMixin:
     icon = 'history'
     template_name_suffix = '_history'
     default_template_name = 'crudlfap/history.html'
     controller = None
@@ -200,19 +232,14 @@
                             '$ref': '#/definitions/' + self.model.__name__
                         },
                         'type': 'array'
                     }
                 },
                 '400': {'description': 'Invalid status value'}
             },
-            'security': [
-                {
-                    'auth': [self.permission_fullcode]
-                }
-            ],
             'summary': self.title,
             'tags': self.swagger_tags
         }
 
 
 class UpdateMixin:
     icon = 'edit'
```

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/filter.py` & `crudlfap-0.9.4/src/crudlfap/mixins/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import django_filters
 from django import forms
 from django.db import models
 
 
 class FilterMixin(object):
+    def get_filter_model(self):
+        return self.filterset_kwargs['queryset'].model
+
     def get_filterset(self):
         """
         Returns an instance of the filterset to be used in this view.
         """
         self.filterset = self.filterset_class(**self.filterset_kwargs)
 
         # filter out choices which have no result to avoid filter pollution
         # with choices which would empty out results
         for name, field in self.filterset.form.fields.items():
             try:
-                mf = self.model._meta.get_field(name)
+                mf = self.filter_model._meta.get_field(name)
             except Exception:
                 continue
 
             if not isinstance(mf, models.ForeignKey):
                 continue
 
             field.queryset = field.queryset.annotate(
@@ -61,28 +64,28 @@
         )
 
     def get_filterset_form_layout(self):
         return None
 
     def get_filterset_meta_attributes(self):
         return dict(
-            model=self.model,
+            model=self.filter_model,
             fields=self.filter_fields,
             filter_overrides=self.filterset_meta_filter_overrides,
             form=self.filterset_form_class,
         )
 
     def get_filterset_meta_class(self):
         return type('Meta', (object,), self.filterset_meta_attributes)
 
     def get_filterset_extra_class_attributes(self):
         extra = dict()
         for field_name in self.filter_fields:
             try:
-                field = self.model._meta.get_field(field_name)
+                field = self.filter_model._meta.get_field(field_name)
             except:  # noqa
                 continue
             choices = getattr(field, 'choices', None)
             if choices is None:
                 continue
             extra[field_name] = django_filters.MultipleChoiceFilter(
                 choices=choices)
@@ -91,11 +94,11 @@
     def get_filterset_class_attributes(self):
         res = dict(Meta=self.filterset_meta_class)
         res.update(self.filterset_extra_class_attributes)
         return res
 
     def get_filterset_class(self):
         return type(
-            '{}FilterSet'.format(self.model.__name__),
+            '{}FilterSet'.format(self.filter_model.__name__),
             (django_filters.FilterSet,),
             self.filterset_class_attributes
         )
```

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/form.py` & `crudlfap-0.9.4/src/crudlfap/mixins/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,18 @@
         if self.request.content_type == 'application/json':
             return self.form_valid_json()
 
         self.message_success()
         return http.HttpResponseRedirect(self.success_url)
 
     def form_valid_json(self):
-        return http.JsonResponse({'status': 'accepted'}, status=201)
+        return http.JsonResponse({
+            'data': self.form.cleaned_data,
+            'status': 'accepted',
+        }, status=201)
 
     def form_invalid_json(self):
         data = dict(
             status='invalid data',
             non_field_errors=self.form.non_field_errors(),
             field_errors=dict(),
         )
@@ -38,15 +41,17 @@
 
     def form_invalid(self):
         """If the form is invalid, render the invalid form."""
         if self.request.content_type == 'application/json':
             return self.form_invalid_json()
 
         self.message_error()
-        return self.render_to_response()
+        response = self.render_to_response()
+        response.status_code = 400
+        return response
 
     def get_title_submit(self):
         """
         Title of the submit button.
 
         Defaults to :py:attr:`~crudlfap.mixins.menu.MenuMixin.title_menu`
         """
@@ -142,19 +147,14 @@
             'parameters': [],
             'produces': ['application/json', 'application/xml'],
             'responses': {
                 '405': {
                     'description': 'Invalid input'
                 },
             },
-            'security': [
-                {
-                    'auth': [self.permission_fullcode]
-                }
-            ],
             'summary': self.swagger_summary,
             'tags': self.swagger_tags,
         }
         for name, field in self.form_class.base_fields.items():
             result['parameters'].append({
                 'description': '. '.join([
                     str(field.label),
```

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/lock.py` & `crudlfap-0.9.4/src/crudlfap/mixins/lock.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/menu.py` & `crudlfap-0.9.4/src/crudlfap/mixins/menu.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/model.py` & `crudlfap-0.9.4/src/crudlfap/mixins/model.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/modelform.py` & `crudlfap-0.9.4/src/crudlfap/mixins/modelform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 
+from django import http
 from django.contrib.admin.models import LogEntry
 from django.contrib.contenttypes.models import ContentType
 from django.forms import models as model_forms
 from django.utils.translation import ugettext as _
 
 from .form import FormMixin
 from .model import ModelMixin
@@ -37,25 +38,32 @@
 log_insert = log  # backward compat
 
 
 class ModelFormMixin(ModelMixin, FormMixin):
     """ModelForm Mixin using readable"""
     menus = ['model']
 
+    def form_valid_json(self):
+        return http.JsonResponse({
+            'data': self.router.serialize(self.object),
+            'status': 'created',
+        }, status=201)
+
     def get_form_kwargs(self):
         self.form_kwargs = super().get_form_kwargs()
         if (
             hasattr(self, 'object')
             and issubclass(self.form_class, model_forms.ModelForm)
         ):
             self.form_kwargs.update({'instance': self.object})
         return self.form_kwargs
 
     def get_form(self):
         self.form = self.form_class(**self.form_kwargs)
+        return self.form
 
     def get_form_fields(self):
         return self.fields
 
     def get_form_base(self):
         return None
 
@@ -82,28 +90,14 @@
     def get_form_valid_message(self):
         return '{}: {}'.format(
             _(self.view_label),
             self.form.instance,
         ).capitalize()
 
     def message_html(self, message):
-        """Add the detail url for form.instance, if possible."""
-        if getattr(self, 'object', None):
-            try:
-                url = self.object.get_absolute_url()
-            except Exception:
-                return message
-
-            return ' '.join((
-                message,
-                '<a href="{}" class="btn-flat toast-action">{}</a>'.format(
-                    url,
-                    _('detail').capitalize(),
-                ),
-            ))
         return message
 
     def get_log_action_flag(self):
         return False
 
     def get_log_message(self):
         return _(self.view_label)
```

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/object.py` & `crudlfap-0.9.4/src/crudlfap/mixins/object.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/objectsform.py` & `crudlfap-0.9.4/src/crudlfap/mixins/objectsform.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/search.py` & `crudlfap-0.9.4/src/crudlfap/mixins/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 
 
 class SearchForm(forms.Form):
     q = forms.CharField(label=_('Search'), required=False)
 
 
 class SearchMixin(object):
+    def get_search_model(self):
+        return self.model
+
     def get_search_fields(self):
         if hasattr(self.router, 'search_fields'):
             return self.router.search_fields
         return [
             f.name
-            for f in self.model._meta.fields
+            for f in self.search_model._meta.fields
             if isinstance(f, models.CharField)
         ]
 
     def get_search_form_class(self):
         if not self.search_fields:
             return
```

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/table.py` & `crudlfap-0.9.4/src/crudlfap/mixins/table.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,36 +22,21 @@
 
     def __init__(self, **kwargs):
         kwargs.setdefault('default', True)
         super().__init__(**kwargs)
 
     def render(self, record, table, value, **kwargs):
         from crudlfap.site import site
-        buttons = []
-        views = site[type(record)].get_menu(
-            'object',
-            table.request,
-            object=record
-        )
-        for view in views:
-            button = html.Component(
-                f'<button class="material-icons mdc-icon-button" ryzom-id="308bade28a8c11ebad3800e18cb957e9" style="color: {getattr(view, "color", "")}; --mdc-ripple-fg-size:28px; --mdc-ripple-fg-scale:1.7142857142857142; --mdc-ripple-left:10px; --mdc-ripple-top:10px;">{getattr(view, "icon", "")}</button>',  # noqa
-                title=view.title.capitalize(),
-                href=view.url + '?next=' + table.request.path_info,
-                style='text-decoration: none',
-                tag='a',
-            )
-            if getattr(view, 'controller', None) == 'modal':
-                button.attrs.up_modal = '.main-inner'
-            else:
-                button.attrs['up-target'] = html.A.attrs['up-target']
-            buttons.append(button)
         out = html.Div(
-            *buttons,
-            style='display:flex;flex-direction:row-reverse'
+            *site[type(record)].get_menu_component(
+                'object',
+                table.request,
+                object=record
+            ).content,
+            style='display:flex;flex-direction:row-reverse',
         ).render()
         return mark_safe(out)
 
 
 class Table(tables.Table):
     def before_render(self, request):
         self.request = request
@@ -65,31 +50,31 @@
 
 
 class TableMixin(object):
     def get_table_fields(self):
         if self.table_sequence:
             self.table_fields = [
                 f.name
-                for f in self.model._meta.fields
+                for f in self.object_list.model._meta.fields
                 if f.name in self.table_sequence
             ]
         else:
             self.table_fields = [
                 f.name
-                for f in self.model._meta.fields
+                for f in self.object_list.model._meta.fields
                 if f.name not in self.exclude
             ]
         return self.table_fields
 
     def get_table_link_fields(self):
-        if not hasattr(self.model, 'get_absolute_url'):
+        if not hasattr(self.object_list.model, 'get_absolute_url'):
             return []
 
         for field in self.table_fields:
-            model_field = self.model._meta.get_field(field)
+            model_field = self.object_list.model._meta.get_field(field)
             if isinstance(model_field, models.CharField):
                 return [field]
 
         return []
 
     def get_table_meta_link_columns(self):
         return {i: UnpolyLinkColumn() for i in self.table_link_fields}
@@ -105,15 +90,15 @@
     def get_table_sequence(self):
         return None
 
     def get_table_columns(self):
         return dict()
 
     def get_table_meta_attributes(self):
-        attrs = dict(model=self.model)
+        attrs = dict(model=self.object_list.model)
 
         if self.table_sequence:
             attrs['sequence'] = self.table_sequence
 
         if self.table_fields:
             attrs['fields'] = self.table_fields
 
@@ -145,15 +130,15 @@
         bases = (self.table_class,)
         if (self.table_class != Table
                 and not issubclass(self.table_class, Table)):
 
             bases = (self.table_class, Table)
 
         return type(
-            '{}Table'.format(self.model.__name__),
+            '{}Table'.format(self.object_list.model.__name__),
             bases,
             self.table_class_attributes
         )
 
     def get_table_kwargs(self):
         return dict(data=self.object_list)
```

### Comparing `crudlfap-0.9.3/src/crudlfap/mixins/template.py` & `crudlfap-0.9.4/src/crudlfap/mixins/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,9 +85,8 @@
                 self.model._meta.model_name,
                 '_' + self.urlname,
             ))
 
         default_template_name = getattr(self, 'default_template_name', None)
         if default_template_name:
             template_names.append(default_template_name)
-        logger.debug('TEMPLATE_NAMES', template_names)
         return template_names
```

### Comparing `crudlfap-0.9.3/src/crudlfap/models.py` & `crudlfap-0.9.4/src/crudlfap/models.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/registry.py` & `crudlfap-0.9.4/src/crudlfap/registry.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/route.py` & `crudlfap-0.9.4/src/crudlfap/route.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/router.py` & `crudlfap-0.9.4/src/crudlfap/router.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 dropdown. If there is only one matching view, it will display only the button.
 """
 from django.apps import apps
 from django.conf import settings
 from django.db import models
 from django.urls import path
 from django.utils.module_loading import import_string
+from django.utils.safestring import mark_safe
+
+from crudlfap import html
 
 from .route import Route
 from .settings import CRUDLFAP_VIEWS
 from .utils import guess_urlfield
 
 crudlfap = apps.get_app_config('crudlfap')  # pylint: disable=invalid-name
 
@@ -123,14 +126,22 @@
 
         :py:class:`ViewsDescriptor` using
         :py:data:`~crudlfap.settings.CRUDLFAP_VIEWS` by default,
         otherwise your list of views.
 
         .. note:: The final views list is generated by the
                   :py:meth:`generate_views` method.
+
+    .. py:attribute:: fields
+
+        Fields that views should use by default.
+
+    .. py:attribute:: json_fields
+
+        Fields that the Router serializer should use by default.
     """
     views = ViewsDescriptor(
         getattr(settings, 'CRUDFLAP_VIEWS', CRUDLFAP_VIEWS)
     )
 
     def __getattr__(self, attr):
         if attr.startswith('get_'):
@@ -326,14 +337,32 @@
             view = v.clone(request=request, **kwargs)()
 
             if view.has_perm():
                 views.append(view)
 
         return views
 
+    def get_menu_component(self, name, request, **kwargs):
+        views = self.get_menu(name, request, **kwargs)
+        buttons = []
+        for view in views:
+            button = html.Component(
+                mark_safe(f'<button class="material-icons mdc-icon-button" ryzom-id="308bade28a8c11ebad3800e18cb957e9" style="color: {getattr(view, "color", "")}; --mdc-ripple-fg-size:28px; --mdc-ripple-fg-scale:1.7142857142857142; --mdc-ripple-left:10px; --mdc-ripple-top:10px;">{getattr(view, "icon", "")}</button>'),  # noqa
+                title=view.title.capitalize(),
+                href=view.url + '?_next=' + request.path_info,
+                style='text-decoration: none',
+                tag='a',
+            )
+            if getattr(view, 'controller', None) == 'modal':
+                button.attrs.up_modal = '.main-inner'
+            else:
+                button.attrs['up-target'] = html.A.attrs['up-target']
+            buttons.append(button)
+        return html.Div(*buttons)
+
     def get_model(self):
         return None
 
     def has_perm(self, view):
         """
         Override this method if you don't use a Django permission backend.
 
@@ -391,7 +420,33 @@
             elif isinstance(field, models.JSONField):
                 field_def['type'] = 'object'
             else:
                 field_def['type'] = 'string'
 
             result['properties'][field.name] = field_def
         return result
+
+    def get_json_fields(self):
+        return [
+            f.name for f in self.model._meta.fields
+        ]
+
+    def get_FIELD_json(self, obj, field):
+        value = getattr(obj, field)
+        if callable(value):
+            value = value()
+        if type(value) in self.registry:
+            value = self.registry[type(value)].serialize(value)
+        elif value and not isinstance(value, (str, int, float, bool)):
+            value = str(value)
+        return value
+
+    def serialize(self, obj, fields=None):
+        fields = fields or self.json_fields
+        return {
+            field: getattr(
+                self,
+                f'get_{field}_json',
+                self.get_FIELD_json,
+            )(obj, field)
+            for field in self.json_fields
+        }
```

### Comparing `crudlfap-0.9.3/src/crudlfap/settings.py` & `crudlfap-0.9.4/src/crudlfap/settings.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/site.py` & `crudlfap-0.9.4/src/crudlfap/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,11 @@
             menus=['main'],
             title=_('API'),
             title_menu=_('Api'),
             title_heading='',
             urlname='api',
             urlpath='api',
             authenticate=False,
+            unpoly=False,
         ),
     ]
 )
```

### Comparing `crudlfap-0.9.3/src/crudlfap/static/swagger-ui-bundle.js` & `crudlfap-0.9.4/src/crudlfap/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/static/swagger-ui-standalone-preset.js` & `crudlfap-0.9.4/src/crudlfap/static/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/static/swagger-ui.css` & `crudlfap-0.9.4/src/crudlfap/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/test_conf.py` & `crudlfap-0.9.4/src/crudlfap/test_conf.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/test_route.py` & `crudlfap-0.9.4/src/crudlfap/test_route.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/test_router.py` & `crudlfap-0.9.4/src/crudlfap/test_router.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/views/api.py` & `crudlfap-0.9.4/src/crudlfap/views/api.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap/views/generic.py` & `crudlfap-0.9.4/src/crudlfap/views/generic.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,14 +70,40 @@
 class DeleteObjectsView(mixins.DeleteMixin, ObjectsFormView):
     """Delete selected objects."""
 
 
 class DetailView(mixins.DetailMixin, ObjectView):
     """Templated model object detail view which takes a field option."""
 
+    def get_swagger_summary(self):
+        return f'{self.model.__name__} Detail'
+
+    def get_swagger_get(self):
+        result = {
+            'operationId': f'find{self.model.__name__}ByStatus',
+            'produces': ['application/json'],
+            'responses': {
+                '200': {
+                    'description': 'successful operation',
+                    'schema': {
+                        'items': {
+                            '$ref': f'#/definitions/{self.model.__name__}'
+                        },
+                        'type': 'array'
+                    }
+                },
+                '404': {
+                    'description': 'Not found'
+                },
+            },
+            'summary': self.swagger_summary,
+            'tags': self.swagger_tags,
+        }
+        return result
+
 
 class HistoryView(mixins.ObjectMixin, generic.DetailView):
     pass
 
 
 class ListView(mixins.ListMixin, mixins.SearchMixin, mixins.FilterMixin,
                mixins.TableMixin, mixins.ObjectsMixin, TemplateView):
@@ -93,58 +119,66 @@
 
         return self.object_list
 
     def get_listactions(self):
         return self.router.get_menu('list_action', self.request)
 
     def get_swagger_get(self):
+        parameters = []
+        if self.filterset:
+            for name, field in self.filterset.form.fields.items():
+                parameters.append({
+                    'collectionFormat': 'single',
+                    'description': field.help_text,
+                    'in': 'query',
+                    'name': name,
+                    'required': field.required,
+                    'type': 'string'
+                })
+
         return {
             # 'description': 'Multiple status are comma separated',
-            'operationId': 'findPetsByStatus',
-            'parameters': [
-                {
-                    'collectionFormat': 'multi',
-                    'description': 'Status values to filter',
-                    'in': 'query',
-                    'items': {
-                        'default': 'available',
-                        'enum': ['available', 'pending', 'sold'],
-                        'type': 'string'
-                    },
-                    'name': 'status',
-                    'required': True,
-                    'type': 'array'
-                }
-            ],
-            'produces': ['application/json', 'application/xml'],
+            'operationId': f'find{self.model.__name__}ByStatus',
+            'parameters': parameters,
+            'produces': ['application/json'],
             'responses': {
                 '200': {
                     'description': 'successful operation',
                     'schema': {
-                        'items': {'$ref': '#/definitions/Pet'},
+                        'items': {
+                            '$ref': f'#/definitions/{self.model.__name__}'
+                        },
                         'type': 'array'
                     }
                 },
-                '400': {'description': 'Invalid status value'}
+                '400': {'description': 'Invalid parameter'}
             },
-            'security': [{'petstore_auth': ['write:pets', 'read:pets']}],
             'summary': self.title,
             'tags': self.swagger_tags,
         }
 
+    def get_json_fields(self):
+        return self.router.json_fields
+
+    def serialize(self, obj):
+        if self.router:
+            return self.router.serialize(obj, self.json_fields)
+        return {
+            field: getattr(
+                self,
+                f'get_{field}_json',
+                'get_FIELD_json',
+            )(obj, field)
+            for field in self.json_fields
+        }
+
     def json_get(self, request, *args, **kwargs):
         rows = []
         for row in self.table.paginated_rows:
-            json_row = dict()
-            for field in self.table_fields:
-                value = getattr(row.record, field, None)
-                if not isinstance(value, (str, int, float, bool, None)):
-                    value = str(value)
-                json_row[field] = value
-            rows.append(json_row)
+            rows.append(self.serialize(row.record))
         data = dict(
             results=rows,
             paginator=dict(
                 page_number=self.table.page.number,
                 per_page=self.table.page.paginator.per_page,
                 total_pages=self.table.page.paginator.num_pages,
                 total_objects=self.table.page.paginator.count,
```

### Comparing `crudlfap-0.9.3/src/crudlfap.egg-info/PKG-INFO` & `crudlfap-0.9.4/src/crudlfap.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,15 @@
 Metadata-Version: 2.1
 Name: crudlfap
-Version: 0.9.3
+Version: 0.9.4
 Summary: Rich frontend for generic views with Django
 Home-page: https://yourlabs.io/oss/crudlfap
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: BSD
-Description: .. image:: https://img.shields.io/readthedocs/crudlfap.svg
-           :target: https://crudlfap.readthedocs.io
-        .. image:: https://yourlabs.io/oss/crudlfap/badges/master/build.svg
-           :target: https://circleci.com/gh/yourlabs/crudlfap
-        .. image:: https://img.shields.io/codecov/c/github/yourlabs/crudlfap/master.svg
-           :target: https://codecov.io/gh/yourlabs/crudlfap
-        .. image:: https://img.shields.io/npm/v/crudlfap.svg
-           :target: https://www.npmjs.com/package/crudlfap
-        .. image:: https://img.shields.io/pypi/v/crudlfap.svg
-           :target: https://pypi.python.org/pypi/crudlfap
-        
-        Welcome to CRUDLFA+ for Django 3.0: because Django is FUN !
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        CRUDLFA+ stands for Create Read Update Delete List Form Autocomplete and more.
-        
-        This plugin for Django makes a rich user interface from Django models, built
-        with Material Components Web Ryzom Components, offering optionnal databinding
-        with channels support.
-        
-        Demo:
-        
-        - last release: https://demo.crudlfap.ci.yourlabs.io/
-        - current master (might be down/broken etc): https://master.crudlfap.ci.yourlabs.io/
-        
-        Try
-        ===
-        
-        This should start the example project from ``src/crudlfap_example`` where each
-        documented example lives::
-        
-            # This installs the repo in ./src/crudlfap and in your python user packages, i run this from ~
-            pip install --user -e git+https://github.com/yourlabs/crudlfap.git#egg=crudlfap[example]
-            cd src/crudlfap
-        
-            ./manage.py migrate
-            ./manage.py createsuperuser
-            ./manage.py runserver
-        
-        Features
-        ========
-        
-        - DRY into ModelRouter for all views of a Model,
-        - extensive CRUD views, actions, etc
-        - Rich frontend interface out of the box, MDC/Ryzom/Unpoly
-        
-        Resources
-        =========
-        
-        - `Documentation
-          <http://oss.yourlabs.me/crudlfap/>`_
-        - `ChatRoom graciously hosted by
-          <https://www.yourlabs.chat>`_ by `YourLabs Business Service
-          <https://www.yourlabs.biz>`_ on `Mattermost
-          <https://mattermost.com/>`_
-        - `Mailing list graciously hosted
-          <http://groups.google.com/group/yourlabs>`_ by `Google
-          <http://groups.google.com>`_
-        - For **Security** issues, please contact yourlabs-security@googlegroups.com
-        - `Git graciously hosted
-          <https://yourlabs.io/oss/crudlfap/>`_ by `YourLabs Business Service
-          <https://www.yourlabs.biz>`_ with `GitLab
-          <https://www.gitlab.org>`_
-        - `Package graciously hosted
-          <http://pypi.python.org/pypi/crudlfap/>`_ by `PyPi
-          <http://pypi.python.org/pypi>`_,
-        - `Continuous integration graciously hosted
-          <https://yourlabs.io/oss/crudlfap/pipelines>`_ by YourLabs Business Service
-        - Browser test graciously hosted by `SauceLabs
-          <https://saucelabs.com>`_
 Keywords: django crud
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -88,7 +18,80 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 Provides-Extra: project
+License-File: LICENSE
+
+.. image:: https://img.shields.io/readthedocs/crudlfap.svg
+   :target: https://crudlfap.readthedocs.io
+.. image:: https://yourlabs.io/oss/crudlfap/badges/master/build.svg
+   :target: https://circleci.com/gh/yourlabs/crudlfap
+.. image:: https://img.shields.io/codecov/c/github/yourlabs/crudlfap/master.svg
+   :target: https://codecov.io/gh/yourlabs/crudlfap
+.. image:: https://img.shields.io/npm/v/crudlfap.svg
+   :target: https://www.npmjs.com/package/crudlfap
+.. image:: https://img.shields.io/pypi/v/crudlfap.svg
+   :target: https://pypi.python.org/pypi/crudlfap
+
+Welcome to CRUDLFA+ for Django 3.0: because Django is FUN !
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+CRUDLFA+ stands for Create Read Update Delete List Form Autocomplete and more.
+
+This plugin for Django makes a rich user interface from Django models, built
+with Material Components Web Ryzom Components, offering optionnal databinding
+with channels support.
+
+Demo:
+
+- last release: https://demo.crudlfap.ci.yourlabs.io/
+- current master (might be down/broken etc): https://master.crudlfap.ci.yourlabs.io/
+
+Try
+===
+
+This should start the example project from ``src/crudlfap_example`` where each
+documented example lives::
+
+    # This installs the repo in ./src/crudlfap and in your python user packages, i run this from ~
+    pip install --user -e git+https://github.com/yourlabs/crudlfap.git#egg=crudlfap[example]
+    cd src/crudlfap
+
+    ./manage.py migrate
+    ./manage.py createsuperuser
+    ./manage.py runserver
+
+Features
+========
+
+- DRY into ModelRouter for all views of a Model,
+- extensive CRUD views, actions, etc
+- Rich frontend interface out of the box, MDC/Ryzom/Unpoly
+
+Resources
+=========
+
+- `Documentation
+  <http://oss.yourlabs.me/crudlfap/>`_
+- `ChatRoom graciously hosted by
+  <https://www.yourlabs.chat>`_ by `YourLabs Business Service
+  <https://www.yourlabs.biz>`_ on `Mattermost
+  <https://mattermost.com/>`_
+- `Mailing list graciously hosted
+  <http://groups.google.com/group/yourlabs>`_ by `Google
+  <http://groups.google.com>`_
+- For **Security** issues, please contact yourlabs-security@googlegroups.com
+- `Git graciously hosted
+  <https://yourlabs.io/oss/crudlfap/>`_ by `YourLabs Business Service
+  <https://www.yourlabs.biz>`_ with `GitLab
+  <https://www.gitlab.org>`_
+- `Package graciously hosted
+  <http://pypi.python.org/pypi/crudlfap/>`_ by `PyPi
+  <http://pypi.python.org/pypi>`_,
+- `Continuous integration graciously hosted
+  <https://yourlabs.io/oss/crudlfap/pipelines>`_ by YourLabs Business Service
+- Browser test graciously hosted by `SauceLabs
+  <https://saucelabs.com>`_
+
```

### Comparing `crudlfap-0.9.3/src/crudlfap.egg-info/SOURCES.txt` & `crudlfap-0.9.4/src/crudlfap.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -81,12 +81,15 @@
 src/crudlfap_example/song/test_security.py
 src/crudlfap_example/song/migrations/0001_initial.py
 src/crudlfap_example/song/migrations/__init__.py
 src/crudlfap_registration/__init__.py
 src/crudlfap_registration/crudlfap.py
 src/crudlfap_registration/html.py
 src/crudlfap_registration/test_registration.py
+src/crudlfap_registration/templates/django_registration/activation_email_body.txt
+src/crudlfap_registration/templates/django_registration/activation_email_subject.txt
 src/crudlfap_sites/__init__.py
 src/crudlfap_sites/crudlfap.py
 src/crudlfap_sites/models.py
 src/crudlfap_sites/migrations/0001_initial.py
+src/crudlfap_sites/migrations/0002_alter_site_settings.py
 src/crudlfap_sites/migrations/__init__.py
```

### Comparing `crudlfap-0.9.3/src/crudlfap_auth/backends.py` & `crudlfap-0.9.4/src/crudlfap_auth/backends.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_auth/crudlfap.py` & `crudlfap-0.9.4/src/crudlfap_auth/crudlfap.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 from . import views
 
 User = apps.get_model(getattr(settings, 'AUTH_USER_MODEL', 'auth.User'))
 
 
 def login_logout(request, menu):
     if request.user.is_authenticated:
-        menu.append(html.A(
-            html.MDCListItem('Logout', icon='logout'),
+        menu.append(html.MDCListItem(
+            'Logout',
+            icon='logout',
             href=reverse('logout'),
             style='text-decoration: none',
+            up_target=html.UNPOLY_TARGET_ALL,
+            tag='a',
         ))
     else:
-        menu.insert(1, html.A(
-            html.MDCListItem('Login', icon='login'),
+        menu.insert(1, html.MDCListItem(
+            'Login',
+            icon='login',
             href=reverse('login'),
             style='text-decoration: none',
+            up_target=html.UNPOLY_TARGET_ALL,
+            tag='a',
         ))
     return menu
 
 
 html.mdcDrawer.menu_hooks.append(login_logout)
```

### Comparing `crudlfap-0.9.3/src/crudlfap_auth/html.py` & `crudlfap-0.9.4/src/crudlfap_auth/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                     A(
                         MDCButtonOutlined('forgot password'),
                         href=reverse('password_reset')
                     ),
                     style='display: flex; justify-content: space-between',
                 ),
                 method='POST',
+                action=view.request.path_info,
                 cls='form card',
             ),
             cls='',
         )
 
 
 @template('registration/logged_out.html', App)
```

### Comparing `crudlfap-0.9.3/src/crudlfap_auth/locale/fr/LC_MESSAGES/django.mo` & `crudlfap-0.9.4/src/crudlfap_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_auth/locale/fr/LC_MESSAGES/django.po` & `crudlfap-0.9.4/src/crudlfap_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_auth/test_urls.py` & `crudlfap-0.9.4/src/crudlfap_auth/test_urls.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_auth/views.py` & `crudlfap-0.9.4/src/crudlfap_auth/views.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/artist/migrations/0001_initial.py` & `crudlfap-0.9.4/src/crudlfap_example/artist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/artist/test_api.py` & `crudlfap-0.9.4/src/crudlfap_example/artist/test_api.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/blog/crudlfap.py` & `crudlfap-0.9.4/src/crudlfap_example/blog/crudlfap.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/blog/migrations/0001_initial.py` & `crudlfap-0.9.4/src/crudlfap_example/blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/blog/models.py` & `crudlfap-0.9.4/src/crudlfap_example/blog/models.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/blog/test_security.py` & `crudlfap-0.9.4/src/crudlfap_example/blog/test_security.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/settings.py` & `crudlfap-0.9.4/src/crudlfap_example/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from crudlfap.settings import *  # noqa
 
+BASE_DIR = Path(__file__).resolve().parent.parent
+
 INSTALLED_APPS += [  # noqa
+    # CRUDLFA+ extras
+    'django_registration',
+    'crudlfap_registration',
+
     # CRUDLFA+ examples
     'crudlfap_example.artist',
     'crudlfap_example.song',
     'crudlfap_example.blog',
-
-    # CRUDLFA+ extras
-    'django_registration',
-    'crudlfap_registration',
 ]
 
-ROOT_URLCONF = 'crudlfap_example.urls'
+ROOT_URLCONF = os.path.dirname(__file__).split('/')[-1] + '.urls'
 
 DATABASES = {
     'default': {
         'ENGINE': os.getenv('DB_ENGINE', 'django.db.backends.sqlite3'),
-        'NAME': os.getenv('DB_NAME', os.path.join(BASE_DIR, 'db.sqlite3')),
+        'NAME': os.getenv('DB_NAME', os.path.join(
+            os.path.dirname(__file__),
+            '..',
+            'db.sqlite3',
+        )),
         'HOST': os.getenv('DB_HOST'),
         'USER': os.getenv('DB_USER'),
         'PASSWORD': os.getenv('DB_PASS'),
     }
 }
 
 install_optional(OPTIONAL_APPS, INSTALLED_APPS)  # noqa
```

### Comparing `crudlfap-0.9.3/src/crudlfap_example/song/crudlfap.py` & `crudlfap-0.9.4/src/crudlfap_example/song/crudlfap.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/song/migrations/0001_initial.py` & `crudlfap-0.9.4/src/crudlfap_example/song/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/song/models.py` & `crudlfap-0.9.4/src/crudlfap_example/song/models.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/song/test_security.py` & `crudlfap-0.9.4/src/crudlfap_example/song/test_security.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_example/urls.py` & `crudlfap-0.9.4/src/crudlfap_example/urls.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_registration/html.py` & `crudlfap-0.9.4/src/crudlfap_registration/html.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_registration/test_registration.py` & `crudlfap-0.9.4/src/crudlfap_registration/test_registration.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_sites/migrations/0001_initial.py` & `crudlfap-0.9.4/src/crudlfap_sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `crudlfap-0.9.3/src/crudlfap_sites/models.py` & `crudlfap-0.9.4/src/crudlfap_sites/models.py`

 * *Files identical despite different names*

