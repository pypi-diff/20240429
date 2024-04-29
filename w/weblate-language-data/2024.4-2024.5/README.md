# Comparing `tmp/weblate_language_data-2024.4.tar.gz` & `tmp/weblate_language_data-2024.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblate_language_data-2024.4.tar", last modified: Thu Apr 25 18:01:33 2024, max compression
+gzip compressed data, was "weblate_language_data-2024.5.tar", last modified: Mon Apr 29 07:37:08 2024, max compression
```

## Comparing `weblate_language_data-2024.4.tar` & `weblate_language_data-2024.5.tar`

### file list

```diff
@@ -1,386 +1,386 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.324134 weblate_language_data-2024.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-25 18:01:22.000000 weblate_language_data-2024.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 18:01:22.000000 weblate_language_data-2024.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-25 18:01:33.324134 weblate_language_data-2024.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-25 18:01:22.000000 weblate_language_data-2024.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-25 18:01:33.324134 weblate_language_data-2024.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.280134 weblate_language_data-2024.4/weblate_language_data/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/ambiguous.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)   196036 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/check_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/country_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/language_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)   212087 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.280134 weblate_language_data-2024.4/weblate_language_data/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/ab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.280134 weblate_language_data-2024.4/weblate_language_data/locale/ab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152813 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.280134 weblate_language_data-2024.4/weblate_language_data/locale/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   158510 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/af/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/afh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/afh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/afh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/ang/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/ang/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ang/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   175381 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/ar_LY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   155746 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/ars/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/ars/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ars/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/ast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/ast/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163571 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/az/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/az/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167021 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/be/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/be/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   173935 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/be_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167280 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/ber/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/ber/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   157067 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ber/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.284134 weblate_language_data-2024.4/weblate_language_data/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   170605 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/bn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   170034 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/bn_BD/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   169607 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/bo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/bo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   154058 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/bo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.256133 weblate_language_data-2024.4/weblate_language_data/locale/br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/br/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167161 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/br/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163456 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/ce/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/ce/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163229 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ce/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/chn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/chn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152826 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/chn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/ckb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/ckb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   170671 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ckb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/crh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/crh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   161449 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/crh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   168577 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/cv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/cv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   159685 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/cv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/cy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.288134 weblate_language_data-2024.4/weblate_language_data/locale/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   162541 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163353 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   164873 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)   152826 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/dv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/dv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152801 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/dv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   171639 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/en_GB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163079 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/enm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/enm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/enm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   166443 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   164166 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   162556 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167881 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   169442 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.292134 weblate_language_data-2024.4/weblate_language_data/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   172459 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/fil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/fil/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163171 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/fil/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.260133 weblate_language_data-2024.4/weblate_language_data/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163274 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/fur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/fur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   159422 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/fur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/fy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/fy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167522 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/fy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/ga/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/ga/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163357 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ga/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   166864 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   168717 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   169731 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163550 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   164116 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.296134 weblate_language_data-2024.4/weblate_language_data/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   168744 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/hy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/ia/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/ia/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   159827 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ia/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   162684 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/ie/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/ie/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   153203 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ie/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/ig/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/ig/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   156237 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ig/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/is/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/is/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163297 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163653 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   181521 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   166347 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/kab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/kab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   165404 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/kab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/kk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/kk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167657 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/km/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/km/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   171360 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/kmr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.300134 weblate_language_data-2024.4/weblate_language_data/locale/kmr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   165822 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/kmr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/kn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/kn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   165989 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/kn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.264134 weblate_language_data-2024.4/weblate_language_data/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167770 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/ksh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/ksh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   168255 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ksh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/ln/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/ln/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   158757 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ln/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163752 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   162017 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/lzh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/lzh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   154373 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/lzh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/mk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/mk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   168262 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/mk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   169493 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ml/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/mr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.304134 weblate_language_data-2024.4/weblate_language_data/locale/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   178836 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/mr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   159131 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/my/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/my/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   173442 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/my/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   164860 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163972 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   158048 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/oc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/oc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   156669 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/oc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/or/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/or/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   170901 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/or/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/pa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/pa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   174974 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/pa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/pa_PK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   156894 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/peo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/peo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/peo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.308134 weblate_language_data-2024.4/weblate_language_data/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   164455 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/ps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/ps/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   161558 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ps/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163647 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.268133 weblate_language_data-2024.4/weblate_language_data/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163645 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   162967 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163323 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/ro_MD/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152812 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   174007 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/sai/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sai/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/sc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163648 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/si/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   162561 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.312134 weblate_language_data-2024.4/weblate_language_data/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167214 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/skr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/skr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   165376 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/skr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   168832 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   166340 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   171675 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   164670 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   163498 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   162511 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/ta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   178422 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/te/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   165212 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/te/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   176334 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/tlh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.316134 weblate_language_data-2024.4/weblate_language_data/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152971 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/tok/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/tok/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   152830 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/tok/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   164802 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/tt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/tt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   159280 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/tt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.272133 weblate_language_data-2024.4/weblate_language_data/locale/tzm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/tzm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   157715 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/tzm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.276134 weblate_language_data-2024.4/weblate_language_data/locale/ug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/ug/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   173523 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.276134 weblate_language_data-2024.4/weblate_language_data/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   173283 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.276134 weblate_language_data-2024.4/weblate_language_data/locale/uz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/uz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   156900 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/uz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.276134 weblate_language_data-2024.4/weblate_language_data/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   170262 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.276134 weblate_language_data-2024.4/weblate_language_data/locale/yue_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   159084 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.276134 weblate_language_data-2024.4/weblate_language_data/locale/zgh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/zgh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   178702 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/zgh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.276134 weblate_language_data-2024.4/weblate_language_data/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.320134 weblate_language_data-2024.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   169095 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.276134 weblate_language_data-2024.4/weblate_language_data/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.324134 weblate_language_data-2024.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   167771 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.324134 weblate_language_data-2024.4/weblate_language_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    25941 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/plural_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    52930 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/plurals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/population.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/rtl.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-25 18:01:23.000000 weblate_language_data-2024.4/weblate_language_data/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:01:33.324134 weblate_language_data-2024.4/weblate_language_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-25 18:01:33.000000 weblate_language_data-2024.4/weblate_language_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-25 18:01:33.000000 weblate_language_data-2024.4/weblate_language_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:01:33.000000 weblate_language_data-2024.4/weblate_language_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 18:01:33.000000 weblate_language_data-2024.4/weblate_language_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 18:01:33.000000 weblate_language_data-2024.4/weblate_language_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.929130 weblate_language_data-2024.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-29 07:37:08.929130 weblate_language_data-2024.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-29 07:37:08.929130 weblate_language_data-2024.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.885130 weblate_language_data-2024.5/weblate_language_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/ambiguous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196036 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/check_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/country_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/language_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   212091 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.885130 weblate_language_data-2024.5/weblate_language_data/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/ab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.885130 weblate_language_data-2024.5/weblate_language_data/locale/ab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152813 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.885130 weblate_language_data-2024.5/weblate_language_data/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   158510 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/af/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/afh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.885130 weblate_language_data-2024.5/weblate_language_data/locale/afh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/afh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/ang/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.885130 weblate_language_data-2024.5/weblate_language_data/locale/ang/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ang/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.885130 weblate_language_data-2024.5/weblate_language_data/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   175381 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/ar_LY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/ar_LY/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   155746 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/ars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/ars/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ars/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/ast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163571 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/az/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/az/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167021 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   173935 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/be_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/be_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167280 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.857130 weblate_language_data-2024.5/weblate_language_data/locale/ber/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/ber/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   157067 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ber/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   170605 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   170034 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/bn_BD/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   169607 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/bo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.889130 weblate_language_data-2024.5/weblate_language_data/locale/bo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   154058 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/bo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/br/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167161 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/br/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163456 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/ce/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/ce/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163229 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ce/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/chn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/chn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152826 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/chn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/ckb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/ckb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   170671 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ckb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/crh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/crh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   161449 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/crh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   168577 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/cv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/cv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   159685 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/cv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   162541 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163353 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.893130 weblate_language_data-2024.5/weblate_language_data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   164873 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)   152826 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/dv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/dv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152801 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/dv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   171639 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/en_GB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163079 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.861130 weblate_language_data-2024.5/weblate_language_data/locale/enm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/enm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/enm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   166443 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/eo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   164166 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   162556 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167881 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   169442 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   172459 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/fil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.897130 weblate_language_data-2024.5/weblate_language_data/locale/fil/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163171 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/fil/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163274 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/fur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/fur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   159422 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/fur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/fy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/fy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167522 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/fy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/ga/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/ga/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163357 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ga/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   166864 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   168717 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   169731 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163550 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   164116 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   168744 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/hy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/ia/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.901130 weblate_language_data-2024.5/weblate_language_data/locale/ia/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   159827 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ia/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   162684 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/ie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/ie/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   153203 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ie/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/ig/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/ig/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   156237 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ig/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.865130 weblate_language_data-2024.5/weblate_language_data/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163297 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163653 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   181521 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   166347 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/kab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/kab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   165404 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/kab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167657 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   171360 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/kmr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.905130 weblate_language_data-2024.5/weblate_language_data/locale/kmr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   165822 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/kmr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/kn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/kn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   165989 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/kn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167770 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/ksh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/ksh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   168255 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ksh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/ln/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/ln/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   158757 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ln/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163752 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   162017 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/lzh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/lzh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   154373 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/lzh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/mk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/mk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   168262 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/mk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   169493 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ml/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/mr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   178836 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/mr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   159131 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/my/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.909130 weblate_language_data-2024.5/weblate_language_data/locale/my/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   173442 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/my/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   164860 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.869130 weblate_language_data-2024.5/weblate_language_data/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163972 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   158048 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/oc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/oc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   156669 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/oc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/or/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/or/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   170901 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/or/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/pa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/pa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   174974 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/pa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/pa_PK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/pa_PK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   156894 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/peo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/peo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/peo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   164455 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/ps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/ps/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   161558 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ps/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.913130 weblate_language_data-2024.5/weblate_language_data/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163647 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163645 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   162931 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163286 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/ro_MD/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/ro_MD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152812 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   174007 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/sai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/sai/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152802 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sai/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/sc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/sc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163648 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/si/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   162561 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167214 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/skr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/skr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   165376 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/skr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.873130 weblate_language_data-2024.5/weblate_language_data/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.917130 weblate_language_data-2024.5/weblate_language_data/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   168832 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   166340 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   171675 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   164670 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   163498 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   162511 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   178422 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/te/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   165212 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/te/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   176334 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152971 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/tok/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/tok/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   152830 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/tok/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.921130 weblate_language_data-2024.5/weblate_language_data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   164802 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/tt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/tt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   159280 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/tt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/tzm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/tzm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   157715 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/tzm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   173523 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   173283 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/uz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/uz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   156900 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/uz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   170262 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/yue_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/yue_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   159084 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/zgh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/zgh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   178702 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/zgh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   169095 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.877130 weblate_language_data-2024.5/weblate_language_data/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   167771 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.925130 weblate_language_data-2024.5/weblate_language_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25941 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/plural_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52930 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/plurals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/rtl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 07:36:59.000000 weblate_language_data-2024.5/weblate_language_data/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:37:08.929130 weblate_language_data-2024.5/weblate_language_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-29 07:37:08.000000 weblate_language_data-2024.5/weblate_language_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-29 07:37:08.000000 weblate_language_data-2024.5/weblate_language_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:37:08.000000 weblate_language_data-2024.5/weblate_language_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 07:37:08.000000 weblate_language_data-2024.5/weblate_language_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 07:37:08.000000 weblate_language_data-2024.5/weblate_language_data.egg-info/top_level.txt
```

### Comparing `weblate_language_data-2024.4/LICENSE` & `weblate_language_data-2024.5/LICENSE`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/PKG-INFO` & `weblate_language_data-2024.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weblate-language-data
-Version: 2024.4
+Version: 2024.5
 Summary: Language definitions for Weblate
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/language-data
 Author: Michal Čihař
 Author-email: michal@weblate.org
 License: MIT
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/language-data/issues
```

