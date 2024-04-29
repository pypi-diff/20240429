# Comparing `tmp/ckanext-wysiwyg-0.1.0.tar.gz` & `tmp/ckanext_wysiwyg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-wysiwyg-0.1.0.tar", last modified: Tue Feb 13 08:28:08 2024, max compression
+gzip compressed data, was "ckanext_wysiwyg-0.1.2.tar", last modified: Mon Apr 29 10:37:10 2024, max compression
```

## Comparing `ckanext-wysiwyg-0.1.0.tar` & `ckanext_wysiwyg-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/
--rw-r--r--   0 berry     (1000) berry     (1000)    34500 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/LICENSE
--rw-r--r--   0 berry     (1000) berry     (1000)      199 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/MANIFEST.in
--rw-r--r--   0 berry     (1000) berry     (1000)     3886 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/PKG-INFO
--rw-r--r--   0 berry     (1000) berry     (1000)     3283 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/README.md
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.211258 ckanext-wysiwyg-0.1.0/ckanext/
--rw-r--r--   0 berry     (1000) berry     (1000)      219 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/ckanext/__init__.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.211258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/__init__.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.211258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.211258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/
--rw-r--r--   0 berry     (1000) berry     (1000)      199 2024-01-28 13:03:53.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/ckeditor5-custom-styles.css
--rw-r--r--   0 berry     (1000) berry     (1000)      667 2024-01-28 13:03:57.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/quill-custom-styles.css
--rw-r--r--   0 berry     (1000) berry     (1000)      103 2024-01-28 13:21:00.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/summernote-custom-styles.css
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.211258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/vendor/
--rw-r--r--   0 berry     (1000) berry     (1000)    10098 2024-01-27 11:35:05.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/vendor/ckeditor5.min.css
--rw-r--r--   0 berry     (1000) berry     (1000)    26620 2024-01-27 18:19:46.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/vendor/quill.min.css
--rw-r--r--   0 berry     (1000) berry     (1000)    30478 2024-01-28 13:21:46.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/vendor/summernote.min.css
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.211258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/vendor/
--rw-r--r--   0 berry     (1000) berry     (1000)  1553083 2024-01-27 11:32:25.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/vendor/ckeditor5.min.js
--rw-r--r--   0 berry     (1000) berry     (1000)   215311 2024-01-27 18:19:23.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/vendor/quill.min.js
--rw-r--r--   0 berry     (1000) berry     (1000)   163150 2024-01-28 13:22:00.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/vendor/summernote.min.js
--rw-r--r--   0 berry     (1000) berry     (1000)      795 2024-01-28 15:37:32.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/wysiwyg-ckeditor5-init.js
--rw-r--r--   0 berry     (1000) berry     (1000)     1835 2024-01-28 15:01:46.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/wysiwyg-quill-init.js
--rw-r--r--   0 berry     (1000) berry     (1000)     1358 2024-01-28 15:37:55.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/wysiwyg-summernote-init.js
--rw-r--r--   0 berry     (1000) berry     (1000)     1239 2024-01-28 12:40:35.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/webassets.yml
--rw-r--r--   0 berry     (1000) berry     (1000)      138 2024-01-28 15:48:37.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/helpers.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/logic/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-01-27 09:16:51.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/logic/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)      277 2024-01-27 09:24:03.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/logic/action.py
--rw-r--r--   0 berry     (1000) berry     (1000)      290 2024-01-27 09:22:00.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/logic/auth.py
--rw-r--r--   0 berry     (1000) berry     (1000)      138 2024-01-28 15:48:33.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/logic/validators.py
--rw-r--r--   0 berry     (1000) berry     (1000)      494 2024-02-02 14:42:32.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/plugin.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.211258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.211258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/display_snippets/
--rw-r--r--   0 berry     (1000) berry     (1000)      142 2024-01-28 15:50:05.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/display_snippets/wysiwyg_ckeditor5.html
--rw-r--r--   0 berry     (1000) berry     (1000)      398 2024-01-28 15:49:30.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/display_snippets/wysiwyg_quill.html
--rw-r--r--   0 berry     (1000) berry     (1000)      208 2024-01-28 15:49:37.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/display_snippets/wysiwyg_summernote.html
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/form_snippets/
--rw-r--r--   0 berry     (1000) berry     (1000)      658 2024-01-27 18:04:01.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/form_snippets/wysiwyg_ckeditor5.html
--rw-r--r--   0 berry     (1000) berry     (1000)      516 2024-01-28 15:02:43.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/form_snippets/wysiwyg_quill.html
--rw-r--r--   0 berry     (1000) berry     (1000)      661 2024-01-28 13:38:36.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/templates/scheming/form_snippets/wysiwyg_summernote.html
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/tests/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/tests/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1378 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/tests/test_plugin.py
--rw-r--r--   0 berry     (1000) berry     (1000)      506 2024-01-28 15:48:06.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/utils.py
--rw-r--r--   0 berry     (1000) berry     (1000)      979 2024-01-28 15:37:52.000000 ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/views.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/
--rw-r--r--   0 berry     (1000) berry     (1000)     3886 2024-02-13 08:28:08.000000 ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/PKG-INFO
--rw-r--r--   0 berry     (1000) berry     (1000)     1752 2024-02-13 08:28:08.000000 ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/SOURCES.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        1 2024-02-13 08:28:08.000000 ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/dependency_links.txt
--rw-r--r--   0 berry     (1000) berry     (1000)      119 2024-02-13 08:28:08.000000 ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/entry_points.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-02-13 08:28:08.000000 ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/namespace_packages.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-02-13 08:28:08.000000 ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/top_level.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/requirements.txt
--rw-r--r--   0 berry     (1000) berry     (1000)     1577 2024-02-13 08:28:08.221258 ckanext-wysiwyg-0.1.0/setup.cfg
--rw-r--r--   0 berry     (1000) berry     (1000)      528 2024-01-27 07:18:11.000000 ckanext-wysiwyg-0.1.0/setup.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/
+-rw-r--r--   0 berry     (1000) berry     (1000)    34500 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/LICENSE
+-rw-r--r--   0 berry     (1000) berry     (1000)      227 2024-04-29 10:35:55.000000 ckanext_wysiwyg-0.1.2/MANIFEST.in
+-rw-r--r--   0 berry     (1000) berry     (1000)     3886 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     3283 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/README.md
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/
+-rw-r--r--   0 berry     (1000) berry     (1000)      219 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/__init__.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/__init__.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/
+-rw-r--r--   0 berry     (1000) berry     (1000)      199 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/ckeditor5-custom-styles.css
+-rw-r--r--   0 berry     (1000) berry     (1000)      103 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/summernote-custom-styles.css
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/vendor/
+-rw-r--r--   0 berry     (1000) berry     (1000)    10098 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/vendor/ckeditor5.min.css
+-rw-r--r--   0 berry     (1000) berry     (1000)    26620 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/vendor/quill.min.css
+-rw-r--r--   0 berry     (1000) berry     (1000)    30478 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/vendor/summernote.min.css
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/js/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/js/vendor/
+-rw-r--r--   0 berry     (1000) berry     (1000)  1553083 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/js/vendor/ckeditor5.min.js
+-rw-r--r--   0 berry     (1000) berry     (1000)   163150 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/js/vendor/summernote.min.js
+-rw-r--r--   0 berry     (1000) berry     (1000)     2007 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/js/wysiwyg-ckeditor5-init.js
+-rw-r--r--   0 berry     (1000) berry     (1000)     2208 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/js/wysiwyg-summernote-init.js
+-rw-r--r--   0 berry     (1000) berry     (1000)      853 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/webassets.yml
+-rw-r--r--   0 berry     (1000) berry     (1000)      138 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/helpers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      138 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/logic/validators.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      469 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/plugin.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/public/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/public/font/
+-rw-r--r--   0 berry     (1000) berry     (1000)    11896 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/public/font/summernote.ttf
+-rw-r--r--   0 berry     (1000) berry     (1000)     7428 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/public/font/summernote.woff
+-rw-r--r--   0 berry     (1000) berry     (1000)     6156 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/public/font/summernote.woff2
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/
+-rw-r--r--   0 berry     (1000) berry     (1000)      462 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/page.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/scheming/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/scheming/display_snippets/
+-rw-r--r--   0 berry     (1000) berry     (1000)       97 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/scheming/display_snippets/wysiwyg_ckeditor5.html
+-rw-r--r--   0 berry     (1000) berry     (1000)      118 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/scheming/display_snippets/wysiwyg_summernote.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/scheming/form_snippets/
+-rw-r--r--   0 berry     (1000) berry     (1000)      560 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/scheming/form_snippets/wysiwyg_ckeditor5.html
+-rw-r--r--   0 berry     (1000) berry     (1000)      561 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/templates/scheming/form_snippets/wysiwyg_summernote.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/tests/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/tests/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1378 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/tests/test_plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      715 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/utils.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      979 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/
+-rw-r--r--   0 berry     (1000) berry     (1000)     3886 2024-04-29 10:37:10.000000 ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     1574 2024-04-29 10:37:10.000000 ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/SOURCES.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        1 2024-04-29 10:37:10.000000 ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/dependency_links.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)      119 2024-04-29 10:37:10.000000 ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/entry_points.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-29 10:37:10.000000 ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/namespace_packages.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-29 10:37:10.000000 ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/top_level.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/requirements.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     1577 2024-04-29 10:37:10.123309 ckanext_wysiwyg-0.1.2/setup.cfg
+-rw-r--r--   0 berry     (1000) berry     (1000)      528 2024-04-22 08:47:43.000000 ckanext_wysiwyg-0.1.2/setup.py
```

### Comparing `ckanext-wysiwyg-0.1.0/LICENSE` & `ckanext_wysiwyg-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/PKG-INFO` & `ckanext_wysiwyg-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-wysiwyg
-Version: 0.1.0
+Version: 0.1.2
 Summary: Add a support of wysiwyg editors for CKAN
 Home-page: https://github.com//ckanext-wysiwyg
 Author: Oleksandr Cherniavskiy
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-wysiwyg-0.1.0/README.md` & `ckanext_wysiwyg-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/vendor/ckeditor5.min.css` & `ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/vendor/ckeditor5.min.css`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/vendor/quill.min.css` & `ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/vendor/quill.min.css`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/css/vendor/summernote.min.css` & `ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/css/vendor/summernote.min.css`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/vendor/ckeditor5.min.js` & `ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/js/vendor/ckeditor5.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/js/vendor/summernote.min.js` & `ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/js/vendor/summernote.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/assets/webassets.yml` & `ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/assets/webassets.yml`

 * *Files 25% similar despite different names*

