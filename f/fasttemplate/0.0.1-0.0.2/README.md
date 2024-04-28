# Comparing `tmp/fasttemplate-0.0.1.tar.gz` & `tmp/fasttemplate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttemplate-0.0.1.tar", max compression
+gzip compressed data, was "fasttemplate-0.0.2.tar", max compression
```

## Comparing `fasttemplate-0.0.1.tar` & `fasttemplate-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0       53 2024-04-27 21:43:51.362929 fasttemplate-0.0.1/README.md
--rw-r--r--   0        0        0     1525 2024-04-26 22:50:19.913426 fasttemplate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      106 2024-04-26 22:50:19.885426 fasttemplate-0.0.1/src/fasttemplate/__init__.py
--rw-r--r--   0        0        0       96 2024-04-22 20:45:26.772140 fasttemplate-0.0.1/src/fasttemplate/__version__.py
--rw-r--r--   0        0        0      936 2024-04-27 19:19:08.751736 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/.github/workflows/tests.yml.mako
--rw-r--r--   0        0        0     1210 2024-04-27 19:19:05.143702 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/.gitignore.mako
--rw-r--r--   0        0        0      811 2024-04-27 19:19:08.767736 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/.pre-commit-config.yaml.mako
--rw-r--r--   0        0        0      109 2024-04-27 16:06:20.689481 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/DESCRIPTION.md
--rw-r--r--   0        0        0      517 2024-04-27 18:42:19.667187 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/Makefile.mako
--rw-r--r--   0        0        0      147 2024-04-27 18:42:19.667187 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/README.md.mako
--rw-r--r--   0        0        0      154 2024-04-27 19:46:35.792577 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/docker-entrypoint.sh.mako
--rw-r--r--   0        0        0     1805 2024-04-27 19:19:11.655763 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/pyproject.toml.mako
--rw-r--r--   0        0        0        0 2024-04-26 22:50:19.929426 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/src/__init__.py.mako
--rw-r--r--   0        0        0       63 2024-04-27 20:20:34.789388 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/src/builder/__init__.py.mako
--rw-r--r--   0        0        0      162 2024-04-27 21:34:05.329618 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/src/builder/builder.py.mako
--rw-r--r--   0        0        0       45 2024-04-27 19:19:08.775736 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/src/main.py.mako
--rw-r--r--   0        0        0      139 2024-04-27 21:03:40.561748 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/src/routers/__init__.py.mako
--rw-r--r--   0        0        0       53 2024-04-27 21:17:24.694473 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/src/routers/root/__init__.py.mako
--rw-r--r--   0        0        0      250 2024-04-27 21:25:45.401509 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/src/routers/root/api.py.mako
--rw-r--r--   0        0        0        0 2024-04-26 22:50:19.929426 fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/tests/__init__.py.mako
--rw-r--r--   0        0        0        0 2024-04-22 20:45:33.484228 fasttemplate-0.0.1/src/fasttemplate/console/__init__.py
--rw-r--r--   0        0        0     1473 2024-04-27 18:42:19.659187 fasttemplate-0.0.1/src/fasttemplate/console/application.py
--rw-r--r--   0        0        0        0 2024-04-22 20:45:33.484228 fasttemplate-0.0.1/src/fasttemplate/console/commands/__init__.py
--rw-r--r--   0        0        0       96 2024-04-22 20:45:33.484228 fasttemplate-0.0.1/src/fasttemplate/console/commands/_base.py
--rw-r--r--   0        0        0      645 2024-04-26 22:50:16.933400 fasttemplate-0.0.1/src/fasttemplate/console/commands/about.py
--rw-r--r--   0        0        0     3776 2024-04-27 18:42:19.659187 fasttemplate-0.0.1/src/fasttemplate/console/commands/asset.py
--rw-r--r--   0        0        0     2842 2024-04-27 19:37:23.687353 fasttemplate-0.0.1/src/fasttemplate/console/commands/new.py
--rw-r--r--   0        0        0        0 2024-04-26 22:50:19.913426 fasttemplate-0.0.1/src/fasttemplate/layouts/__init__.py
--rw-r--r--   0        0        0     4702 2024-04-27 21:36:47.415055 fasttemplate-0.0.1/src/fasttemplate/layouts/_base.py
--rw-r--r--   0        0        0       56 2024-04-26 22:50:19.933426 fasttemplate-0.0.1/src/fasttemplate/layouts/fastapi/__init__.py
--rw-r--r--   0        0        0       87 2024-04-26 22:50:19.933426 fasttemplate-0.0.1/src/fasttemplate/layouts/fastapi/layout.py
--rw-r--r--   0        0        0      528 2024-04-27 19:35:08.635607 fasttemplate-0.0.1/src/fasttemplate/layouts/manager.py
--rw-r--r--   0        0        0        0 2024-04-22 20:45:26.772140 fasttemplate-0.0.1/src/fasttemplate/utils/__init__.py
--rw-r--r--   0        0        0       62 2024-04-22 20:45:26.772140 fasttemplate-0.0.1/src/fasttemplate/utils/_compat.py
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 fasttemplate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     2094 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/README.md
+-rw-r--r--   0        0        0     1711 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/__version__.py
+-rw-r--r--   0        0        0      936 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/.github/workflows/tests.yml.mako
+-rw-r--r--   0        0        0     1210 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/.gitignore.mako
+-rw-r--r--   0        0        0      811 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/.pre-commit-config.yaml.mako
+-rw-r--r--   0        0        0      109 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/DESCRIPTION.md
+-rw-r--r--   0        0        0      517 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/Makefile.mako
+-rw-r--r--   0        0        0      147 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/README.md.mako
+-rw-r--r--   0        0        0      154 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/docker-entrypoint.sh.mako
+-rw-r--r--   0        0        0     1805 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/pyproject.toml.mako
+-rw-r--r--   0        0        0        0 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/src/__init__.py.mako
+-rw-r--r--   0        0        0       63 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/src/builder/__init__.py.mako
+-rw-r--r--   0        0        0      162 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/src/builder/builder.py.mako
+-rw-r--r--   0        0        0       45 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/src/main.py.mako
+-rw-r--r--   0        0        0      139 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/src/routers/__init__.py.mako
+-rw-r--r--   0        0        0       53 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/src/routers/root/__init__.py.mako
+-rw-r--r--   0        0        0      250 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/src/routers/root/api.py.mako
+-rw-r--r--   0        0        0        0 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/tests/__init__.py.mako
+-rw-r--r--   0        0        0        0 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/console/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/console/application.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/console/commands/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/console/commands/_base.py
+-rw-r--r--   0        0        0      645 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/console/commands/about.py
+-rw-r--r--   0        0        0     3776 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/console/commands/asset.py
+-rw-r--r--   0        0        0     2858 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/console/commands/new.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/layouts/__init__.py
+-rw-r--r--   0        0        0     4821 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/layouts/_base.py
+-rw-r--r--   0        0        0       56 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/layouts/fastapi/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/layouts/fastapi/layout.py
+-rw-r--r--   0        0        0      528 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/layouts/manager.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/utils/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-28 22:24:34.616046 fasttemplate-0.0.2/src/fasttemplate/utils/_compat.py
+-rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 fasttemplate-0.0.2/PKG-INFO
```

### Comparing `fasttemplate-0.0.1/pyproject.toml` & `fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/pyproject.toml.mako`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 [tool.poetry]
-name = "fasttemplate"
-version = "0.0.1"
-description = "FastAPI project builer"
-authors = ["Ivan Koldakov <coldie322@gmail.com>"]
+name = "${project['name']}"
+version = "${project['version']}"
+description = "${project['description']}"
+% if author:
+  % if author["name"] and author["email"]:
+authors = ["${author['name']} <${author['email']}>"]
+  % endif
+  % if author["name"] and not author["email"]:
+authors = ["${author['name']}"]
+  % endif
+  % if not author["name"] and author["email"]:
+authors = ["<${author['email']}>"]
+  % endif
+% endif
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
-cleo = "^2.1.0"
-mako = "^1.3.3"
+fastapi = "^0.110.2"
+hypercorn = "^0.16.0"
+uvloop = "^0.19.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 
-[tool.poetry.scripts]
-fasttemplate = "fasttemplate.console.application:main"
-
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -90,15 +98,16 @@
 
 [tool.mypy]
 python_version = "3.12"
 follow_imports = "skip"
 ignore_missing_imports = true
 check_untyped_defs = true
 files = [
-    "src",
-    "tests",
+    % for path in project["mypy_files"]:
+    "${path}",
+    % endfor
 ]
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
```

