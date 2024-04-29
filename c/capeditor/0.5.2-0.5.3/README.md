# Comparing `tmp/capeditor-0.5.2.tar.gz` & `tmp/capeditor-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.5.2.tar", last modified: Fri Apr  5 13:32:04 2024, max compression
+gzip compressed data, was "capeditor-0.5.3.tar", last modified: Mon Apr 29 12:44:58 2024, max compression
```

## Comparing `capeditor-0.5.2.tar` & `capeditor-0.5.3.tar`

### file list

```diff
@@ -1,139 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 13:31:56.000000 capeditor-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-05 13:32:04.596223 capeditor-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-04-05 13:31:56.000000 capeditor-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.572223 capeditor-0.5.2/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    28279 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/cap_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/caputils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/forms/capimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.576223 capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/0002_alter_capsetting_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/0003_capsetting_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/0004_predefinedalertarea.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/pubsub/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/pubsub/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/pubsub/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/shareable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/shareable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14809 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/shareable/png.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/cap_detail_page.css
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/import_cap_preview.css
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/mapbox-gl-draw.css
--rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.580223 capeditor-0.5.2/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.584223 capeditor-0.5.2/capeditor/static/capeditor/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.588223 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.588223 capeditor-0.5.2/capeditor/static/capeditor/images/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/alert.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/area.png
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/certainty.png
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/extreme.png
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/minor.png
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/moderate.png
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/severe.png
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/images/urgency.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.592223 capeditor-0.5.2/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/cap_accordion.js
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/conditional_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/mapbox-gl-draw.js
--rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/turf.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.592223 capeditor-0.5.2/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.568223 capeditor-0.5.2/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/icons/cap-alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/load_cap_alert.html
--rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/preview_cap_alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-05 13:31:56.000000 capeditor-0.5.2/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:32:04.596223 capeditor-0.5.2/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:32:04.000000 capeditor-0.5.2/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 13:31:56.000000 capeditor-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 13:32:04.596223 capeditor-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-29 12:44:50.000000 capeditor-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-04-29 12:44:58.094514 capeditor-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-04-29 12:44:50.000000 capeditor-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28279 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/cap_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/caputils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/forms/capimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.070514 capeditor-0.5.3/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.070514 capeditor-0.5.3/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0002_alter_capsetting_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0003_capsetting_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0004_predefinedalertarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0005_alter_capsetting_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/pubsub/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/pubsub/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/pubsub/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/cap_detail_page.css
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/import_cap_preview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/mapbox-gl-draw.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/static/capeditor/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.090514 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.090514 capeditor-0.5.3/capeditor/static/capeditor/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/area.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/certainty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/extreme.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/minor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/moderate.png
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/severe.png
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/urgency.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.090514 capeditor-0.5.3/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/cap_accordion.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/conditional_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/mapbox-gl-draw.js
+-rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/turf.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/icons/cap-alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/load_cap_alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/preview_cap_alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 12:44:50.000000 capeditor-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-29 12:44:58.094514 capeditor-0.5.3/setup.cfg
```

### Comparing `capeditor-0.5.2/PKG-INFO` & `capeditor-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.2
+Version: 0.5.3
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -23,18 +23,14 @@
 Requires-Dist: python-magic
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: wagtail-icon-chooser>=0.0.4
 Requires-Dist: adm-boundary-manager>=0.0.6
 Requires-Dist: wagtail-humanitarian-icons>=2.0.0
 Requires-Dist: wagtail-modelchooser>=4.0.1
 Requires-Dist: paho-mqtt
