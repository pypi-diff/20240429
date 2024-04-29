# Comparing `tmp/fps_auth-0.5.0.tar.gz` & `tmp/fps_auth-0.5.1.tar.gz`

## Comparing `fps_auth-0.5.0.tar` & `fps_auth-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.5.0/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.5.0/fps_auth/__init__.py
--rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 fps_auth-0.5.0/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.5.0/fps_auth/config.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fps_auth-0.5.0/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.5.0/fps_auth/main.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fps_auth-0.5.0/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.5.0/fps_auth/py.typed
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 fps_auth-0.5.0/fps_auth/routes.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_auth-0.5.0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.5.0/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.5.0/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 fps_auth-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fps_auth-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.5.1/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/config.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/main.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/py.typed
+-rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/routes.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_auth-0.5.1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.5.1/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.5.1/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 fps_auth-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fps_auth-0.5.1/PKG-INFO
```

### Comparing `fps_auth-0.5.0/fps_auth/backends.py` & `fps_auth-0.5.1/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.0/fps_auth/config.py` & `fps_auth-0.5.1/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.0/fps_auth/db.py` & `fps_auth-0.5.1/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.0/fps_auth/main.py` & `fps_auth-0.5.1/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.0/fps_auth/routes.py` & `fps_auth-0.5.1/fps_auth/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                     users = (await session.execute(statement)).unique().all()
                 return [usr.User for usr in users if usr.User.is_active]
 
             @router.get("/api/me")
             async def get_api_me(
                 permissions: Optional[str] = None,
                 user: UserRead = Depends(backend.current_user()),
+                update_user = Depends(backend.update_user),
             ):
                 checked_permissions: Dict[str, List[str]] = {}
                 if permissions is None:
                     permissions = "{}"
                 else:
                     permissions = permissions.replace("'", '"')
                 permissions_dict = json.loads(permissions)
@@ -92,14 +93,22 @@
 
                 keys = ["username", "name", "display_name", "initials", "avatar_url", "color"]
                 identity = {k: getattr(user, k) for k in keys}
                 if not identity["name"] and not identity["display_name"]:
                     moon = get_anonymous_username()
                     identity["name"] = f"Anonymous {moon}"
                     identity["display_name"] = f"Anonymous {moon}"
+                    identity["initials"] = f"A{moon[0]}"
+                    await update_user(
+                        dict(
+                            name=identity["name"],
+                            display_name=identity["display_name"],
+                            permissions=checked_permissions,
+                        )
+                    )
                 return {
                     "identity": identity,
                     "permissions": checked_permissions,
                 }
 
             # redefine GET /me because we want our current_user dependency
             # it is first defined in users_router and so it wins over the one in
```

### Comparing `fps_auth-0.5.0/.gitignore` & `fps_auth-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.0/COPYING.md` & `fps_auth-0.5.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.0/pyproject.toml` & `fps_auth-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.0/PKG-INFO` & `fps_auth-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_auth
-Version: 0.5.0
+Version: 0.5.1
 Summary: An FPS plugin for the authentication API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