### Comparing `fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/.github/workflows/tests.yml.mako` & `fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/.github/workflows/tests.yml.mako`

 * *Files identical despite different names*

### Comparing `fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/.gitignore.mako` & `fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/.gitignore.mako`

 * *Files identical despite different names*

### Comparing `fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/.pre-commit-config.yaml.mako` & `fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/.pre-commit-config.yaml.mako`

 * *Files identical despite different names*

### Comparing `fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/Makefile.mako` & `fasttemplate-0.0.2/src/fasttemplate/assets/fastapi/default/Makefile.mako`

 * *Files identical despite different names*

### Comparing `fasttemplate-0.0.1/src/fasttemplate/assets/fastapi/default/pyproject.toml.mako` & `fasttemplate-0.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
-name = "${project['name']}"
-version = "${project['version']}"
-description = "${project['description']}"
-% if author:
-  % if author["name"] and author["email"]:
-authors = ["${author['name']} <${author['email']}>"]
-  % endif
-  % if author["name"] and not author["email"]:
-authors = ["${author['name']}"]
-  % endif
-  % if not author["name"] and author["email"]:
-authors = ["<${author['email']}>"]
-  % endif
-% endif
+name = "fasttemplate"
+version = "0.0.2"
+description = "Python project builer"
+authors = ["Ivan Koldakov <coldie322@gmail.com>"]
 readme = "README.md"