-Requires-Dist: cairosvg
-Requires-Dist: geopandas
-Requires-Dist: matplotlib
-Requires-Dist: cartopy
 Requires-Dist: xmltodict
 
 # CAP Composer  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1">
 
 [![Upload Python Package](https://github.com/wmo-raf/cap-composer/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-composer/actions/workflows/publish.yml)
 
 A [Wagtail](https://wagtail.io/) based Common Alerting Protocol (CAP) Warning Composer. This is a web-based tool for
```

### Comparing `capeditor-0.5.2/README.md` & `capeditor-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/blocks.py` & `capeditor-0.5.3/capeditor/blocks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/cap_settings.py` & `capeditor-0.5.3/capeditor/cap_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     ContactBlock
 )
 from capeditor.forms.widgets import HazardEventTypeWidget, PolygonDrawWidget
 
 
 @register_setting
 class CapSetting(BaseSiteSetting, ClusterableModel):
-    sender = models.CharField(max_length=255, blank=True, null=True, verbose_name=_("CAP Sender Identifier"),
-                              help_text=_("Can be the website link or email of the sending institution"))
+    sender = models.CharField(max_length=255, blank=True, null=True, verbose_name=_("CAP Sender Email"),
+                              help_text=_("Email of the sending institution"))
     sender_name = models.CharField(max_length=255, blank=True, null=True, verbose_name=_("CAP Sender Name"),
                                    help_text=_("Name of the sending institution"))
     logo = models.ForeignKey("wagtailimages.Image", null=True, blank=True, on_delete=models.SET_NULL, related_name="+",
                              verbose_name=_("Logo of the sending institution"))
 
     contacts = StreamField([
         ("contact", ContactBlock(label=_("Contact")))
```

### Comparing `capeditor-0.5.2/capeditor/caputils.py` & `capeditor-0.5.3/capeditor/caputils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/constants.py` & `capeditor-0.5.3/capeditor/constants.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/forms/capimporter.py` & `capeditor-0.5.3/capeditor/forms/capimporter.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/forms/fields.py` & `capeditor-0.5.3/capeditor/forms/fields.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/forms/widgets.py` & `capeditor-0.5.3/capeditor/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/migrations/0001_initial.py` & `capeditor-0.5.3/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/migrations/0002_alter_capsetting_options_and_more.py` & `capeditor-0.5.3/capeditor/migrations/0002_alter_capsetting_options_and_more.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/migrations/0003_capsetting_logo.py` & `capeditor-0.5.3/capeditor/migrations/0003_capsetting_logo.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/migrations/0004_predefinedalertarea.py` & `capeditor-0.5.3/capeditor/migrations/0004_predefinedalertarea.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/models.py` & `capeditor-0.5.3/capeditor/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import os
 import uuid
 
-from adminboundarymanager.models import AdminBoundarySettings
-from django.conf import settings
 from django.utils import timezone
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from shapely.geometry import shape
 from wagtail import blocks
 from wagtail.admin.forms import WagtailAdminPageForm
 from wagtail.admin.panels import MultiFieldPanel
@@ -18,15 +15,14 @@
     CONTACT_HELP_TEXT,
     AUDIENCE_HELP_TEXT,
     AlertAddress,
     AlertReference,
     AlertIncident
 )
 from capeditor.constants import SEVERITY_MAPPING, URGENCY_MAPPING, CERTAINTY_MAPPING
-from capeditor.shareable.png import cap_geojson_to_image, CapAlertCardImage
 from .cap_settings import *
 
 
 class CapAlertPageForm(WagtailAdminPageForm):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -152,23 +148,20 @@
                             verbose_name=_("Code"))
     note = models.TextField(blank=True, null=True,
                             help_text=_("The text describing the purpose or significance of the alert message."
                                         "The message note is primarily intended for use with "
                                         "<status> 'Exercise' and <msgType> 'Error'"), verbose_name=_("Note"))
     info = StreamField([
         ("alert_info", AlertInfo(label=_("Alert Information")))
-    ], block_counts={
-        'alert_info': {'min_num': 1},
-    }, use_json_field=True, blank=True,
-        null=True, verbose_name=_("Alert Information"), )
+    ], use_json_field=True, min_num=1, max_num=1, block_counts={'alert_info': {'max_num': 1, "min_num": 1}, },
+        verbose_name=_("Alert Information"), )
 
     addresses = StreamField([
         ("recipient", AlertAddress(label=_("Recipient")))
-    ], use_json_field=True, blank=True,
-        null=True, verbose_name=_("Addresses"),
+    ], use_json_field=True, blank=True, null=True, verbose_name=_("Addresses"),
         help_text=_("The group listing of intended recipients of the alert message, if scope is Private"))
 
     references = StreamField([
         ("reference", AlertReference(label=_("Reference Alert")))
     ], use_json_field=True, blank=True,
         null=True, verbose_name=_("Reference Alerts"))
 