```diff
@@ -13,33 +13,14 @@
 wysiwyg-ckeditor5-css:
   filter: cssrewrite
   output: ckanext-wysiwyg/%(version)s-wysiwyg-ckeditor5.css
   contents:
     - css/vendor/ckeditor5.min.css
     - css/ckeditor5-custom-styles.css
 
-# QUILL
-
-wysiwyg-quill-js:
-  filter: rjsmin
-  output: ckanext-wysiwyg/%(version)s-wysiwyg-quill-js
-  contents:
-    - js/vendor/quill.min.js
-    - js/wysiwyg-quill-init.js
-  extra:
-    preload:
-      - base/main
-
-wysiwyg-quill-css:
-  filter: cssrewrite
-  output: ckanext-wysiwyg/%(version)s-wysiwyg-quill.css
-  contents:
-    - css/vendor/quill.min.css
-    - css/quill-custom-styles.css
-
 # SUMMETNOTE
 
 wysiwyg-summernote-js:
   filter: rjsmin
   output: ckanext-wysiwyg/%(version)s-wysiwyg-summernote-js
   contents:
     - js/vendor/summernote.min.js
```

### Comparing `ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/tests/test_plugin.py` & `ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/ckanext/wysiwyg/views.py` & `ckanext_wysiwyg-0.1.2/ckanext/wysiwyg/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/PKG-INFO` & `ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-wysiwyg
-Version: 0.1.0
+Version: 0.1.2
 Summary: Add a support of wysiwyg editors for CKAN
 Home-page: https://github.com//ckanext-wysiwyg
 Author: Oleksandr Cherniavskiy
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-wysiwyg-0.1.0/ckanext_wysiwyg.egg-info/SOURCES.txt` & `ckanext_wysiwyg-0.1.2/ckanext_wysiwyg.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,34 +8,31 @@
 ckanext/wysiwyg/__init__.py
 ckanext/wysiwyg/helpers.py
 ckanext/wysiwyg/plugin.py
 ckanext/wysiwyg/utils.py
 ckanext/wysiwyg/views.py
 ckanext/wysiwyg/assets/webassets.yml
 ckanext/wysiwyg/assets/css/ckeditor5-custom-styles.css