+homepage = "https://github.com/koldakov/fasttemplate"
+repository = "https://github.com/koldakov/fasttemplate"
+keywords = [
+    "packaging",
+    "poetry",
+    "skeleton",
+    "fastapi",
+]
 
 [tool.poetry.dependencies]
 python = "^3.12"
-fastapi = "^0.110.2"
-hypercorn = "^0.16.0"
-uvloop = "^0.19.0"
+cleo = "^2.1.0"
+mako = "^1.3.3"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 
+[tool.poetry.scripts]
+fasttemplate = "fasttemplate.console.application:main"
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -98,16 +98,15 @@
 
 [tool.mypy]
 python_version = "3.12"
 follow_imports = "skip"
 ignore_missing_imports = true
 check_untyped_defs = true
 files = [
-    % for path in project["mypy_files"]:
-    "${path}",
-    % endfor
+    "src",
+    "tests",
 ]
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
```

### Comparing `fasttemplate-0.0.1/src/fasttemplate/console/application.py` & `fasttemplate-0.0.2/src/fasttemplate/console/application.py`

 * *Files identical despite different names*

### Comparing `fasttemplate-0.0.1/src/fasttemplate/console/commands/about.py` & `fasttemplate-0.0.2/src/fasttemplate/console/commands/about.py`

 * *Files identical despite different names*

### Comparing `fasttemplate-0.0.1/src/fasttemplate/console/commands/asset.py` & `fasttemplate-0.0.2/src/fasttemplate/console/commands/asset.py`

 * *Files identical despite different names*

### Comparing `fasttemplate-0.0.1/src/fasttemplate/console/commands/new.py` & `fasttemplate-0.0.2/src/fasttemplate/console/commands/new.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 <info>Project configuration:
     src = {src}
     project path = {layout.project_dir}
     asset type = {asset.type}
     asset name = {asset.name}
 </info>
-Now you can go to the project: <info>cd {layout.project_dir}</info> and start!
+Now you can go to the project: <info>cd {layout.project_dir} && make install</info> and start!
 
 <comment>Happy coding!</comment>\
 """
         )
 
     def handle(self) -> int:
         layout: LayoutBase = self.layout
```

### Comparing `fasttemplate-0.0.1/src/fasttemplate/layouts/_base.py` & `fasttemplate-0.0.2/src/fasttemplate/layouts/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,16 +88,21 @@
     def _get_author(self, author: Author | None, /) -> Author | None:
         """
         TODO: Read username/login from GIT
         """
         if author:
             return author
 
+        login: str
+        try:
+            login = getlogin()
+        except OSError:
+            login = "My Greate Name"
         return Author(
-            name=getlogin(),
+            name=login,
         )
 
     def _validate_asset(self) -> None:
         if self.asset not in self.assets:
             raise AssetDoesNotExistError(f"Asset {self.asset} does not exist.")
 
     def _get_project_fields(self) -> dict:
```

### Comparing `fasttemplate-0.0.1/src/fasttemplate/layouts/manager.py` & `fasttemplate-0.0.2/src/fasttemplate/layouts/manager.py`

 * *Files identical despite different names*