@@ -313,52 +306,7 @@
 
                 info_features = info.value.features
                 for feature in info_features:
                     feature["properties"].update(**properties)
                     features.append(feature)
 
         return features
-
-    def generate_alert_card_image(self):
-
-        site = Site.objects.get(is_default_site=True)
-
-        abm_settings = AdminBoundarySettings.for_site(site)
-        cap_settings = CapSetting.for_site(site)
-        abm_extents = abm_settings.combined_countries_bounds
-
-        info = self.infos[0]
-
-        features = self.get_geojson_features()
-        if features:
-            feature_coll = {
-                "type": "FeatureCollection",
-                "features": features,
-            }
-
-            if abm_extents:
-                # format to what matplotlib expects
-                abm_extents = [abm_extents[0], abm_extents[2], abm_extents[1], abm_extents[3]]
-
-            cap_detail = {
-                "title": self.title,
-                "event": info.get("event"),
-                "sent_on": self.sent,
-                "org_name": cap_settings.sender_name,
-                "severity": info.get("severity"),
-                "properties": info.get("properties"),
-            }
-
-            org_logo = cap_settings.logo
-            if org_logo:
-                cap_detail.update({
-                    "org_logo_file": os.path.join(settings.MEDIA_ROOT, org_logo.file.path)
-                })
-
-                map_img_buffer = cap_geojson_to_image(feature_coll, abm_extents)
-
-                image_content_file = CapAlertCardImage(map_img_buffer, cap_detail,
-                                                       f"{self.identifier}.png").render()
-
-                return image_content_file
-
-        return None
```

### Comparing `capeditor-0.5.2/capeditor/pubsub/base.py` & `capeditor-0.5.3/capeditor/pubsub/base.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/pubsub/mqtt.py` & `capeditor-0.5.3/capeditor/pubsub/mqtt.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/pubsub/publish.py` & `capeditor-0.5.3/capeditor/pubsub/publish.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/renderers.py` & `capeditor-0.5.3/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/serializers.py` & `capeditor-0.5.3/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.5.3/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/css/import_cap_preview.css` & `capeditor-0.5.3/capeditor/static/capeditor/css/import_cap_preview.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/css/mapbox-gl-draw.css` & `capeditor-0.5.3/capeditor/static/capeditor/css/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/css/maplibre-gl.css` & `capeditor-0.5.3/capeditor/static/capeditor/css/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.5.3/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.5.3/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/fonts/mapbox-gl-draw.css` & `capeditor-0.5.3/capeditor/static/capeditor/fonts/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/images/alert.png` & `capeditor-0.5.3/capeditor/static/capeditor/images/alert.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/images/alert.svg` & `capeditor-0.5.3/capeditor/static/capeditor/images/alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/images/area.png` & `capeditor-0.5.3/capeditor/static/capeditor/images/area.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/images/certainty.png` & `capeditor-0.5.3/capeditor/static/capeditor/images/certainty.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/images/extreme.png` & `capeditor-0.5.3/capeditor/static/capeditor/images/extreme.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/images/minor.png` & `capeditor-0.5.3/capeditor/static/capeditor/images/minor.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/images/moderate.png` & `capeditor-0.5.3/capeditor/static/capeditor/images/moderate.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/images/severe.png` & `capeditor-0.5.3/capeditor/static/capeditor/images/severe.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/conditional_fields.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/mapbox-gl-draw.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/mapbox-gl-draw.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/maplibre-gl.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/turf.min.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/turf.min.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-draw-widget.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-draw-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.5.3/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.5.3/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.5.3/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/templates/capeditor/load_cap_alert.html` & `capeditor-0.5.3/capeditor/templates/capeditor/load_cap_alert.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/templates/capeditor/preview_cap_alert.html` & `capeditor-0.5.3/capeditor/templates/capeditor/preview_cap_alert.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.5.3/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html` & `capeditor-0.5.3/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/templates/capeditor/widgets/polygon_draw_widget.html` & `capeditor-0.5.3/capeditor/templates/capeditor/widgets/polygon_draw_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/views.py` & `capeditor-0.5.3/capeditor/views.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor/wagtail_hooks.py` & `capeditor-0.5.3/capeditor/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.2/capeditor.egg-info/PKG-INFO` & `capeditor-0.5.3/capeditor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.2
+Version: 0.5.3
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -23,18 +23,14 @@
 Requires-Dist: python-magic
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: wagtail-icon-chooser>=0.0.4
 Requires-Dist: adm-boundary-manager>=0.0.6
 Requires-Dist: wagtail-humanitarian-icons>=2.0.0
 Requires-Dist: wagtail-modelchooser>=4.0.1
 Requires-Dist: paho-mqtt
