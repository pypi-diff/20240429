# Comparing `tmp/djrender-0.1b3.tar.gz` & `tmp/djrender-0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djrender-0.1b3.tar", last modified: Wed Apr 10 12:42:57 2024, max compression
+gzip compressed data, was "djrender-0.1b4.tar", last modified: Mon Apr 29 10:58:00 2024, max compression
```

## Comparing `djrender-0.1b3.tar` & `djrender-0.1b4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 12:42:57.966195 djrender-0.1b3/
--rw-rw-r--   0 karl      (1000) karl      (1000)      104 2024-04-09 12:29:00.000000 djrender-0.1b3/MANIFEST.in
--rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-10 12:42:57.966195 djrender-0.1b3/PKG-INFO
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 12:42:57.962195 djrender-0.1b3/django_render/
--rw-rw-r--   0 karl      (1000) karl      (1000)      468 2024-04-10 12:42:05.000000 djrender-0.1b3/django_render/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      345 2024-04-10 12:42:05.000000 djrender-0.1b3/django_render/apps.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3248 2024-04-10 12:42:05.000000 djrender-0.1b3/django_render/decorators.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3199 2024-04-10 12:42:05.000000 djrender-0.1b3/django_render/response.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1754 2024-04-09 12:29:00.000000 djrender-0.1b3/django_render/telepath.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 12:42:57.958195 djrender-0.1b3/django_render/templates/
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 12:42:57.962195 djrender-0.1b3/django_render/templates/django_render/
--rw-rw-r--   0 karl      (1000) karl      (1000)     3508 2024-04-10 12:42:05.000000 djrender-0.1b3/django_render/templates/django_render/bootstrap.html
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 12:42:57.966195 djrender-0.1b3/django_render/test/
--rw-rw-r--   0 karl      (1000) karl      (1000)       73 2024-04-09 12:29:00.000000 djrender-0.1b3/django_render/test/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      186 2024-04-09 12:29:00.000000 djrender-0.1b3/django_render/test/apps.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3653 2024-04-09 12:29:00.000000 djrender-0.1b3/django_render/test/settings.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 12:42:57.966195 djrender-0.1b3/django_render/test/tests/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b3/django_render/test/tests/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)      118 2024-04-09 12:29:00.000000 djrender-0.1b3/django_render/test/urls.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 12:42:57.966195 djrender-0.1b3/django_render/ui/
--rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b3/django_render/ui/__init__.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     3594 2024-04-09 12:29:00.000000 djrender-0.1b3/django_render/ui/forms.py
--rw-rw-r--   0 karl      (1000) karl      (1000)     1422 2024-04-10 12:42:05.000000 djrender-0.1b3/django_render/views.py
-drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-10 12:42:57.966195 djrender-0.1b3/djrender.egg-info/
--rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-10 12:42:57.000000 djrender-0.1b3/djrender.egg-info/PKG-INFO
--rw-rw-r--   0 karl      (1000) karl      (1000)      622 2024-04-10 12:42:57.000000 djrender-0.1b3/djrender.egg-info/SOURCES.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-10 12:42:57.000000 djrender-0.1b3/djrender.egg-info/dependency_links.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-09 12:36:52.000000 djrender-0.1b3/djrender.egg-info/not-zip-safe
--rw-rw-r--   0 karl      (1000) karl      (1000)       36 2024-04-10 12:42:57.000000 djrender-0.1b3/djrender.egg-info/requires.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-10 12:42:57.000000 djrender-0.1b3/djrender.egg-info/top_level.txt
--rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-04-10 12:42:57.966195 djrender-0.1b3/setup.cfg
--rw-rw-r--   0 karl      (1000) karl      (1000)     1510 2024-04-09 12:36:33.000000 djrender-0.1b3/setup.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 10:58:00.799706 djrender-0.1b4/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      104 2024-04-09 12:29:00.000000 djrender-0.1b4/MANIFEST.in
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-29 10:58:00.799706 djrender-0.1b4/PKG-INFO
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 10:58:00.795706 djrender-0.1b4/django_render/
+-rw-rw-r--   0 karl      (1000) karl      (1000)      468 2024-04-29 10:57:29.000000 djrender-0.1b4/django_render/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      345 2024-04-10 12:42:05.000000 djrender-0.1b4/django_render/apps.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      346 2024-04-29 10:57:29.000000 djrender-0.1b4/django_render/decorators.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3187 2024-04-29 10:57:29.000000 djrender-0.1b4/django_render/middleware.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3173 2024-04-29 10:57:29.000000 djrender-0.1b4/django_render/response.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1754 2024-04-09 12:29:00.000000 djrender-0.1b4/django_render/telepath.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 10:58:00.791706 djrender-0.1b4/django_render/templates/
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 10:58:00.795706 djrender-0.1b4/django_render/templates/django_render/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3508 2024-04-10 12:42:05.000000 djrender-0.1b4/django_render/templates/django_render/bootstrap.html
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 10:58:00.795706 djrender-0.1b4/django_render/test/
+-rw-rw-r--   0 karl      (1000) karl      (1000)       73 2024-04-09 12:29:00.000000 djrender-0.1b4/django_render/test/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      186 2024-04-09 12:29:00.000000 djrender-0.1b4/django_render/test/apps.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3653 2024-04-09 12:29:00.000000 djrender-0.1b4/django_render/test/settings.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 10:58:00.795706 djrender-0.1b4/django_render/test/tests/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b4/django_render/test/tests/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)      118 2024-04-09 12:29:00.000000 djrender-0.1b4/django_render/test/urls.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 10:58:00.799706 djrender-0.1b4/django_render/ui/
+-rw-rw-r--   0 karl      (1000) karl      (1000)        0 2024-04-09 12:29:00.000000 djrender-0.1b4/django_render/ui/__init__.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     3594 2024-04-09 12:29:00.000000 djrender-0.1b4/django_render/ui/forms.py
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1312 2024-04-29 10:57:29.000000 djrender-0.1b4/django_render/views.py
+drwxrwxr-x   0 karl      (1000) karl      (1000)        0 2024-04-29 10:58:00.799706 djrender-0.1b4/djrender.egg-info/
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1138 2024-04-29 10:58:00.000000 djrender-0.1b4/djrender.egg-info/PKG-INFO
+-rw-rw-r--   0 karl      (1000) karl      (1000)      650 2024-04-29 10:58:00.000000 djrender-0.1b4/djrender.egg-info/SOURCES.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-29 10:58:00.000000 djrender-0.1b4/djrender.egg-info/dependency_links.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)        1 2024-04-29 10:58:00.000000 djrender-0.1b4/djrender.egg-info/not-zip-safe
+-rw-rw-r--   0 karl      (1000) karl      (1000)       36 2024-04-29 10:58:00.000000 djrender-0.1b4/djrender.egg-info/requires.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       14 2024-04-29 10:58:00.000000 djrender-0.1b4/djrender.egg-info/top_level.txt
+-rw-rw-r--   0 karl      (1000) karl      (1000)       38 2024-04-29 10:58:00.799706 djrender-0.1b4/setup.cfg
+-rw-rw-r--   0 karl      (1000) karl      (1000)     1510 2024-04-29 10:57:25.000000 djrender-0.1b4/setup.py
```

### Comparing `djrender-0.1b3/PKG-INFO` & `djrender-0.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djrender
-Version: 0.1b3
+Version: 0.1b4
 Summary: A framework for building React frontends for Django projects
 Home-page: https://django-render.org
 Author: Karl Hobley
 Author-email: karl@kaed.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://django-render.org/docs/
 Project-URL: Source, https://github.com/kaedroho/django-render/
