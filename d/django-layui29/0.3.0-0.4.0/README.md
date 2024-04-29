# Comparing `tmp/django_layui29-0.3.0.tar.gz` & `tmp/django_layui29-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_layui29-0.3.0.tar", max compression
+gzip compressed data, was "django_layui29-0.4.0.tar", max compression
```

## Comparing `django_layui29-0.3.0.tar` & `django_layui29-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1262 2024-04-14 05:19:29.566270 django_layui29-0.3.0/LICENSE
--rw-r--r--   0        0        0      942 2024-04-23 11:59:56.699567 django_layui29-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 05:19:29.568366 django_layui29-0.3.0/src/django_layui29/__init__.py
--rw-r--r--   0        0        0       63 2024-04-14 05:19:29.568505 django_layui29-0.3.0/src/django_layui29/admin.py
--rw-r--r--   0        0        0      157 2024-04-14 05:19:29.568618 django_layui29-0.3.0/src/django_layui29/apps.py
--rw-r--r--   0        0        0        0 2024-04-14 05:19:29.568732 django_layui29-0.3.0/src/django_layui29/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-04-14 05:19:29.568860 django_layui29-0.3.0/src/django_layui29/models.py
--rw-r--r--   0        0        0      618 2024-04-14 05:19:29.569205 django_layui29-0.3.0/src/django_layui29/static/layui29/css/center.css
--rw-r--r--   0        0        0      662 2024-04-14 05:19:29.569326 django_layui29-0.3.0/src/django_layui29/static/layui29/css/global.css
--rw-r--r--   0        0        0     1051 2024-04-16 09:27:19.862964 django_layui29-0.3.0/src/django_layui29/static/layui29/js/base.js
--rw-r--r--   0        0        0     1681 2024-04-16 09:25:36.599514 django_layui29-0.3.0/src/django_layui29/static/layui29/js/js.cookie.min.js
--rw-r--r--   0        0        0      688 2024-04-23 11:55:11.219106 django_layui29-0.3.0/src/django_layui29/templates/layui29/base.html
--rw-r--r--   0        0        0     2587 2024-04-23 11:57:40.311596 django_layui29-0.3.0/src/django_layui29/templates/layui29/component/base/header.html
--rw-r--r--   0        0        0     1772 2024-04-16 09:33:15.587946 django_layui29-0.3.0/src/django_layui29/templates/layui29/component/base/left_nav.html
--rw-r--r--   0        0        0     8696 2024-04-16 09:32:40.052522 django_layui29-0.3.0/src/django_layui29/templates/layui29/layout/admin.html
--rw-r--r--   0        0        0      464 2024-04-14 05:19:29.569815 django_layui29-0.3.0/src/django_layui29/templates/layui29/layout/center.html
--rw-r--r--   0        0        0      338 2024-04-23 11:54:35.415857 django_layui29-0.3.0/src/django_layui29/templates/layui29/layout/normal.html
--rw-r--r--   0        0        0       60 2024-04-14 05:19:29.569937 django_layui29-0.3.0/src/django_layui29/tests.py
--rw-r--r--   0        0        0       77 2024-04-16 09:22:21.866608 django_layui29-0.3.0/src/django_layui29/utils.py
--rw-r--r--   0        0        0       63 2024-04-14 05:19:29.570083 django_layui29-0.3.0/src/django_layui29/views.py
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 django_layui29-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1262 2024-04-14 05:19:29.566270 django_layui29-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1033 2024-04-29 06:11:20.721730 django_layui29-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-29 06:11:20.721870 django_layui29-0.4.0/src/django_layui29/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-14 05:19:29.568505 django_layui29-0.4.0/src/django_layui29/admin.py
+-rw-r--r--   0        0        0      157 2024-04-14 05:19:29.568618 django_layui29-0.4.0/src/django_layui29/apps.py
+-rw-r--r--   0        0        0       31 2024-04-29 03:56:54.725124 django_layui29-0.4.0/src/django_layui29/form.py
+-rw-r--r--   0        0        0        0 2024-04-14 05:19:29.568732 django_layui29-0.4.0/src/django_layui29/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-14 05:19:29.568860 django_layui29-0.4.0/src/django_layui29/models.py
+-rw-r--r--   0        0        0      618 2024-04-14 05:19:29.569205 django_layui29-0.4.0/src/django_layui29/static/layui29/css/center.css
+-rw-r--r--   0        0        0      662 2024-04-14 05:19:29.569326 django_layui29-0.4.0/src/django_layui29/static/layui29/css/global.css
+-rw-r--r--   0        0        0     1051 2024-04-16 09:27:19.862964 django_layui29-0.4.0/src/django_layui29/static/layui29/js/base.js
+-rw-r--r--   0        0        0     1681 2024-04-16 09:25:36.599514 django_layui29-0.4.0/src/django_layui29/static/layui29/js/js.cookie.min.js
+-rw-r--r--   0        0        0      688 2024-04-29 05:58:23.614933 django_layui29-0.4.0/src/django_layui29/templates/layui29/base.html
+-rw-r--r--   0        0        0     2657 2024-04-29 06:02:51.918161 django_layui29-0.4.0/src/django_layui29/templates/layui29/component/base/header.html
+-rw-r--r--   0        0        0     1772 2024-04-16 09:33:15.587946 django_layui29-0.4.0/src/django_layui29/templates/layui29/component/base/left_nav.html
+-rw-r--r--   0        0        0     4346 2024-04-29 05:31:14.679802 django_layui29-0.4.0/src/django_layui29/templates/layui29/component/tables.html
+-rw-r--r--   0        0        0     8696 2024-04-16 09:32:40.052522 django_layui29-0.4.0/src/django_layui29/templates/layui29/layout/admin.html
+-rw-r--r--   0        0        0      464 2024-04-14 05:19:29.569815 django_layui29-0.4.0/src/django_layui29/templates/layui29/layout/center.html
+-rw-r--r--   0        0        0      398 2024-04-29 06:01:45.808541 django_layui29-0.4.0/src/django_layui29/templates/layui29/layout/normal.html
+-rw-r--r--   0        0        0       60 2024-04-14 05:19:29.569937 django_layui29-0.4.0/src/django_layui29/tests.py
+-rw-r--r--   0        0        0       77 2024-04-16 09:22:21.866608 django_layui29-0.4.0/src/django_layui29/utils.py
+-rw-r--r--   0        0        0       63 2024-04-14 05:19:29.570083 django_layui29-0.4.0/src/django_layui29/views.py
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 django_layui29-0.4.0/PKG-INFO
```

### Comparing `django_layui29-0.3.0/LICENSE` & `django_layui29-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_layui29-0.3.0/pyproject.toml` & `django_layui29-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [tool.poetry]
 name = "django_layui29"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["svtter <svtter@163.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 django = "<6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-xdist = "^3.0.2"
 pytest-django = "^4.5.2"
 pre-commit = "^2.20.0"
 mkdocs = "^1.4.3"
 djlint = "^1.34.1"
+bumpversion = "^0.6.0"
+
+
+[tool.poetry.group.tables.dependencies]
+django-tables2 = "^2.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # -- FILE: pytest.ini (or tox.ini)
 [tool.pytest.ini_options]
```

### Comparing `django_layui29-0.3.0/src/django_layui29/static/layui29/css/center.css` & `django_layui29-0.4.0/src/django_layui29/static/layui29/css/center.css`

 * *Files identical despite different names*

### Comparing `django_layui29-0.3.0/src/django_layui29/static/layui29/css/global.css` & `django_layui29-0.4.0/src/django_layui29/static/layui29/css/global.css`

 * *Files identical despite different names*

### Comparing `django_layui29-0.3.0/src/django_layui29/static/layui29/js/base.js` & `django_layui29-0.4.0/src/django_layui29/static/layui29/js/base.js`

 * *Files identical despite different names*

### Comparing `django_layui29-0.3.0/src/django_layui29/static/layui29/js/js.cookie.min.js` & `django_layui29-0.4.0/src/django_layui29/static/layui29/js/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django_layui29-0.3.0/src/django_layui29/templates/layui29/base.html` & `django_layui29-0.4.0/src/django_layui29/templates/layui29/base.html`

 * *Files identical despite different names*

### Comparing `django_layui29-0.3.0/src/django_layui29/templates/layui29/component/base/header.html` & `django_layui29-0.4.0/src/django_layui29/templates/layui29/component/base/header.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-<div class="layui-header">
+{% comment %} TODO: admin panel color {% endcomment %}
+<div class="layui-header layui-bg-black">
     <div class="layui-logo layui-hide-xs layui-bg-black">
         <a class="system-title" href="#" >{{ system_name }}</a>
     </div>
     <!-- 头部区域（可配合layui 已有的水平导航） -->
     <ul class="layui-nav layui-layout-left">
         <!-- 移动端显示 -->
         <li class="layui-nav-item layui-show-xs-inline-block layui-hide-sm"
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+{% comment %} TODO: admin panel color {% endcomment %}
 _{_{_ _s_y_s_t_e_m___n_a_m_e_ _}_}
     * Hi
     * _å_¸_¸_è_§__å_¸__å_±_
     * _è_°__è_¯__é__¢_æ__¿
     * _ä_¸_­_å_¿__å_¸__å_±_
     * _ç_®_¡_ç___å_¸__å_±_
     * nav group
```

### Comparing `django_layui29-0.3.0/src/django_layui29/templates/layui29/component/base/left_nav.html` & `django_layui29-0.4.0/src/django_layui29/templates/layui29/component/base/left_nav.html`

 * *Files identical despite different names*

### Comparing `django_layui29-0.3.0/src/django_layui29/templates/layui29/layout/admin.html` & `django_layui29-0.4.0/src/django_layui29/templates/layui29/layout/admin.html`

 * *Files identical despite different names*

### Comparing `django_layui29-0.3.0/PKG-INFO` & `django_layui29-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_layui29
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: svtter
 Author-email: svtter@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

