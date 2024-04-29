# Comparing `tmp/django_user_sessions_ng-0.1.3.tar.gz` & `tmp/django_user_sessions_ng-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_user_sessions_ng-0.1.3.tar", max compression
+gzip compressed data, was "django_user_sessions_ng-0.1.4.tar", max compression
```

## Comparing `django_user_sessions_ng-0.1.3.tar` & `django_user_sessions_ng-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       89 2024-04-28 00:08:03.904461 django_user_sessions_ng-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2024-04-26 18:51:04.822052 django_user_sessions_ng-0.1.3/LICENSE
--rw-r--r--   0        0        0     4069 2024-04-27 23:46:48.394594 django_user_sessions_ng-0.1.3/README.md
--rw-r--r--   0        0        0      118 2024-04-27 20:16:03.525794 django_user_sessions_ng-0.1.3/django_user_sessions_ng/__init__.py
--rw-r--r--   0        0        0     2399 2024-04-27 23:33:42.676124 django_user_sessions_ng-0.1.3/django_user_sessions_ng/admin.py
--rw-r--r--   0        0        0      397 2024-04-27 22:34:31.767976 django_user_sessions_ng-0.1.3/django_user_sessions_ng/apps.py
--rw-r--r--   0        0        0      159 2024-04-26 21:20:22.210905 django_user_sessions_ng-0.1.3/django_user_sessions_ng/backends/__init__.py
--rw-r--r--   0        0        0      280 2024-04-27 13:33:28.785336 django_user_sessions_ng-0.1.3/django_user_sessions_ng/backends/cached_db.py
--rw-r--r--   0        0        0     1968 2024-04-27 21:42:40.617595 django_user_sessions_ng-0.1.3/django_user_sessions_ng/backends/db.py
--rw-r--r--   0        0        0      906 2024-04-27 22:16:16.481844 django_user_sessions_ng-0.1.3/django_user_sessions_ng/geoip.py
--rw-r--r--   0        0        0        0 2024-04-26 19:01:36.789758 django_user_sessions_ng-0.1.3/django_user_sessions_ng/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 19:01:36.789758 django_user_sessions_ng-0.1.3/django_user_sessions_ng/management/commands/__init__.py
--rw-r--r--   0        0        0       97 2024-04-26 19:01:36.789758 django_user_sessions_ng-0.1.3/django_user_sessions_ng/management/commands/clearsessions.py
--rw-r--r--   0        0        0     2769 2024-04-27 20:01:09.222690 django_user_sessions_ng-0.1.3/django_user_sessions_ng/management/commands/download_geoip_db.py
--rw-r--r--   0        0        0      675 2024-04-28 00:07:25.700570 django_user_sessions_ng-0.1.3/django_user_sessions_ng/middleware.py
--rw-r--r--   0        0        0     1873 2024-04-27 22:17:16.172541 django_user_sessions_ng-0.1.3/django_user_sessions_ng/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-26 19:01:36.789758 django_user_sessions_ng-0.1.3/django_user_sessions_ng/migrations/__init__.py
--rw-r--r--   0        0        0     2247 2024-04-27 23:35:08.997049 django_user_sessions_ng-0.1.3/django_user_sessions_ng/models.py
--rw-r--r--   0        0        0     1630 2024-04-28 00:08:08.414526 django_user_sessions_ng-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4952 1970-01-01 00:00:00.000000 django_user_sessions_ng-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      173 2024-04-29 18:57:18.529341 django_user_sessions_ng-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2024-04-26 18:51:04.822052 django_user_sessions_ng-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4069 2024-04-27 23:46:48.394594 django_user_sessions_ng-0.1.4/README.md
+-rw-r--r--   0        0        0      118 2024-04-27 20:16:03.525794 django_user_sessions_ng-0.1.4/django_user_sessions_ng/__init__.py
+-rw-r--r--   0        0        0     2399 2024-04-27 23:33:42.676124 django_user_sessions_ng-0.1.4/django_user_sessions_ng/admin.py
+-rw-r--r--   0        0        0      397 2024-04-27 22:34:31.767976 django_user_sessions_ng-0.1.4/django_user_sessions_ng/apps.py
+-rw-r--r--   0        0        0      159 2024-04-26 21:20:22.210905 django_user_sessions_ng-0.1.4/django_user_sessions_ng/backends/__init__.py
+-rw-r--r--   0        0        0      280 2024-04-27 13:33:28.785336 django_user_sessions_ng-0.1.4/django_user_sessions_ng/backends/cached_db.py
+-rw-r--r--   0        0        0     1968 2024-04-27 21:42:40.617595 django_user_sessions_ng-0.1.4/django_user_sessions_ng/backends/db.py
+-rw-r--r--   0        0        0      906 2024-04-27 22:16:16.481844 django_user_sessions_ng-0.1.4/django_user_sessions_ng/geoip.py
+-rw-r--r--   0        0        0        0 2024-04-26 19:01:36.789758 django_user_sessions_ng-0.1.4/django_user_sessions_ng/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 19:01:36.789758 django_user_sessions_ng-0.1.4/django_user_sessions_ng/management/commands/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-26 19:01:36.789758 django_user_sessions_ng-0.1.4/django_user_sessions_ng/management/commands/clearsessions.py
+-rw-r--r--   0        0        0     2769 2024-04-27 20:01:09.222690 django_user_sessions_ng-0.1.4/django_user_sessions_ng/management/commands/download_geoip_db.py
+-rw-r--r--   0        0        0      671 2024-04-29 18:57:40.653046 django_user_sessions_ng-0.1.4/django_user_sessions_ng/middleware.py
+-rw-r--r--   0        0        0     1873 2024-04-27 22:17:16.172541 django_user_sessions_ng-0.1.4/django_user_sessions_ng/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-26 19:01:36.789758 django_user_sessions_ng-0.1.4/django_user_sessions_ng/migrations/__init__.py
+-rw-r--r--   0        0        0     2247 2024-04-27 23:35:08.997049 django_user_sessions_ng-0.1.4/django_user_sessions_ng/models.py
+-rw-r--r--   0        0        0     1630 2024-04-29 18:57:24.439441 django_user_sessions_ng-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4952 1970-01-01 00:00:00.000000 django_user_sessions_ng-0.1.4/PKG-INFO
```

### Comparing `django_user_sessions_ng-0.1.3/LICENSE` & `django_user_sessions_ng-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_user_sessions_ng-0.1.3/README.md` & `django_user_sessions_ng-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_user_sessions_ng-0.1.3/django_user_sessions_ng/admin.py` & `django_user_sessions_ng-0.1.4/django_user_sessions_ng/admin.py`

 * *Files identical despite different names*

### Comparing `django_user_sessions_ng-0.1.3/django_user_sessions_ng/backends/db.py` & `django_user_sessions_ng-0.1.4/django_user_sessions_ng/backends/db.py`

 * *Files identical despite different names*

### Comparing `django_user_sessions_ng-0.1.3/django_user_sessions_ng/geoip.py` & `django_user_sessions_ng-0.1.4/django_user_sessions_ng/geoip.py`

 * *Files identical despite different names*

### Comparing `django_user_sessions_ng-0.1.3/django_user_sessions_ng/management/commands/download_geoip_db.py` & `django_user_sessions_ng-0.1.4/django_user_sessions_ng/management/commands/download_geoip_db.py`

 * *Files identical despite different names*

### Comparing `django_user_sessions_ng-0.1.3/django_user_sessions_ng/middleware.py` & `django_user_sessions_ng-0.1.4/django_user_sessions_ng/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,11 +6,9 @@
 
 
 class SessionMiddleware(DjangoSessionMiddleware):
     def process_request(self, request: HttpRequest) -> None:
         session_key = request.COOKIES.get(settings.SESSION_COOKIE_NAME, None)
         ip = get_client_ip(request)[0]
         user_agent = request.headers.get("User-Agent", None)