### Comparing `weblate_language_data-2024.4/README.rst` & `weblate_language_data-2024.5/README.rst`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/pyproject.toml` & `weblate_language_data-2024.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/setup.cfg` & `weblate_language_data-2024.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weblate-language-data
-version = 2024.4
+version = 2024.5
 description = Language definitions for Weblate
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://weblate.org/
 author = Michal Čihař
 author_email = michal@weblate.org
 license = MIT
```

### Comparing `weblate_language_data-2024.4/setup.py` & `weblate_language_data-2024.5/setup.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/aliases.py` & `weblate_language_data-2024.5/weblate_language_data/aliases.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/check_languages.py` & `weblate_language_data-2024.5/weblate_language_data/check_languages.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/countries.py` & `weblate_language_data-2024.5/weblate_language_data/countries.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/country_codes.py` & `weblate_language_data-2024.5/weblate_language_data/country_codes.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/language_codes.py` & `weblate_language_data-2024.5/weblate_language_data/language_codes.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/languages.py` & `weblate_language_data-2024.5/weblate_language_data/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -5814,16 +5814,16 @@
     ),
     (
         "tg",
         # Translators: Language name for ISO code "tg". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
         _("Tajik"),
-        1,
-        "0",
+        2,
+        "n > 1",
     ),
     (
         "th",
         # Translators: Language name for ISO code "th". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
         _("Thai"),
```

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ab/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ab/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/af/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/af/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/afh/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/afh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ang/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ang/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ar/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ars/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ars/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ast/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/az/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/be/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ber/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ber/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/bg/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/bn/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/bo/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/bo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/br/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ca/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ce/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ce/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/chn/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/chn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ckb/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ckb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/crh/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/crh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/cs/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/cv/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/cv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/cy/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/da/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/de/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/django.pot` & `weblate_language_data-2024.5/weblate_language_data/locale/django.pot`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/dv/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/dv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/el/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/enm/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/enm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/eo/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/es/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/et/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/eu/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/fa/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/fi/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/fil/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/fil/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/fr/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/fur/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/fur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/fy/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/fy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ga/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ga/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/gl/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/he/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/hi/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/hr/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/hu/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/hy/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/hy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ia/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ia/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/id/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ie/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ie/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ig/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ig/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/is/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/it/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ja/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ka/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/kab/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/kab/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/kk/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/km/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/km/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/kmr/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/kmr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/kn/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/kn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ko/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ksh/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ksh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ln/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ln/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/lt/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/lv/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/lzh/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/lzh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/mk/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/mk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ml/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ml/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/mr/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/mr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ms/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/my/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/my/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/nb/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/nl/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/nn/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/oc/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/oc/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/or/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/or/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/pa/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/pa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/peo/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/peo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/pl/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ps/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ps/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/pt/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 # ssantos <ssantos@web.de>, 2020, 2021, 2022, 2023, 2024.
 # Dinis Medeiros <dinismedeiros@gmail.com>, 2021.
 # Hugo Carvalho <hugokarvalho@hotmail.com>, 2023.
+# Manuela Silva <mmsrs@sky.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
 "POT-Creation-Date: 2024-03-13 13:21+0100\n"
-"PO-Revision-Date: 2024-02-09 17:15+0000\n"
-"Last-Translator: ssantos <ssantos@web.de>\n"
+"PO-Revision-Date: 2024-04-28 18:28+0000\n"
+"Last-Translator: Manuela Silva <mmsrs@sky.com>\n"
 "Language-Team: Portuguese (Portugal) <https://hosted.weblate.org/projects/"
 "weblate/languages/pt_PT/>\n"
 "Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.4-dev\n"
+"X-Generator: Weblate 5.5.1\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -32,16 +33,17 @@
 #. or other variant.
 msgid "Abkhazian"
 msgstr "Abcásio"
 
 #. Translators: Language name for ISO code "abr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
+#, fuzzy
 msgid "Abron"
-msgstr ""
+msgstr "Abron"
 
 #. Translators: Language name for ISO code "ace". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Acehnese"
 msgstr "Achém"
 
@@ -68,18 +70,16 @@
 #. or other variant.
 msgid "Avestan"
 msgstr "Avestan"
 
 #. Translators: Language name for ISO code "aeb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Arabic (Libya)"
 msgid "Arabic (Tunisian)"
-msgstr "Árabe (Líbia)"
+msgstr "Árabe (Tunisino)"
 
 #. Translators: Language name for ISO code "af". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afrikaans"
 msgstr "Africânder"
 
@@ -113,29 +113,27 @@
 msgid "Akkadian"
 msgstr "Acádio"
 
 #. Translators: Language name for ISO code "ale". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Aleut"
-msgstr "aleúte"
+msgstr "Aleúte"
 
 #. Translators: Language name for ISO code "aln". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Albanian"
 msgid "Albanian (Gheg)"
 msgstr "Albanês"
 
 #. Translators: Language name for ISO code "alt". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Altai (Southern)"
-msgstr "Línguas altaicas (sul)"
+msgstr "Altai (sul)"
 
 #. Translators: Language name for ISO code "am". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Amharic"
 msgstr "Amárico"
 
@@ -145,15 +143,15 @@
 msgid "Aragonese"
 msgstr "Aragonês"
 
 #. Translators: Language name for ISO code "ang". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "English (Old)"
-msgstr "Inglês (antigo)"
+msgstr "Inglês (Antigo)"
 
 #. Translators: Language name for ISO code "anp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Angika"
 msgstr "Angika"
 
@@ -223,15 +221,15 @@
 msgid "Arabic (Yemen)"
 msgstr "Árabe (Iêmen)"
 
 #. Translators: Language name for ISO code "arc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Aramaic"
-msgstr "aramaico"
+msgstr "Aramaico"
 
 #. Translators: Language name for ISO code "arn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mapudungun"
 msgstr "Mapudungun"
 
@@ -255,21 +253,19 @@
 msgid "Arabic (Najdi)"
 msgstr "Árabe (Najdi)"
 
 #. Translators: Language name for ISO code "arw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arawak"
-msgstr "arauaqui"
+msgstr "Arauaqui"
 
 #. Translators: Language name for ISO code "arz". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Arabic (Egypt)"
 msgid "Arabic (Egyptian)"
 msgstr "Árabe (Egipto)"
 
 #. Translators: Language name for ISO code "as". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Assamese"
@@ -335,15 +331,15 @@
 msgid "Bashkir"
 msgstr "Bashkir"
 
 #. Translators: Language name for ISO code "bal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Baluchi"
-msgstr "balúchi"
+msgstr "Balúchi"
 
 #. Translators: Language name for ISO code "ban". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Balinese"
 msgstr "Balinês"
 
@@ -359,21 +355,21 @@
 msgid "Basa (Cameroon)"
 msgstr "Basa (Camarões)"
 
 #. Translators: Language name for ISO code "bbc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Batak Toba"
-msgstr ""
+msgstr "Batak Toba"
 
 #. Translators: Language name for ISO code "bci". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Baoulé"
-msgstr ""
+msgstr "Baoulé"
 
 #. Translators: Language name for ISO code "be". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Belarusian"
 msgstr "Bielorrusso"
```

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ro/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 #
 # Christian Eichert <c@zp1.net>, 2021.
 # Licaon Kter <licaon.kter@protonmail.com>, 2021, 2022, 2023, 2024.
 # Simona Iacob <s@zp1.net>, 2021, 2022, 2023.
 # Vlăduț Ilie <vladilie94@gmail.com>, 2023, 2024.
+# Nicoara Alex <alex.nicoara@yahoo.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
 "POT-Creation-Date: 2024-03-13 13:21+0100\n"
-"PO-Revision-Date: 2024-02-09 06:41+0000\n"
-"Last-Translator: Vlăduț Ilie <vladilie94@gmail.com>\n"
+"PO-Revision-Date: 2024-04-29 05:02+0000\n"
+"Last-Translator: Nicoara Alex <alex.nicoara@yahoo.com>\n"
 "Language-Team: Romanian <https://hosted.weblate.org/projects/weblate/"
 "languages/ro/>\n"
 "Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
 "20)) ? 1 : 2;\n"
-"X-Generator: Weblate 5.4-dev\n"
+"X-Generator: Weblate 5.5.1\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -71,17 +72,16 @@
 #. or other variant.
 msgid "Avestan"
 msgstr "Avestană"
 
 #. Translators: Language name for ISO code "aeb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Arabic (Tunisian)"
-msgstr "Ucrainian"
+msgstr "Arabă (Tunisiană)"
 
 #. Translators: Language name for ISO code "af". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afrikaans"
 msgstr "Afrikaans"
 
@@ -120,17 +120,16 @@
 #. or other variant.
 msgid "Aleut"
 msgstr "Aleută"
 
 #. Translators: Language name for ISO code "aln". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Albanian (Gheg)"
-msgstr "Albaneză"
+msgstr "Albaneză (Gheg)"
 
 #. Translators: Language name for ISO code "alt". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Altai (Southern)"
 msgstr "Altai (Sud)"
 
@@ -241,18 +240,16 @@
 #. or other variant.
 msgid "Arapaho"
 msgstr "Arapaho"
 
 #. Translators: Language name for ISO code "arq". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Arabic (Algeria)"
 msgid "Arabic (Algerian)"
-msgstr "Arabă (Algeria)"
+msgstr "Arabă (Algeriană)"
 
 #. Translators: Language name for ISO code "ars". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arabic (Najdi)"
 msgstr "Arabă (Najdi)"
 
@@ -261,18 +258,16 @@
 #. or other variant.
 msgid "Arawak"
 msgstr "Arawakă"
 
 #. Translators: Language name for ISO code "arz". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Arabic (Egypt)"
 msgid "Arabic (Egyptian)"
-msgstr "Arabă (Egipt)"
+msgstr "Arabă (Egipteană)"
 
 #. Translators: Language name for ISO code "as". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Assamese"
 msgstr "Asameză"
 
@@ -360,21 +355,21 @@
 msgid "Basa (Cameroon)"
 msgstr "Basa (Camerun)"
 
 #. Translators: Language name for ISO code "bbc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Batak Toba"
-msgstr ""
+msgstr "Batak Toba"
 
 #. Translators: Language name for ISO code "bci". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Baoulé"
-msgstr ""
+msgstr "Baoulé"
 
 #. Translators: Language name for ISO code "be". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Belarusian"
 msgstr "Bielorusă"
 
@@ -401,17 +396,16 @@
 #. or other variant.
 msgid "Berber"
 msgstr "Berber"
 
 #. Translators: Language name for ISO code "bew". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Betawi"
-msgstr "Baltic"
+msgstr "Betawi"
 
 #. Translators: Language name for ISO code "bez". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bena"
 msgstr "Bena"
 
@@ -426,37 +420,34 @@
 #. or other variant.
 msgid "Haryanvi"
 msgstr "haryanvi"
 
 #. Translators: Language name for ISO code "bgn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Balochi (Western)"
-msgstr "Ucrainian"
+msgstr "Balochi (Vestul)"
 
 #. Translators: Language name for ISO code "bh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bihari"
 msgstr "Bihari"
 
 #. Translators: Language name for ISO code "bhb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Bhili"
-msgstr "Caută"
+msgstr "Bhili"
 
 #. Translators: Language name for ISO code "bhi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Bhilali"
-msgstr "Thailandeză"
+msgstr "Bhilali"
 
 #. Translators: Language name for ISO code "bho". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bhojpuri"
 msgstr "Bhojpuri"
```

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ru/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sai/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sai/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sc/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sc/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/si/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sk/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/skr/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/skr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sl/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sq/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sr/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sv/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/sw/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ta/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ta/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/te/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/te/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/th/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/tlh/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/tlh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/tok/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/tok/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/tr/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/tt/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/tt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/tzm/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/tzm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/ug/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/ug/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/uk/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/uz/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/uz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/vi/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/zgh/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/zgh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po` & `weblate_language_data-2024.5/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/plural_tags.py` & `weblate_language_data-2024.5/weblate_language_data/plural_tags.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/plurals.py` & `weblate_language_data-2024.5/weblate_language_data/plurals.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data/population.py` & `weblate_language_data-2024.5/weblate_language_data/population.py`

 * *Files identical despite different names*

### Comparing `weblate_language_data-2024.4/weblate_language_data.egg-info/PKG-INFO` & `weblate_language_data-2024.5/weblate_language_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weblate-language-data
-Version: 2024.4
+Version: 2024.5
 Summary: Language definitions for Weblate
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/language-data
 Author: Michal Čihař
 Author-email: michal@weblate.org
 License: MIT
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/language-data/issues
```

### Comparing `weblate_language_data-2024.4/weblate_language_data.egg-info/SOURCES.txt` & `weblate_language_data-2024.5/weblate_language_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

