# Comparing `tmp/tryton-7.0.9.tar.gz` & `tmp/tryton-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryton-7.0.9.tar", last modified: Wed Apr 17 10:29:33 2024, max compression
+gzip compressed data, was "tryton-7.2.0.tar", last modified: Mon Apr 29 15:55:22 2024, max compression
```

## Comparing `tryton-7.0.9.tar` & `tryton-7.2.0.tar`

### file list

```diff
@@ -1,367 +1,369 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.066291 tryton-7.0.9/
--rw-r--r--   0 ced       (1000) ced       (1000)    19719 2024-04-17 10:29:30.000000 tryton-7.0.9/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-17 10:29:29.000000 tryton-7.0.9/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:39.000000 tryton-7.0.9/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:38.000000 tryton-7.0.9/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-17 10:29:33.066291 tryton-7.0.9/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:39.000000 tryton-7.0.9/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2055 2024-03-28 16:16:25.000000 tryton-7.0.9/bin/tryton
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-10-30 17:06:39.000000 tryton-7.0.9/catalan.nsh
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/darwin/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/darwin/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3255 2023-10-30 17:06:39.000000 tryton-7.0.9/darwin/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-10-30 17:06:39.000000 tryton-7.0.9/darwin/gtk-3.0/gtk.immodules
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.046292 tryton-7.0.9/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-03-03 16:24:03.000000 tryton-7.0.9/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5990 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/glossary.rst
--rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-10-30 17:06:38.000000 tryton-7.0.9/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/installation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    19246 2023-10-30 17:06:39.000000 tryton-7.0.9/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-10-30 17:06:39.000000 tryton-7.0.9/english.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-10-30 17:06:39.000000 tryton-7.0.9/farsi.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-10-30 17:06:39.000000 tryton-7.0.9/french.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-10-30 17:06:38.000000 tryton-7.0.9/german.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-02-05 16:24:27.000000 tryton-7.0.9/make-darwin-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:39.000000 tryton-7.0.9/make-win32-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-30 17:06:39.000000 tryton-7.0.9/portuguese.nsh
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4583 2024-04-12 21:56:05.000000 tryton-7.0.9/setup-freeze.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-17 10:29:33.066291 tryton-7.0.9/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-10-30 17:06:39.000000 tryton-7.0.9/setup.nsi
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4471 2024-03-03 16:24:03.000000 tryton-7.0.9/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-10-30 17:06:38.000000 tryton-7.0.9/slovenian.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1095 2023-10-30 17:06:39.000000 tryton-7.0.9/spanish.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-10-30 17:06:39.000000 tryton-7.0.9/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.046292 tryton-7.0.9/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)     1926 2024-04-04 07:40:11.000000 tryton-7.0.9/tryton/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.046292 tryton-7.0.9/tryton/action/
--rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/action/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6758 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/action/main.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2874 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3323 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/client.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/common/
--rw-r--r--   0 ced       (1000) ced       (1000)     2446 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2023-12-10 21:35:03.000000 tryton-7.0.9/tryton/common/button.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6611 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrendererbinary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrendererbutton.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrendererclickablepixbuf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrenderercombo.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrendererfloat.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/common/cellrendererinteger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrenderertext.py
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/cellrenderertoggle.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46739 2024-03-22 17:55:23.000000 tryton-7.0.9/tryton/common/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3018 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/completion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20371 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/datetime_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-02-29 11:44:54.000000 tryton-7.0.9/tryton/common/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    29157 2024-02-10 10:23:40.000000 tryton-7.0.9/tryton/common/domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/common/entry_position.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/environment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/focus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/htmltextbuffer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3644 2024-01-08 10:54:03.000000 tryton-7.0.9/tryton/common/number_entry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/popup_menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/richtext.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8414 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/common/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/common/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/underline.py
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/common/widget_style.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9219 2024-03-28 16:16:27.000000 tryton-7.0.9/tryton/config.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/bg/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     8720 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21782 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/ca/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19513 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20686 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/cs/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     4634 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18114 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/de/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    20063 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21253 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/es/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19796 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21178 2023-10-30 17:06:38.000000 tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/es_419/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7108 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    16239 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/et/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    13478 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18791 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/fa/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16677 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    22692 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/fi/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    13894 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/fi/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/fr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    20251 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21375 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/hu/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17161 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20782 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/id/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     6983 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    15755 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/it/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15005 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19686 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/ja_JP/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    36736 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.039626 tryton-7.0.9/tryton/data/locale/lo/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18359 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    27264 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/lt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16199 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20775 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/nl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.049625 tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19315 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20414 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/pl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17530 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20107 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/pt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15086 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20284 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/ro/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19246 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20482 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/ru/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     9949 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    22266 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/sl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18946 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20016 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/tr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     1696 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    14431 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/tryton.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13615 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/tryton.pot
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/uk/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    22964 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    25044 2023-12-27 10:44:39.000000 tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/locale/zh_CN/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.052959 tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18164 2024-04-17 10:29:26.000000 tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19261 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/tryton/data/pixmaps/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.056292 tryton-7.0.9/tryton/data/pixmaps/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-add.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-archive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-attach.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-back.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-barcode-scanner.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-bookmark.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-cancel.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-clear.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-copy.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-create.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-date.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-delete.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-download.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-drag.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-email.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-error.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-exit.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-export.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-filter.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-bold.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-italic.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-format-underline.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-forward.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-history.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-icon.png
--rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-icon.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-import.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-info.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-launch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-link.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-log.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-menu.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-note.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-ok.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-print.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-public.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-question.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-refresh.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-remove.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-save.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-search.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-send.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-sound-off.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-sound-on.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-star-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-star.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-switch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-translate.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-unarchive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-undo.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      200 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-warning.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    26698 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.icns
--rw-r--r--   0 ced       (1000) ced       (1000)    62686 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.ico
--rw-r--r--   0 ced       (1000) ced       (1000)     1603 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.056292 tryton-7.0.9/tryton/data/sounds/
--rw-r--r--   0 ced       (1000) ced       (1000)    18650 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/sounds/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    25190 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/sounds/danger.wav
--rw-r--r--   0 ced       (1000) ced       (1000)    47812 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/data/sounds/success.wav
--rw-r--r--   0 ced       (1000) ced       (1000)     1879 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/device_cookie.py
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1388 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/fingerprints.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.056292 tryton-7.0.9/tryton/gui/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    42407 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/main.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1726 2024-04-17 10:29:29.000000 tryton-7.0.9/tryton/gui/window/about.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/board.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3495 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/code_scanner.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30052 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/dblogin.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13574 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    34445 2024-04-12 20:15:11.000000 tryton-7.0.9/tryton/gui/window/form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/infobar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/limit.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3646 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1673 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/nomodal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/preference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/revision.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/tabcontent.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_board/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_board/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5502 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_board/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_board/view_board.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/model/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    44068 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/model/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18228 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/model/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27092 2024-02-10 10:27:39.000000 tryton-7.0.9/tryton/gui/window/view_form/model/record.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/screen/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/screen/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    52434 2024-03-25 21:58:10.000000 tryton-7.0.9/tryton/gui/window/view_form/screen/screen.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6078 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.059625 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9781 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22953 2024-02-05 00:30:16.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8334 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5951 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6598 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/checkbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22073 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/dictionary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3984 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/image.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12808 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14428 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22966 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1397 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/progressbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7436 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/state_widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-01-08 10:54:03.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/textbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5102 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/url.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10682 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/bar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15976 2024-04-12 21:12:01.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/graph.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/pie.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51037 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6984 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list_form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13785 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/editabletree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    50474 2024-03-22 17:55:23.000000 tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25839 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/view_form/view/screen_container.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13513 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/win_csv.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21205 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/gui/window/win_export.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19456 2024-04-12 22:39:54.000000 tryton-7.0.9/tryton/gui/window/win_form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9387 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/win_import.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/win_search.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/gui/window/window.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14885 2024-01-12 13:56:12.000000 tryton-7.0.9/tryton/gui/window/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13612 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/jsonrpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/plugins/
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/plugins/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/plugins/translation/
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/plugins/translation/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22106 2024-04-12 20:33:48.000000 tryton-7.0.9/tryton/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4903 2024-02-05 16:24:27.000000 tryton-7.0.9/tryton/rpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/test_common.py
--rw-r--r--   0 ced       (1000) ced       (1000)    43500 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/test_common_domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/test_common_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton/tests/test_common_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6659 2023-11-15 17:10:10.000000 tryton-7.0.9/tryton/translate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-10-30 17:06:39.000000 tryton-7.0.9/tryton.desktop
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/tryton.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-17 10:29:32.000000 tryton-7.0.9/tryton.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    10918 2024-04-17 10:29:33.000000 tryton-7.0.9/tryton.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:29:32.000000 tryton-7.0.9/tryton.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:28.000000 tryton-7.0.9/tryton.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-17 10:29:32.000000 tryton-7.0.9/tryton.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        7 2024-04-17 10:29:32.000000 tryton-7.0.9/tryton.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.042959 tryton-7.0.9/win32/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:29:33.062958 tryton-7.0.9/win32/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-10-30 17:06:39.000000 tryton-7.0.9/win32/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)        0 2023-10-30 17:06:39.000000 tryton-7.0.9/win32/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.139330 tryton-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19169 2024-04-29 15:30:59.000000 tryton-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-29 15:30:59.000000 tryton-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 tryton-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-02-04 18:51:26.000000 tryton-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-29 15:55:22.135997 tryton-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-04-15 07:12:15.000000 tryton-7.2.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2055 2024-03-17 11:01:36.000000 tryton-7.2.0/bin/tryton
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-01-16 14:00:21.000000 tryton-7.2.0/catalan.nsh
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/darwin/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/darwin/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3255 2023-01-16 14:00:21.000000 tryton-7.2.0/darwin/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-01-16 14:00:21.000000 tryton-7.2.0/darwin/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-04-27 16:30:39.000000 tryton-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5990 2023-04-15 07:12:15.000000 tryton-7.2.0/doc/glossary.rst
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 tryton-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:15.000000 tryton-7.2.0/doc/installation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 tryton-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-02-04 18:51:27.000000 tryton-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    19223 2024-04-27 16:30:39.000000 tryton-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-01-16 14:00:21.000000 tryton-7.2.0/english.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-01-16 14:00:21.000000 tryton-7.2.0/farsi.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-01-16 14:00:21.000000 tryton-7.2.0/french.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-01-16 14:00:21.000000 tryton-7.2.0/german.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2024-04-22 12:14:36.000000 tryton-7.2.0/make-darwin-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 tryton-7.2.0/make-win32-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-01-16 14:00:21.000000 tryton-7.2.0/portuguese.nsh
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4571 2024-04-29 13:17:17.000000 tryton-7.2.0/setup-freeze.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-29 15:55:22.139330 tryton-7.2.0/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-04-15 07:12:15.000000 tryton-7.2.0/setup.nsi
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4471 2024-04-27 16:30:39.000000 tryton-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-01-16 14:00:21.000000 tryton-7.2.0/slovenian.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1095 2023-01-16 14:00:21.000000 tryton-7.2.0/spanish.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2024-03-17 11:01:36.000000 tryton-7.2.0/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.119331 tryton-7.2.0/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1926 2024-04-29 15:30:54.000000 tryton-7.2.0/tryton/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.119331 tryton-7.2.0/tryton/action/
+-rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/action/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6758 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/action/main.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2874 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      990 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3323 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/client.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/common/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2446 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/common/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2024-04-22 12:01:28.000000 tryton-7.2.0/tryton/common/button.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6611 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/common/cellrendererbinary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrendererbutton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/common/cellrendererclickablepixbuf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrenderercombo.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrendererfloat.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrendererinteger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrenderertext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrenderertoggle.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    49195 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/common/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3035 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/common/completion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20394 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/common/datetime_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/common/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    29157 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/common/domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/common/entry_position.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/common/environment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/focus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/htmltextbuffer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3644 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/common/number_entry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/common/popup_menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/richtext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8538 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/common/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      766 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/common/tempfile.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/underline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/common/widget_style.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9270 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/config.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/tryton/data/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/bg/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8720 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22191 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/ca/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19439 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21181 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/cs/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4634 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18523 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/de/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19988 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21762 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/es/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19720 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21683 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/es_419/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7060 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    16689 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/et/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13450 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19223 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/fa/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16677 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    23114 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/fi/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    14303 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/fi/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/fr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    20364 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21907 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/hu/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17126 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21213 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/id/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6983 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    16252 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/it/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15005 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20145 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/ja_JP/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    36736 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/lo/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18359 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    27674 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/lt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16169 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21211 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/nl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19339 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20912 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/pl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17502 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20594 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/pt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15086 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20696 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/ro/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19655 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21097 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/ru/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9949 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22633 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/sl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18877 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20515 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/tr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1696 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    14840 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/tryton.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14091 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/tryton.pot
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/uk/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    22925 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    25573 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/zh_CN/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18082 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19744 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/tryton/data/pixmaps/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.129330 tryton-7.2.0/tryton/data/pixmaps/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-add.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-archive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-attach.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-back.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-02-04 18:51:26.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-barcode-scanner.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-bookmark.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-cancel.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-clear.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-copy.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-create.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-date.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-delete.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-download.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-drag.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-email.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-error.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-exit.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-export.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-filter.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-bold.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-italic.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-underline.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-forward.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-history.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-icon.png
+-rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-icon.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-import.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-info.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-launch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-link.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-log.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-menu.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-note.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-ok.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-print.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-public.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-question.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-refresh.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-remove.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-save.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-search.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-send.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-sound-off.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-sound-on.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-star-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-star.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-switch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-translate.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-unarchive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-undo.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      200 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-warning.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    26698 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.icns
+-rw-r--r--   0 ced       (1000) ced       (1000)    62686 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.ico
+-rw-r--r--   0 ced       (1000) ced       (1000)     1603 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.129330 tryton-7.2.0/tryton/data/sounds/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18650 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/sounds/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    25190 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/sounds/danger.wav
+-rw-r--r--   0 ced       (1000) ced       (1000)    47812 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/sounds/success.wav
+-rw-r--r--   0 ced       (1000) ced       (1000)     1889 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/device_cookie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1388 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/fingerprints.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.129330 tryton-7.2.0/tryton/gui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    42451 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/main.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2024-04-29 15:30:59.000000 tryton-7.2.0/tryton/gui/window/about.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/board.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3495 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/code_scanner.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30067 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/gui/window/dblogin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13577 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    34496 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/infobar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/limit.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4568 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1673 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/nomodal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/preference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/revision.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/tabcontent.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_board/
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_board/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5502 2024-04-13 15:40:11.000000 tryton-7.2.0/tryton/gui/window/view_board/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_board/view_board.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    44900 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/model/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18391 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/model/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    28847 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/model/record.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/screen/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/screen/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    53483 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/screen/screen.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6078 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9781 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22623 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8334 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5951 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6525 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/checkbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22276 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/dictionary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3984 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/image.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12987 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14507 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23379 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1397 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/progressbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-05-30 16:04:29.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7600 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/state_widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/textbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5102 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/url.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10682 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/bar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15976 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/graph.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/pie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51754 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6984 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list_form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13835 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/editabletree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51643 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25839 2024-02-22 09:33:24.000000 tryton-7.2.0/tryton/gui/window/view_form/view/screen_container.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13513 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/win_csv.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21199 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/gui/window/win_export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19456 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/win_form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9601 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/win_import.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/win_search.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/window.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14972 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13986 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/jsonrpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/plugins/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1449 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/plugins/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/plugins/translation/
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/plugins/translation/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23751 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/rpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-06-10 11:39:56.000000 tryton-7.2.0/tryton/tests/test_common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    43500 2024-04-13 15:19:53.000000 tryton-7.2.0/tryton/tests/test_common_domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/tests/test_common_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/tests/test_common_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6659 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/translate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton.desktop
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-29 15:55:21.000000 tryton-7.2.0/tryton.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    10960 2024-04-29 15:55:22.000000 tryton-7.2.0/tryton.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:55:21.000000 tryton-7.2.0/tryton.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 tryton-7.2.0/tryton.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:55:21.000000 tryton-7.2.0/tryton.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        7 2024-04-29 15:55:21.000000 tryton-7.2.0/tryton.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/win32/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/win32/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-01-16 14:00:21.000000 tryton-7.2.0/win32/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)        0 2023-01-16 14:00:21.000000 tryton-7.2.0/win32/gtk-3.0/gtk.immodules
```

### Comparing `tryton-7.0.9/CHANGELOG` & `tryton-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,17 @@
 
-Version 7.0.9 - 2024-04-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.8 - 2024-04-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.7 - 2024-03-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.6 - 2024-02-15
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
-Version 7.0.2 - 2023-11-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2023-11-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
+* Read xxx2Many fields using the dotted notation
+* Display XML ID on Log window
+* Use operators when converting PYSON to string
+* Add contextual menu to copy cell and column
+* Allow resetting forgotten password
+* Clean temporary files and directories at exit
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Support create record from autocomplete
 * Support scanning code
```

### Comparing `tryton-7.0.9/COPYRIGHT` & `tryton-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/LICENSE` & `tryton-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/PKG-INFO` & `tryton-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 7.0.9
+Version: 7.2.0
 Summary: Tryton desktop client
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/latest/client-desktop/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
```

### Comparing `tryton-7.0.9/bin/tryton` & `tryton-7.2.0/bin/tryton`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/catalan.nsh` & `tryton-7.2.0/catalan.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/darwin/gtk-3.0/gdk-pixbuf.loaders` & `tryton-7.2.0/darwin/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/darwin/gtk-3.0/gtk.immodules` & `tryton-7.2.0/darwin/gtk-3.0/gtk.immodules`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/doc/conf.py` & `tryton-7.2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/doc/glossary.rst` & `tryton-7.2.0/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/doc/installation.rst` & `tryton-7.2.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/doc/usage.rst` & `tryton-7.2.0/doc/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -442,16 +442,16 @@
 The Syntax
 ++++++++++
 
 A query is composed of search clauses.
 A clause is composed of a field name (with ``:`` at the end), an operator and a
 value.
 The field name is optional and defaults to the record name.
-The operator is also optional and defaults to ``like`` or ``equal`` depending
-on the type of the field.
+The operator is also optional and defaults to ``ilike`` or ``=`` depending on
+the type of the field.
 The default operator is ``=`` except for fields of type ``char``, ``text`` and
 ``many2one`` which is ``ilike``.
 
 Field Names
 +++++++++++
 
 All field names shown in the :term:`tree view` can be searched. Field names
@@ -475,18 +475,14 @@
    * ``>``: greater then
    * ``>=``: greater then or equal to
    * ``!=``: not equal
    * ``!``: not equal or not like (depending of the type of field)
 
    For example: ``Name: != Dwight``
 
-.. note::
-   The ``ilike`` operator is never explicit and ``%`` is appended to the value
-   to make it behaves like ``starts with``.
-
 Values
 ++++++
 
 The format of the value depends on the type of the field.
 A list of values can be set using ``;`` as separator.
 
    For example: ``Name: Michael; Pam``
@@ -502,20 +498,25 @@
    included.
 
 There are two wildcards:
 
    * ``%``: matches any string of zero or more characters.
    * ``_``: matches any single character.
 
-It is possible to escape special characters in values by using double quotes.
+It is possible to escape special characters in values by using double quotes or
+prepending ``\\``.
 
    For example: ``Name: "Michael:Scott"``
 
    Here it will search with the value ``Michael:Scott``.
 
+   Or: ``Name: Michael\\_Scott``
+
+   Here it will search with the value ``Michael\_Scott``.
+
 Clause composition
 ++++++++++++++++++
 
 The clauses can be composed using the two boolean operators ``&`` (for `logical
 conjunction`_) and ``|`` (for `logical disjunction`_).
 By default, there is an implicit ``&`` between each clause if no operator is
 specified.