-ckanext/wysiwyg/assets/css/quill-custom-styles.css
 ckanext/wysiwyg/assets/css/summernote-custom-styles.css
 ckanext/wysiwyg/assets/css/vendor/ckeditor5.min.css
 ckanext/wysiwyg/assets/css/vendor/quill.min.css
 ckanext/wysiwyg/assets/css/vendor/summernote.min.css
 ckanext/wysiwyg/assets/js/wysiwyg-ckeditor5-init.js
-ckanext/wysiwyg/assets/js/wysiwyg-quill-init.js
 ckanext/wysiwyg/assets/js/wysiwyg-summernote-init.js
 ckanext/wysiwyg/assets/js/vendor/ckeditor5.min.js
-ckanext/wysiwyg/assets/js/vendor/quill.min.js
 ckanext/wysiwyg/assets/js/vendor/summernote.min.js
 ckanext/wysiwyg/logic/__init__.py
-ckanext/wysiwyg/logic/action.py
-ckanext/wysiwyg/logic/auth.py
 ckanext/wysiwyg/logic/validators.py
+ckanext/wysiwyg/public/font/summernote.ttf
+ckanext/wysiwyg/public/font/summernote.woff
+ckanext/wysiwyg/public/font/summernote.woff2
+ckanext/wysiwyg/templates/page.html
 ckanext/wysiwyg/templates/scheming/display_snippets/wysiwyg_ckeditor5.html