```

### Comparing `djrender-0.1b3/django_render/decorators.py` & `djrender-0.1b4/django_render/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import json
-from functools import wraps
 from pathlib import Path
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.shortcuts import render
 from django.templatetags.static import static
 
 from .response import BaseResponse, RedirectResponse, ReloadResponse
 
 
-def djangorender_view(fn):
-    """
-    Wraps a view to make it load with Django Render
-    """
-
-    @wraps(fn)
-    def wrapper(request, *args, **kwargs):
-        response = fn(request, *args, **kwargs)
+class DjangoRenderMiddleware:
+    def __init__(self, get_response):
+        self.get_response = get_response
+
+    def __call__(self, request):
+        response = self.get_response(request)
 
         if response.status_code == 301:
             return response
 
         # If the request was made by Django Render
         # (using `fetch()`, rather than a regular browser request)
         if request.META.get("HTTP_X_REQUESTED_WITH") == "DjangoRender":
@@ -82,9 +79,7 @@
             # Copy status_code and cookies from the original response
             new_response.status_code = response.status_code
             new_response.cookies = response.cookies
 
             return new_response
 
         return response
-
-    return wrapper
```

### Comparing `djrender-0.1b3/django_render/response.py` & `djrender-0.1b4/django_render/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 def get_messages(request):
     return [
         {
             "level": (
                 "error"
                 if message.level == messages.ERROR
-                else "warning" if message.level == messages.WARNING else "success"
+                else "warning"
+                if message.level == messages.WARNING
+                else "success"
             ),
             "html": conditional_escape(message.message),
         }
         for message in messages.get_messages(request)
     ]
 
 