```

### Comparing `tryton-7.0.9/english.nsh` & `tryton-7.2.0/english.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/farsi.nsh` & `tryton-7.2.0/farsi.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/french.nsh` & `tryton-7.2.0/french.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/german.nsh` & `tryton-7.2.0/german.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/portuguese.nsh` & `tryton-7.2.0/portuguese.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/setup-freeze.py` & `tryton-7.2.0/setup-freeze.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,22 +120,21 @@
 version = Popen(
     'python3 ./setup.py --version', stdout=PIPE, shell=True, encoding='utf-8'
     ).stdout.read()
 version = version.strip()
 
 setup(name='tryton',
     version=version,
-    packages=find_packages(),
     options={
         'build_exe': {
             'no_compress': True,
             'include_files': include_files,
             'excludes': ['tkinter'],
             'silent': True,
-            'packages': ['gi'],
+            'packages': find_packages() + ['gi'],
             'include_msvcr': True,
             },
         'bdist_mac': {
             'iconfile': os.path.join(
                 'tryton', 'data', 'pixmaps', 'tryton', 'tryton.icns'),
             'bundle_name': 'Tryton',
             }
```

### Comparing `tryton-7.0.9/setup.nsi` & `tryton-7.2.0/setup.nsi`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/setup.py` & `tryton-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/slovenian.nsh` & `tryton-7.2.0/slovenian.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/spanish.nsh` & `tryton-7.2.0/spanish.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/__init__.py` & `tryton-7.2.0/tryton/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-__version__ = "7.0.9"
+__version__ = "7.2.0"
 import locale
 
 import gi
 
 gi.require_version('Gtk', '3.0')
 gi.require_version('Gdk', '3.0')
 gi.require_foreign('cairo')
```

### Comparing `tryton-7.0.9/tryton/action/main.py` & `tryton-7.2.0/tryton/action/main.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/bus.py` & `tryton-7.2.0/tryton/bus.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/client.py` & `tryton-7.2.0/tryton/client.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/__init__.py` & `tryton-7.2.0/tryton/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/button.py` & `tryton-7.2.0/tryton/common/button.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/cellrendererbinary.py` & `tryton-7.2.0/tryton/common/cellrendererbinary.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/cellrendererbutton.py` & `tryton-7.2.0/tryton/common/cellrendererbutton.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/cellrendererclickablepixbuf.py` & `tryton-7.2.0/tryton/common/cellrendererclickablepixbuf.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/cellrendererfloat.py` & `tryton-7.2.0/tryton/common/cellrendererfloat.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/cellrendererinteger.py` & `tryton-7.2.0/tryton/common/cellrendererinteger.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/cellrenderertext.py` & `tryton-7.2.0/tryton/common/cellrenderertext.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/common.py` & `tryton-7.2.0/tryton/common/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
+import base64
 import colorsys
+import concurrent.futures
 import gettext
 import locale
 import logging
 import os
 import platform
 import re
 import subprocess
-import tempfile
 import unicodedata
 import xml.etree.ElementTree as ET
-from collections import defaultdict
+from collections import OrderedDict, defaultdict
 from decimal import Decimal
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from pathlib import PurePath
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 
 try:
     from http import HTTPStatus
@@ -27,121 +28,119 @@
 import socket
 import sys
 import traceback
 import urllib.error
 import urllib.parse
 import urllib.request
 import webbrowser
-from functools import lru_cache, wraps
+from functools import wraps
 from string import Template
 from threading import Lock, Thread
 
 import tryton.rpc as rpc
+from tryton.cache import CacheDict
 from tryton.config import CONFIG, PIXMAPS_DIR, SOUNDS_DIR, TRYTON_ICON
 
 try:
     import ssl
 except ImportError:
     ssl = None
 import zipfile
 
 from gi.repository import Gdk, GdkPixbuf, Gio, GLib, GObject, Gtk
 
 from tryton import __version__
 from tryton.exceptions import TrytonError, TrytonServerError
 from tryton.pyson import PYSONEncoder
 
+from . import tempfile
 from .underline import set_underline
 from .widget_style import widget_class
 
 _ = gettext.gettext
 logger = logging.getLogger(__name__)
 
 
 class IconFactory:
 
     batchnum = 10
-    _tryton_icons = []
-    _name2id = {}
+    _name2id = OrderedDict()
     _icons = {}
     _local_icons = {}
     _pixbufs = defaultdict(dict)
+    _url_pixbufs = CacheDict(cache_len=CONFIG['image.cache_size'])
+    _empty_pixbufs = {}
+    _empty_gif = base64.b64decode(
+        'R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7')
+    _executor = concurrent.futures.ThreadPoolExecutor(max_workers=5)
 
     @classmethod
     def load_local_icons(cls):
         for fname in os.listdir(PIXMAPS_DIR):
             name = os.path.splitext(fname)[0]
             path = os.path.join(PIXMAPS_DIR, fname)
             cls._local_icons[name] = path
 
     @classmethod
     def load_icons(cls, refresh=False):
-        if not refresh:
-            cls._name2id.clear()
-            cls._icons.clear()
-        del cls._tryton_icons[:]
-
         try:
             icons = rpc.execute('model', 'ir.ui.icon', 'list_icons',
                 rpc.CONTEXT)
         except TrytonServerError:
             icons = []
-        for icon_id, icon_name in icons:
-            if refresh and icon_name in cls._icons:
-                continue
-            cls._tryton_icons.append((icon_id, icon_name))
-            cls._name2id[icon_name] = icon_id
+        cls._name2id = name2id = OrderedDict((n, i) for i, n in icons)
+        if not refresh:
+            cls._icons.clear()
+        return name2id
 
     @classmethod
-    def register_icon(cls, iconname):
-        # iconname might be '' when page do not define icon
-        if (not iconname
-                or iconname in cls._icons
-                or iconname in cls._local_icons):
-            return
-        if iconname not in cls._name2id:
-            cls.load_icons(refresh=True)
-        try:
-            icon_ref = (cls._name2id[iconname], iconname)
-        except KeyError:
-            logger.error(f"Unknown icon {iconname}")
-            cls._icons[iconname] = None
-            return
-        idx = cls._tryton_icons.index(icon_ref)
-        to_load = slice(max(0, idx - cls.batchnum // 2),
+    def _get_icon(cls, iconname):
+        data = cls._icons.get(iconname)
+        if data is not None:
+            return data
+        path = cls._local_icons.get(iconname)
+        if path is not None:
+            with open(path, 'rb') as fp:
+                return fp.read()
+
+        name2id = cls._name2id
+        if iconname not in name2id:
+            name2id = cls.load_icons(refresh=True)
+            if iconname not in name2id:
+                logger.error(f"Unknown icon {iconname}")
+                cls._icons[iconname] = None
+                return
+        names = [n for n in name2id if n not in cls._icons or n == iconname]
+        idx = names.index(iconname)
+        to_load = slice(
+            max(0, idx - cls.batchnum // 2),
             idx + cls.batchnum // 2)
-        ids = [e[0] for e in cls._tryton_icons[to_load]]
+        ids = [name2id[n] for n in names[to_load]]
         try:
             icons = rpc.execute('model', 'ir.ui.icon', 'read', ids,
                 ['name', 'icon'], rpc.CONTEXT)
         except TrytonServerError:
             icons = []
+        data = None
         for icon in icons:
             name = icon['name']
-            data = icon['icon'].encode('utf-8')
-            cls._icons[name] = data
-            cls._tryton_icons.remove((icon['id'], icon['name']))
-            del cls._name2id[icon['name']]
+            icondata = icon['icon'].encode('utf-8')
+            cls._icons[name] = icondata
+            if name == iconname:
+                data = icondata
+        return data
 
     @classmethod
     def get_pixbuf(cls, iconname, size=16, color=None, badge=None):
         if not iconname:
             return
         colors = CONFIG['icon.colors'].split(',')
-        cls.register_icon(iconname)
         if iconname not in cls._pixbufs[(size, badge)]:
-            data = None
-            if iconname in cls._icons:
-                data = cls._icons[iconname]
-            elif iconname in cls._local_icons:
-                path = cls._local_icons[iconname]
-                with open(path, 'rb') as fp:
-                    data = fp.read()
+            data = cls._get_icon(iconname)
             if not data:
-                logger.error("Unknown icon %s" % iconname)
                 return
             if not color:
                 color = colors[0]
             try:
                 ET.register_namespace('', 'http://www.w3.org/2000/svg')
                 root = ET.fromstring(data)
                 root.attrib['fill'] = color
@@ -195,24 +194,48 @@
         if size_param:
             query = urllib.parse.parse_qsl(parts[4])
             query.append((size_param, size))
             parts[4] = urllib.parse.urlencode(query)
         return urllib.parse.urlunsplit(parts)
 
     @classmethod
-    @lru_cache(maxsize=CONFIG['image.cache_size'])
-    def get_pixbuf_url(cls, url, size=16, size_param=None):
+    def _get_pixbuf_url(cls, url, size=16):
         if not url:
             return
-        url = cls._convert_url(url, size, size_param=size_param)
+        pixbuf = None
+        logger.info(f'GET {url}')
         try:
             with urllib.request.urlopen(url) as response:
-                return data2pixbuf(response.read(), size, size)
+                pixbuf = data2pixbuf(response.read(), size, size)
         except urllib.error.URLError:
             logger.info("Can not fetch %s", url, exc_info=True)
+        cls._url_pixbufs[url] = pixbuf
+        return pixbuf
+
+    @classmethod
+    def get_pixbuf_url(cls, url, size=16, size_param=None, callback=None):
+        if not url:
+            return
+
+        url = cls._convert_url(url, size, size_param=size_param)
+        pixbuf = cls._url_pixbufs.get(url)
+        if pixbuf is not None:
+            return pixbuf
+
+        if callback:
+            def fetch(url, size):
+                pixbuf = cls._get_pixbuf_url(url, size)
+                GLib.idle_add(lambda: callback(pixbuf))
+            cls._executor.submit(fetch, url, size)
+            if size not in cls._empty_pixbufs:
+                cls._empty_pixbufs[size] = _data2pixbuf(
+                    cls._empty_gif, size, size)
+            return cls._empty_pixbufs[size]
+        else:
+            return cls._get_pixbuf_url(url, size, size_param)
 
 
 IconFactory.load_local_icons()
 
 
 class ModelAccess(object):
 
@@ -225,29 +248,36 @@
             self._access.clear()
         del self._models[:]
 
         try:
             self._models = rpc.execute('model', 'ir.model', 'list_models',
                 rpc.CONTEXT)
         except TrytonServerError:
-            pass
+            logger.error("Unable to get model list.")
 
     def __getitem__(self, model):
         if model in self._access:
             return self._access[model]
         if model not in self._models:
             self.load_models(refresh=True)
         idx = self._models.index(model)
         to_load = slice(max(0, idx - self.batchnum // 2),
             idx + self.batchnum // 2)
         try:
             access = rpc.execute('model', 'ir.model.access', 'get_access',
                 self._models[to_load], rpc.CONTEXT)
         except TrytonServerError:
-            access = {}
+            logger.error("Unable to get access for %s.", model)
+            access = {
+                model: {
+                    'read': True,
+                    'write': False,
+                    'create': False,
+                    'delete': False},
+                }
         self._access.update(access)
         return self._access[model]
 
 
 MODELACCESS = ModelAccess()
 
 
@@ -795,15 +825,15 @@
 class ConcurrencyDialog(UniqueDialog):
 
     def build_dialog(self, parent):
         tooltips = Tooltips()
         dialog = Gtk.MessageDialog(
             transient_for=parent, modal=True, destroy_with_parent=True,
             message_type=Gtk.MessageType.QUESTION,
-            buttons=Gtk.ButtonsType.NONE, text=_('Concurrency Exception'))
+            buttons=Gtk.ButtonsType.NONE, text=_("Concurrency Warning"))
         dialog.format_secondary_text(
             _('This record has been modified while you were editing it.'))
         cancel_button = dialog.add_button(
             set_underline(_("Cancel")), Gtk.ResponseType.CANCEL)
         tooltips.set_tip(cancel_button, _('Cancel saving'))
         compare_button = dialog.add_button(
             set_underline(_("Compare")), Gtk.ResponseType.APPLY)
@@ -840,42 +870,47 @@
 
 class ErrorDialog(UniqueDialog):
 
     def build_dialog(self, parent, title, details):
         dialog = Gtk.MessageDialog(
             transient_for=parent, modal=True, destroy_with_parent=True,
             message_type=Gtk.MessageType.ERROR, buttons=Gtk.ButtonsType.NONE)
-        dialog.set_default_size(600, 400)
+        dialog.set_default_size(600, 200)
         dialog.set_position(Gtk.WindowPosition.CENTER)
 
         dialog.add_button(set_underline(_("Close")), Gtk.ResponseType.CANCEL)
         dialog.set_default_response(Gtk.ResponseType.CANCEL)
 
         dialog.set_markup(
             '<b>%s</b>' % GLib.markup_escape_text(_('Application Error')))
         dialog.format_secondary_markup(
             '<b>%s</b>' % GLib.markup_escape_text(title))
 
         scrolledwindow = Gtk.ScrolledWindow()
         scrolledwindow.set_policy(
             Gtk.PolicyType.AUTOMATIC, Gtk.PolicyType.AUTOMATIC)
         scrolledwindow.set_shadow_type(Gtk.ShadowType.NONE)
+        scrolledwindow.set_min_content_height(300)
 
         viewport = Gtk.Viewport()
         viewport.set_shadow_type(Gtk.ShadowType.NONE)
 
         textview = Gtk.TextView(editable=False, sensitive=True, monospace=True)
         buf = Gtk.TextBuffer()
         buf.set_text(details)
         textview.set_buffer(buf)
 
         viewport.add(textview)
         scrolledwindow.add(viewport)
+        expander = Gtk.Expander()
+        expander.set_label(_("Details"))
+        expander.add(scrolledwindow)
+        expander.set_resize_toplevel(True)
         dialog.vbox.pack_start(
-            scrolledwindow, expand=True, fill=True, padding=0)
+            expander, expand=False, fill=True, padding=0)
 
         button_roundup = Gtk.LinkButton.new_with_label(
             CONFIG['bug.url'], _("Report Bug"))
         button_roundup.get_child().set_halign(Gtk.Align.START)
         button_roundup.connect('activate-link',
             lambda widget: webbrowser_open(CONFIG['bug.url'], new=2))
         dialog.vbox.pack_start(
@@ -969,18 +1004,21 @@
     rpc_execute = kwargs.get('rpc_execute', rpc.execute)
 
     if isinstance(exception, TrytonServerError):
         if exception.faultCode == 'UserWarning':
             name, msg, description = exception.args
             res = userwarning(description, msg)
             if res in ('always', 'ok'):
-                RPCExecute(
-                    'model', 'res.user.warning', 'skip',
-                    name, (res == 'always'),
-                    process_exception=False)
+                try:
+                    RPCExecute(
+                        'model', 'res.user.warning', 'skip',
+                        name, (res == 'always'),
+                        process_exception=False)
+                except RPCException:
+                    pass
                 return rpc_execute(*args)
         elif exception.faultCode == 'UserError':
             msg, description, domain = exception.args
             if domain:
                 domain, fields = domain
                 domain_parser = DomainParser(fields)
                 if domain_parser.stringable(domain):
@@ -1010,20 +1048,19 @@
                             msg_type=Gtk.MessageType.ERROR)
                     Main().on_quit()
                     sys.exit()
                 finally:
                     PLOCK.release()
                 if args:
                     return rpc_execute(*args)
-        elif exception.faultCode == str(int(HTTPStatus.TOO_MANY_REQUESTS)):
+        elif exception.faultCode in map(str, HTTPStatus):
+            err_msg = '[%s] %s' % (exception.faultCode, exception.faultString)
             message(
-                _('Too many requests. Try again later.'),
+                _('Error: "%s". Try again later.') % err_msg,
                 msg_type=Gtk.MessageType.ERROR)
-        elif exception.faultCode == str(int(HTTPStatus.NOT_FOUND)):
-            message(_("Not found."), msg_type=Gtk.MessageType.ERROR)
         else:
             error(exception, exception.faultString)
     else:
         error(exception, traceback.format_exc())
     raise RPCException(exception)
 
 
@@ -1100,29 +1137,52 @@
                 elif (exception.faultCode
                         == str(int(HTTPStatus.NOT_FOUND))):
                     message(_("Not Found."), msg_type=Gtk.MessageType.ERROR)
                     raise TrytonError('QueryCanceled')
                 if exception.faultCode != 'LoginException':
                     raise
                 name, msg, type = exception.args
-                value = getattr(self, 'get_%s' % type)(msg)
+                value = getattr(self, 'get_%s' % type)(msg, name)
                 if value is None:
                     raise TrytonError('QueryCanceled')
                 parameters[name] = value
                 continue
             else:
                 return
 
     @classmethod
-    def get_char(cls, message):
+    def get_char(cls, message, name):
         return ask(message)
 
     @classmethod
-    def get_password(cls, message):
-        return ask(message, visibility=False)
+    def get_password(cls, message_, name):
+        class AskPasswordDialog(AskDialog):
+            def build_dialog(self, *args, **kwargs):
+                tooltips = Tooltips()
+                dialog = super().build_dialog(*args, **kwargs)
+                box = dialog.get_message_area()
+                button = Gtk.Button.new_with_label(
+                    _("Reset forgotten password"))
+                button.set_alignment(0, 0.5)
+                button.set_relief(Gtk.ReliefStyle.NONE)
+                tooltips.set_tip(
+                    button, _("Send you an email to reset your password."))
+                button.connect('clicked', self.reset_password)
+                box.pack_start(button, False, False, 0)
+                return dialog
+
+            def reset_password(self, button):
+                rpc.reset_password()
+                message(
+                    _("A request to reset your password has been sent.\n"
+                        "Please check your mailbox."))
+                self.entry.grab_focus()
+        if name == 'password':
+            ask = AskPasswordDialog()
+        return ask(message_, visibility=False)
 
 
 class Logout:
     def __init__(self):
         try:
             rpc.logout()
         except TrytonServerError:
@@ -1250,15 +1310,15 @@
                 return process_exception(
                     self.exception, *self.args, rpc_execute=rpc_execute)
             except RPCException as exception:
                 self.exception = exception
 
         def return_():
             if self.exception:
-                raise self.exception
+                raise RPCException(self.exception)
             else:
                 return self.res
 
         if self.callback:
             self.callback(return_)
         else:
             return return_()
@@ -1271,28 +1331,33 @@
     args = args + (rpc_context,)
     process_exception = kwargs.get('process_exception', True)
     callback = kwargs.get('callback')
     return RPCProgress('execute', args).run(process_exception, callback)
 
 
 def RPCContextReload(callback=None):
+    def clean(context):
+        return {
+            k: v for k, v in context.items()
+            if k != 'locale' and not k.endswith('.rec_name')}
+
     def update(context):
         rpc.context_reset()
         try:
-            rpc.CONTEXT.update(context())
+            rpc.CONTEXT.update(clean(context()))
         except RPCException:
             pass
         if callback:
             callback()
     context = RPCExecute(
         'model', 'res.user', 'get_preferences', True,
         callback=update if callback else None)
     if not callback:
         rpc.context_reset()
-        rpc.CONTEXT.update(context)
+        rpc.CONTEXT.update(clean(context))
 
 
 class Tooltips(object):
     _tooltips = None
 
     def set_tip(self, widget, tip_text):
         if hasattr(widget, 'set_tooltip_text'):
```

### Comparing `tryton-7.0.9/tryton/common/completion.py` & `tryton-7.2.0/tryton/common/completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import gettext
 import logging
 
 from gi.repository import GLib, Gtk
 
-from tryton.common import RPCExecute
+from tryton.common import RPCException, RPCExecute
 from tryton.config import CONFIG
 from tryton.exceptions import TrytonError, TrytonServerError
 
 _ = gettext.gettext
 logger = logging.getLogger(__name__)
 
 
@@ -68,14 +68,14 @@
             # Force display of popup
             entry.emit('changed')
         try:
             RPCExecute(
                 'model', model, 'autocomplete', search_text, domain,
                 CONFIG['client.limit'], order, context=context,
                 process_exception=False, callback=callback)
-        except Exception:
+        except RPCException:
             logger.warning(
                 "Unable to search for completion of %s", model,
                 exc_info=True)
         return False
     search_text = entry.get_text()
     GLib.timeout_add(300, update, search_text, domain)
```

### Comparing `tryton-7.0.9/tryton/common/datetime_.py` & `tryton-7.2.0/tryton/common/datetime_.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 from dateutil.parser import parse
 from dateutil.relativedelta import relativedelta
 from gi.repository import Gdk, GObject, Gtk
 
 from .common import IconFactory
 
-__all__ = ['Date', 'CellRendererDate', 'Time', 'CellRendererTime', 'DateTime']
+__all__ = [
+    'Date', 'CellRendererDate', 'Time', 'CellRendererTime', 'DateTime',
+    'date_parse']
 
 _ = gettext.gettext
 
 
 def _fix_format(format_):
     if '%Y' in format_:
         if (datetime.date.min.strftime('%Y') != '0001'
```

### Comparing `tryton-7.0.9/tryton/common/domain_inversion.py` & `tryton-7.2.0/tryton/common/domain_inversion.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/domain_parser.py` & `tryton-7.2.0/tryton/common/domain_parser.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/environment.py` & `tryton-7.2.0/tryton/common/environment.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/focus.py` & `tryton-7.2.0/tryton/common/focus.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/htmltextbuffer.py` & `tryton-7.2.0/tryton/common/htmltextbuffer.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/number_entry.py` & `tryton-7.2.0/tryton/common/number_entry.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/popup_menu.py` & `tryton-7.2.0/tryton/common/popup_menu.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/richtext.py` & `tryton-7.2.0/tryton/common/richtext.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/selection.py` & `tryton-7.2.0/tryton/common/selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,21 @@
         key = freeze_value(value)
         selection = self.attrs.get('selection', [])[:]
         help_ = self.attrs.get('help_selection', {})
         if (not isinstance(selection, (list, tuple))
                 and key not in self._values2selection):
             try:
                 if self.attrs.get('selection_change_with'):
-                    selection = RPCExecute('model', self.model_name, selection,
-                        value)
+                    selection = RPCExecute(
+                        'model', self.model_name, selection, value,
+                        process_exception=False)
                 else:
-                    selection = RPCExecute('model', self.model_name, selection)
+                    selection = RPCExecute(
+                        'model', self.model_name, selection,
+                        process_exception=False)
             except RPCException:
                 selection = []
             self._values2selection[key] = selection
         elif key in self._values2selection:
             selection = self._values2selection[key]
         if self.attrs.get('sort', True):
             selection.sort(key=operator.itemgetter(1))
```

### Comparing `tryton-7.0.9/tryton/common/timedelta.py` & `tryton-7.2.0/tryton/common/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/common/underline.py` & `tryton-7.2.0/tryton/common/underline.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/config.py` & `tryton-7.2.0/tryton/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import gettext
 import locale
 import logging
 import optparse
 import os
 import shutil
 import sys
-import tempfile
+from tempfile import NamedTemporaryFile
 
 from gi.repository import GdkPixbuf
 
 from tryton import __version__
 
 logger = logging.getLogger(__name__)
 _ = gettext.gettext
@@ -77,14 +77,15 @@
             'login.login': 'demo',
             'login.service': '',
             'login.service.port': 8001,
             'login.host': demo_server,
             'login.db': demo_database,
             'login.expanded': False,
             'client.title': 'Tryton',
+            'rpc.cache_size': 1024,
             'client.modepda': False,
             'client.toolbar': 'default',
             'client.save_tree_width': True,
             'client.save_tree_state': True,
             'client.spellcheck': False,
             'client.code_scanner_sound': True,
             'client.lang': locale.getdefaultlocale()[0],
@@ -181,15 +182,15 @@
 
     def load(self):
         parser = configparser.ConfigParser()
         try:
             parser.read([self.rcfile])
         except configparser.Error:
             config_dir = os.path.dirname(self.rcfile)
-            with tempfile.NamedTemporaryFile(
+            with NamedTemporaryFile(
                     delete=False, prefix='tryton_', suffix='.conf',
                     dir=config_dir) as temp_file:
                 temp_name = temp_file.name
             shutil.copy(self.rcfile, temp_name)
             logger.error(
                 f"Failed to parse {self.rcfile}. "
                 f"A backup can be found at {temp_name}", exc_info=True)
```

### Comparing `tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: bg\n"
 "Language-Team: bg <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/bg/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 msgid "specify the server hostname:port"
 msgstr "укажете адреса на сървъра"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Не може да зададе локални настройки %s"
 
 #, fuzzy
 msgid ", "
 msgstr ", "
 
@@ -131,23 +135,35 @@
 msgid "Download"
 msgstr ""
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Не може да се свърже със сървъра!"
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-msgid "Not found."
+msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 #, fuzzy
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr ""
 
@@ -1153,15 +1169,24 @@
 #, fuzzy
 msgid "Image size too large."
 msgstr "Размера на изображението е много голям!"
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+msgid "Copy Row"
+msgstr ""
+
+msgid "Copy Rows"
+msgstr ""
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ""
 
 msgid "Open filters"
 msgstr ""
```

### Comparing `tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/tryton.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ca\n"
 "Language-Team: ca <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -600,17 +600,14 @@
 
 msgid "No result found."
 msgstr "No s'han trobat resultats."
 
 msgid "Not Found."
 msgstr "No s'han trobat."
 
-msgid "Not found."
-msgstr "No s'han trobat."
-
 msgid "Note (%d/%d)"
 msgstr "Nota (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Notes (%s)"
 
 msgid "Notes..."
@@ -654,17 +651,14 @@
 
 msgid "PDA Mode"
 msgstr "Mode PDA"
 
 msgid "PNG image (*.png)"
 msgstr "Imatge PNG (*.png)"
 
-msgid "Paste"
-msgstr "Enganxa"
-
 msgid "Paste copied text"
 msgstr "Enganxa el text seleccionat"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Activa el so del escàner de codis"
 
 msgid "Pre-validation"
@@ -978,15 +972,15 @@
 msgid "Underline"
 msgstr "Subratllat"
 
 msgid "Unknown"
 msgstr "Desconegut"
 
 msgid "Unknown column header \"%s\""
-msgstr "Capçalera de columan desconeguda: \"%s\""
+msgstr "Capçalera de columna desconeguda: \"%s\""
 
 msgid "Unmark line for deletion"
 msgstr "Desmarca la línia per ser eliminada"
 
 msgid "Unselect all"
 msgstr "Deselecciona tot"
```

### Comparing `tryton-7.0.9/tryton/data/locale/ca/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 msgid "specify the server hostname:port"
 msgstr "Indica el nom:port del servidor"
 
 msgid "disable thread usage"
 msgstr "desactiva l'ús de fils"
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "No s'ha pogut establir l'idioma %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -126,23 +130,35 @@
 
 msgid "Download"
 msgstr "Baixa"
 
 msgid "Could not get a session."
 msgstr "No s'ha pogut obtenir una sessió."
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Massa peticions. Proveu-ho de nou més tard."
 
-msgid "Not found."
-msgstr "No s'han trobat."
+msgid "Too many requests. Try again later."
+msgstr "Massa peticions. Proveu-ho de nou més tard."
 
 msgid "Not Found."
 msgstr "No s'han trobat."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Cerca...</i>"
 
 msgid "<i>Create...</i>"
@@ -991,15 +1007,15 @@
 msgstr "Primer heu de seleccionar un fitxer a importar."
 
 msgid "Detection failed"
 msgstr "Ha fallat la detecció"
 
 #, python-format
 msgid "Unknown column header \"%s\""
-msgstr "Capçalera de columan desconeguda: \"%s\""
+msgstr "Capçalera de columna desconeguda: \"%s\""
 
 msgid "Error"
 msgstr "Error"
 
 msgid "Import failed"
 msgstr "Ha fallat la importació"
 
@@ -1080,15 +1096,27 @@
 
 msgid "Image size too large."
 msgstr "La mida de la imatge és massa gran."
 
 msgid "Copy"
 msgstr "Copia"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Copia l'URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Copia l'URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Enganxa"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Obre filtres"
```

### Comparing `tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/cs/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/tryton.po`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 msgid "specify the server hostname:port"
 msgstr "zadejte název hostitele pro server"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Nemohu nastavit lokalizaci %s"
 
 #, fuzzy
 msgid ", "
 msgstr ", "
 
@@ -131,23 +135,35 @@
 msgid "Download"
 msgstr ""
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Nelze se spojit se serverem!"
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-msgid "Not found."
+msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 #, fuzzy
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr ""
 
@@ -1170,15 +1186,24 @@
 #, fuzzy
 msgid "Image size too large."
 msgstr "Rozměry obrázku jsou příliš velké!"
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+msgid "Copy Row"
+msgstr ""
+
+msgid "Copy Rows"
+msgstr ""
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ""
 
 msgid "Open filters"
 msgstr ""
```

### Comparing `tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -600,17 +600,14 @@
 
 msgid "No result found."
 msgstr "Kein Ergebnis."
 
 msgid "Not Found."
 msgstr "Nicht gefunden."
 
-msgid "Not found."
-msgstr "Nicht gefunden."
-
 msgid "Note (%d/%d)"
 msgstr "Notiz (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Notizen (%s)"
 
 msgid "Notes..."
@@ -654,17 +651,14 @@
 
 msgid "PDA Mode"
 msgstr "Einspaltiger Modus"
 
 msgid "PNG image (*.png)"
 msgstr "PNG-Bild (*.png)"
 
-msgid "Paste"
-msgstr "Einfügen"
-
 msgid "Paste copied text"
 msgstr "Ausgewählten Text einfügen"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Ton für Barcode Scanner wiedergeben"
 
 msgid "Pre-validation"
```

### Comparing `tryton-7.0.9/tryton/data/locale/de/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 msgid "specify the server hostname:port"
 msgstr "Den Server mit Hostname:Port angeben."
 
 msgid "disable thread usage"
 msgstr "Threading deaktivieren"
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Kann locale %s nicht setzen."
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -128,23 +132,35 @@
 
 msgid "Download"
 msgstr "Herunterladen"
 
 msgid "Could not get a session."
 msgstr "Die Session-Anforderung ist fehlgeschlagen."
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Zu viele Anfragen. Bitte versuchen Sie es später erneut."
 
-msgid "Not found."
-msgstr "Nicht gefunden."
+msgid "Too many requests. Try again later."
+msgstr "Zu viele Anfragen. Bitte versuchen Sie es später erneut."
 
 msgid "Not Found."
 msgstr "Nicht gefunden."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Suche...</i>"
 
 msgid "<i>Create...</i>"
@@ -1087,15 +1103,27 @@
 
 msgid "Image size too large."
 msgstr "Bild ist zu groß."
 
 msgid "Copy"
 msgstr "Kopieren"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "URL kopieren"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "URL kopieren"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Einfügen"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Filter öffnen"
```

### Comparing `tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/tryton.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -600,17 +600,14 @@
 
 msgid "No result found."
 msgstr "No se han encontrado resultados."
 
 msgid "Not Found."
 msgstr "No se ha encontrado."
 
-msgid "Not found."
-msgstr "No se ha encontrado."
-
 msgid "Note (%d/%d)"
 msgstr "Nota (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Notas (%s)"
 
 msgid "Notes..."
@@ -654,17 +651,14 @@
 
 msgid "PDA Mode"
 msgstr "Modo PDA"
 
 msgid "PNG image (*.png)"
 msgstr "Imagen PNG (*.png)"
 
-msgid "Paste"
-msgstr "Pegar"
-
 msgid "Paste copied text"
 msgstr "Pegar texto seleccionado"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Activar el sonido del escáner de códigos"
 
 msgid "Pre-validation"
```

### Comparing `tryton-7.0.9/tryton/data/locale/es/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/tryton.po`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 msgid "specify the server hostname:port"
 msgstr "Indica el nombre:puerto del servidor"
 
 msgid "disable thread usage"
 msgstr "desactivar el uso de hilos"
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "No se ha podido establecer el idioma %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -130,23 +134,35 @@
 
 msgid "Download"
 msgstr "Descargar"
 
 msgid "Could not get a session."
 msgstr "No se ha podido obtener una sesión."
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Demasiadas peticiones. Inténtelo de nuevo más tarde."
 
-msgid "Not found."
-msgstr "No se ha encontrado."
+msgid "Too many requests. Try again later."
+msgstr "Demasiadas peticiones. Inténtelo de nuevo más tarde."
 
 msgid "Not Found."
 msgstr "No se ha encontrado."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Buscar...</i>"
 
 msgid "<i>Create...</i>"
@@ -1084,15 +1100,27 @@
 
 msgid "Image size too large."
 msgstr "El tamaño de la imagen es muy grande."
 
 msgid "Copy"
 msgstr "Copiar"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Copiar la URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Copiar la URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Pegar"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Abrir filtros"
```

### Comparing `tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es_419\n"
 "Language-Team: es_419 <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -216,17 +216,14 @@
 
 msgid "No action defined."
 msgstr "No se ha definido ninguna acción."
 
 msgid "No other language available."
 msgstr "No hay otro idioma disponible."
 
-msgid "Not found."
-msgstr "No se ha encontrado."
-
 msgid "OK"
 msgstr "Aceptar"
 
 msgid "Open"
 msgstr "Abrir"
 
 msgid "Open related records"
```

### Comparing `tryton-7.0.9/tryton/data/locale/es_419/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.po`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr ""
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr ""
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -125,23 +129,35 @@
 
 msgid "Download"
 msgstr "Descargar"
 
 msgid "Could not get a session."
 msgstr ""
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Demasiadas peticiones. Inténtalo de nuevo más tarde."
 
-msgid "Not found."
-msgstr "No se ha encontrado."
+msgid "Too many requests. Try again later."
+msgstr "Demasiadas peticiones. Inténtalo de nuevo más tarde."
 
 msgid "Not Found."
 msgstr ""
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr ""
 
 msgid "<i>Create...</i>"
@@ -1082,15 +1098,24 @@
 
 msgid "Image size too large."
 msgstr ""
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+msgid "Copy Row"
+msgstr ""
+
+msgid "Copy Rows"
+msgstr ""
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ""
 
 msgid "Open filters"
 msgstr ""
```

### Comparing `tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/tryton.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: et\n"
 "Language-Team: et <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -477,17 +477,14 @@
 
 msgid "PDA Mode"
 msgstr "PDA reziim"
 
 msgid "PNG image (*.png)"
 msgstr "PNG pilt (*.png)"
 
-msgid "Paste"
-msgstr "Aseta"
-
 msgid "Paste copied text"
 msgstr "Aseta valitud tekst"
 
 msgid "Pre-validation"
 msgstr "Eelkontroll"
 
 msgid "Preference"
```

### Comparing `tryton-7.0.9/tryton/data/locale/et/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr "määra server:port"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Ei saa seadistada lokaati %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -127,25 +131,36 @@
 msgid "Download"
 msgstr "Allalaadimine"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Ei saanud serveriga ühendust"
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-#, fuzzy
-msgid "Not found."
-msgstr "Tulemusi ei leitud."
+msgid "Too many requests. Try again later."
+msgstr ""
 
 #, fuzzy
 msgid "Not Found."
 msgstr "Tulemusi ei leitud."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Otsi...</i>"
 
 msgid "<i>Create...</i>"
@@ -1111,15 +1126,27 @@
 
 msgid "Image size too large."
 msgstr "Pilt on liiga suur."
 
 msgid "Copy"
 msgstr "Kopeeri"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Kopeeri URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Kopeeri URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Aseta"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Ava filtrid"
```

### Comparing `tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fa\n"
 "Language-Team: fa <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/fa/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr "تعیین نام میزبان سرور : درگاه"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "قادر به تنظیم محلی: \"%s\" نیست"
 
 msgid ", "
 msgstr "، "
 
 msgid ",..."
@@ -127,37 +131,48 @@
 msgid "Download"
 msgstr "دانلود"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "نمی تواند به سرور متصل شود"
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-#, fuzzy
-msgid "Not found."
-msgstr "نتیجه ای پیدا نشد."
+msgid "Too many requests. Try again later."
+msgstr ""
 
 #, fuzzy
 msgid "Not Found."
 msgstr "نتیجه ای پیدا نشد."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>جستجو...</i>"
 
 msgid "<i>Create...</i>"
 msgstr "<i>ایجاد...</i>"
 
 #, fuzzy, python-format
 msgid "Create \"%s\"..."
-msgstr "ایجاد "%s"..."
+msgstr "ایجاد \"%s\"..."
 
 msgid "Value"
 msgstr "مقدار"
 
 msgid "Displayed value"
 msgstr "مقدار نمایش داده شده"
 
@@ -1117,15 +1132,26 @@
 
 msgid "Image size too large."
 msgstr "اندازه تصویر بیش از حد بزرگ است."
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_رونوشت URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_رونوشت URL"
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "بازکردن فیلترها"
```

### Comparing `tryton-7.0.9/tryton/data/locale/fi/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/fi/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr ""
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr ""
 
 #, fuzzy
 msgid ", "
 msgstr ", "
 
@@ -126,23 +130,35 @@
 
 msgid "Download"
 msgstr ""
 
 msgid "Could not get a session."
 msgstr ""
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-msgid "Not found."
+msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 #, fuzzy
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr ""
 
@@ -1078,15 +1094,24 @@
 
 msgid "Image size too large."
 msgstr ""
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+msgid "Copy Row"
+msgstr ""
+
+msgid "Copy Rows"
+msgstr ""
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 #, fuzzy
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
```

### Comparing `tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/tryton.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -384,14 +384,17 @@
 
 msgid "Encoding:"
 msgstr "Codage :"
 
 msgid "Error"
 msgstr "Erreur"
 
+msgid "Error \"%s\". Try again later."
+msgstr "Erreur « %s ». Réessayez plus tard."
+
 msgid "Expand all rows"
 msgstr "Déplier toutes les lignes"
 
 msgid "Expand row"
 msgstr "Déplier la ligne"
 
 msgid "Expand/Collapse"
@@ -474,14 +477,17 @@
 
 msgid "Incompatible version of the server."
 msgstr "Version du serveur incompatible."
 
 msgid "Insert copied rows"
 msgstr "Insérer des lignes copiées"
 
+msgid "Invalid response id (%s) expected %s"
+msgstr "ID (%s) de réponse non valide, attendu %s"
+
 msgid "Italic"
 msgstr "Italique"
 
 msgid "Justify"
 msgstr "Justifier"
 
 msgid "Keyboard Shortcuts..."
@@ -600,17 +606,14 @@
 
 msgid "No result found."
 msgstr "Aucun résultat trouvé."
 
 msgid "Not Found."
 msgstr "Pas trouvé."
 
-msgid "Not found."
-msgstr "Pas trouvé."
-
 msgid "Note (%d/%d)"
 msgstr "Note (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Notes (%s)"
 
 msgid "Notes..."
@@ -654,17 +657,14 @@
 
 msgid "PDA Mode"
 msgstr "Mode PDA"
 
 msgid "PNG image (*.png)"
 msgstr "image PNG (*.png)"
 
-msgid "Paste"
-msgstr "Coller"
-
 msgid "Paste copied text"
 msgstr "Coller le texte copié"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Jouer du son pour le scanner de code"
 
 msgid "Pre-validation"
```

### Comparing `tryton-7.0.9/tryton/data/locale/fr/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 msgid "specify the server hostname:port"
 msgstr "spécifier le nom du serveur:port"
 
 msgid "disable thread usage"
 msgstr "désactiver l'utilisation des threads"
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr "ID (%s) de réponse non valide, attendu %s"
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Impossible de sélectionner la locale %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -128,23 +132,35 @@
 
 msgid "Download"
 msgstr "Télécharger"
 
 msgid "Could not get a session."
 msgstr "Impossible d'obtenir une session."
 
+#, python-format
+msgid "Error \"%s\". Try again later."
+msgstr "Erreur « %s ». Réessayez plus tard."
+
 msgid "Too many requests. Try again later."
 msgstr "Trop de demandes. Réessayez plus tard."
 
-msgid "Not found."
-msgstr "Pas trouvé."
-
 msgid "Not Found."
 msgstr "Pas trouvé."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Recherche...</i>"
 
 msgid "<i>Create...</i>"
@@ -1084,15 +1100,27 @@
 
 msgid "Image size too large."
 msgstr "Taille de l'image trop grande."
 
 msgid "Copy"
 msgstr "Copier"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Copier l'URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Copier l'URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Coller"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Ouvrir les filtres"
```

### Comparing `tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu\n"
 "Language-Team: hu <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -531,17 +531,14 @@
 
 msgid "PDA Mode"
 msgstr "Tablet mód"
 
 msgid "PNG image (*.png)"
 msgstr "PNG kép (*.png)"
 
-msgid "Paste"
-msgstr "Beillesztés"
-
 msgid "Paste copied text"
 msgstr "Kijelölt szöveg beillesztése"
 
 msgid "Pre-validation"
 msgstr "Adatkitöltés ellenőrzése"
 
 msgid "Preference"
```

### Comparing `tryton-7.0.9/tryton/data/locale/hu/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/tryton.po`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr "adja meg a kiszolgálónév:portot"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Nem lehet beállítani a %s nyelvet"
 
 #, fuzzy
 msgid ", "
 msgstr ", "
 
@@ -129,25 +133,36 @@
 msgid "Download"
 msgstr "Letöltés"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Nem sikerült csatlakozni a kiszolgálóhoz."
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-#, fuzzy
-msgid "Not found."
-msgstr "Nincs találat"
+msgid "Too many requests. Try again later."
+msgstr ""
 
 #, fuzzy
 msgid "Not Found."
 msgstr "Nincs találat"
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Keresés...</i>"
 
 msgid "<i>Create...</i>"
@@ -1096,15 +1111,27 @@
 #, fuzzy
 msgid "Image size too large."
 msgstr "Kép túl nagy!"
 
 msgid "Copy"
 msgstr "Másolás"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "Másolás"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "Másolás"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Beillesztés"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Szűrők megnyitása"
```

### Comparing `tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: id\n"
 "Language-Team: id <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/id/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 msgid "specify the server hostname:port"
 msgstr "tentukan nama host server:port"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr ""
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -123,21 +127,33 @@
 msgid "Download"
 msgstr "Unduh"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Tidak dapat terhubung ke server."
 
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
+msgstr "Terlalu banyak permintaan. Coba lagi nanti."
+
 msgid "Too many requests. Try again later."
 msgstr "Terlalu banyak permintaan. Coba lagi nanti."
 
-msgid "Not found."
+msgid "Not Found."
 msgstr ""
 
-msgid "Not Found."
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
 msgstr ""
 
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Cari...</i>"
@@ -1077,15 +1093,26 @@
 
 msgid "Image size too large."
 msgstr "Ukuran gambar terlalu besar."
 
 msgid "Copy"
 msgstr "Salin"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Salin URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Salin URL"
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr ""
```

### Comparing `tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/it/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 msgid "specify the server hostname:port"
 msgstr "specifica hostname:porta del server"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Impossibile impostare la localizzazione %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -127,25 +131,36 @@
 msgid "Download"
 msgstr "Scarica"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Impossibile connettersi al server."
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Troppe richieste. Riprovare più tardi."
 
-#, fuzzy
-msgid "Not found."
-msgstr "Nessun risultato trovato."
+msgid "Too many requests. Try again later."
+msgstr "Troppe richieste. Riprovare più tardi."
 
 #, fuzzy
 msgid "Not Found."
 msgstr "Nessun risultato trovato."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Cerca...</i>"
 
 msgid "<i>Create...</i>"
@@ -1104,15 +1119,26 @@
 
 msgid "Image size too large."
 msgstr ""
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Copia URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Copia URL"
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ""
 
 msgid "Open filters"
 msgstr ""
```

### Comparing `tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja_JP\n"
 "Language-Team: ja_JP <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lo\n"
 "Language-Team: lo <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/lo/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 msgid "specify the server hostname:port"
 msgstr "ລະບຸ ທີ່ຢູ່ ຂອງ ເຄື່ອງແມ່ຂ່າຍ"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "ບໍ່ສາມາດຕັ້ງຄ່າ ທ້ອງຖິ່ນ %s ໄດ້."
 
 msgid ", "
 msgstr ","
 
 msgid ",..."
@@ -130,25 +134,36 @@
 msgid "Download"
 msgstr ""
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "ບໍ່ສາມາດເຊື່ອມຕໍ່ກັບແມ່ຂ່າຍໄດ້"
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-#, fuzzy
-msgid "Not found."
-msgstr "ບໍ່ພົບຜົນຊອກຫາ"
+msgid "Too many requests. Try again later."
+msgstr ""
 
 #, fuzzy
 msgid "Not Found."
 msgstr "ບໍ່ພົບຜົນຊອກຫາ"
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>ຊອກຫາ...</i>"
 
 msgid "<i>Create...</i>"
@@ -1131,15 +1146,26 @@
 
 msgid "Image size too large."
 msgstr "ຂະໜາດຮູບ ໃຫຍ່ໂພດ."
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_ກ່າຍ URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_ກ່າຍ URL"
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "ໄຂໂຕກັ່ນຕອງ"
```

### Comparing `tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lt\n"
 "Language-Team: lt <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "(n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -514,17 +514,14 @@
 
 msgid "PDA Mode"
 msgstr "PDA režimas"
 
 msgid "PNG image (*.png)"
 msgstr "PNG paveikslėlis (*.png)"
 
-msgid "Paste"
-msgstr "Įdėti"
-
 msgid "Paste copied text"
 msgstr "Įdėti nukopijuotą tekstą"
 
 msgid "Pre-validation"
 msgstr "Išankstinis patikrinimas"
 
 msgid "Preference"
```

### Comparing `tryton-7.0.9/tryton/data/locale/lt/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr "nurodyti tarnybinę stotį pavadinimas:prievadas"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Nepavyko nustatyti lokalės %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -127,25 +131,36 @@
 msgid "Download"
 msgstr "Atsisiųsti"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Nepavyko prisijungti prie serverio"
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-#, fuzzy
-msgid "Not found."
-msgstr "Nerasta rezultatų."
+msgid "Too many requests. Try again later."
+msgstr ""
 
 #, fuzzy
 msgid "Not Found."
 msgstr "Nerasta rezultatų."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Ieškoti...</i>"
 
 msgid "<i>Create...</i>"
@@ -1109,15 +1124,27 @@
 
 msgid "Image size too large."
 msgstr "Paveikslėlis yra per didelis."
 
 msgid "Copy"
 msgstr "Kopijuoti"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Kopijuoti URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Kopijuoti URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Įdėti"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Atverti filtrus"
```

### Comparing `tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl\n"
 "Language-Team: nl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -384,14 +384,17 @@
 
 msgid "Encoding:"
 msgstr "Codering:"
 
 msgid "Error"
 msgstr "Fout"
 
+msgid "Error \"%s\". Try again later."
+msgstr "Te veel verzoeken\"%s\". Probeer het later nog eens."
+
 msgid "Expand all rows"
 msgstr "Alle rijen uitvouwen"
 
 msgid "Expand row"
 msgstr "Rij uitvouwen"
 
 msgid "Expand/Collapse"
@@ -600,17 +603,14 @@
 
 msgid "No result found."
 msgstr "Geen resultaat gevonden."
 
 msgid "Not Found."
 msgstr "Niet gevonden."
 
-msgid "Not found."
-msgstr "Niet gevonden."
-
 msgid "Note (%d/%d)"
 msgstr "Notitie (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Notities (%s)"
 
 msgid "Notes..."
@@ -654,17 +654,14 @@
 
 msgid "PDA Mode"
 msgstr "PDA-modus"
 
 msgid "PNG image (*.png)"
 msgstr "PNG afbeelding (*.png)"
 
-msgid "Paste"
-msgstr "Plakken"
-
 msgid "Paste copied text"
 msgstr "Plak geselecteerde tekst"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Geluid afspelen bij barcode scanner"
 
 msgid "Pre-validation"
```

### Comparing `tryton-7.0.9/tryton/data/locale/nl/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/tryton.po`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 msgid "specify the server hostname:port"
 msgstr "specificeer de hostnaam:poort"
 
 msgid "disable thread usage"
 msgstr "schakel gebruik van threads uit"
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Kan omgeving %s niet instellen"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -126,23 +130,35 @@
 
 msgid "Download"
 msgstr "Download"
 
 msgid "Could not get a session."
 msgstr "Kan geen sessie krijgen."
 
+#, python-format
+msgid "Error \"%s\". Try again later."
+msgstr "Te veel verzoeken\"%s\". Probeer het later nog eens."
+
 msgid "Too many requests. Try again later."
 msgstr "Te veel verzoeken. Probeer het later nog eens."
 
-msgid "Not found."
-msgstr "Niet gevonden."
-
 msgid "Not Found."
 msgstr "Niet gevonden."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Zoek...</i>"
 
 msgid "<i>Create...</i>"
@@ -1080,15 +1096,27 @@
 
 msgid "Image size too large."
 msgstr "Afbeelding te groot."
 
 msgid "Copy"
 msgstr "Kopieer"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Kopieer URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Kopieer URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Plakken"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Open filters"
```

### Comparing `tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pl\n"
 "Language-Team: pl <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -583,17 +583,14 @@
 
 msgid "PDA Mode"
 msgstr "Tryb PDA"
 
 msgid "PNG image (*.png)"
 msgstr "Obrazek w formacie PNG (*.png)"
 
-msgid "Paste"
-msgstr "Wklej"
-
 msgid "Paste copied text"
 msgstr "Wklej zaznaczony tekst"
 
 msgid "Pre-validation"
 msgstr "Wstępna walidacja"
 
 msgid "Preference"
```

### Comparing `tryton-7.0.9/tryton/data/locale/pl/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr "podaj nazwę:port serwera"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Nie można ustawić lokalizacji %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -126,25 +130,36 @@
 msgid "Download"
 msgstr "Pobierz"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Nie można połączyć się z serwerem."
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Za dużo połączeń. Spróbuj później."
 
-#, fuzzy
-msgid "Not found."
-msgstr "Nie znaleziono wyniku."
+msgid "Too many requests. Try again later."
+msgstr "Za dużo połączeń. Spróbuj później."
 
 #, fuzzy
 msgid "Not Found."
 msgstr "Nie znaleziono wyniku."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Szukaj...</i>"
 
 msgid "<i>Create...</i>"
@@ -1093,15 +1108,27 @@
 
 msgid "Image size too large."
 msgstr "Za duży rozmiar obrazka."
 
 msgid "Copy"
 msgstr "Kopiuj"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "Skopiuj adres URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "Skopiuj adres URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Wklej"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Otwórz filtry"
```

### Comparing `tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pt\n"
 "Language-Team: pt <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/pt/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 msgid "specify the server hostname:port"
 msgstr "Especifique o servidor hostname:porta"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Não foi possível definir as configurações regionais %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -129,25 +133,36 @@
 msgid "Download"
 msgstr "Baixar"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Não foi possível se conectar ao servidor"
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-#, fuzzy
-msgid "Not found."
-msgstr "Nenhum resultado encontrado."
+msgid "Too many requests. Try again later."
+msgstr ""
 
 #, fuzzy
 msgid "Not Found."
 msgstr "Nenhum resultado encontrado."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Buscar...</i>"
 
 msgid "<i>Create...</i>"
@@ -1116,15 +1131,26 @@
 
 msgid "Image size too large."
 msgstr "Imagem muito grande."
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Copiar URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Copiar URL"
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Abrir filtros"
```

### Comparing `tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/tryton.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ro\n"
 "Language-Team: ro <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
 "20)) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -100,14 +100,17 @@
 
 msgid "Add a note to the record"
 msgstr "Adăugați o notă la înregistrare"
 
 msgid "Add an attachment to the record"
 msgstr "Adăugați un atașament la înregistrare"
 
+msgid "Add and New"
+msgstr "Adăugare şi Nou"
+
 msgid "Add existing record"
 msgstr "Adăugare înregistrare existentă"
 
 msgid "Add field names"
 msgstr "Adăugare denumire de câmp"
 
 msgid "Add new profile"
@@ -136,14 +139,17 @@
 
 msgid "Application Error"
 msgstr "Eroare de aplicație"
 
 msgid "Application Shortcuts"
 msgstr "Comenzi rapide pentru aplicații"
 
+msgid "Apply changes"
+msgstr "Aplicare schimbări"
+
 msgid "Are you sure to remove this record?"
 msgstr "Sigur eliminați această înregistrare?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Sigur eliminați această înregistrare?"
 
 msgid "Attachment (%s)"
@@ -217,14 +223,20 @@
 
 msgid "Close"
 msgstr "Închidere"
 
 msgid "Close Tab"
 msgstr "Închidere fila"
 
+msgid "Code"
+msgstr "Cod"
+
+msgid "Code Scanner"
+msgstr "Scanner"
+
 msgid "Collapse all rows"
 msgstr "Reducere toate rândurile"
 
 msgid "Collapse row"
 msgstr "Reducere rând"
 
 msgid "Compare"
@@ -256,14 +268,17 @@
 
 msgid "Could not connect to the server."
 msgstr "Nu s-a putut efectua conexiunea la server."
 
 msgid "Could not get a session."
 msgstr "Nu s-a putut găsi o sesiune."
 
+msgid "Create \"%s\"..."
+msgstr "Creare \"%s\"..."
+
 msgid "Create a new record"
 msgstr "Creați o înregistrare nouă"
 
 msgid "Create a new record <F3>"
 msgstr "Creați o nouă înregistrare <F3>"
 
 msgid "Create new relation"
@@ -313,14 +328,17 @@
 
 msgid "Detection failed"
 msgstr "Detecție eșuată"
 
 msgid "Digits"
 msgstr "Cifre"
 
+msgid "Discard changes"
+msgstr "Omitere schimbări"
+
 msgid "Display format"
 msgstr "Formatul afisare"
 
 msgid "Displayed date format"
 msgstr "Formatul datei afișat"
 
 msgid "Displayed value"
@@ -583,17 +601,14 @@
 
 msgid "No result found."
 msgstr "Niciun rezultat găsit."
 
 msgid "Not Found."
 msgstr "Niciun rezultat găsit."
 
-msgid "Not found."
-msgstr "Nimic găsit."
-
 msgid "Note (%d/%d)"
 msgstr "Notă (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Note (%s)"
 
 msgid "Notes..."
@@ -637,20 +652,20 @@
 
 msgid "PDA Mode"
 msgstr "Modul PDA"
 
 msgid "PNG image (*.png)"
 msgstr "Imagine PNG (* .png)"
 
-msgid "Paste"
-msgstr "Lipire"
-
 msgid "Paste copied text"
 msgstr "Inserare text copiat"
 
+msgid "Play Sound for Code Scanner"
+msgstr "Rulare Sunet pentru Scanner"
+
 msgid "Pre-validation"
 msgstr "Pre-validare"
 
 msgid "Preference"
 msgstr "Preferințe"
 
 msgid "Preferences"
@@ -671,15 +686,15 @@
 msgid "Previous entry"
 msgstr "Inregistrare anterioară"
 
 msgid "Previous tab"
 msgstr "Fila anterioară"
 
 msgid "Print"
-msgstr "Tiparire"
+msgstr "Tipărire"
 
 msgid "Print report"
 msgstr "Tipărire raport"
 
 msgid "Print..."
 msgstr "Imprimare..."
 
@@ -766,20 +781,26 @@
 
 msgid "Save Column Width"
 msgstr "Salvați lățimea coloanei"
 
 msgid "Save Tree State"
 msgstr "Salvare stare arbore"
 
+msgid "Save and New"
+msgstr "Salvare şi Nou"
+
 msgid "Save this record"
 msgstr "Salvare înregistrare"
 
 msgid "Save your current version"
 msgstr "Salvați versiunea curentă"
 
+msgid "Scan"
+msgstr "Scanare"
+
 msgid "Search"
 msgstr "Căutare"
 
 msgid "Search %s"
 msgstr "Căutare %s"
 
 msgid "Search Limit Settings"
@@ -951,14 +972,17 @@
 
 msgid "Underline"
 msgstr "Subliniere"
 
 msgid "Unknown"
 msgstr "Necunoscut"
 
+msgid "Unknown column header \"%s\""
+msgstr "Antet necunoscut de coloană \"%s\""
+
 msgid "Unmark line for deletion"
 msgstr "Deselectare rând pentru ștergere"
 
 msgid "Unselect all"
 msgstr "Deselectare tot"
 
 msgid "Use locale format"
```

### Comparing `tryton-7.0.9/tryton/data/locale/ro/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 msgid "specify the server hostname:port"
 msgstr "specificați numele gazdă server: port"
 
 msgid "disable thread usage"
 msgstr "dezactivare utilizarea thread-urilor"
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Imposibil de setat regiunea locală %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -122,33 +126,45 @@
 
 msgid "Download"
 msgstr "Descarca"
 
 msgid "Could not get a session."
 msgstr "Nu s-a putut găsi o sesiune."
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Prea multe cereri. Încercați mai târziu."
 
-msgid "Not found."
-msgstr "Nimic găsit."
+msgid "Too many requests. Try again later."
+msgstr "Prea multe cereri. Încercați mai târziu."
 
 msgid "Not Found."
 msgstr "Niciun rezultat găsit."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Căutare...</i>"
 
 msgid "<i>Create...</i>"
 msgstr "<i>Creare...</i>"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Create \"%s\"..."
 msgstr "Creare \"%s\"..."
 
 msgid "Value"
 msgstr "Valoare"
 
 msgid "Displayed value"
@@ -292,15 +308,15 @@
 msgid "Save Tree State"
 msgstr "Salvare stare arbore"
 
 msgid "Spell Checking"
 msgstr "Verificare ortografia"
 
 msgid "Play Sound for Code Scanner"
-msgstr ""
+msgstr "Rulare Sunet pentru Scanner"
 
 msgid "PDA Mode"
 msgstr "Modul PDA"
 
 msgid "Search Limit..."
 msgstr "Limita de căutare ..."
 
@@ -504,18 +520,18 @@
 msgstr "Dimitrios Moustos"
 
 #, python-format
 msgid "Attachments (%s)"
 msgstr "Atașamente (%s)"
 
 msgid "Code Scanner"
-msgstr ""
+msgstr "Scanner"
 
 msgid "Code"
-msgstr ""
+msgstr "Cod"
 
 msgid "Profile Editor"
 msgstr "Editor de profil"
 
 msgid "Profile"
 msgstr "Profil"
 
@@ -670,15 +686,15 @@
 msgid "Report"
 msgstr "Raport"
 
 msgid "Open report"
 msgstr "Deschidere Raport"
 
 msgid "Print"
-msgstr "Tiparire"
+msgstr "Tipărire"
 
 msgid "Print report"
 msgstr "Tipărire raport"
 
 msgid "_Copy URL"
 msgstr "_Copiere URL"
 
@@ -934,28 +950,27 @@
 msgid "Link"
 msgstr "Legătură"
 
 msgid "Delete"
 msgstr "Ștergere"
 
 msgid "Discard changes"
-msgstr ""
+msgstr "Omitere schimbări"
 
 msgid "Save and New"
-msgstr ""
+msgstr "Salvare şi Nou"
 
-#, fuzzy
 msgid "Add and New"
-msgstr "Adaugă valoare"
+msgstr "Adăugare şi Nou"
 
 msgid "Add"
 msgstr "Adăuga"
 
 msgid "Apply changes"
-msgstr ""
+msgstr "Aplicare schimbări"
 
 msgid "Switch"
 msgstr "Schimba"
 
 msgid "Remove <Del>"
 msgstr "Eliminare <Del>"
 
@@ -988,15 +1003,15 @@
 msgstr "Mai întâi trebuie să selectați un fișier de import."
 
 msgid "Detection failed"
 msgstr "Detecție eșuată"
 
 #, python-format
 msgid "Unknown column header \"%s\""
-msgstr ""
+msgstr "Antet necunoscut de coloană \"%s\""
 
 msgid "Error"
 msgstr "Eroare"
 
 msgid "Import failed"
 msgstr "Import eşuat"
 
@@ -1054,15 +1069,15 @@
 msgid "Pre-validation"
 msgstr "Pre-validare"
 
 msgid ":"
 msgstr ":"
 
 msgid "Scan"
-msgstr ""
+msgstr "Scanare"
 
 msgid "Image Size"
 msgstr "Marimea imaginii"
 
 msgid "Width:"
 msgstr "Lăţime:"
 
@@ -1077,15 +1092,27 @@
 
 msgid "Image size too large."
 msgstr "Dimensiunea imaginii este prea mare."
 
 msgid "Copy"
 msgstr "Copiere"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Copiere URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Copiere URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Lipire"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Deschide filtre"
```

### Comparing `tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ru\n"
 "Language-Team: ru <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/ru/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/tryton.po`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 msgid "specify the server hostname:port"
 msgstr "укажите имя сервера"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Не удается установить локализацию %s"
 
 #, fuzzy
 msgid ", "
 msgstr ", "
 
@@ -132,25 +136,36 @@
 msgid "Download"
 msgstr ""
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Не удается подключиться к серверу!"
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-#, fuzzy
-msgid "Not found."
-msgstr "Ничего не найдено."
+msgid "Too many requests. Try again later."
+msgstr ""
 
 #, fuzzy
 msgid "Not Found."
 msgstr "Ничего не найдено."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 #, fuzzy
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Поиск...</i>"
 
@@ -1156,15 +1171,24 @@
 #, fuzzy
 msgid "Image size too large."
 msgstr "Размер изображения слишком большой!"
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+msgid "Copy Row"
+msgstr ""
+
+msgid "Copy Rows"
+msgstr ""
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr ""
```

### Comparing `tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/tryton.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: sl\n"
 "Language-Team: sl <LL@li.org>\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
@@ -601,17 +601,14 @@
 
 msgid "No result found."
 msgstr "Brez rezultatov."
 
 msgid "Not Found."
 msgstr "Ni najdeno."
 
-msgid "Not found."
-msgstr "Ni najdeno."
-
 msgid "Note (%d/%d)"
 msgstr "Zapisek (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Zapiski (%s)"
 
 msgid "Notes..."
@@ -655,17 +652,14 @@
 
 msgid "PDA Mode"
 msgstr "Tablični način"
 
 msgid "PNG image (*.png)"
 msgstr "PNG podoba (*.png)"
 
-msgid "Paste"
-msgstr "Prilepi"
-
 msgid "Paste copied text"
 msgstr "Prilepi vsebino"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Predvajaj zvok za čitalnik kod"
 
 msgid "Pre-validation"
```

### Comparing `tryton-7.0.9/tryton/data/locale/sl/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr "določi ime in vrata strežniškega gostitelja"
 
 msgid "disable thread usage"
 msgstr "onemogoči uporabo niti"
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Ni možno nastaviti krajevnih nastavitev %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -126,23 +130,35 @@
 
 msgid "Download"
 msgstr "Prenesi"
 
 msgid "Could not get a session."
 msgstr "Ni mogoče vzpostaviti seje."
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Preveč poslanih zahtev. Poskusite kasneje."
 
-msgid "Not found."
-msgstr "Ni najdeno."
+msgid "Too many requests. Try again later."
+msgstr "Preveč poslanih zahtev. Poskusite kasneje."
 
 msgid "Not Found."
 msgstr "Ni najdeno."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Išči...</i>"
 
 msgid "<i>Create...</i>"
@@ -1081,15 +1097,27 @@
 
 msgid "Image size too large."
 msgstr "Podoba je prevelika."
 
 msgid "Copy"
 msgstr "Kopiraj"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Kopiraj URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Kopiraj URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Prilepi"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Odpri filtre"
```

### Comparing `tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/tryton.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.0.9/tryton/data/locale/tr/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr "Server hostname belirle: port"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Lokal %s ayarlanamadı"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -127,23 +131,35 @@
 
 msgid "Download"
 msgstr ""
 
 msgid "Could not get a session."
 msgstr ""
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error \"%s\". Try again later."
 msgstr ""
 
-msgid "Not found."
+msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr ""
 
 msgid "<i>Create...</i>"
@@ -1080,15 +1096,24 @@
 
 msgid "Image size too large."
 msgstr ""
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+msgid "Copy Row"
+msgstr ""
+
+msgid "Copy Rows"
+msgstr ""
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr ""
```

### Comparing `tryton-7.0.9/tryton/data/locale/tryton.pot` & `tryton-7.2.0/tryton/data/locale/tryton.pot`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 msgid "specify the server hostname:port"
 msgstr ""
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr ""
 
 msgid ", "
 msgstr ""
 
 msgid ",..."
@@ -68,15 +72,15 @@
 
 msgid "No"
 msgstr ""
 
 msgid "Yes"
 msgstr ""
 
-msgid "Concurrency Exception"
+msgid "Concurrency Warning"
 msgstr ""
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 
 msgid "Cancel saving"
 msgstr ""
@@ -99,14 +103,17 @@
 
 msgid "Close"
 msgstr ""
 
 msgid "Application Error"
 msgstr ""
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr ""
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -115,26 +122,41 @@
 
 msgid "A new version is available!"
 msgstr ""
 
 msgid "Download"
 msgstr ""
 
+msgid "Concurrency Exception"
+msgstr ""
+
 msgid "Could not get a session."
 msgstr ""
 
-msgid "Too many requests. Try again later."
+#, python-format
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
-msgid "Not found."
+msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr ""
 
 msgid "<i>Search...</i>"
 msgstr ""
 
 msgid "<i>Create...</i>"
@@ -1068,15 +1090,24 @@
 
 msgid "Image size too large."
 msgstr ""
 
 msgid "Copy"
 msgstr ""
 
-msgid "Paste"
+msgid "Copy Row"
+msgstr ""
+
+msgid "Copy Rows"
+msgstr ""
+
+msgid "Copy Column"
+msgstr ""
+
+msgid "Paste Rows"
 msgstr ""
 
 msgid ".."
 msgstr ""
 
 msgid "Open filters"
 msgstr ""
```

### Comparing `tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/tryton.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -598,17 +598,14 @@
 
 msgid "PDA Mode"
 msgstr "Спрощений режим"
 
 msgid "PNG image (*.png)"
 msgstr "Зображення PNG (*.png)"
 
-msgid "Paste"
-msgstr "Вставити"
-
 msgid "Paste copied text"
 msgstr "Вставити скопійований текст"
 
 msgid "Pre-validation"
 msgstr "Попередня перевірка"
 
 msgid "Preference"
```

### Comparing `tryton-7.0.9/tryton/data/locale/uk/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 msgid "specify the server hostname:port"
 msgstr "вкажіть ім'я сервера:порт"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "Неможливо встановити локалізацію %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -123,25 +127,36 @@
 msgid "Download"
 msgstr "Завантажити"
 
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Не вдалося підключитися до сервера."
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "Дуже багато запитів. Спробуйте ще раз пізніше."
 
-#, fuzzy
-msgid "Not found."
-msgstr "Нічого не знайдено."
+msgid "Too many requests. Try again later."
+msgstr "Дуже багато запитів. Спробуйте ще раз пізніше."
 
 #, fuzzy
 msgid "Not Found."
 msgstr "Нічого не знайдено."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Пошук...</i>"
 
 msgid "<i>Create...</i>"
@@ -1086,15 +1101,27 @@
 
 msgid "Image size too large."
 msgstr "Розмір зображення завеликий."
 
 msgid "Copy"
 msgstr "Копіювати"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "_Копіювати URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "_Копіювати URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "Вставити"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Відкрити фільтри"
```

### Comparing `tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo` & `tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-17 12:29+0200\n"
+"POT-Creation-Date: 2024-04-29 17:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -600,17 +600,14 @@
 
 msgid "No result found."
 msgstr "无符合条件的数据."
 
 msgid "Not Found."
 msgstr "无符合条件的数据."
 
-msgid "Not found."
-msgstr "无符合条件的数据."
-
 msgid "Note (%d/%d)"
 msgstr "批注 (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "注释(%s)"
 
 msgid "Notes..."
@@ -654,17 +651,14 @@
 
 msgid "PDA Mode"
 msgstr "PDA 模式"
 
 msgid "PNG image (*.png)"
 msgstr "PNG 图片格式 (*.png)"
 
-msgid "Paste"
-msgstr "粘贴"
-
 msgid "Paste copied text"
 msgstr "粘贴"
 
 msgid "Play Sound for Code Scanner"
 msgstr "为代码扫描仪播放声音"
 
 msgid "Pre-validation"
```

### Comparing `tryton-7.0.9/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po` & `tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 msgid "specify the server hostname:port"
 msgstr "设置服务器主机名:端口号"
 
 msgid "disable thread usage"
 msgstr "禁用线程"
 
 #, python-format
+msgid "Invalid response id (%s) expected %s"
+msgstr ""
+
+#, python-format
 msgid "Unable to set locale %s"
 msgstr "无法设置 locale %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
@@ -125,23 +129,35 @@
 
 msgid "Download"
 msgstr "下载"
 
 msgid "Could not get a session."
 msgstr "无法获取会话。"
 
-msgid "Too many requests. Try again later."
+#, fuzzy, python-format
+msgid "Error \"%s\". Try again later."
 msgstr "请求太多，请稍后重试."
 
-msgid "Not found."
-msgstr "无符合条件的数据."
+msgid "Too many requests. Try again later."
+msgstr "请求太多，请稍后重试."
 
 msgid "Not Found."
 msgstr "无符合条件的数据."
 
+msgid "Reset forgotten password"
+msgstr ""
+
+msgid "Send you an email to reset your password."
+msgstr ""
+
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>查找...</i>"
 
 msgid "<i>Create...</i>"
@@ -1079,15 +1095,27 @@
 
 msgid "Image size too large."
 msgstr "图片尺寸过大."
 
 msgid "Copy"
 msgstr "复制"
 
-msgid "Paste"
+#, fuzzy
+msgid "Copy Row"
+msgstr "复制（_C）URL"
+
+#, fuzzy
+msgid "Copy Rows"
+msgstr "复制（_C）URL"
+
+msgid "Copy Column"
+msgstr ""
+
+#, fuzzy
+msgid "Paste Rows"
 msgstr "粘贴"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "打开筛选器"
```

### Comparing `tryton-7.0.9/tryton/data/pixmaps/tryton/LICENSE` & `tryton-7.2.0/tryton/data/pixmaps/tryton/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-icon.png` & `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-icon.png`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-icon.svg` & `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-icon.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton-unarchive.svg` & `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-unarchive.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.icns` & `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.icns`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.ico` & `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.ico`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/pixmaps/tryton/tryton.svg` & `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/sounds/LICENSE` & `tryton-7.2.0/tryton/data/sounds/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/sounds/danger.wav` & `tryton-7.2.0/tryton/data/sounds/danger.wav`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/data/sounds/success.wav` & `tryton-7.2.0/tryton/data/sounds/success.wav`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/device_cookie.py` & `tryton-7.2.0/tryton/device_cookie.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def renew():
     from tryton.common import common
 
     def set_cookie(new_cookie):
         try:
             new_cookie = new_cookie()
-        except Exception:
+        except common.RPCException:
             logger.error("Cannot renew device cookie", exc_info=True)
         else:
             _set(new_cookie)
 
     current_cookie = get()
     common.RPCExecute(
         'model', 'res.user.device', 'renew', current_cookie,
```

### Comparing `tryton-7.0.9/tryton/fingerprints.py` & `tryton-7.2.0/tryton/fingerprints.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/main.py` & `tryton-7.2.0/tryton/gui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,16 @@
                 gmodel.search_text = search_text
                 # Force display of popup
                 widget.emit('changed')
                 end()
 
             RPCExecute('model', 'ir.model', 'global_search', search_text,
                 CONFIG['client.limit'], self.menu_screen.model_name,
-                context=self.menu_screen.context, callback=set_result)
+                context=self.menu_screen.context, callback=set_result,
+                process_exception=False)
             return False
 
         def changed(widget):
             search_text = widget.get_text()
             GLib.timeout_add(300, update, widget, search_text)
 
         def activate(widget):
@@ -466,15 +467,15 @@
             Window.create(self.menu_screen.model_name + '.favorite',
                 mode=['tree', 'form'],
                 name=_("Favorites"))
         try:
             favorites = RPCExecute('model',
                 self.menu_screen.model_name + '.favorite', 'get',
                 process_exception=False)
-        except Exception:
+        except RPCException:
             return False
         for id_, name, icon in favorites:
             menuitem = Gtk.MenuItem(label=name)
             menuitem.connect('activate', _action_favorite, id_)
             self.menu_favorite.add(menuitem)
         self.menu_favorite.add(Gtk.SeparatorMenuItem())
         manage_favorites = Gtk.MenuItem(label=_("Manage..."),
```

### Comparing `tryton-7.0.9/tryton/gui/window/about.py` & `tryton-7.2.0/tryton/gui/window/about.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/attachment.py` & `tryton-7.2.0/tryton/gui/window/attachment.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/board.py` & `tryton-7.2.0/tryton/gui/window/board.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/code_scanner.py` & `tryton-7.2.0/tryton/gui/window/code_scanner.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/dblogin.py` & `tryton-7.2.0/tryton/gui/window/dblogin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import configparser
 import gettext
 import logging
 import os
 import re
 import shutil
-import tempfile
 import threading
+from tempfile import NamedTemporaryFile
 
 from gi.repository import GLib, GObject, Gtk
 
 import tryton.common as common
 import tryton.rpc as rpc
 from tryton import __version__
 from tryton.common.underline import set_underline
@@ -497,15 +497,15 @@
         current_demo = f"demo{series}.tryton.org"
         try:
             self.profiles.read(self.profile_cfg)
         except configparser.Error:
             # reset self.profiles as parsing errors may leave wrong data in
             # the parser
             self.profiles = configparser.ConfigParser()
-            with tempfile.NamedTemporaryFile(
+            with NamedTemporaryFile(
                     delete=False, prefix='profiles_', suffix='.cfg',
                     dir=config_dir) as temp_file:
                 temp_name = temp_file.name
             shutil.copy(self.profile_cfg, temp_name)
             logger.error(
                 f"Failed to parse {self.profiles_cfg}. "
                 f"A backup can be found at {temp_name}",
```

### Comparing `tryton-7.0.9/tryton/gui/window/email_.py` & `tryton-7.2.0/tryton/gui/window/email_.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             # Force display of popup
             self.emit('changed')
 
         try:
             RPCExecute(
                 'model', 'ir.email', 'complete', text, CONFIG['client.limit'],
                 process_exception=False, callback=callback)
-        except Exception:
+        except RPCException:
             logger.warning(
                 _("Unable to complete email entry"), exc_info=True)
         return False
 
     def _changed(self):
         def keypress():
             if not self.props.window:
```

### Comparing `tryton-7.0.9/tryton/gui/window/form.py` & `tryton-7.2.0/tryton/gui/window/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 "Form"
 import csv
 import gettext
 import locale
 import os
-import tempfile
 from itertools import zip_longest
 
 from gi.repository import Gdk, GLib, Gtk
 
 import tryton.common as common
 from tryton import plugins
 from tryton.action import Action
-from tryton.common import RPCException, RPCExecute, sur, sur_3b
+from tryton.common import RPCException, RPCExecute, sur, sur_3b, tempfile
 from tryton.common.common import selection as selection_
 from tryton.common.popup_menu import popup
 from tryton.common.underline import set_underline
 from tryton.gui import Main
 from tryton.gui.window import Window
 from tryton.gui.window.attachment import Attachment
 from tryton.gui.window.email_ import Email
@@ -102,15 +101,17 @@
 
     def widget_get(self):
         return self.screen.widget
 
     def compare(self, model, attributes):
         if not attributes:
             return False
-        return (self.model == model
+        return (
+            self.screen.view_index == 0
+            and self.model == model
             and self.res_id == attributes.get('res_id')
             and self.attributes.get('domain') == attributes.get('domain')
             and self.attributes.get('view_ids') == attributes.get('view_ids')
             and (attributes.get('view_ids')
                 or (self.attributes.get('mode') or ['tree', 'form']) == (
                     attributes.get('mode') or ['tree', 'form']))
             and self.screen.local_context == attributes.get('context')
```

### Comparing `tryton-7.0.9/tryton/gui/window/infobar.py` & `tryton-7.2.0/tryton/gui/window/infobar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/limit.py` & `tryton-7.2.0/tryton/gui/window/limit.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/log.py` & `tryton-7.2.0/tryton/gui/window/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         title = _("Logs (%s)") % record.rec_name()
 
         context = record.get_context()
         try:
             log, = RPCExecute(
                 'model', record.model_name, 'read', [record.id],
                 ['create_uid.rec_name', 'create_date',
-                    'write_uid.rec_name', 'write_date'], context=context)
+                    'write_uid.rec_name', 'write_date',
+                    'xml_id'], context=context)
         except RPCException:
             return
 
         date_format = context.get('date_format', '%x')
         datetime_format = date_format + ' %H:%M:%S.%f'
 
         grid = Gtk.Grid(
@@ -49,19 +50,40 @@
         grid.attach(entry_id, 3, 1, 1, 1)
         label_id = Gtk.Label(
             label=set_underline(_("ID:")),
             use_underline=True, halign=Gtk.Align.END)
         label_id.set_mnemonic_widget(entry_id)
         grid.attach(label_id, 2, 1, 1, 1)
 
+        if log.get('xml_id'):
+            module, xml_id = log['xml_id'].split('.', 1)
+
+            entry_module = Gtk.Entry(editable=False)
+            entry_module.set_text(module)
+            grid.attach(entry_module, 1, 2, 1, 1)
+            label_module = Gtk.Label(
+                label=set_underline(_("Module:")),
+                use_underline=True, halign=Gtk.Align.END)
+            label_module.set_mnemonic_widget(entry_module)
+            grid.attach(label_module, 0, 2, 1, 1)
+
+            entry_xml_id = Gtk.Entry(editable=False)
+            entry_xml_id.set_text(xml_id)
+            grid.attach(entry_xml_id, 3, 2, 1, 1)
+            label_xml_id = Gtk.Label(
+                label=set_underline(_("XML ID:")),
+                use_underline=True, halign=Gtk.Align.END)
+            label_xml_id.set_mnemonic_widget(entry_xml_id)
+            grid.attach(label_xml_id, 2, 2, 1, 1)
+
         for i, (user, user_label, date, date_label) in enumerate([
                     ('create_uid.', _("Created by:"),
                         'create_date', _("Created at:")),
                     ('write_uid.', _("Last Modified by:"),
-                        'write_date', _("Last Modified at:"))], 2):
+                        'write_date', _("Last Modified at:"))], 3):
             entry_user = Gtk.Entry(editable=False, width_chars=50)
             user = log.get(user)
             if user:
                 user = user.get('rec_name', '')
             entry_user.set_text(user or '')
             grid.attach(entry_user, 1, i, 1, 1)
             label_user = Gtk.Label(
```

### Comparing `tryton-7.0.9/tryton/gui/window/nomodal.py` & `tryton-7.2.0/tryton/gui/window/nomodal.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/note.py` & `tryton-7.2.0/tryton/gui/window/note.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/preference.py` & `tryton-7.2.0/tryton/gui/window/preference.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/revision.py` & `tryton-7.2.0/tryton/gui/window/revision.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/tabcontent.py` & `tryton-7.2.0/tryton/gui/window/tabcontent.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_board/action.py` & `tryton-7.2.0/tryton/gui/window/view_board/action.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_board/view_board.py` & `tryton-7.2.0/tryton/gui/window/view_board/view_board.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/model/field.py` & `tryton-7.2.0/tryton/gui/window/view_form/model/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 import decimal
+import functools
 import locale
 import logging
 import math
+import operator
 import os
-import tempfile
 from decimal import Decimal
 from itertools import chain
 
 import tryton.common as common
 from tryton.common import (
     EvalEnvironment, RPCException, RPCExecute, concat, domain_inversion,
     eval_domain, extract_reference_models, filter_leaf, inverse_leaf,
-    localize_domain, merge, prepare_reference_domain, simplify, unique_value)
+    localize_domain, merge, prepare_reference_domain, simplify, tempfile,
+    unique_value)
 from tryton.common.htmltextbuffer import guess_decode
 from tryton.config import CONFIG
 from tryton.pyson import PYSONDecoder
 
 logger = logging.getLogger(__name__)
 
 
@@ -695,41 +697,61 @@
         for record2 in record.value[self.name]:
             if not (record2.deleted or record2.removed):
                 result.append(
                     record2.get_on_change_value(
                         skip={self.attrs.get('relation_field', '')}))
         return result
 
-    def _set_value(self, record, value, default=False, modified=False):
+    def _set_value(
+            self, record, value, default=False, modified=False, data=None):
         self._set_default_value(record)
         group = record.value[self.name]
         if value is None:
             value = []
         if not value or isinstance(value[0], int):
             mode = 'list ids'
         else:
             mode = 'list values'
 
-        if mode == 'list values':
+        if mode == 'list values' or data:
             context = self.get_context(record)
-            field_names = set(f for v in value for f in v
-                if f not in group.fields and '.' not in f)
-            if field_names:
+            if mode == 'list values':
+                fields = set(f for v in value for f in v)
+            else:
+                fields = functools.reduce(
+                    operator.or_, (d.keys() for d in data), set())
+            field_names = {f for f in fields
+                if (f not in group.fields
+                    and '.' not in f
+                    and ':' not in f
+                    and not f.startswith('_'))}
+            attr_fields = functools.reduce(
+                operator.or_,
+                (v['fields'] for v in self.attrs.get('views', {}).values()),
+                {})
+            fields = {n: attr_fields[n]
+                for n in field_names
+                if n in attr_fields}
+            if to_fetch := (field_names - attr_fields.keys()):
                 try:
-                    fields = RPCExecute('model', self.attrs['relation'],
-                        'fields_get', list(field_names), context=context)
+                    fields |= RPCExecute('model', self.attrs['relation'],
+                        'fields_get', list(to_fetch), context=context)
                 except RPCException:
                     return
+
+            if fields:
                 group.load_fields(fields)
 
         if mode == 'list ids':
             records_to_remove = [r for r in group if r.id not in value]
             for record_to_remove in records_to_remove:
                 group.remove(record_to_remove, remove=True, modified=False)
-            group.load(value, modified=modified or default)
+            group.load(
+                value, modified=modified or default,
+                preloaded={v['id']: v for v in (data or [])})
         else:
             for vals in value:
                 if 'id' in vals:
                     new_record = group.get(vals['id'])
                     if not new_record:
                         new_record = group.new(
                             default=False, obj_id=vals['id'])
@@ -742,15 +764,15 @@
                     group.add(new_record, modified=False)
                 else:
                     new_record.set(vals, modified=False)
                     group.append(new_record)
             # Trigger modified only once
             group.record_modified()
 
-    def set(self, record, value, _default=False):
+    def set(self, record, value, _default=False, preloaded=None):
         group = record.value.get(self.name)
         fields = {}
         if group is not None:
             fields = group.fields.copy()
             # Unconnect to prevent infinite loop
             group.parent = None
             group.destroy()
@@ -762,15 +784,15 @@
 
         record.value[self.name] = None
         self._set_default_value(record, fields=fields)
         group = record.value[self.name]
 
         # Prevent to trigger group-cleared
         group.parent = None
-        self._set_value(record, value, default=_default)
+        self._set_value(record, value, default=_default, data=preloaded)
         group.parent = record
 
     def set_client(self, record, value, force_change=False):
         # domain inversion could try to set None as value
         if value is None:
             value = []
         # domain inversion could try to set id as value
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/model/group.py` & `tryton-7.2.0/tryton/gui/window/view_form/model/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             try:
                 res += RPCExecute('model', self.model_name, fnct, ids,
                     context=self.context)
             except RPCException:
                 return []
         return list({}.fromkeys(res))
 
-    def load(self, ids, modified=False, position=-1):
+    def load(self, ids, modified=False, position=-1, preloaded=None):
         if not ids:
             return True
 
         if len(ids) > 1:
             self.lock_signal = True
 
         new_records = []
@@ -252,14 +252,16 @@
             if not new_record:
                 new_record = Record(self.model_name, id, group=self)
                 if position == -1:
                     self.append(new_record)
                 else:
                     self.insert(position, new_record)
                     position += 1
+            if preloaded and (already_loaded := preloaded.get(id)):
+                new_record.set(already_loaded, modified=False, validate=False)
             new_records.append(new_record)
 
         # Remove previously removed or deleted records
         for record in self.record_removed[:]:
             if record.id in ids:
                 self.record_removed.remove(record)
         for record in self.record_deleted[:]:
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/model/record.py` & `tryton-7.2.0/tryton/gui/window/view_form/model/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,47 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+import functools
 import logging
+import operator
 
 import tryton.common as common
 from tryton.common import RPCException, RPCExecute
 from tryton.config import CONFIG
 from tryton.pyson import PYSONDecoder
 
 from . import field as fields
 
 logger = logging.getLogger(__name__)
 
 
+def get_x2m_sub_fields(f_attrs, prefix):
+    if f_attrs['loading'] == 'eager' and f_attrs.get('views'):
+        sub_fields = functools.reduce(
+            operator.or_,
+            (v.get('fields', {}) for v in f_attrs['views'].values()),
+            {})
+        x2m_sub_fields = []
+        for s_field, f_def in sub_fields.items():
+            x2m_sub_fields.append(f"{prefix}.{s_field}")
+            if f_def['type'] in {'many2one', 'one2one', 'reference'}:
+                x2m_sub_fields.append(f"{prefix}.{s_field}.rec_name")
+            elif f_def['type'] in {'selection', 'multiselection'}:
+                x2m_sub_fields.append(f"{prefix}.{s_field}:string")
+            elif f_def['type'] in {'one2many', 'many2many'}:
+                x2m_sub_fields.extend(
+                    get_x2m_sub_fields(f_def, f"{prefix}.{s_field}"))
+        x2m_sub_fields.extend(
+            f"{prefix}.{f}"
+            for f in ['_timestamp', '_write', '_delete'])
+        return x2m_sub_fields
+    else:
+        return []
+
+
 class Record:
 
     id = -1
 
     def __init__(self, model_name, obj_id, group=None):
         super(Record, self).__init__()
         self.model_name = model_name
@@ -75,21 +101,27 @@
                     if field.attrs.get('loading', 'eager') == 'eager')
             else:
                 fields = self.group.fields.items()
 
             fnames = [fname for fname, field in fields
                 if fname not in self._loaded
                 and (not views or (views & field.views))]
+            related_read_limit = 0
             for fname in list(fnames):
                 f_attrs = self.group.fields[fname].attrs
                 if f_attrs['type'] in {'many2one', 'one2one', 'reference'}:
                     fnames.append('%s.rec_name' % fname)
                 elif (f_attrs['type'] in {'selection', 'multiselection'}
                         and f_attrs.get('loading', 'lazy') == 'eager'):
                     fnames.append('%s:string' % fname)
+                elif f_attrs['type'] in {'many2many', 'one2many'}:
+                    sub_fields = get_x2m_sub_fields(f_attrs, fname)
+                    fnames.extend(sub_fields)
+                    if sub_fields:
+                        related_read_limit += len(sub_fields)
             if 'rec_name' not in fnames:
                 fnames.append('rec_name')
             fnames.extend(['_timestamp', '_write', '_delete'])
 
             record_context = self.get_context()
             if loading == 'eager':
                 limit = CONFIG['client.limit'] // min(len(fnames), 10)
@@ -128,14 +160,17 @@
                                 id2record[record.id] = record
                         n += 1
 
             ctx = record_context.copy()
             ctx.update(dict(('%s.%s' % (self.model_name, fname), 'size')
                     for fname, field in self.group.fields.items()
                     if field.attrs['type'] == 'binary' and fname in fnames))
+            if related_read_limit:
+                ctx['related_read_limit'] = (
+                    CONFIG['client.limit'] // min(related_read_limit, 10))
             exception = False
             try:
                 values = RPCExecute('model', self.model_name, 'read',
                     list(id2record.keys()), fnames, context=ctx,
                     process_exception=process_exception)
             except RPCException:
                 values = [{'id': x} for x in id2record]
@@ -492,15 +527,17 @@
                     self.value[related] = val[related]
                 else:
                     self.value.pop(related, None)
             self.group.fields[fieldname].set(self, value)
             self._loaded.add(fieldname)
             fieldnames.append(fieldname)
         for fieldname, value in later.items():
-            self.group.fields[fieldname].set(self, value)
+            if isinstance(
+                    field := self.group.fields[fieldname], fields.O2MField):
+                field.set(self, value, preloaded=val.get(f"{fieldname}."))
             self._loaded.add(fieldname)
             fieldnames.append(fieldname)
         if validate:
             self.validate(fieldnames, softvalidation=True)
         if modified:
             self.set_modified()
 
@@ -676,26 +713,30 @@
     def do_autocomplete(self, fieldname):
         self.autocompletion[fieldname] = []
         autocomplete = self.group.fields[fieldname].attrs['autocomplete']
         args = self._get_on_change_args(autocomplete)
         try:
             res = RPCExecute(
                 'model', self.model_name,
-                'autocomplete_' + fieldname, args, context=self.get_context())
+                'autocomplete_' + fieldname, args, context=self.get_context(),
+                process_exception=False)
         except RPCException:
             # ensure res is a list
             res = []
         self.autocompletion[fieldname] = res
 
     def on_scan_code(self, code, depends):
         depends = self.expr_eval(depends)
         values = self._get_on_change_args(depends)
-        changes = RPCExecute(
-            'model', self.model_name, 'on_scan_code', values, code,
-            context=self.get_context(), process_exception=False)
+        try:
+            changes = RPCExecute(
+                'model', self.model_name, 'on_scan_code', values, code,
+                context=self.get_context(), process_exception=False)
+        except RPCException:
+            changes = []
         self.set_on_change(changes)
         self.set_modified()
         return bool(changes)
 
     def set_field_context(self):
         from .group import Group
         for name, field in self.group.fields.items():
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/screen/screen.py` & `tryton-7.2.0/tryton/gui/window/view_form/screen/screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,19 +112,18 @@
                 while isinstance(child, (Gtk.ScrolledWindow, Gtk.Viewport)):
                     child = child.get_child()
                 child.get_parent().remove(child)
                 parent.add(child)
                 return child
 
             # Remove first level Viewport and ScrolledWindow to fill the Vbox
-            for widget in [
-                    self.context_screen.screen_container.viewport,
-                    self.context_screen.current_view.widget.get_children()[0],
-                    ]:
-                remove_bin(widget)
+            remove_bin(self.context_screen.screen_container.viewport)
+            if self.context_screen.current_view:
+                remove_bin(
+                    self.context_screen.current_view.widget.get_children()[0])
 
             self.screen_container.filter_vbox.pack_start(
                 context_widget, expand=False, fill=True, padding=0)
             self.screen_container.filter_vbox.reorder_child(
                 context_widget, 0)
             self.context_screen.widget.show()
 
@@ -304,15 +303,16 @@
                 break
             self.offset = max(self.offset - self.limit, 0)
         if not only_ids:
             if self.limit is not None and len(ids) == self.limit:
                 try:
                     self.search_count = RPCExecute(
                         'model', self.model_name, 'search_count',
-                        domain, 0, self.count_limit, context=context)
+                        domain, 0, self.count_limit, context=context,
+                        process_exception=False)
                 except RPCException:
                     self.search_count = 0
             else:
                 self.search_count = len(ids)
         self.screen_container.but_prev.set_sensitive(bool(self.offset))
         if (self.limit is not None
                 and len(ids) == self.limit
@@ -516,15 +516,16 @@
         self.windows.clear()
         for view in self.views:
             view.destroy()
         del self.views[:]
         self.group.destroy()
 
     def default_row_activate(self):
-        if (self.current_view.view_type == 'tree'
+        if (self.current_view
+                and self.current_view.view_type == 'tree'
                 and int(self.current_view.attributes.get('keyword_open', 0))):
             return Action.exec_keyword('tree_open', {
                 'model': self.model_name,
                 'id': self.current_record.id if self.current_record else None,
                 'ids': [r.id for r in self.selected_records],
                 }, context=self.local_context, warning=False)
         else:
@@ -532,14 +533,18 @@
                 self.switch_view(view_type='form')
             return True
 
     @property
     def number_of_views(self):
         return len(self.views) + len(self.view_to_load)
 
+    @property
+    def view_index(self):
+        return self.__current_view
+
     def switch_view(
             self, view_type=None, view_id=None, creatable=None, display=True):
         if view_id is not None:
             view_id = int(view_id)
         if self.current_view:
             self.current_view.set_value()
             if (self.current_record
@@ -638,15 +643,15 @@
             self, view_id, view['type'], xml_dom, view.get('field_childs'))
         self.views.append(view)
 
         return view
 
     def new(self, default=True, defaults=None):
         previous_view = self.current_view
-        if self.current_view.view_type == 'calendar':
+        if self.current_view and self.current_view.view_type == 'calendar':
             selected_date = self.current_view.get_selected_date()
         if self.current_view and not self.current_view.creatable:
             self.switch_view(creatable=True)
             if not self.current_view.creatable:
                 return None
         if self.current_record:
             group = self.current_record.group
@@ -691,34 +696,37 @@
                 if initial_value is not None:
                     self.current_record.reset(initial_value)
                 else:
                     self.remove(records=[self.current_record])
 
     def save_current(self):
         if not self.current_record:
-            if self.current_view.view_type == 'tree' and len(self.group):
+            if (self.current_view
+                    and self.current_view.view_type == 'tree'
+                    and len(self.group)):
                 self.current_record = self.group[0]
             else:
                 return True
-        self.current_view.set_value()
         saved = False
         record_id = None
-        fields = self.current_view.get_fields()
+        if self.current_view:
+            self.current_view.set_value()
+            fields = self.current_view.get_fields()
         path = self.current_record.get_path(self.group)
-        if self.current_view.view_type == 'tree':
+        if self.current_view and self.current_view.view_type == 'tree':
             # False value must be not saved
             saved = all((
                     x is not False and x >= 0
                     for x in self.group.save()))
             record_id = self.current_record.id if self.current_record else None
         elif self.current_record.validate(fields):
             record_id = self.current_record.save(force_reload=True)
             # False value must be not saved
             saved = record_id is not False and record_id >= 0
-        else:
+        elif self.current_view:
             self.set_cursor()
             self.current_view.display()
             return False
         if path and record_id:
             path = path[:-1] + ((path[-1][0], record_id),)
         self.current_record = self.group.get_by_path(path)
         self.display()
@@ -738,33 +746,35 @@
             return
         elif current_view.view_type in ('tree', 'form', 'list-form'):
             current_view.set_cursor(new=new, reset_view=reset_view)
 
     def get(self):
         if not self.current_record:
             return None
-        self.current_view.set_value()
+        if self.current_view:
+            self.current_view.set_value()
         return self.current_record.get()
 
     def get_on_change_value(self):
         if not self.current_record:
             return None
-        self.current_view.set_value()
+        if self.current_view:
+            self.current_view.set_value()
         return self.current_record.get_on_change_value()
 
     def modified(self):
-        if self.current_view.view_type != 'tree':
+        if self.current_view and self.current_view.view_type != 'tree':
             if self.current_record:
                 if self.current_record.modified or self.current_record.id < 0:
                     return True
         else:
             for record in self.group:
                 if record.modified or record.id < 0:
                     return True
-        if self.current_view.modified:
+        if self.current_view and self.current_view.modified:
             return True
         return False
 
     def reload(self, ids, written=False):
         self.group.reload(ids)
         if written:
             self.group.written(ids)
@@ -825,14 +835,16 @@
         if new_ids:
             self.current_record = self.group.get(new_ids[0])
         self.display(set_cursor=True)
         return True
 
     def set_tree_state(self):
         view = self.current_view
+        if not view:
+            return
         if view.view_type not in {'tree', 'form', 'list-form'}:
             return
         if id(view) in self.tree_states_done:
             return
         if view.view_type == 'form' and self.tree_states_done:
             return
         if (view.view_type in {'tree', 'list-form'}
@@ -919,35 +931,36 @@
                         selected_paths, separators=(',', ':'))
                     try:
                         RPCExecute('model', 'ir.ui.view_tree_state', 'set',
                             self.model_name, json_domain, view.children_field,
                             json_paths, json_selected_path,
                             process_exception=False)
                         clear_cache('model.ir.ui.view_tree_state.get')
-                    except Exception:
+                    except RPCException:
                         logger.warn(
                             _('Unable to set view tree state'), exc_info=True)
 
     def get_tree_domain(self, parent):
         if parent:
             domain = (self.domain + [(self.exclude_field, '=', parent)])
         else:
             domain = self.domain
         json_domain = json.dumps(
             domain, cls=JSONEncoder, separators=(',', ':'))
         return json_domain
 
     def load(self, ids, set_cursor=True, modified=False, position=-1):
         self.group.load(ids, modified=modified, position=position)
-        self.current_view.reset()
+        if self.current_view:
+            self.current_view.reset()
         self.current_record = None
         self.display(set_cursor=set_cursor)
 
     def display(self, set_cursor=False):
-        if self.views:
+        if self.views and self.current_view:
             self.search_active(self.current_view.view_type
                 in ('tree', 'graph', 'calendar'))
             for view in self.views:
                 # Always display tree view to update model
                 # because view can be used even if it is not shown
                 # like for save_tree_state
                 if (view == self.current_view
@@ -971,15 +984,16 @@
                 self.set_cursor(reset_view=False)
         self.set_tree_state()
         # Force record_message
         self.current_record = self.current_record
 
     def _get_next_record(self, test=False):
         view = self.current_view
-        if (view.view_type in {'tree', 'form'}
+        if (view
+                and view.view_type in {'tree', 'form'}
                 and self.current_record
                 and self.current_record.group):
             group = self.current_record.group
             record = self.current_record
             while group:
                 children = record.children_group(view.children_field)
                 if children:
@@ -999,20 +1013,22 @@
                         break
                     next = parent.next.get(id(parent.group))
                 if not next:
                     break
                 record = next
                 break
             return record
-        elif (view.view_type == 'list-form' and len(self.group)
+        elif (view
+                and view.view_type == 'list-form'
+                and len(self.group)
                 and self.current_record in self.group):
             idx = self.group.index(self.current_record)
             if 0 <= idx < len(self.group) - 1:
                 return self.group[idx + 1]
-        elif view.view_type == 'calendar':
+        elif view and view.view_type == 'calendar':
             record = self.current_record
             goocalendar = view.widgets.get('goocalendar')
             if goocalendar:
                 date = goocalendar.selected_date
                 year = date.year
                 month = date.month
                 start = datetime.datetime(year, month, 1)
@@ -1038,23 +1054,26 @@
 
     def has_next(self):
         next_record = self._get_next_record(test=True)
         return next_record and next_record != self.current_record
 
     def display_next(self):
         view = self.current_view
-        view.set_value()
+        if view:
+            view.set_value()
         self.set_cursor(reset_view=False)
         self.current_record = self._get_next_record()
         self.set_cursor(reset_view=False)
-        view.display()
+        if view:
+            view.display()
 
     def _get_prev_record(self, test=False):
         view = self.current_view
-        if (view.view_type in {'tree', 'form'}
+        if (view
+                and view.view_type in {'tree', 'form'}
                 and self.current_record
                 and self.current_record.group):
             group = self.current_record.group
             record = self.current_record
             idx = group.index(record) - 1
             if idx >= 0:
                 record = group[idx]
@@ -1064,15 +1083,15 @@
                     if children:
                         record = children[-1]
             else:
                 parent = record.parent
                 if parent and record.model_name == parent.model_name:
                     record = parent
             return record
-        elif view.view_type == 'calendar':
+        elif view and view.view_type == 'calendar':
             record = self.current_record
             goocalendar = view.widgets.get('goocalendar')
             if goocalendar:
                 date = goocalendar.selected_date
                 year = date.year
                 month = date.month
                 start = datetime.datetime(year, month, 1)
@@ -1089,33 +1108,37 @@
                 else:
                     for idx, event in enumerate(events):
                         if event.record == record:
                             prev_id = idx - 1
                             if prev_id >= 0:
                                 return events[prev_id].record
                             break
-        elif (view.view_type == 'list-form' and len(self.group)
+        elif (view
+                and view.view_type == 'list-form'
+                and len(self.group)
                 and self.current_record in self.group):
             idx = self.group.index(self.current_record)
             if 0 < idx <= len(self.group) - 1:
                 return self.group[idx - 1]
         else:
             return self.group[-1] if len(self.group) else None
 
     def has_prev(self):
         prev_record = self._get_prev_record(test=True)
         return prev_record and prev_record != self.current_record
 
     def display_prev(self):
         view = self.current_view
-        view.set_value()
+        if view:
+            view.set_value()
         self.set_cursor(reset_view=False)
         self.current_record = self._get_prev_record()
         self.set_cursor(reset_view=False)
-        view.display()
+        if view:
+            view.display()
 
     def invalid_message(self, record=None):
         if record is None:
             record = self.current_record
         domain_string = _('"%s" is not valid according to its domain.')
         domain_parser = DomainParser(
             {n: f.attrs for n, f in record.group.fields.items()})
@@ -1141,14 +1164,16 @@
     def selected_records(self):
         return self.current_view.selected_records if self.current_view else []
 
     @property
     def selected_paths(self):
         if self.current_view and self.current_view.view_type == 'tree':
             return self.current_view.get_selected_paths()
+        else:
+            return []
 
     @property
     def listed_records(self):
         if (self.current_view
                 and self.current_view.view_type in {
                     'tree', 'calendar', 'list-form'}):
             return self.current_view.listed_records
@@ -1180,42 +1205,43 @@
                 return False
             states = record.expr_eval(button.attrs.get('states', {}))
             return not (states.get('invisible') or states.get('readonly'))
 
         if not self.selected_records:
             return []
 
-        buttons = self.current_view.get_buttons()
+        buttons = self.current_view.get_buttons() if self.current_view else []
 
         for record in self.selected_records:
             buttons = [b for b in buttons if is_active(record, b)]
             if not buttons:
                 break
         return buttons
 
     def button(self, button):
         'Execute button on the selected records'
-        self.current_view.set_value()
-        fields = self.current_view.get_fields()
+        if self.current_view:
+            self.current_view.set_value()
+            fields = self.current_view.get_fields()
         for record in self.selected_records:
             domain = record.expr_eval(
                 button.get('states', {})).get('pre_validate', [])
             if not record.validate(fields, pre_validate=domain):
                 warning(self.invalid_message(record), _('Pre-validation'))
                 self.display(set_cursor=True)
                 if domain:
                     # Reset valid state with normal domain
                     record.validate(fields)
                 return
         if button.get('confirm', False) and not sur(button['confirm']):
             return
         if button.get('type', 'class') == 'class':
-            if not self.current_record.save(force_reload=False):
+            record_id = self.current_record.save(force_reload=False)
+            if record_id is False or record_id < 0:
                 return
-        if button.get('type', 'class') == 'class':
             self._button_class(button)
         else:
             self._button_instance(button)
 
     def _button_instance(self, button):
         record = self.current_record
         args = record.expr_eval(button.get('change', []))
@@ -1236,14 +1262,15 @@
             context['_timestamp'].update(record.get_timestamp())
         try:
             action = RPCExecute('model', self.model_name, button['name'],
                 ids, context=context)
         except RPCException:
             action = None
         self.reload(ids, written=True)
+        self.record_saved()
         if isinstance(action, str):
             self.client_action(action)
         elif action:
             Action.execute(action, {
                     'model': self.model_name,
                     'id': self.current_record.id,
                     'ids': ids,
@@ -1272,15 +1299,17 @@
             self.display_prev()
         elif action == 'close':
             from tryton.gui import Main
             Main().sig_win_close()
         elif action.startswith('switch'):
             self.switch_view(*action.split(None, 2)[1:])
         elif action == 'reload':
-            if (self.current_view.view_type in ['tree', 'graph', 'calendar']
+            if (self.current_view
+                    and self.current_view.view_type in [
+                        'tree', 'graph', 'calendar']
                     and not self.parent):
                 self.search_filter()
         elif action == 'reload menu':
             from tryton.gui import Main
             RPCContextReload(Main().sig_win_menu)
         elif action == 'reload context':
             RPCContextReload()
@@ -1296,34 +1325,35 @@
                         context, cls=JSONEncoder, separators=(',', ':'))))
         if self.context_screen:
             query_string.append(
                 ('context_model', self.context_screen.model_name))
         if name:
             query_string.append(
                 ('name', json.dumps(name, separators=(',', ':'))))
-        if self.screen_container.tab_domain:
-            query_string.append(('tab_domain', json.dumps(
-                        self.screen_container.tab_domain,
-                        cls=JSONEncoder, separators=(',', ':'))))
         path = [CONFIG['login.db'], 'model', self.model_name]
         view_ids = [v.view_id for v in self.views] + self.view_ids
-        if self.current_view.view_type != 'form':
+        if self.current_view and self.current_view.view_type != 'form':
+            if self.screen_container.tab_domain:
+                query_string.append(('tab_domain', json.dumps(
+                            self.screen_container.tab_domain,
+                            cls=JSONEncoder, separators=(',', ':'))))
             if self.search_value:
                 search_value = self.search_value
             else:
                 search_string = self.screen_container.get_text()
                 search_value = self.domain_parser.parse(search_string)
             if search_value:
                 query_string.append(('search_value', json.dumps(
                             search_value, cls=JSONEncoder,
                             separators=(',', ':'))))
         elif self.current_record and self.current_record.id > -1:
             path.append(str(self.current_record.id))
-            i = view_ids.index(self.current_view.view_id)
-            view_ids = view_ids[i:] + view_ids[:i]
+            if self.current_view:
+                i = view_ids.index(self.current_view.view_id)
+                view_ids = view_ids[i:] + view_ids[:i]
         if view_ids:
             query_string.append(('views', json.dumps(
                         view_ids, separators=(',', ':'))))
         query_string = urllib.parse.urlencode(query_string)
         return urllib.parse.urlunparse(('tryton',
                 CONFIG['login.host'],
                 '/'.join(path), query_string, '', ''))
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/__init__.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/calendar_.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,17 @@
 
     def _parse_field(self, node, attributes):
         name = attributes['name']
         if name and name == self.exclude_field:
             self.container.add(None, attributes)
             return
 
+        if attributes.get('loading') == 'eager':
+            self.field_attrs[name]['loading'] = 'eager'
+
         widget = self.WIDGETS[attributes['widget']](self.view, attributes)
         self.view.widgets[name].append(widget)
 
         if widget.expand:
             attributes.setdefault('yexpand', True)
             attributes.setdefault('yfill', True)
 
@@ -336,26 +339,15 @@
         notebook.set_scrollable(True)
         notebook.set_border_width(3)
         if attributes.get('height') or attributes.get('width'):
             notebook.set_size_request(
                 int(attributes.get('width', -1)),
                 int(attributes.get('height', -1)))
 
-        # Force to display the first time it switches on a page
-        # This avoids glitch in position of widgets
-        def switch(notebook, page, page_num):
-            if not self.view.widget:
-                # Not yet finish to parse
-                return
-            notebook.grab_focus()
-            self.view.display()
-            notebook.disconnect(handler_id)
-        handler_id = notebook.connect('switch-page', switch)
         self.view.state_widgets.append(notebook)
-
         self.view.notebooks.append(notebook)
         self.container.add(notebook, attributes)
         self.parse_child(node, notebook)
 
     def _parse_page(self, node, attributes):
         tab_box = Gtk.HBox(spacing=3)
         if 'name' in attributes and attributes['name'] == self.exclude_field:
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/binary.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/binary.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/calendar_.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/char.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/char.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,13 @@
 
         self.visibility_checkbox = Gtk.CheckButton()
         self.visibility_checkbox.connect('toggled', self.toggle_visibility)
         Tooltips().set_tip(self.visibility_checkbox, _('Show plain text'))
         self.widget.pack_start(
             self.visibility_checkbox, expand=False, fill=True, padding=0)
 
-    def _readonly_set(self, value):
-        super(Char, self)._readonly_set(value)
-        self.entry.set_editable(not value)
-        self.visibility_checkbox.props.visible = not value
-
     def toggle_visibility(self, button):
-        self.entry.props.visibility = not self.entry.props.visibility
+        if self.autocomplete:
+            entry = self.entry.get_child()
+        else:
+            entry = self.entry
+        entry.props.visibility = not self.entry.props.visibility
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/checkbox.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/checkbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/dictionary.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,14 +466,15 @@
 
         self.tooltips = Tooltips()
         self.tooltips.set_tip(self.but_add, _('Add value'))
         self.tooltips.enable()
 
         self._readonly = False
         self._record_id = None
+        self._popup = False
 
     @property
     def _invalid_widget(self):
         return self.wid_text
 
     def _new_remove_btn(self):
         but_remove = Gtk.Button()
@@ -487,36 +488,40 @@
             self._sig_add()
 
     def _sig_add(self, *args):
         context = self.field.get_context(self.record)
         value = self.wid_text.get_text()
         domain = self.field.domain_get(self.record)
 
+        if self._popup:
+            return
+        else:
+            self._popup = True
+
         def callback(result):
             if result:
                 self.add_new_keys([r[0] for r in result])
             self.wid_text.set_text('')
+            self._popup = False
 
         win = WinSearch(self.schema_model, callback, sel_multi=True,
             context=context, domain=domain, new=False)
         win.screen.search_filter(quote(value))
         win.show()
 
     def add_new_keys(self, ids):
         new_keys = self.field.add_new_keys(ids, self.record)
         self.send_modified()
-        focus = False
-        for key_name in new_keys:
-            if key_name not in self.fields:
-                self.add_line(key_name)
-                if not focus:
-                    # Use idle add because it can be called from the callback
-                    # of WinSearch while the popup is still there
-                    GLib.idle_add(self.fields[key_name].widget.grab_focus)
-                    focus = True
+        value = self.field.get_client(self.record)
+        value.update({k: None for k in new_keys})
+        self.display()
+
+        # Use idle add because it can be called from the callback
+        # of WinSearch while the popup is still there
+        GLib.idle_add(self.fields[new_keys[0]].widget.grab_focus)
 
     def _sig_remove(self, button, key, modified=True):
         self.fields[key].disconnect_signals()
         del self.fields[key]
         del self.buttons[key]
         for widget in self.rows[key]:
             self.grid.remove(widget)
@@ -554,24 +559,24 @@
                 not self._readonly
                 and int(self.attrs.get('create', 1))))
         for button in self.buttons.values():
             button.set_sensitive(bool(
                     not self._readonly
                     and self.attrs.get('delete', True)))
 
-    def add_line(self, key):
+    def add_line(self, key, position):
         key_schema = self.field.keys[key]
         self.fields[key] = DICT_ENTRIES[key_schema['type']](key, self)
         field = self.fields[key]
         text = key_schema['string'] + _(':')
         label = Gtk.Label(
             label=set_underline(text),
             use_underline=True, halign=Gtk.Align.END)
-        self.grid.attach_next_to(
-            label, None, Gtk.PositionType.BOTTOM, 1, 1)
+        self.grid.insert_row(position)
+        self.grid.attach(label, 0, position, 1, 1)
         label.set_mnemonic_widget(field.widget)
         label.show()
         hbox = Gtk.HBox(hexpand=True)
         hbox.pack_start(
             field.widget, expand=field.expand, fill=field.fill, padding=0)
         self.grid.attach_next_to(
             hbox, label, Gtk.PositionType.RIGHT, 1, 1)
@@ -600,34 +605,38 @@
 
         value = self.field.get_client(self.record) if self.field else {}
         new_key_names = set(value.keys()) - set(self.field.keys)
         if new_key_names:
             self.field.add_keys(list(new_key_names), self.record)
         decoder = PYSONDecoder()
 
+        # We remove first the old keys in order to keep the order when
+        # inserting the new ones
+        for key in set(self.fields.keys()) - set(value.keys()):
+            self._sig_remove(None, key, modified=False)
+
         def filter_func(item):
             key, value = item
             return key in self.field.keys
 
         def key(item):
             key, value = item
             return self.field.keys[key]['sequence'] or 0
 
-        for key, val in sorted(filter(filter_func, value.items()), key=key):
+        for position, (key, val) in enumerate(
+                sorted(filter(filter_func, value.items()), key=key)):
             if key not in self.fields:
-                self.add_line(key)
+                self.add_line(key, position)
             widget = self.fields[key]
             widget.set_value(val)
             widget.set_readonly(self._readonly)
             key_domain = decoder.decode(
                 self.field.keys[key].get('domain') or '[]')
             widget_class(
                 widget.widget, 'invalid', not eval_domain(key_domain, value))
-        for key in set(self.fields.keys()) - set(value.keys()):
-            self._sig_remove(None, key, modified=False)
 
         self._set_button_sensitive()
 
     def _completion_match_selected(self, completion, model, iter_):
         record_id, = model.get(iter_, 1)
         self.add_new_keys([record_id])
         self.wid_text.set_text('')
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/document.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/document.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/float.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/float.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/image.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/image.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/integer.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/integer.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/many2many.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/many2many.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
         tooltips = common.Tooltips()
 
         self.wid_text = Gtk.Entry()
         self.wid_text.set_placeholder_text(_('Search'))
         self.wid_text.set_property('width_chars', 13)
         self.wid_text.connect('focus-out-event', self._focus_out)
-        self.focus_out = True
         hbox.pack_start(self.wid_text, expand=True, fill=True, padding=0)
 
         if int(self.attrs.get('completion', 1)):
             self.wid_completion = get_completion(
                 search=self.read_access,
                 create=self.create_access)
             self.wid_completion.connect('match-selected',
@@ -109,14 +108,16 @@
 
         self.title.set_mnemonic_widget(
             self.screen.current_view.mnemonic_widget)
 
         self.screen.widget.connect('key_press_event', self.on_keypress)
         self.wid_text.connect('key_press_event', self.on_keypress)
 
+        self._popup = False
+
     def on_keypress(self, widget, event):
         editable = self.wid_text.get_editable()
         activate_keys = [Gdk.KEY_Tab, Gdk.KEY_ISO_Left_Tab]
         remove_keys = [Gdk.KEY_Delete, Gdk.KEY_KP_Delete]
         if not self.wid_completion:
             activate_keys.append(Gdk.KEY_Return)
         if widget == self.screen.widget:
@@ -157,33 +158,34 @@
         return self.get_access('read')
 
     @property
     def create_access(self):
         return int(self.attrs.get('create', 1)) and self.get_access('create')
 
     def _sig_add(self, *args):
-        if not self.focus_out:
-            return
         domain = self.field.domain_get(self.record)
         add_remove = self.record.expr_eval(self.attrs.get('add_remove'))
         if add_remove:
             domain = [domain, add_remove]
         context = self.field.get_search_context(self.record)
         order = self.field.get_search_order(self.record)
         value = self.wid_text.get_text()
 
-        self.focus_out = False
+        if self._popup:
+            return
+        else:
+            self._popup = True
 
         def callback(result):
-            self.focus_out = True
             if result:
                 ids = [x[0] for x in result]
                 self.screen.load(ids, modified=True)
             self.screen.set_cursor()
             self.wid_text.set_text('')
+            self._popup = False
         win = WinSearch(self.attrs['relation'], callback, sel_multi=True,
             context=context, domain=domain, order=order,
             view_ids=self.attrs.get('view_ids', '').split(','),
             views_preload=self.attrs.get('views', {}),
             new=self.create_access,
             title=self.attrs.get('string'))
         win.screen.search_filter(quote(value))
@@ -211,14 +213,18 @@
             view_ids=view_ids,
             mode=['form'], views_preload=self.attrs.get('views', {}),
             context=context, breadcrumb=breadcrumb)
 
     def _sig_edit(self):
         if not self.screen.current_record:
             return
+        if self._popup:
+            return
+        else:
+            self._popup = True
         # Create a new screen that is not linked to the parent otherwise on the
         # save of the record will trigger the save of the parent
         screen = self._get_screen_form()
         screen.load([self.screen.current_record.id])
         screen.current_record = screen.group.get(self.screen.current_record.id)
 
         def callback(result):
@@ -227,30 +233,34 @@
                 added = 'id' in self.screen.current_record.modified_fields
                 # Force a reload on next display
                 self.screen.current_record.cancel()
                 if added:
                     self.screen.current_record.modified_fields.setdefault('id')
                 # Force a display to clear the CellCache
                 self.screen.display()
+            self._popup = False
         WinForm(screen, callback)
 
     def _sig_new(self, defaults=None):
+        if self._popup:
+            return
+        else:
+            self._popup = True
         screen = self._get_screen_form()
         defaults = defaults.copy() if defaults is not None else {}
         defaults['rec_name'] = self.wid_text.get_text()
 
         def callback(result):
-            self.focus_out = True
             if result:
                 record = screen.current_record
                 self.screen.load([record.id], modified=True)
             self.wid_text.set_text('')
             self.wid_text.grab_focus()
+            self._popup = False
 
-        self.focus_out = False
         WinForm(
             screen, callback, new=True, save_current=True, defaults=defaults)
 
     def _readonly_set(self, value):
         self._readonly = value
         self._set_button_sensitive()
         self.wid_text.set_sensitive(not value)
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/many2one.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/many2one.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.wid_text.connect('key-press-event', self.send_modified)
         self.wid_text.connect('key_press_event', self.sig_key_press)
         self.wid_text.connect('populate-popup', self._populate_popup)
         self.wid_text.connect('focus-out-event',
             lambda x, y: self._focus_out())
         self.wid_text.connect('changed', self.sig_changed)
         self.changed = True
-        self.focus_out = True
+        self._popup = False
 
         if int(self.attrs.get('completion', 1)):
             self.wid_text.connect('changed', self._update_completion)
         self.wid_completion = None
 
         self.wid_text.connect('icon-press', self.sig_edit)
 
@@ -99,21 +99,24 @@
     def id_from_value(value):
         return value
 
     def sig_activate(self):
         model = self.get_model()
         if not model or not common.MODELACCESS[model]['read']:
             return
-        if not self.focus_out or not self.field:
+        if not self.field:
             return
         self.changed = False
         value = self.field.get(self.record)
         model = self.get_model()
 
-        self.focus_out = False
+        if self._popup:
+            return
+        else:
+            self._popup = True
         if model and not self.has_target(value):
             if (not self._readonly
                     and (self.wid_text.get_text()
                         or self.field.get_state_attrs(
                             self.record)['required'])):
                 domain = self.field.domain_get(self.record)
                 context = self.field.get_search_context(self.record)
@@ -122,28 +125,28 @@
 
                 def callback(result):
                     if result:
                         self.field.set_client(self.record,
                             self.value_from_id(*result[0]), force_change=True)
                     else:
                         self.wid_text.set_text('')
-                    self.focus_out = True
+                    self._popup = False
                     self.changed = True
 
                 win = WinSearch(model, callback, sel_multi=False,
                     context=context, domain=domain, order=order,
                     view_ids=self.attrs.get('view_ids', '').split(','),
                     views_preload=self.attrs.get('views', {}),
                     new=self.create_access,
                     title=self.attrs.get('string'),
                     exclude_field=self.attrs.get('relation_field'))
                 win.screen.search_filter(quote(text))
                 win.show()
                 return
-        self.focus_out = True
+        self._popup = False
         self.changed = True
         return
 
     def get_screen(self, search=False):
         domain = self.field.domain_get(self.record)
         if search:
             context = self.field.get_search_context(self.record)
@@ -160,87 +163,92 @@
             views_preload=self.attrs.get('views', {}), readonly=self._readonly,
             exclude_field=self.attrs.get('relation_field'),
             breadcrumb=breadcrumb)
 
     def sig_new(self, defaults=None):
         if not self.create_access:
             return
-        self.focus_out = False
+        if self._popup:
+            return
+        else:
+            self._popup = True
         screen = self.get_screen(search=True)
         defaults = defaults.copy() if defaults is not None else {}
         defaults['rec_name'] = self.wid_text.get_text()
 
         def callback(result):
             if result:
                 self.field.set_client(self.record,
                     self.value_from_id(screen.current_record.id,
                         screen.current_record.rec_name()))
-            self.focus_out = True
+            self._popup = False
         WinForm(
             screen, callback, new=True, save_current=True, defaults=defaults)
 
     def sig_edit(self, entry=None, icon_pos=None, *args):
         if entry:
             entry.grab_focus()
         model = self.get_model()
         if not model or not common.MODELACCESS[model]['read']:
             return
-        if not self.focus_out or not self.field:
+        if not self.field:
             return
         self.changed = False
-        self.focus_out = False
         value = self.field.get(self.record)
 
         if (icon_pos == Gtk.EntryIconPosition.SECONDARY
                 and not self._readonly
                 and self.has_target(value)):
             self.field.set_client(self.record, self.value_from_id(None, ''))
             self.wid_text.set_text('')
             self.changed = True
-            self.focus_out = True
             return
 
+        if self._popup:
+            return
+        else:
+            self._popup = True
         if self.has_target(value):
             m2o_id = self.id_from_value(self.field.get(self.record))
             screen = self.get_screen()
             screen.load([m2o_id])
             screen.current_record = screen.group.get(m2o_id)
 
             def callback(result):
                 if result:
                     self.field.set_client(self.record,
                         self.value_from_id(screen.current_record.id,
                             screen.current_record.rec_name()),
                         force_change=True)
-                self.focus_out = True
+                self._popup = False
                 self.changed = True
             WinForm(screen, callback, save_current=True)
             return
         if not self._readonly:
             domain = self.field.domain_get(self.record)
             context = self.field.get_search_context(self.record)
             order = self.field.get_search_order(self.record)
             text = self.wid_text.get_text()
 
             def callback(result):
                 if result:
                     self.field.set_client(self.record,
                         self.value_from_id(*result[0]), force_change=True)
-                self.focus_out = True
+                self._popup = False
                 self.changed = True
             win = WinSearch(model, callback, sel_multi=False,
                 context=context, domain=domain, order=order,
                 view_ids=self.attrs.get('view_ids', '').split(','),
                 views_preload=self.attrs.get('views', {}),
                 new=self.create_access, title=self.attrs.get('string'),
                 exclude_field=self.attrs.get('relation_field'))
             win.screen.search_filter(quote(text))
             win.show()
             return
-        self.focus_out = True
+        self._popup = False
         self.changed = True
 
     def sig_key_press(self, widget, event, *args):
         editable = self.wid_text.get_editable()
         activate_keys = [Gdk.KEY_Tab, Gdk.KEY_ISO_Left_Tab]
         if not self.wid_completion:
             activate_keys.append(Gdk.KEY_Return)
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/multiselection.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/multiselection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/one2many.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/one2many.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
         self.but_next.add(common.IconFactory.get_image(
                 'tryton-forward', Gtk.IconSize.SMALL_TOOLBAR))
         self.but_next.set_relief(Gtk.ReliefStyle.NONE)
         hbox.pack_start(self.but_next, expand=False, fill=False, padding=0)
 
         hbox.pack_start(Gtk.VSeparator(), expand=False, fill=True, padding=0)
 
-        self.focus_out = True
         self.wid_completion = None
         if attrs.get('add_remove'):
 
             self.wid_text = Gtk.Entry()
             self.wid_text.set_placeholder_text(_('Search'))
             self.wid_text.set_property('width_chars', 13)
             self.wid_text.connect('focus-out-event', self._focus_out)
@@ -178,14 +177,16 @@
         self.title.set_mnemonic_widget(
             self.screen.current_view.mnemonic_widget)
 
         self.screen.widget.connect('key_press_event', self.on_keypress)
         if self.attrs.get('add_remove'):
             self.wid_text.connect('key_press_event', self.on_keypress)
 
+        self._popup = False
+
     def get_access(self, type_):
         model = self.attrs['relation']
         if model:
             return common.MODELACCESS[model][type_]
         else:
             return True
 
@@ -366,20 +367,25 @@
 
         if self.attrs.get('product'):
             self._new_product(defaults)
         else:
             self._new_single(defaults)
 
     def _new_single(self, defaults=None):
+        if self._popup:
+            return
+        else:
+            self._popup = True
         sequence = self._sequence()
 
         def update_sequence():
             if sequence:
                 self.screen.group.set_sequence(
                     field=sequence, position=self.screen.new_position)
+            self._popup = False
 
         if self.screen.current_view.creatable:
             self.screen.new()
             self.screen.current_view.widget.set_sensitive(True)
             update_sequence()
         else:
             field_size = self.record.expr_eval(self.attrs.get('size')) or -1
@@ -388,14 +394,18 @@
                 self.screen, lambda a: update_sequence(), new=True,
                 defaults=defaults, many=field_size)
 
     def _new_product(self, defaults=None):
         fields = self.attrs['product'].split(',')
         product = {}
 
+        if self._popup:
+            return
+        else:
+            self._popup = True
         first = self.screen.new(default=False)
         default = first.default_get(defaults=defaults)
         first.set_default(default)
 
         def search_set(*args):
             if not fields:
                 return make_product()
@@ -416,14 +426,15 @@
                 context=context, domain=domain, order=order,
                 title=self.attrs.get('string'))
             win_search.win.connect('destroy', search_set)
             win_search.screen.search_filter()
             win_search.show()
 
         def make_product():
+            self._popup = False
             self.screen.group.remove(first, remove=True)
             if not product:
                 return
 
             fields = list(product.keys())
             for values in itertools.product(*list(product.values())):
                 record = self.screen.new(default=False)
@@ -444,15 +455,22 @@
     def _sig_edit(self, widget=None):
         if not common.MODELACCESS[self.screen.model_name]['read']:
             return
         if not self._validate():
             return
         record = self.screen.current_record
         if record:
-            WinForm(self.screen, lambda a: None)
+            if self._popup:
+                return
+            else:
+                self._popup = True
+
+            def callback(result):
+                self._popup = False
+            WinForm(self.screen, callback)
 
     def _sig_next(self, widget):
         if not self._validate():
             return
         self.screen.display_next()
 
     def _sig_previous(self, widget):
@@ -471,40 +489,41 @@
                 return
         self.screen.remove(remove=remove)
 
     def _sig_undelete(self, button):
         self.screen.unremove()
 
     def _sig_add(self, *args):
-        if not self.focus_out:
-            return
         if not self.write_access or not self.read_access:
             return
         self.view.set_value()
         domain = self.field.domain_get(self.record)
         context = self.field.get_search_context(self.record)
         domain = [domain, self.record.expr_eval(self.attrs.get('add_remove'))]
         removed_ids = self.field.get_removed_ids(self.record)
         domain = ['OR', domain, ('id', 'in', removed_ids)]
         text = self.wid_text.get_text()
 
-        self.focus_out = False
+        if self._popup:
+            return
+        else:
+            self._popup = True
 
         sequence = self._sequence()
 
         def callback(result):
-            self.focus_out = True
             if result:
                 ids = [x[0] for x in result]
                 self.screen.load(ids, modified=True)
                 if sequence:
                     self.screen.group.set_sequence(
                         field=sequence, position=self.screen.new_position)
             self.screen.set_cursor()
             self.wid_text.set_text('')
+            self._popup = False
 
         order = self.field.get_search_order(self.record)
         win = WinSearch(self.attrs['relation'], callback, sel_multi=True,
             context=context, domain=domain, order=order,
             view_ids=self.attrs.get('view_ids', '').split(','),
             views_preload=self.attrs.get('views', {}),
             new=self.but_new.get_property('sensitive'),
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/progressbar.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/progressbar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/pyson.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/pyson.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/reference.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/reference.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/richtextbox.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/richtextbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/selection.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/selection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/state_widget.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/state_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         else:
             state_changes = {}
         required = ((field and field.attrs.get('required'))
                 or state_changes.get('required'))
         readonly = ((field and field.attrs.get('readonly'))
                 or state_changes.get('readonly', not bool(field)))
         common.apply_label_attributes(self, readonly, required)
+        self.set_max_width_chars(80)
+        self.set_line_wrap(True)
 
 
 class VBox(StateMixin, Gtk.VBox):
     pass
 
 
 class Image(StateMixin, Gtk.Image):
@@ -183,22 +185,24 @@
             if tab_domains:
                 for i, (_, tab_domain) in enumerate(tab_domains):
                     common.RPCExecute(
                         'model', action['res_model'], 'search_count',
                         ['AND', domain, tab_domain], 0, 100, context=context,
                         callback=functools.partial(
                             self._set_count, idx=i, current=self._current,
-                            counter=counter, label=label))
+                            counter=counter, label=label),
+                        process_exception=False)
             else:
                 common.RPCExecute(
                     'model', action['res_model'], 'search_count',
                     domain, 0, 100, context=context,
                     callback=functools.partial(
                         self._set_count, current=self._current,
-                        counter=counter, label=label))
+                        counter=counter, label=label),
+                    process_exception=False)
 
     def _set_count(self, value, idx=0, current=None, counter=None, label=''):
         if current != self._current or not self.get_parent():
             return
         try:
             count = value()
             if count > 99:
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/textbox.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/textbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/timedelta.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/url.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/url.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/form_gtk/widget.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/widget.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/graph.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/bar.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/bar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/graph.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/line.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/line.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/graph_gtk/pie.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/pie.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/list.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
+import csv
 import gettext
 import json
 import locale
 import sys
 from functools import wraps
+from io import StringIO
 
 from gi.repository import Gdk, GLib, GObject, Gtk
 from pygtkcompat.generictreemodel import GenericTreeModel
 
 import tryton.common as common
 from tryton.common import (
     RPCException, RPCExecute, Tooltips, domain_inversion, node_attributes,
@@ -716,53 +718,49 @@
         iter_ = model.iter_children(iter_)
         while iter_:
             record = model.get_value(iter_, 0)
             if record.exception:
                 record.cancel()
             iter_ = model.iter_next(iter_)
 
-    def on_copy(self):
+    def on_copy(self, columns=None):
+        if columns is None:
+            columns = self.treeview.get_columns()
+
+        def copy_foreach(treemodel, path, iter, add):
+            record = treemodel.get_value(iter, 0)
+            values = []
+            for col in columns:
+                if not col.get_visible() or not col.name:
+                    continue
+                widget = self.get_column_widget(col)
+                values.append(widget.get_textual_value(record))
+            add(values)
+
         for clipboard_type in [
                 Gdk.SELECTION_CLIPBOARD, Gdk.SELECTION_PRIMARY]:
             clipboard = self.treeview.get_clipboard(clipboard_type)
             selection = self.treeview.get_selection()
-            data = []
-            selection.selected_foreach(self.copy_foreach, data)
-            clipboard.set_text('\n'.join(data), -1)
-
-    def copy_foreach(self, treemodel, path, iter, data):
-        record = treemodel.get_value(iter, 0)
-        values = []
-        for col in self.treeview.get_columns():
-            if not col.get_visible() or not col.name:
-                continue
-            widget = self.get_column_widget(col)
-            values.append('"'
-                + str(widget.get_textual_value(record)).replace('"', '""')
-                + '"')
-        data.append('\t'.join(values))
-        return
+            data = StringIO()
+            writer = csv.writer(data, delimiter='\t', lineterminator='\n')
+            selection.selected_foreach(copy_foreach, writer.writerow)
+            clipboard.set_text(data.getvalue(), -1)
 
     def on_paste(self):
         if not self.editable:
             return
 
-        def unquote(value):
-            if value[:1] == '"' and value[-1:] == '"':
-                return value[1:-1]
-            return value
-        data = []
+        reader = None
         for clipboard_type in [
                 Gdk.SELECTION_CLIPBOARD, Gdk.SELECTION_PRIMARY]:
             clipboard = self.treeview.get_clipboard(clipboard_type)
             text = clipboard.wait_for_text()
             if not text:
                 continue
-            data = [[unquote(v) for v in l.split('\t')]
-                for l in text.splitlines()]
+            reader = csv.reader(StringIO(text), delimiter='\t')
             break
         col = self.treeview.get_cursor()[1]
         columns = [c for c in self.treeview.get_columns()
             if c.get_visible() and c.name]
         if col in columns:
             idx = columns.index(col)
             columns = columns[idx:]
@@ -770,15 +768,15 @@
             record = self.record
             group = record.group
             idx = group.index(record)
         else:
             group = self.group
             idx = len(group)
         default = None
-        for line in data:
+        for line in reader:
             if idx >= len(group):
                 record = group.new(default=False)
                 if default is None:
                     default = record.default_get()
                 record.set_default(default)
                 group.add(record)
             record = group[idx]
@@ -896,20 +894,35 @@
         if event.button == 3:
             try:
                 path, col, x, y = treeview.get_path_at_pos(
                     int(event.x), int(event.y))
             except TypeError:
                 # Outside row
                 return False
+            selection = treeview.get_selection()
             menu = Gtk.Menu()
-            copy_item = Gtk.MenuItem(label=_('Copy'))
-            copy_item.connect('activate', lambda x: self.on_copy())
-            menu.append(copy_item)
+            if selection.count_selected_rows():
+                if selection.count_selected_rows() == 1:
+                    copy_item = Gtk.MenuItem(label=_("Copy"))
+                    copy_item.connect(
+                        'activate', lambda x: self.on_copy([col]))
+                    menu.append(copy_item)
+                    copy_row_label = _("Copy Row")
+                else:
+                    copy_row_label = _("Copy Rows")
+                    if col:
+                        copy_column_item = Gtk.MenuItem(label=_("Copy Column"))
+                        copy_column_item.connect(
+                            'activate', lambda x: self.on_copy(columns=[col]))
+                        menu.append(copy_column_item)
+                copy_row_item = Gtk.MenuItem(label=copy_row_label)
+                copy_row_item.connect('activate', lambda x: self.on_copy())
+                menu.append(copy_row_item)
             if self.editable:
-                paste_item = Gtk.MenuItem(label=_('Paste'))
+                paste_item = Gtk.MenuItem(label=_("Paste Rows"))
                 paste_item.connect('activate', lambda x: self.on_paste())
                 menu.append(paste_item)
 
             def pop(menu, group, record):
                 # Don't activate actions if parent is modified
                 parent = record.parent if record else None
                 while parent:
@@ -935,15 +948,14 @@
                         continue
                     label = field.attrs['string']
                     context = field.get_context(record)
                     populate(
                         menu, model, record_id, title=label, field=field,
                         context=context)
 
-            selection = treeview.get_selection()
             if selection.count_selected_rows() == 1:
                 group = self.group
                 if selection.get_mode() == Gtk.SelectionMode.SINGLE:
                     model = selection.get_selected()[0]
                 elif selection.get_mode() == Gtk.SelectionMode.MULTIPLE:
                     model = selection.get_selected_rows()[0]
                 record = model.get_value(model.get_iter(path), 0)
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/list_form.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/list_form.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/editabletree.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/editabletree.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,16 @@
     def set_value(self):
         path, column = self.get_cursor()
         if not path or not column or not column.name:
             return True
         for renderer in column.get_cells():
             if renderer.props.editing:
                 widget = self.view.get_column_widget(column)
-                self.on_editing_done(widget.editable, renderer)
+                editable = widget.get_editable(renderer)
+                self.on_editing_done(editable, renderer)
         return True
 
     def on_keypressed(self, entry, event, renderer):
         path = self.get_cursor()[0]
         column = self.get_column_from_renderer(renderer)
         model = self.get_model()
         record = model.get_value(model.get_iter(path), 0)
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/list_gtk/widget.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from tryton.common.cellrenderercombo import CellRendererCombo
 from tryton.common.cellrendererfloat import CellRendererFloat
 from tryton.common.cellrendererinteger import CellRendererInteger
 from tryton.common.cellrenderertext import (
     CellRendererText, CellRendererTextCompletion)
 from tryton.common.cellrenderertoggle import CellRendererToggle
 from tryton.common.completion import get_completion, update_completion
-from tryton.common.datetime_ import CellRendererDate, CellRendererTime
+from tryton.common.datetime_ import (
+    CellRendererDate, CellRendererTime, date_parse)
 from tryton.common.domain_parser import quote
 from tryton.common.selection import (
     PopdownMixin, SelectionMixin, selection_shortcuts)
 from tryton.config import CONFIG
 from tryton.gui.window.view_form.screen import Screen
 from tryton.gui.window.win_form import WinForm
 from tryton.gui.window.win_search import WinSearch
@@ -210,16 +211,20 @@
         cell.set_property('visible', not invisible)
         if self.icon:
             if self.icon in record.group.fields:
                 value = record[self.icon].get_client(record) or ''
             else:
                 value = self.icon
             if self.attrs.get('icon_type') == 'url':
+                def callback(pixbuf):
+                    self.display_counters.pop(record.id, None)
+                    self.view.treeview.queue_resize()  # trigger a redraw
                 pixbuf = common.IconFactory.get_pixbuf_url(
-                    value, size_param=self.attrs.get('url_size'))
+                    value, size_param=self.attrs.get('url_size'),
+                    callback=callback)
             else:
                 pixbuf = common.IconFactory.get_pixbuf(
                     value, Gtk.IconSize.BUTTON)
             cell.set_property('pixbuf', pixbuf)
         else:
             text = self.attrs.get('string', '')
             if not text:
@@ -372,14 +377,22 @@
             self.editable = None
             self.editing = None
         self.editable = editable
         self.editing = self._get_record_field_from_path(path)
         editable.connect('remove-widget', remove)
         return False
 
+    def get_editable(self, renderer):
+        if self.renderer == renderer:
+            return self.editable
+        for cell in self.prefixes + self.suffixes:
+            editable = cell.get_editable(renderer)
+            if editable:
+                return editable
+
 
 class Char(GenericText):
 
     @realized
     @CellCache.cache
     def setter(self, column, cell, store, iter_, user_data=None):
         super(Char, self).setter(column, cell, store, iter_, user_data)
@@ -397,27 +410,27 @@
         if renderer is None:
             renderer = CellRendererInteger
         super(Int, self).__init__(view, attrs, renderer=renderer)
         self.factor = float(attrs.get('factor', 1))
         self.symbol = attrs.get('symbol')
         self.grouping = bool(int(attrs.get('grouping', 1)))
         if self.symbol:
-            self.renderer_prefix = Symbol(view, attrs, 0)
-            self.renderer_suffix = Symbol(view, attrs, 1)
+            self._cell_prefix = Symbol(view, attrs, 0)
+            self._cell_suffix = Symbol(view, attrs, 1)
 
     @property
     def prefixes(self):
         if self.symbol:
-            return [self.renderer_prefix]
+            return [self._cell_prefix]
         return []
 
     @property
     def suffixes(self):
         if self.symbol:
-            return [self.renderer_suffix]
+            return [self._cell_suffix]
         return []
 
     @catch_errors()
     def get_textual_value(self, record):
         record.load(self.attrs['name'], process_exception=False)
         return record[self.attrs['name']].get_client(
             record, factor=self.factor, grouping=self.grouping)
@@ -489,14 +502,25 @@
         record.load(self.attrs['name'], process_exception=False)
         value = record[self.attrs['name']].get_client(record)
         if value:
             return value.strftime(self.renderer.props.format)
         else:
             return ''
 
+    def value_from_text(self, record, text, callback=None):
+        if isinstance(text, str):
+            field = record[self.attrs['name']]
+            try:
+                # Use a datetime instance and rely on field to convert to the
+                # proper type
+                text = date_parse(text, self.get_format(record, field))
+            except (ValueError, OverflowError):
+                text = None
+        return super().value_from_text(record, text, callback=callback)
+
 
 class Time(Date):
 
     def __init__(self, view, attrs, renderer=None):
         if renderer is None:
             renderer = CellRendererTime
         super(Time, self).__init__(view, attrs, renderer=renderer)
@@ -550,28 +574,28 @@
 
     def __init__(self, view, attrs, renderer=None):
         if renderer is None:
             renderer = CellRendererText
         super(Binary, self).__init__(view, attrs, renderer=renderer)
         self.renderer.set_property('editable', False)
         self.renderer.set_property('xalign', self.align)
-        self.renderer_save = _BinarySave(self)
-        self.renderer_select = _BinarySelect(self)
+        self._cell_save = _BinarySave(self)
+        self._cell_select = _BinarySelect(self)
         if self.attrs.get('filename'):
-            self.renderer_open = _BinaryOpen(self)
+            self._cell_open = _BinaryOpen(self)
         else:
-            self.renderer_open = None
+            self._cell_open = None
 
     @property
     def prefixes(self):
-        return filter(None, [self.renderer_open])
+        return filter(None, [self._cell_open])
 
     @property
     def suffixes(self):
-        return [self.renderer_save, self.renderer_select]
+        return [self._cell_save, self._cell_select]
 
     @catch_errors()
     def get_textual_value(self, record):
         record.load(self.attrs['name'], process_exception=False)
         field = record[self.attrs['name']]
         if hasattr(field, 'get_size'):
             size = field.get_size(record)
@@ -798,14 +822,15 @@
 
 class M2O(GenericText):
 
     def __init__(self, view, attrs, renderer=None):
         if renderer is None and int(attrs.get('completion', 1)):
             renderer = partial(CellRendererTextCompletion, self.set_completion)
         super(M2O, self).__init__(view, attrs, renderer=renderer)
+        self._popup = False
 
     def get_model(self, record, field):
         return self.attrs['relation']
 
     def has_target(self, value):
         return value is not None
 
@@ -826,15 +851,16 @@
             if callback:
                 callback()
             return
 
         if model and common.get_toplevel_window().get_focus():
             field = record[self.attrs['name']]
             win = self.search_remote(record, field, text, callback=callback)
-            win.show()
+            if win:
+                win.show()
 
     def editing_started(self, cell, editable, path):
         super(M2O, self).editing_started(cell, editable, path)
         record, field = self._get_record_field_from_path(path)
         model = self.get_model(record, field)
 
         def changed(editable):
@@ -895,15 +921,17 @@
             return
         elif not access['read']:
             return
 
         domain = field.domain_get(record)
         context = field.get_context(record)
         if not create and changed:
-            self.search_remote(record, field, text, callback=callback).show()
+            win = self.search_remote(record, field, text, callback=callback)
+            if win:
+                win.show()
             return
         target_id = self.id_from_value(field.get(record))
 
         breadcrumb = list(self.view.screen.breadcrumb)
         breadcrumb.append(
             field.attrs.get('string') or common.MODELNAME.get(model))
         screen = Screen(model, domain=domain, context=context,
@@ -935,21 +963,27 @@
         model = self.get_model(record, field)
         domain = field.domain_get(record)
         context = field.get_search_context(record)
         order = field.get_search_order(record)
         access = common.MODELACCESS[model]
         create_access = int(self.attrs.get('create', 1)) and access['create']
 
+        if self._popup:
+            return
+        else:
+            self._popup = True
+
         def search_callback(found):
             value = None
             if found:
                 value = self.value_from_id(model, *found[0])
                 field.set_client(record, value)
             if callback:
                 callback()
+            self._popup = False
         win = WinSearch(model, search_callback, sel_multi=False,
             context=context, domain=domain,
             order=order, view_ids=self.attrs.get('view_ids', '').split(','),
             new=create_access, title=self.attrs.get('string'))
         win.screen.search_filter(quote(text))
         return win
 
@@ -1229,19 +1263,19 @@
         return ';'.join(values)
 
 
 class Reference(M2O):
 
     def __init__(self, view, attrs, renderer=None):
         super(Reference, self).__init__(view, attrs, renderer=renderer)
-        self.renderer_selection = _ReferenceSelection(view, attrs)
+        self._cell_selection = _ReferenceSelection(view, attrs)
 
     @property
     def prefixes(self):
-        return [self.renderer_selection]
+        return [self._cell_selection]
 
     def get_model(self, record, field):
         value = field.get_client(record)
         if value:
             model, value = value
             return model
```

### Comparing `tryton-7.0.9/tryton/gui/window/view_form/view/screen_container.py` & `tryton-7.2.0/tryton/gui/window/view_form/view/screen_container.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/win_csv.py` & `tryton-7.2.0/tryton/gui/window/win_csv.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/win_export.py` & `tryton-7.2.0/tryton/gui/window/win_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 import base64
 import csv
 import datetime
 import gettext
 import json
 import locale
 import os
-import tempfile
 import urllib.parse
 from itertools import zip_longest
 from numbers import Number
 
 from gi.repository import Gdk, GObject, Gtk
 
 import tryton.common as common
-from tryton.common import RPCException, RPCExecute
+from tryton.common import RPCException, RPCExecute, tempfile
 from tryton.config import CONFIG
 from tryton.gui.window.win_csv import WinCSV
 from tryton.jsonrpc import JSONEncoder
 from tryton.rpc import CONNECTION, clear_cache
 
 _ = gettext.gettext
```

### Comparing `tryton-7.0.9/tryton/gui/window/win_form.py` & `tryton-7.2.0/tryton/gui/window/win_form.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/win_import.py` & `tryton-7.2.0/tryton/gui/window/win_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import base64
 import csv
+import datetime as dt
 import gettext
 import locale
 from decimal import Decimal
 
 from gi.repository import Gtk
 
 import tryton.common as common
 from tryton.common import RPCException, RPCExecute
-from tryton.common.datetime_ import date_parse
 from tryton.gui.window.win_csv import WinCSV
 
 _ = gettext.gettext
 
 
 class WinImport(WinCSV):
     "Window import"
@@ -208,21 +208,26 @@
                         type_ = self.fields_data[field]['type']
                         if type_ == 'integer':
                             val = locale.atoi(val)
                         elif type_ == 'float':
                             val = locale.atof(val)
                         elif type_ == 'numeric':
                             val = Decimal(locale.delocalize(val))
-                        elif type_ in ['date', 'datetime']:
-                            val = date_parse(val, common.date_format())
+                        elif type_ == 'date':
+                            val = dt.datetime.strptime(
+                                val, common.date_format()).date()
+                        elif type_ == 'datetime':
+                            val = dt.datetime.strptime(
+                                val, common.date_format() + ' %X')
                         elif type_ == 'binary':
                             val = base64.b64decode(val)
                     row.append(val)
                 data.append(row)
-        except (IOError, UnicodeDecodeError, csv.Error) as exception:
+        except (IOError, UnicodeDecodeError, csv.Error, ValueError) \
+                as exception:
             common.warning(str(exception), _("Import failed"))
             return
         try:
             count = RPCExecute(
                 'model', self.model, 'import_data', fields, data,
                 context=self.context)
         except RPCException:
```

### Comparing `tryton-7.0.9/tryton/gui/window/win_search.py` & `tryton-7.2.0/tryton/gui/window/win_search.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/window.py` & `tryton-7.2.0/tryton/gui/window/window.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/gui/window/wizard.py` & `tryton-7.2.0/tryton/gui/window/wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,24 +146,25 @@
 
     def destroy(self, action=None):
         if self.screen:
             self.screen.destroy()
 
     def end(self, callback=None):
         def end_callback(action):
-            self.destroy(action=action())
-            if callback:
-                callback()
-        try:
-            RPCExecute('wizard', self.action, 'delete', self.session_id,
-                process_exception=False, callback=end_callback)
-        except Exception:
-            logger.warn(
-                "Unable to delete session %s of wizard %s",
-                self.session_id, self.action, exc_info=True)
+            try:
+                self.destroy(action=action())
+                if callback:
+                    callback()
+            except RPCException:
+                logger.warn(
+                    "Unable to delete session %s of wizard %s",
+                    self.session_id, self.action, exc_info=True)
+        RPCExecute(
+            'wizard', self.action, 'delete', self.session_id,
+            process_exception=False, callback=end_callback)
 
     def clean(self):
         for widget in self.widget.get_children():
             self.widget.remove(widget)
         self.states = {}
 
     def response(self, widget, response):
@@ -398,14 +399,16 @@
     def close(self, widget, event=None):
         widget.stop_emission_by_name('close')
         if self.end_state in self.states:
             self.states[self.end_state].clicked()
         return True
 
     def show(self):
+        if not self.screen:
+            return
         view = self.screen.current_view
         if view.view_type == 'form':
             expand = False
             for name in view.get_fields():
                 for widget in view.widgets[name]:
                     if widget.expand:
                         expand = True
```

### Comparing `tryton-7.0.9/tryton/jsonrpc.py` & `tryton-7.2.0/tryton/jsonrpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import base64
 import datetime
 import errno
+import gettext
 import hashlib
 import http.client
 import json
 import logging
 import socket
 import ssl
 import threading
 import xmlrpc.client
-from collections import defaultdict
 from contextlib import contextmanager
 from decimal import Decimal
 from functools import partial, reduce
 from urllib.parse import quote, urljoin
 
+from .cache import CacheDict
+from .config import CONFIG
+
 __all__ = ["ResponseError", "Fault", "ProtocolError", "Transport",
     "ServerProxy", "ServerPool"]
 CONNECT_TIMEOUT = 5
 DEFAULT_TIMEOUT = None
 logger = logging.getLogger(__name__)
+_ = gettext.gettext
 
 
 def deepcopy(obj):
     """Recursively copy python mutable datastructures"""
     if isinstance(obj, (list, tuple)):
         return [deepcopy(o) for o in obj]
     elif isinstance(obj, dict):
@@ -134,15 +138,14 @@
     def close(self):
         return json.loads(''.join(self.data), object_hook=object_hook)
 
 
 class Transport(xmlrpc.client.SafeTransport):
 
     accept_gzip_encoding = True
-    encode_threshold = 1400  # common MTU
 
     def __init__(
             self, fingerprints=None, ca_certs=None, session=None):
         xmlrpc.client.Transport.__init__(self)
         self._connection = (None, None)
         self.__fingerprints = fingerprints
         self.__ca_certs = ca_certs
@@ -190,60 +193,71 @@
         if self._connection and host == self._connection[0]:
             return self._connection[1]
         chost, self._extra_headers, x509 = self.get_host_info(host)
 
         ssl_ctx = ssl.create_default_context(cafile=self.__ca_certs)
 
         def http_connection():
-            self._connection = host, http.client.HTTPConnection(chost,
-                timeout=CONNECT_TIMEOUT)
-            self._connection[1].connect()
-            sock = self._connection[1].sock
-            sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
-            sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+            connection = http.client.HTTPConnection(
+                chost, timeout=CONNECT_TIMEOUT)
+            self._connection = host, connection
+            connection.connect()
+            sock = connection.sock
+            if sock:
+                sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+            return connection
 
         def https_connection(allow_http=False):
-            self._connection = host, http.client.HTTPSConnection(chost,
-                timeout=CONNECT_TIMEOUT, context=ssl_ctx)
+            connection = http.client.HTTPSConnection(
+                chost, timeout=CONNECT_TIMEOUT, context=ssl_ctx)
+            self._connection = host, connection
             try:
-                self._connection[1].connect()
-                sock = self._connection[1].sock
-                sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
-                sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
-                try:
-                    peercert = sock.getpeercert(True)
-                except socket.error:
-                    peercert = None
+                connection.connect()
+                sock = connection.sock
+                if sock:
+                    sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+                    try:
+                        peercert = sock.getpeercert(True)
+                    except socket.error:
+                        peercert = None
 
                 def format_hash(value):
                     return reduce(lambda x, y: x + y[1].upper()
                         + ((y[0] % 2 and y[0] + 1 < len(value)) and ':' or ''),
                         enumerate(value), '')
-                return format_hash(hashlib.sha1(peercert).hexdigest())
+                return connection, format_hash(
+                    hashlib.sha1(peercert).hexdigest())
             except (socket.error, ssl.SSLError, ssl.CertificateError):
                 if allow_http:
-                    http_connection()
+                    return http_connection(), None
                 else:
                     raise
 
         fingerprint = ''
         if (self.__fingerprints is not None
                 and self.__fingerprints.exists(chost)):
             if self.__fingerprints.get(chost):
-                fingerprint = https_connection()
+                connection, fingerprint = https_connection()
             else:
-                http_connection()
+                connection = http_connection()
         else:
-            fingerprint = https_connection(allow_http=True)
+            connection, fingerprint = https_connection(allow_http=True)
 
         if self.__fingerprints is not None:
             self.__fingerprints.set(chost, fingerprint)
-        self._connection[1].timeout = DEFAULT_TIMEOUT
-        self._connection[1].sock.settimeout(DEFAULT_TIMEOUT)
-        return self._connection[1]
+        connection.timeout = DEFAULT_TIMEOUT
+        sock = connection.sock
+        if sock:
+            sock.settimeout(DEFAULT_TIMEOUT)
+        return connection
+
+    @property
+    def encode_threshold(self):
+        if self.session:
+            return 1400  # common MTU
 
 
 class ServerProxy(xmlrpc.client.ServerProxy):
     __id = 0
 
     def __init__(self, host, port, database='', verbose=0,
             fingerprints=None, ca_certs=None, session=None, cache=None):
@@ -294,15 +308,16 @@
                     )
         except xmlrpc.client.ProtocolError as e:
             raise Fault(str(e.errcode), e.errmsg)
         except Exception:
             self.__transport.close()
             raise
         if response['id'] != id_:
-            raise ResponseError('Invalid response id (%s) excpected %s' %
+            raise ResponseError(
+                _("Invalid response id (%s) expected %s") %
                 (response['id'], id_))
         if response.get('error'):
             raise Fault(*response['error'])
         if self.__cache and response.get('cache'):
             self.__cache.set(
                 methodname, dumper(params), response['cache'],
                 response['result'])
@@ -388,15 +403,18 @@
         if self._cache:
             self._cache.clear(prefix)
 
 
 class _Cache:
 
     def __init__(self):
-        self.store = defaultdict(dict)
+        cache_size = CONFIG['rpc.cache_size']
+        self.store = CacheDict(
+            cache_len=cache_size,
+            default_factory=lambda: CacheDict(cache_len=cache_size))
 
     def cached(self, prefix):
         return prefix in self.store
 
     def set(self, prefix, key, expire, value):
         if isinstance(expire, (int, float)):
             expire = datetime.timedelta(seconds=expire)
```

### Comparing `tryton-7.0.9/tryton/plugins/__init__.py` & `tryton-7.2.0/tryton/plugins/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,19 @@
         os.path.join(CURRENT_DIR, 'plugins'),
         ]
     paths = list(filter(os.path.isdir, paths))
 
     imported = set()
     for path in paths:
         finder = importlib.machinery.FileFinder(
-            path, (
-                importlib.machinery.SourceFileLoader,
-                importlib.machinery.SOURCE_SUFFIXES))
+            path,
+            (importlib.machinery.SourceFileLoader,
+                importlib.machinery.SOURCE_SUFFIXES),
+            (importlib.machinery.SourcelessFileLoader,
+                importlib.machinery.BYTECODE_SUFFIXES))
         for plugin in os.listdir(path):
             module = os.path.splitext(plugin)[0]
             if (module.startswith('_') or module in imported):
                 continue
             module = 'tryton.plugins.%s' % module
             spec = finder.find_spec(module)
             if not spec:
```

### Comparing `tryton-7.0.9/tryton/plugins/translation/__init__.py` & `tryton-7.2.0/tryton/plugins/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/pyson.py` & `tryton-7.2.0/tryton/pyson.py`

 * *Files 6% similar despite different names*

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
+        return '<=' if self._equal else '<'
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
+        return '>=' if self._equal else '>'
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

### Comparing `tryton-7.0.9/tryton/rpc.py` & `tryton-7.2.0/tryton/rpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,32 @@
         except (Fault, socket.error, http.client.CannotSendRequest):
             pass
         CONNECTION.close()
         CONNECTION = None
     _USER = None
 
 
+def reset_password():
+    from tryton import common
+    host = CONFIG['login.host']
+    hostname = common.get_hostname(host)
+    port = common.get_port(host)
+    database = CONFIG['login.db']
+    username = CONFIG['login.login']
+    language = CONFIG['client.lang']
+    if not all([host, database, username]):
+        return
+    try:
+        connection = ServerProxy(hostname, port, database)
+        logger.info('common.db.reset_password(%s, %s)', (username, language))
+        connection.common.db.reset_password(username, language)
+    except Fault as exception:
+        logger.debug(exception.faultCode)
+
+
 def execute(*args):
     global CONNECTION, _USER
     if CONNECTION is None:
         raise TrytonServerError('403')
     try:
         name = '.'.join(args[:3])
         args = args[3:]
```

### Comparing `tryton-7.0.9/tryton/tests/test_common.py` & `tryton-7.2.0/tryton/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/tests/test_common_domain_parser.py` & `tryton-7.2.0/tryton/tests/test_common_domain_parser.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/tests/test_common_selection.py` & `tryton-7.2.0/tryton/tests/test_common_selection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/tests/test_common_timedelta.py` & `tryton-7.2.0/tryton/tests/test_common_timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton/translate.py` & `tryton-7.2.0/tryton/translate.py`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton.desktop` & `tryton-7.2.0/tryton.desktop`

 * *Files identical despite different names*

### Comparing `tryton-7.0.9/tryton.egg-info/PKG-INFO` & `tryton-7.2.0/tryton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 7.0.9
+Version: 7.2.0
 Summary: Tryton desktop client
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/latest/client-desktop/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
```

### Comparing `tryton-7.0.9/tryton.egg-info/SOURCES.txt` & `tryton-7.2.0/tryton.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 doc/index.rst
 doc/installation.rst
 doc/releases.rst
 doc/requirements-doc.txt
 doc/usage.rst
 tryton/__init__.py
 tryton/bus.py
+tryton/cache.py
 tryton/client.py
 tryton/config.py
 tryton/device_cookie.py
 tryton/exceptions.py
 tryton/fingerprints.py
 tryton/jsonrpc.py
 tryton/pyson.py
@@ -67,14 +68,15 @@
 tryton/common/environment.py
 tryton/common/focus.py
 tryton/common/htmltextbuffer.py
 tryton/common/number_entry.py
 tryton/common/popup_menu.py
 tryton/common/richtext.py
 tryton/common/selection.py
+tryton/common/tempfile.py
 tryton/common/timedelta.py
 tryton/common/underline.py
 tryton/common/widget_style.py
 tryton/data/locale/tryton.pot
 tryton/data/locale/bg/LC_MESSAGES/tryton.mo
 tryton/data/locale/bg/LC_MESSAGES/tryton.po
 tryton/data/locale/ca/LC_MESSAGES/tryton.mo
```

### Comparing `tryton-7.0.9/win32/gtk-3.0/gdk-pixbuf.loaders` & `tryton-7.2.0/win32/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

