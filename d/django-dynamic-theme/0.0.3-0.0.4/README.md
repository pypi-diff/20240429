# Comparing `tmp/django_dynamic_theme-0.0.3.tar.gz` & `tmp/django_dynamic_theme-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_theme-0.0.3.tar", max compression
+gzip compressed data, was "django_dynamic_theme-0.0.4.tar", max compression
```

## Comparing `django_dynamic_theme-0.0.3.tar` & `django_dynamic_theme-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1068 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/LICENSE
--rw-r--r--   0        0        0     1644 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/__init__.py
--rw-r--r--   0        0        0      713 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/admin.py
--rw-r--r--   0        0        0      498 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/apps.py
--rw-r--r--   0        0        0      475 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/context_processor.py
--rw-r--r--   0        0        0      516 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0001_initial.py
--rw-r--r--   0        0        0      436 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0002_background_name.py
--rw-r--r--   0        0        0      484 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0003_alter_background_primary_bg.py
--rw-r--r--   0        0        0     1241 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py
--rw-r--r--   0        0        0      733 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py
--rw-r--r--   0        0        0      526 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0006_alter_theme_background.py
--rw-r--r--   0        0        0      664 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py
--rw-r--r--   0        0        0      434 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0008_alter_theme_default.py
--rw-r--r--   0        0        0      976 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0009_navbar.py
--rw-r--r--   0        0        0      507 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0010_theme_navbar.py
--rw-r--r--   0        0        0      612 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0011_navbar_font_size.py
--rw-r--r--   0        0        0      479 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0012_navbar_text_color.py
--rw-r--r--   0        0        0      566 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0013_navbar_text_opacity.py
--rw-r--r--   0        0        0      604 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py
--rw-r--r--   0        0        0        0 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/__init__.py
--rw-r--r--   0        0        0     4942 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/models.py
--rw-r--r--   0        0        0      582 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/signals.py
--rw-r--r--   0        0        0        0 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/utill/__init__.py
--rw-r--r--   0        0        0      506 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/utill/color_converter.py
--rw-r--r--   0        0        0      740 2024-04-06 23:56:32.748440 django_dynamic_theme-0.0.3/django_dynamic_theme/utill/scss_editor.py
--rw-r--r--   0        0        0      743 2024-04-06 23:56:32.752440 django_dynamic_theme-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2270 1970-01-01 00:00:00.000000 django_dynamic_theme-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1644 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/__init__.py
+-rw-r--r--   0        0        0      713 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/admin.py
+-rw-r--r--   0        0        0      498 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/apps.py
+-rw-r--r--   0        0        0      475 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/context_processor.py
+-rw-r--r--   0        0        0      516 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0001_initial.py
+-rw-r--r--   0        0        0      436 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0002_background_name.py
+-rw-r--r--   0        0        0      484 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0003_alter_background_primary_bg.py
+-rw-r--r--   0        0        0     1241 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py
+-rw-r--r--   0        0        0      733 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py
+-rw-r--r--   0        0        0      526 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0006_alter_theme_background.py
+-rw-r--r--   0        0        0      664 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py
+-rw-r--r--   0        0        0      434 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0008_alter_theme_default.py
+-rw-r--r--   0        0        0      976 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0009_navbar.py
+-rw-r--r--   0        0        0      507 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0010_theme_navbar.py
+-rw-r--r--   0        0        0      612 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0011_navbar_font_size.py
+-rw-r--r--   0        0        0      479 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0012_navbar_text_color.py
+-rw-r--r--   0        0        0      566 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0013_navbar_text_opacity.py
+-rw-r--r--   0        0        0      604 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/__init__.py
+-rw-r--r--   0        0        0     4942 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/models.py
+-rw-r--r--   0        0        0      582 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/signals.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/utill/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/utill/color_converter.py
+-rw-r--r--   0        0        0      740 2024-04-29 21:41:53.056316 django_dynamic_theme-0.0.4/django_dynamic_theme/utill/scss_editor.py
+-rw-r--r--   0        0        0      743 2024-04-29 21:41:53.060316 django_dynamic_theme-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 django_dynamic_theme-0.0.4/PKG-INFO
```

### Comparing `django_dynamic_theme-0.0.3/LICENSE` & `django_dynamic_theme-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/README.md` & `django_dynamic_theme-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/admin.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/admin.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0001_initial.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0006_alter_theme_background.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0006_alter_theme_background.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0009_navbar.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0009_navbar.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0011_navbar_font_size.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0011_navbar_font_size.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0013_navbar_text_opacity.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0013_navbar_text_opacity.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/models.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/models.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/signals.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/signals.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/django_dynamic_theme/utill/scss_editor.py` & `django_dynamic_theme-0.0.4/django_dynamic_theme/utill/scss_editor.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.3/pyproject.toml` & `django_dynamic_theme-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "django-dynamic-theme"
-version = "0.0.3"
+version = "0.0.4"
 description = "This enables the administrator of a django website to change the theme on the fly."
 authors = ["Segelzwerg <25705862+Segelzwerg@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
 django = "^5.0"
 setuptools = "^69.2.0"
 django-colorfield = "^0.11.0"
 django-compressor = "^4.4"
 django-libsass = "^0.9"
```

### Comparing `django_dynamic_theme-0.0.3/PKG-INFO` & `django_dynamic_theme-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: django-dynamic-theme
-Version: 0.0.3
+Version: 0.0.4
 Summary: This enables the administrator of a django website to change the theme on the fly.
 Author: Segelzwerg
 Author-email: 25705862+Segelzwerg@users.noreply.github.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=5.0,<6.0)
 Requires-Dist: django-colorfield (>=0.11.0,<0.12.0)
 Requires-Dist: django-compressor (>=4.4,<5.0)
 Requires-Dist: django-libsass (>=0.9,<0.10)
 Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 2.1 Name: django-dynamic-theme Version: 0.0.3 Summary: This
+Metadata-Version: 2.1 Name: django-dynamic-theme Version: 0.0.4 Summary: This
 enables the administrator of a django website to change the theme on the fly.
 Author: Segelzwerg Author-email: 25705862+Segelzwerg@users.noreply.github.com
-Requires-Python: >=3.12,<4.0 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12 Requires-Dist: django
-(>=5.0,<6.0) Requires-Dist: django-colorfield (>=0.11.0,<0.12.0) Requires-Dist:
-django-compressor (>=4.4,<5.0) Requires-Dist: django-libsass (>=0.9,<0.10)
-Requires-Dist: setuptools (>=69.2.0,<70.0.0) Description-Content-Type: text/
-markdown ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
-django-dynamic-theme) [![](https://img.shields.io/pypi/djversions/django-
-dynamic-theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://
+Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: django (>=5.0,<6.0) Requires-Dist: django-colorfield
+(>=0.11.0,<0.12.0) Requires-Dist: django-compressor (>=4.4,<5.0) Requires-Dist:
+django-libsass (>=0.9,<0.10) Requires-Dist: setuptools (>=69.2.0,<70.0.0)
+Description-Content-Type: text/markdown ![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/django-dynamic-theme) [![](https://
+img.shields.io/pypi/djversions/django-dynamic-
+theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://
 www.djangoproject.com/) [![Documentation Status](https://readthedocs.org/
 projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-
 theme.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
 gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://
 codecov.io/gh/Segelzwerg/django-dynamic-theme) # Django Dynamic Theme This
 allows an administrator of a django website to change the theme on the fly. ##
 Installation ```sh pip install django-dynamic-theme ``` ## Quickstart 1. Add
```

