# Comparing `tmp/wikidot-3.0.4.tar.gz` & `tmp/wikidot-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikidot-3.0.4.tar", last modified: Fri Apr 19 01:53:09 2024, max compression
+gzip compressed data, was "wikidot-3.0.5.tar", last modified: Mon Apr 29 03:19:05 2024, max compression
```

## Comparing `wikidot-3.0.4.tar` & `wikidot-3.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 01:52:49.000000 wikidot-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 01:52:49.000000 wikidot-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-19 01:53:09.006564 wikidot-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-19 01:52:49.000000 wikidot-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 01:52:49.000000 wikidot-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:53:09.006564 wikidot-3.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:08.998564 wikidot-3.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.002564 wikidot-3.0.4/src/wikidot/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.002564 wikidot-3.0.4/src/wikidot/common/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/common/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.002564 wikidot-3.0.4/src/wikidot/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/connector/ajax.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/connector/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/page_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/page_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/page_votes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/private_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/site.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/site_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot/util/parser/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/parser/odate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/parser/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/quick_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/requestutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/stringutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot/util/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/table/char_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.406314 wikidot-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 03:18:45.000000 wikidot-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 03:18:45.000000 wikidot-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-29 03:19:05.402314 wikidot-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-29 03:18:45.000000 wikidot-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-29 03:18:45.000000 wikidot-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:19:05.406314 wikidot-3.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.394314 wikidot-3.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.398314 wikidot-3.0.5/src/wikidot/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.398314 wikidot-3.0.5/src/wikidot/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/common/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.398314 wikidot-3.0.5/src/wikidot/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/connector/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/connector/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.402314 wikidot-3.0.5/src/wikidot/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/page_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/page_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/page_votes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/site_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/module/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.402314 wikidot-3.0.5/src/wikidot/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.402314 wikidot-3.0.5/src/wikidot/util/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/parser/odate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/parser/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/quick_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/requestutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/stringutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.402314 wikidot-3.0.5/src/wikidot/util/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-29 03:18:45.000000 wikidot-3.0.5/src/wikidot/util/table/char_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:19:05.402314 wikidot-3.0.5/src/wikidot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-29 03:19:05.000000 wikidot-3.0.5/src/wikidot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-29 03:19:05.000000 wikidot-3.0.5/src/wikidot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:19:05.000000 wikidot-3.0.5/src/wikidot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-29 03:19:05.000000 wikidot-3.0.5/src/wikidot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 03:19:05.000000 wikidot-3.0.5/src/wikidot.egg-info/top_level.txt
```

### Comparing `wikidot-3.0.4/LICENSE` & `wikidot-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/PKG-INFO` & `wikidot-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidot
-Version: 3.0.4
+Version: 3.0.5
 Summary: Wikidot Utility Library
 Author-email: ukwhatn <ukwhatn@gmail.com>
 Project-URL: Homepage, https://github.com/ukwhatn/wikidot.py
 Project-URL: Bug Tracker, https://github.com/ukwhatn/wikidot.py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wikidot-3.0.4/README.md` & `wikidot-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/pyproject.toml` & `wikidot-3.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wikidot"
-version = "3.0.4"
+version = "3.0.5"
 authors = [{ name = "ukwhatn", email = "ukwhatn@gmail.com" }]
 description = "Wikidot Utility Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
```

### Comparing `wikidot-3.0.4/src/wikidot/common/decorators.py` & `wikidot-3.0.5/src/wikidot/common/decorators.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/common/exceptions.py` & `wikidot-3.0.5/src/wikidot/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/connector/ajax.py` & `wikidot-3.0.5/src/wikidot/connector/ajax.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/module/auth.py` & `wikidot-3.0.5/src/wikidot/module/auth.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/module/client.py` & `wikidot-3.0.5/src/wikidot/module/client.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/module/page.py` & `wikidot-3.0.5/src/wikidot/module/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 elif key in ["rating_votes"]:
                     key = "votes_count"
 
                 page_params[key] = value
 
             # タグのリストを統合
             for key in ["tags", "_tags"]:
-                if page_params[key] is None:
+                if key not in page_params or page_params[key] is None:
                     page_params[key] = []
 
             page_params["tags"] = page_params["tags"] + page_params["_tags"]
             del page_params["_tags"]
 
             # ページオブジェクトを作成
             pages.append(Page(site, **page_params))
```

### Comparing `wikidot-3.0.4/src/wikidot/module/page_revision.py` & `wikidot-3.0.5/src/wikidot/module/page_revision.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/module/page_votes.py` & `wikidot-3.0.5/src/wikidot/module/page_votes.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/module/private_message.py` & `wikidot-3.0.5/src/wikidot/module/private_message.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/module/site.py` & `wikidot-3.0.5/src/wikidot/module/site.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/module/site_application.py` & `wikidot-3.0.5/src/wikidot/module/site_application.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/module/user.py` & `wikidot-3.0.5/src/wikidot/module/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """ユーザーオブジェクトのリスト"""
 
     def __iter__(self) -> Iterator["AbstractUser"]:
         return super().__iter__()
 
     @staticmethod
     def from_names(
-            client: "Client", names: list[str], raise_when_not_found: bool = False
+        client: "Client", names: list[str], raise_when_not_found: bool = False
     ) -> "UserCollection":
         """ユーザー名のリストからユーザーオブジェクトのリストを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
@@ -143,15 +143,15 @@
     # name: str | None
     # unix_name: str | None
     # avatar_url: str | None
     ip: None = None
 
     @staticmethod
     def from_name(
-            client: "Client", name: str, raise_when_not_found: bool = False
+        client: "Client", name: str, raise_when_not_found: bool = False
     ) -> "User":
         """ユーザー名からユーザーオブジェクトを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
```

### Comparing `wikidot-3.0.4/src/wikidot/util/parser/odate.py` & `wikidot-3.0.5/src/wikidot/util/parser/odate.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/util/parser/user.py` & `wikidot-3.0.5/src/wikidot/util/parser/user.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/util/quick_module.py` & `wikidot-3.0.5/src/wikidot/util/quick_module.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/util/requestutil.py` & `wikidot-3.0.5/src/wikidot/util/requestutil.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/util/stringutil.py` & `wikidot-3.0.5/src/wikidot/util/stringutil.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot/util/table/char_table.py` & `wikidot-3.0.5/src/wikidot/util/table/char_table.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.4/src/wikidot.egg-info/PKG-INFO` & `wikidot-3.0.5/src/wikidot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidot
-Version: 3.0.4
+Version: 3.0.5
 Summary: Wikidot Utility Library
 Author-email: ukwhatn <ukwhatn@gmail.com>
 Project-URL: Homepage, https://github.com/ukwhatn/wikidot.py
 Project-URL: Bug Tracker, https://github.com/ukwhatn/wikidot.py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wikidot-3.0.4/src/wikidot.egg-info/SOURCES.txt` & `wikidot-3.0.5/src/wikidot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