@@ -104,11 +106,7 @@
         self.request = request
         super().__init__(*args, **kwargs)
 
     def get_data(self):
         return {
             "messages": get_messages(self.request),
         }
-
-
-class NotFoundResponse(Response):
-    status_code = 404
```

### Comparing `djrender-0.1b3/django_render/telepath.py` & `djrender-0.1b4/django_render/telepath.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b3/django_render/templates/django_render/bootstrap.html` & `djrender-0.1b4/django_render/templates/django_render/bootstrap.html`

 * *Files identical despite different names*

### Comparing `djrender-0.1b3/django_render/test/settings.py` & `djrender-0.1b4/django_render/test/settings.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b3/django_render/ui/forms.py` & `djrender-0.1b4/django_render/ui/forms.py`

 * *Files identical despite different names*

### Comparing `djrender-0.1b3/django_render/views.py` & `djrender-0.1b4/django_render/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.utils.decorators import method_decorator
 from django.views.generic.base import ContextMixin, View
 
 from .decorators import djangorender_view
-from .response import NotFoundResponse, Response
+from .response import Response
 
 
-class ResponseMixin:
+class DjangoRenderMixin:
     """A mixin that can be used to render a view with a React component."""
 
     title = None
     view_name = None
     overlay = False
     response_class = Response
 
@@ -28,24 +28,19 @@
             self.view_name,
             props,
             overlay=self.overlay,
             title=self.title,
         )
 
 
-class DjangoRenderView(ResponseMixin, ContextMixin, View):
+class DjangoRenderView(DjangoRenderMixin, ContextMixin, View):
     """
     A class-based view that can be used to render views with React.
     """
 
     @method_decorator(djangorender_view)
     def dispatch(self, request, *args, **kwargs):
         return super().dispatch(request, *args, **kwargs)
 
     def get(self, request, *args, **kwargs):
         context = self.get_context_data(**kwargs)
         return self.render_to_response(context)
-
-
-@djangorender_view
-def handler_404(request, exception=None):
-    return NotFoundResponse(request)
```

### Comparing `djrender-0.1b3/djrender.egg-info/PKG-INFO` & `djrender-0.1b4/djrender.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djrender
-Version: 0.1b3
+Version: 0.1b4
 Summary: A framework for building React frontends for Django projects
 Home-page: https://django-render.org
 Author: Karl Hobley
 Author-email: karl@kaed.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://django-render.org/docs/
 Project-URL: Source, https://github.com/kaedroho/django-render/
```

### Comparing `djrender-0.1b3/djrender.egg-info/SOURCES.txt` & `djrender-0.1b4/djrender.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 setup.py
 django_render/__init__.py
 django_render/apps.py
 django_render/decorators.py
+django_render/middleware.py
 django_render/response.py
 django_render/telepath.py
 django_render/views.py
 django_render/templates/django_render/bootstrap.html
 django_render/test/__init__.py
 django_render/test/apps.py
 django_render/test/settings.py
```

### Comparing `djrender-0.1b3/setup.py` & `djrender-0.1b4/setup.py`

 * *Files identical despite different names*

