# Comparing `tmp/mizdb_watchlist-0.1.8.tar.gz` & `tmp/mizdb_watchlist-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizdb_watchlist-0.1.8.tar", max compression
+gzip compressed data, was "mizdb_watchlist-1.0.0.tar", max compression
```

## Comparing `mizdb_watchlist-0.1.8.tar` & `mizdb_watchlist-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1064 2024-04-10 07:12:07.170823 mizdb_watchlist-0.1.8/LICENSE
--rw-r--r--   0        0        0    12422 2024-04-10 07:12:07.170823 mizdb_watchlist-0.1.8/README.md
--rw-r--r--   0        0        0     1807 2024-04-10 10:51:33.181394 mizdb_watchlist-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-08 11:26:36.034385 mizdb_watchlist-0.1.8/src/mizdb_watchlist/__init__.py
--rw-r--r--   0        0        0      673 2024-04-10 07:12:07.172823 mizdb_watchlist-0.1.8/src/mizdb_watchlist/actions.py
--rw-r--r--   0        0        0     1882 2024-04-10 07:12:07.172823 mizdb_watchlist-0.1.8/src/mizdb_watchlist/admin.py
--rw-r--r--   0        0        0      135 2024-03-13 09:45:12.311706 mizdb_watchlist-0.1.8/src/mizdb_watchlist/apps.py
--rw-r--r--   0        0        0     1445 2024-04-10 07:12:07.172823 mizdb_watchlist-0.1.8/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2491 2024-04-10 07:12:07.172823 mizdb_watchlist-0.1.8/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11133 2024-03-21 11:53:37.021286 mizdb_watchlist-0.1.8/src/mizdb_watchlist/manager.py
--rw-r--r--   0        0        0     1426 2024-04-10 07:12:07.172823 mizdb_watchlist-0.1.8/src/mizdb_watchlist/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-08 13:08:01.107636 mizdb_watchlist-0.1.8/src/mizdb_watchlist/migrations/__init__.py
--rw-r--r--   0        0        0      884 2024-03-21 11:53:37.021286 mizdb_watchlist-0.1.8/src/mizdb_watchlist/models.py
--rw-r--r--   0        0        0     1473 2024-04-10 09:44:48.305711 mizdb_watchlist-0.1.8/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist.css
--rw-r--r--   0        0        0     3024 2024-04-10 07:12:07.172823 mizdb_watchlist-0.1.8/src/mizdb_watchlist/static/mizdb_watchlist/js/watchlist.js
--rw-r--r--   0        0        0      365 2024-04-10 07:12:07.172823 mizdb_watchlist-0.1.8/src/mizdb_watchlist/templates/admin/watchlist.html
--rw-r--r--   0        0        0      486 2024-04-10 10:41:21.947288 mizdb_watchlist-0.1.8/src/mizdb_watchlist/templates/mizdb_watchlist/toggle_button.html
--rw-r--r--   0        0        0     2543 2024-04-10 09:40:52.774442 mizdb_watchlist-0.1.8/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist.html
--rw-r--r--   0        0        0      288 2024-03-08 13:08:01.200638 mizdb_watchlist-0.1.8/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_icon.svg
--rw-r--r--   0        0        0      549 2024-04-10 10:45:29.864808 mizdb_watchlist-0.1.8/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_link.html
--rw-r--r--   0        0        0        0 2024-03-08 13:08:01.201638 mizdb_watchlist-0.1.8/src/mizdb_watchlist/templatetags/__init__.py
--rw-r--r--   0        0        0     2935 2024-04-10 10:46:27.031839 mizdb_watchlist-0.1.8/src/mizdb_watchlist/templatetags/mizdb_watchlist.py
--rw-r--r--   0        0        0      337 2024-03-20 09:40:52.082653 mizdb_watchlist-0.1.8/src/mizdb_watchlist/urls.py
--rw-r--r--   0        0        0     6395 2024-04-10 07:12:07.172823 mizdb_watchlist-0.1.8/src/mizdb_watchlist/views.py
--rw-r--r--   0        0        0    13150 1970-01-01 00:00:00.000000 mizdb_watchlist-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-03 06:48:04.367968 mizdb_watchlist-1.0.0/LICENSE
+-rw-r--r--   0        0        0    14381 2024-04-29 11:08:22.188172 mizdb_watchlist-1.0.0/README.md
+-rw-r--r--   0        0        0     1807 2024-04-29 11:09:09.512422 mizdb_watchlist-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-11 07:55:02.082282 mizdb_watchlist-1.0.0/src/mizdb_watchlist/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-03 06:48:04.370968 mizdb_watchlist-1.0.0/src/mizdb_watchlist/actions.py
+-rw-r--r--   0        0        0     1882 2024-04-23 12:41:11.658027 mizdb_watchlist-1.0.0/src/mizdb_watchlist/admin.py
+-rw-r--r--   0        0        0      135 2024-03-12 07:47:13.602157 mizdb_watchlist-1.0.0/src/mizdb_watchlist/apps.py
+-rw-r--r--   0        0        0     1445 2024-04-23 12:41:11.659027 mizdb_watchlist-1.0.0/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2491 2024-04-03 06:48:04.370968 mizdb_watchlist-1.0.0/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11133 2024-04-03 06:48:04.371968 mizdb_watchlist-1.0.0/src/mizdb_watchlist/manager.py
+-rw-r--r--   0        0        0     1426 2024-04-23 12:41:11.659027 mizdb_watchlist-1.0.0/src/mizdb_watchlist/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-03-11 07:55:02.082282 mizdb_watchlist-1.0.0/src/mizdb_watchlist/migrations/__init__.py
+-rw-r--r--   0        0        0      884 2024-04-03 06:48:04.371968 mizdb_watchlist-1.0.0/src/mizdb_watchlist/models.py
+-rw-r--r--   0        0        0     1404 2024-04-29 11:08:22.192172 mizdb_watchlist-1.0.0/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist.css
+-rw-r--r--   0        0        0      123 2024-04-29 11:08:22.192172 mizdb_watchlist-1.0.0/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist_toggle.css
+-rw-r--r--   0        0        0     5815 2024-04-29 11:08:22.193172 mizdb_watchlist-1.0.0/src/mizdb_watchlist/static/mizdb_watchlist/js/watchlist.js
+-rw-r--r--   0        0        0      497 2024-04-29 11:08:22.193172 mizdb_watchlist-1.0.0/src/mizdb_watchlist/static/mizdb_watchlist/js/watchlist_init.js
+-rw-r--r--   0        0        0      365 2024-04-23 12:41:11.659027 mizdb_watchlist-1.0.0/src/mizdb_watchlist/templates/admin/watchlist.html
+-rw-r--r--   0        0        0      431 2024-04-29 11:08:22.193172 mizdb_watchlist-1.0.0/src/mizdb_watchlist/templates/mizdb_watchlist/toggle_button.html
+-rw-r--r--   0        0        0     2543 2024-04-23 12:41:11.660027 mizdb_watchlist-1.0.0/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist.html
+-rw-r--r--   0        0        0      288 2024-03-11 09:33:17.648399 mizdb_watchlist-1.0.0/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_icon.svg
+-rw-r--r--   0        0        0      549 2024-04-23 12:41:11.660027 mizdb_watchlist-1.0.0/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_link.html
+-rw-r--r--   0        0        0        0 2024-03-11 07:55:02.083282 mizdb_watchlist-1.0.0/src/mizdb_watchlist/templatetags/__init__.py
+-rw-r--r--   0        0        0     3047 2024-04-29 11:08:22.194172 mizdb_watchlist-1.0.0/src/mizdb_watchlist/templatetags/mizdb_watchlist.py
+-rw-r--r--   0        0        0      337 2024-03-19 12:28:14.463165 mizdb_watchlist-1.0.0/src/mizdb_watchlist/urls.py
+-rw-r--r--   0        0        0     6385 2024-04-29 11:08:22.194172 mizdb_watchlist-1.0.0/src/mizdb_watchlist/views.py
+-rw-r--r--   0        0        0    15109 1970-01-01 00:00:00.000000 mizdb_watchlist-1.0.0/PKG-INFO
```

### Comparing `mizdb_watchlist-0.1.8/LICENSE` & `mizdb_watchlist-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/README.md` & `mizdb_watchlist-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 action for adding multiple items, and a default template for rendering the
 overview of what's on the watchlist.
 
 The watchlist items are stored in a Watchlist model for authenticated users.
 For unauthenticated users, the watchlist is stored in a Django session instead.
 
 The styling was written with [Bootstrap](https://getbootstrap.com/) in mind.
-Alternatively, some rudimentary styling is provided with `mizdb_watchlist/css/watchlist.css`.
-You can use this for the admin site or if you don't want to use Bootstrap.
+Alternatively, some rudimentary styling is provided with `mizdb_watchlist/css/watchlist.css`
+and `mizdb_watchlist/css/watchlist_toggle.css`.
+You can use these for the admin site or if you don't want to use Bootstrap.
 
 [comment]: <> (@formatter:off)
 <!-- TOC -->
 * [mizdb-watchlist](#mizdb-watchlist)
   * [Installation](#installation)
   * [Manipulating the watchlist](#manipulating-the-watchlist)
     * [Toggle button](#toggle-button)
@@ -23,14 +24,15 @@
     * [views.WatchlistMixin](#viewswatchlistmixin)
   * [Displaying the watchlist](#displaying-the-watchlist)
     * [Link to the watchlist](#link-to-the-watchlist)
   * [Admin integration](#admin-integration)
     * [Admin toggle button & watchlist link](#admin-toggle-button--watchlist-link)
     * [admin.WatchlistMixin](#adminwatchlistmixin)
     * [Admin action](#admin-action)
+  * [Initializing buttons](#initializing-buttons)
   * [Demo & Development](#demo--development)
     * [Tests](#tests)
     * [Linting & Formatting](#linting--formatting)
     * [Demo](#demo)
 <!-- TOC -->
 [comment]: <> (@formatter:on)
 
@@ -81,18 +83,25 @@
 Use the `toggle_button` template tag to a button to your page:
 
 [comment]: <> (@formatter:off)
 ```html
 {% load static mizdb_watchlist %}
 {% block extrahead %}
   <script src="{% static 'mizdb_watchlist/js/watchlist.js' %}"></script>
+
+  {# watchlist_init.js will initialize any watchlist buttons on the page #}
+  <script src="{% static 'mizdb_watchlist/js/watchlist_init.js' %}"></script>
+
+  {# Optional stylesheet, to make the button change color when toggled: #}
+  <link rel="stylesheet" href="{% static 'mizdb_watchlist/css/watchlist_toggle.css' %}">
+
 {% endblock extrahead %}
 
 {% block content %}
-  <h5>{{ object }} {% toggle_button view.request object %}</h5>
+  <h5>{{ object }} {% toggle_button view.request object classes='foo bar' %}</h5>
   ...
 {% endblock content %}
 ```
 [comment]: <> (@formatter:on)
 
 > ℹ️ **Note**:
 >
@@ -104,14 +113,15 @@
 | Argument     | Default value | Description                                                                               |
 |--------------|---------------|-------------------------------------------------------------------------------------------|
 | request      | **required**  | the view's request                                                                        |
 | obj          | **required**  | the model object to add or remove                                                         |
 | text         | `""`          | optional text for the button                                                              |
 | url          | `None`        | the URL for the view that handles the toggling. Defaults to `reverse("watchlist:toggle")` |
 | on_watchlist | `None`        | an optional boolean that indicates whether the item is on the watchlist                   |
+| classes      | `""`          | additional CSS classes for the button                                                     |
 
 ### ListViews and the `on_watchlist` QuerySet annotation
 
 Note that if a value for the `on_watchlist` argument is not provided to the toggle
 button tag (i.e. the value is `None`), the tag will make a query to check if the
 item is on the watchlist. This is acceptable if you are only rendering one toggle
 button per page. But if you are rendering multiple toggle buttons per page, for
@@ -190,14 +200,15 @@
 ```html
 <!-- template for MyWatchlistView -->
 {% extends "base.html" %}
 {% load static %}
 
 {% block extrahead %}
   <script src="{% static 'mizdb_watchlist/js/watchlist.js' %}"></script>
+  <script src="{% static 'mizdb_watchlist/js/watchlist_init.js' %}"></script>
 {% endblock %}
 
 {% block content %}
   {% include "mizdb_watchlist/watchlist.html" %}
 {% endblock content %}
 ```
 [comment]: <> (@formatter:on)
@@ -283,14 +294,15 @@
 {% extends "admin/change_form.html" %}
 {% load static mizdb_watchlist %}
 
 {% block extrahead %}
   {{ block.super }}
   <link rel="stylesheet" href="{% static 'mizdb_watchlist/css/watchlist.css' %}">
   <script src="{% static 'mizdb_watchlist/js/watchlist.js' %}"></script>
+  <script src="{% static 'mizdb_watchlist/js/watchlist_init.js' %}"></script>
 {% endblock extrahead %}
 
 {% block content_subtitle %}
   {% if subtitle %}
     <h2>{{ subtitle }} {% toggle_button request original %}</h2>
   {% endif %}
 {% endblock %}
@@ -352,14 +364,52 @@
     actions = [add_to_watchlist, ...]
 
 
 # or for the entire admin site:
 my_admin_site.add_action(add_to_watchlist)
 ```
 
+## Initializing watchlist buttons
+
+In the above examples, `watchlist_init.js` was used to initialize any button
+that interacts with the watchlist.
+However, you can initialize the buttons yourself by using the `initToggleButton`,
+`initRemoveButton` and `initRemoveAllButton` functions provided by the global
+attribute `WatchlistButton`.
+
+For example like this:
+
+```javascript
+document.addEventListener('DOMContentLoaded', () => {
+  const myToggleButton = document.querySelector('.my-toggle-button')
+  WatchlistButton.initToggleButton(myToggleButton)
+})
+```
+
+This also lets you provide a callback function that is called after the button
+was pressed and the response from the server was handled.  
+The callback will be called with the button that was pressed and the response
+data.
+
+```javascript
+document.addEventListener('DOMContentLoaded', () => {
+  const myToggleButton = document.querySelector('.my-toggle-button')
+  const myCallback = (btn, data) => {
+    if (data.on_watchlist) {
+      btn.classList.remove('btn-primary')
+      btn.classList.add('btn-success')
+    } else {
+      btn.classList.add('btn-primary')
+      btn.classList.remove('btn-success')
+    }
+  }
+  WatchlistButton.initToggleButton(myToggleButton, myCallback)
+})
+```
+
 ## Demo & Development
 
 Install (requires [poetry](https://python-poetry.org/docs/) and npm):
 
 ```commandline
 make init
 ```
```

### Comparing `mizdb_watchlist-0.1.8/pyproject.toml` & `mizdb_watchlist-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mizdb-watchlist"
-version = "0.1.8"
+version = "1.0.0"
 description = "A watchlist for Django model objects."
 authors = [
   "Philip Becker <yummytea1@gmail.com>" ,
 ]
 readme = "README.md"
 packages = [{include = "mizdb_watchlist", from = "src"}]
 classifiers = [
```

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/actions.py` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/actions.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/admin.py` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/admin.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.mo` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.po` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/manager.py` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/manager.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/migrations/0001_initial.py` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/models.py` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/models.py`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist.css` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/static/mizdb_watchlist/css/watchlist.css`

 * *Files 11% similar despite different names*

```diff
@@ -31,18 +31,14 @@
 }
 
 .watchlist-remove-btn {
     border-color: red;
     color: red;
 }
 
-.watchlist-toggle-btn.on-watchlist {
-    color: rgb(24, 188, 156);
-}
-
 .d-flex {
     display: flex;
 }
 
 .justify-content-between {
     justify-content: space-between;
 }
@@ -97,8 +93,8 @@
 
 .model-watchlist-container > div {
     padding-bottom: 10px;
 }
 
 .watchlist-remove-all-btn {
     padding: 0.75rem 0.75rem;
-}
+}
```

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist.html` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist.html`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_link.html` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/templates/mizdb_watchlist/watchlist_link.html`

 * *Files identical despite different names*

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/templatetags/mizdb_watchlist.py` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/templatetags/mizdb_watchlist.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 @register.inclusion_tag("mizdb_watchlist/toggle_button.html")
 def toggle_button(
     request: HttpRequest,
     obj: Model,
     text: str = "",
     url: Optional[str] = None,
     on_watchlist: Optional[bool] = None,
+    classes: str = "",
 ) -> dict:
     """
     Render a watchlist toggle button for the given model object.
 
     This inclusion tag renders the template for the toggle button.
     The button is used to add or remove the given model object from the user's
     watchlist, depending on whether it is already on the watchlist.
@@ -46,14 +47,15 @@
         text (str): the text displayed next to the watchlist/bookmark icon
         url (str): the URL for the view that handles the toggling. If None, the
             URL with the name `watchlist:toggle` will be used.
         on_watchlist (bool): indicates whether the model object is already on
             the user's watchlist. If None, the tag will check the watchlist
             storage. This will generate a database query if the watchlist uses
             the Watchlist model!
+        classes (str): additional CSS classes for the button
 
     Example:
         In the template for a generic ListView:
 
         {% for object in object_list %}
             {{ object }}{% toggle_button view.request object text='foobar' %}
         {% endfor %}
@@ -82,8 +84,9 @@
         on_watchlist = get_manager(request).on_watchlist(obj)
     return {
         "object_id": obj.pk,
         "model_label": obj._meta.label_lower,
         "text": text,
         "toggle_url": url,
         "on_watchlist": on_watchlist,
+        "classes": classes,
     }
```

### Comparing `mizdb_watchlist-0.1.8/src/mizdb_watchlist/views.py` & `mizdb_watchlist-1.0.0/src/mizdb_watchlist/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import OrderedDict
 
 from django.apps import apps
 from django.core.exceptions import ObjectDoesNotExist
-from django.http import HttpResponse, HttpResponseBadRequest, JsonResponse
+from django.http import HttpResponseBadRequest, JsonResponse
 from django.urls import NoReverseMatch, reverse
 from django.views.decorators.csrf import csrf_protect
 from django.views.generic.base import ContextMixin
 
 from mizdb_watchlist.manager import ANNOTATION_FIELD, get_manager
 
 ON_WATCHLIST_VAR = ANNOTATION_FIELD
@@ -158,19 +158,19 @@
     except (KeyError, ValueError):
         return HttpResponseBadRequest()
     try:
         manager = get_manager(request)
         manager.remove(_get_model_object(model_label, pk))
     except (LookupError, ObjectDoesNotExist):
         pass
-    return HttpResponse()
+    return JsonResponse({})
 
 
 @csrf_protect
 def watchlist_remove_all(request):
     """Remove all objects of a given model from the watchlist."""
     try:
         model = apps.get_model(request.POST["model_label"])
     except (KeyError, LookupError):
         return HttpResponseBadRequest()
     get_manager(request).remove_model(model)
-    return HttpResponse()
+    return JsonResponse({})
```

### Comparing `mizdb_watchlist-0.1.8/PKG-INFO` & `mizdb_watchlist-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizdb-watchlist
-Version: 0.1.8
+Version: 1.0.0
 Summary: A watchlist for Django model objects.
 Home-page: https://github.com/Actionb/mizdb-watchlist
 License: MIT
 Author: Philip Becker
 Author-email: yummytea1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Django
@@ -26,16 +26,17 @@
 action for adding multiple items, and a default template for rendering the
 overview of what's on the watchlist.
 
 The watchlist items are stored in a Watchlist model for authenticated users.
 For unauthenticated users, the watchlist is stored in a Django session instead.
 
 The styling was written with [Bootstrap](https://getbootstrap.com/) in mind.
-Alternatively, some rudimentary styling is provided with `mizdb_watchlist/css/watchlist.css`.
-You can use this for the admin site or if you don't want to use Bootstrap.
+Alternatively, some rudimentary styling is provided with `mizdb_watchlist/css/watchlist.css`
+and `mizdb_watchlist/css/watchlist_toggle.css`.
+You can use these for the admin site or if you don't want to use Bootstrap.
 
 [comment]: <> (@formatter:off)
 <!-- TOC -->
 * [mizdb-watchlist](#mizdb-watchlist)
   * [Installation](#installation)
   * [Manipulating the watchlist](#manipulating-the-watchlist)
     * [Toggle button](#toggle-button)
@@ -43,14 +44,15 @@
     * [views.WatchlistMixin](#viewswatchlistmixin)
   * [Displaying the watchlist](#displaying-the-watchlist)
     * [Link to the watchlist](#link-to-the-watchlist)
   * [Admin integration](#admin-integration)
     * [Admin toggle button & watchlist link](#admin-toggle-button--watchlist-link)
     * [admin.WatchlistMixin](#adminwatchlistmixin)
     * [Admin action](#admin-action)
+  * [Initializing buttons](#initializing-buttons)
   * [Demo & Development](#demo--development)
     * [Tests](#tests)
     * [Linting & Formatting](#linting--formatting)
     * [Demo](#demo)
 <!-- TOC -->
 [comment]: <> (@formatter:on)
 
@@ -101,18 +103,25 @@
 Use the `toggle_button` template tag to a button to your page:
 
 [comment]: <> (@formatter:off)
 ```html
 {% load static mizdb_watchlist %}
 {% block extrahead %}
   <script src="{% static 'mizdb_watchlist/js/watchlist.js' %}"></script>
+
+  {# watchlist_init.js will initialize any watchlist buttons on the page #}
+  <script src="{% static 'mizdb_watchlist/js/watchlist_init.js' %}"></script>
+
+  {# Optional stylesheet, to make the button change color when toggled: #}
+  <link rel="stylesheet" href="{% static 'mizdb_watchlist/css/watchlist_toggle.css' %}">
+
 {% endblock extrahead %}
 
 {% block content %}
-  <h5>{{ object }} {% toggle_button view.request object %}</h5>
+  <h5>{{ object }} {% toggle_button view.request object classes='foo bar' %}</h5>
   ...
 {% endblock content %}
 ```
 [comment]: <> (@formatter:on)
 
 > ℹ️ **Note**:
 >
@@ -124,14 +133,15 @@
 | Argument     | Default value | Description                                                                               |
 |--------------|---------------|-------------------------------------------------------------------------------------------|
 | request      | **required**  | the view's request                                                                        |
 | obj          | **required**  | the model object to add or remove                                                         |
 | text         | `""`          | optional text for the button                                                              |
 | url          | `None`        | the URL for the view that handles the toggling. Defaults to `reverse("watchlist:toggle")` |
 | on_watchlist | `None`        | an optional boolean that indicates whether the item is on the watchlist                   |
+| classes      | `""`          | additional CSS classes for the button                                                     |
 
 ### ListViews and the `on_watchlist` QuerySet annotation
 
 Note that if a value for the `on_watchlist` argument is not provided to the toggle
 button tag (i.e. the value is `None`), the tag will make a query to check if the
 item is on the watchlist. This is acceptable if you are only rendering one toggle
 button per page. But if you are rendering multiple toggle buttons per page, for
@@ -210,14 +220,15 @@
 ```html
 <!-- template for MyWatchlistView -->
 {% extends "base.html" %}
 {% load static %}
 
 {% block extrahead %}
   <script src="{% static 'mizdb_watchlist/js/watchlist.js' %}"></script>
+  <script src="{% static 'mizdb_watchlist/js/watchlist_init.js' %}"></script>
 {% endblock %}
 
 {% block content %}
   {% include "mizdb_watchlist/watchlist.html" %}
 {% endblock content %}
 ```
 [comment]: <> (@formatter:on)
@@ -303,14 +314,15 @@
 {% extends "admin/change_form.html" %}
 {% load static mizdb_watchlist %}
 
 {% block extrahead %}
   {{ block.super }}
   <link rel="stylesheet" href="{% static 'mizdb_watchlist/css/watchlist.css' %}">
   <script src="{% static 'mizdb_watchlist/js/watchlist.js' %}"></script>
+  <script src="{% static 'mizdb_watchlist/js/watchlist_init.js' %}"></script>
 {% endblock extrahead %}
 
 {% block content_subtitle %}
   {% if subtitle %}
     <h2>{{ subtitle }} {% toggle_button request original %}</h2>
   {% endif %}
 {% endblock %}
@@ -372,14 +384,52 @@
     actions = [add_to_watchlist, ...]
 
 
 # or for the entire admin site:
 my_admin_site.add_action(add_to_watchlist)
 ```
 
+## Initializing watchlist buttons
+
+In the above examples, `watchlist_init.js` was used to initialize any button
+that interacts with the watchlist.
+However, you can initialize the buttons yourself by using the `initToggleButton`,
+`initRemoveButton` and `initRemoveAllButton` functions provided by the global
+attribute `WatchlistButton`.
+
+For example like this:
+
+```javascript
+document.addEventListener('DOMContentLoaded', () => {
+  const myToggleButton = document.querySelector('.my-toggle-button')
+  WatchlistButton.initToggleButton(myToggleButton)
+})
+```
+
+This also lets you provide a callback function that is called after the button
+was pressed and the response from the server was handled.  
+The callback will be called with the button that was pressed and the response
+data.
+
+```javascript
+document.addEventListener('DOMContentLoaded', () => {
+  const myToggleButton = document.querySelector('.my-toggle-button')
+  const myCallback = (btn, data) => {
+    if (data.on_watchlist) {
+      btn.classList.remove('btn-primary')
+      btn.classList.add('btn-success')
+    } else {
+      btn.classList.add('btn-primary')
+      btn.classList.remove('btn-success')
+    }
+  }
+  WatchlistButton.initToggleButton(myToggleButton, myCallback)
+})
+```
+
 ## Demo & Development
 
 Install (requires [poetry](https://python-poetry.org/docs/) and npm):
 
 ```commandline
 make init
 ```
```