-Requires-Dist: cairosvg
-Requires-Dist: geopandas
-Requires-Dist: matplotlib
-Requires-Dist: cartopy
 Requires-Dist: xmltodict
 
 # CAP Composer  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1">
 
 [![Upload Python Package](https://github.com/wmo-raf/cap-composer/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-composer/actions/workflows/publish.yml)
 
 A [Wagtail](https://wagtail.io/) based Common Alerting Protocol (CAP) Warning Composer. This is a web-based tool for
```

### Comparing `capeditor-0.5.2/capeditor.egg-info/SOURCES.txt` & `capeditor-0.5.3/capeditor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,21 +38,20 @@
 capeditor/locale/fr/LC_MESSAGES/django.po
 capeditor/locale/sw/LC_MESSAGES/django.mo
 capeditor/locale/sw/LC_MESSAGES/django.po
 capeditor/migrations/0001_initial.py
 capeditor/migrations/0002_alter_capsetting_options_and_more.py
 capeditor/migrations/0003_capsetting_logo.py
 capeditor/migrations/0004_predefinedalertarea.py
+capeditor/migrations/0005_alter_capsetting_sender.py
 capeditor/migrations/__init__.py
 capeditor/pubsub/__init__.py
 capeditor/pubsub/base.py
 capeditor/pubsub/mqtt.py
 capeditor/pubsub/publish.py
-capeditor/shareable/__init__.py
-capeditor/shareable/png.py
 capeditor/static/capeditor/css/cap_detail_page.css
 capeditor/static/capeditor/css/import_cap_preview.css
 capeditor/static/capeditor/css/mapbox-gl-draw.css
 capeditor/static/capeditor/css/maplibre-gl.css
 capeditor/static/capeditor/css/widget/boundary-widget.css
 capeditor/static/capeditor/css/widget/circle-widget.css
 capeditor/static/capeditor/css/widget/polygon-draw-widget.css
```

### Comparing `capeditor-0.5.2/setup.cfg` & `capeditor-0.5.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.5.2
+version = 0.5.3
 description = Wagtail based CAP composer
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-composer
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
@@ -30,17 +30,13 @@
 	python-magic
 	shapely>=2.0.1
 	wagtail-icon-chooser>=0.0.4
 	adm-boundary-manager>=0.0.6
 	wagtail-humanitarian-icons>=2.0.0
 	wagtail-modelchooser>=4.0.1
 	paho-mqtt
-	cairosvg
-	geopandas
-	matplotlib
-	cartopy
 	xmltodict
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