-ckanext/wysiwyg/templates/scheming/display_snippets/wysiwyg_quill.html
 ckanext/wysiwyg/templates/scheming/display_snippets/wysiwyg_summernote.html
 ckanext/wysiwyg/templates/scheming/form_snippets/wysiwyg_ckeditor5.html
-ckanext/wysiwyg/templates/scheming/form_snippets/wysiwyg_quill.html
 ckanext/wysiwyg/templates/scheming/form_snippets/wysiwyg_summernote.html
 ckanext/wysiwyg/tests/__init__.py
 ckanext/wysiwyg/tests/test_plugin.py
 ckanext_wysiwyg.egg-info/PKG-INFO
 ckanext_wysiwyg.egg-info/SOURCES.txt
 ckanext_wysiwyg.egg-info/dependency_links.txt
 ckanext_wysiwyg.egg-info/entry_points.txt
```

### Comparing `ckanext-wysiwyg-0.1.0/setup.cfg` & `ckanext_wysiwyg-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-wysiwyg
-version = 0.1.0
+version = 0.1.2
 description = Add a support of wysiwyg editors for CKAN
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com//ckanext-wysiwyg
 author = Oleksandr Cherniavskiy
 author_email = mutantsan@gmail.com
 license = AGPL
```

### Comparing `ckanext-wysiwyg-0.1.0/setup.py` & `ckanext_wysiwyg-0.1.2/setup.py`

 * *Files identical despite different names*