-        if user_agent:
-            device = str(user_agents.parse(user_agent))
-
+        device = str(user_agents.parse(user_agent)) if user_agent else None
         request.session = self.SessionStore(ip=ip, device=device, session_key=session_key)
```

### Comparing `django_user_sessions_ng-0.1.3/django_user_sessions_ng/migrations/0001_initial.py` & `django_user_sessions_ng-0.1.4/django_user_sessions_ng/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_user_sessions_ng-0.1.3/django_user_sessions_ng/models.py` & `django_user_sessions_ng-0.1.4/django_user_sessions_ng/models.py`

 * *Files identical despite different names*

### Comparing `django_user_sessions_ng-0.1.3/pyproject.toml` & `django_user_sessions_ng-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-user-sessions-ng"
-version = "0.1.3"
+version = "0.1.4"
 description = "Django User Sessions NG - a Django package to manage multiple user sessions."
 authors = ["yujinio <root@yujin.io>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "sessions", "session-management", "django-user-sessions-ng"]
 repository = "https://github.com/yujinio/django-user-sessions-ng"
 include = ["README.md", "LICENSE", "CHANGELOG.md"]
```

### Comparing `django_user_sessions_ng-0.1.3/PKG-INFO` & `django_user_sessions_ng-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-user-sessions-ng
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django User Sessions NG - a Django package to manage multiple user sessions.
 Home-page: https://github.com/yujinio/django-user-sessions-ng
 License: MIT
 Keywords: django,sessions,session-management,django-user-sessions-ng
 Author: yujinio
 Author-email: root@yujin.io
 Requires-Python: >=3.11,<4.0
```

