# Comparing `tmp/pallets_sphinx_themes-2.1.2.tar.gz` & `tmp/pallets_sphinx_themes-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pallets_sphinx_themes-2.1.2.tar", last modified: Fri Apr 19 17:31:25 2024, max compression
+gzip compressed data, was "pallets_sphinx_themes-2.1.3.tar", last modified: Mon Apr 29 16:44:54 2024, max compression
```

## Comparing `pallets_sphinx_themes-2.1.2.tar` & `pallets_sphinx_themes-2.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     6185 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/CHANGES.rst
--rw-r--r--   0        0        0     1475 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/LICENSE.txt
--rw-r--r--   0        0        0      376 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/README.md
--rw-r--r--   0        0        0     1638 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/pyproject.toml
--rw-r--r--   0        0        0        6 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/requirements/build.in
--rw-r--r--   0        0        0      227 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/requirements/build.txt
--rw-r--r--   0        0        0       15 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/requirements/dev.in
--rw-r--r--   0        0        0      852 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/requirements/dev.txt
--rw-r--r--   0        0        0     5323 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/__init__.py
--rw-r--r--   0        0        0     1326 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/theme_check.py
--rw-r--r--   0        0        0        0 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/__init__.py
--rw-r--r--   0        0        0      453 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/babel/static/babel.css
--rw-r--r--   0        0        0       47 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/babel/theme.conf
--rw-r--r--   0        0        0      174 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/click/__init__.py
--rw-r--r--   0        0        0     7677 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/click/domain.py
--rw-r--r--   0        0        0      585 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/click/static/click.css
--rw-r--r--   0        0        0       70 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/click/theme.conf
--rw-r--r--   0        0        0      237 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/flask/static/flask.css
--rw-r--r--   0        0        0       47 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/flask/theme.conf
--rw-r--r--   0        0        0     1548 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/jinja/__init__.py
--rw-r--r--   0        0        0     8756 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/jinja/domain.py
--rw-r--r--   0        0        0      425 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/jinja/static/jinja.css
--rw-r--r--   0        0        0       70 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/jinja/theme.conf
--rw-r--r--   0        0        0      449 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/platter/static/platter.css
--rw-r--r--   0        0        0       49 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/platter/theme.conf
--rw-r--r--   0        0        0      391 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/404.html
--rw-r--r--   0        0        0     4052 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/__init__.py
--rw-r--r--   0        0        0       38 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/ethicalads.html
--rw-r--r--   0        0        0      768 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/layout.html
--rw-r--r--   0        0        0       66 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/localtoc.html
--rw-r--r--   0        0        0      173 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/project.html
--rw-r--r--   0        0        0      645 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/relations.html
--rw-r--r--   0        0        0     8187 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css
--rw-r--r--   0        0        0     1582 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js
--rw-r--r--   0        0        0      181 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/theme.conf
--rw-r--r--   0        0        0      253 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/versions.html
--rw-r--r--   0        0        0      237 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/werkzeug/static/werkzeug.css
--rw-r--r--   0        0        0       50 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/werkzeug/theme.conf
--rw-r--r--   0        0        0     4516 2024-04-19 17:31:25.000000 pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/versions.py
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 pallets_sphinx_themes-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6292 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/CHANGES.rst
+-rw-r--r--   0        0        0     1475 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      376 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/README.md
+-rw-r--r--   0        0        0     1638 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/requirements/build.in
+-rw-r--r--   0        0        0      227 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/requirements/build.txt
+-rw-r--r--   0        0        0       15 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/requirements/dev.in
+-rw-r--r--   0        0        0      852 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/requirements/dev.txt
+-rw-r--r--   0        0        0     5323 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/__init__.py
+-rw-r--r--   0        0        0     1326 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/theme_check.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/__init__.py
+-rw-r--r--   0        0        0      453 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/babel/static/babel.css
+-rw-r--r--   0        0        0       47 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/babel/theme.conf
+-rw-r--r--   0        0        0      174 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/click/__init__.py
+-rw-r--r--   0        0        0     7839 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/click/domain.py
+-rw-r--r--   0        0        0      585 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/click/static/click.css
+-rw-r--r--   0        0        0       70 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/click/theme.conf
+-rw-r--r--   0        0        0      237 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/flask/static/flask.css
+-rw-r--r--   0        0        0       47 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/flask/theme.conf
+-rw-r--r--   0        0        0     1548 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/jinja/__init__.py
+-rw-r--r--   0        0        0     8918 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/jinja/domain.py
+-rw-r--r--   0        0        0      425 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/jinja/static/jinja.css
+-rw-r--r--   0        0        0       70 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/jinja/theme.conf
+-rw-r--r--   0        0        0      449 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/platter/static/platter.css
+-rw-r--r--   0        0        0       49 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/platter/theme.conf
+-rw-r--r--   0        0        0      391 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/404.html
+-rw-r--r--   0        0        0     4052 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/ethicalads.html
+-rw-r--r--   0        0        0      768 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/layout.html
+-rw-r--r--   0        0        0       66 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/localtoc.html
+-rw-r--r--   0        0        0      173 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/project.html
+-rw-r--r--   0        0        0      645 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/relations.html
+-rw-r--r--   0        0        0     8187 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css
+-rw-r--r--   0        0        0     1582 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js
+-rw-r--r--   0        0        0      181 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/theme.conf
+-rw-r--r--   0        0        0      253 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/versions.html
+-rw-r--r--   0        0        0      237 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/werkzeug/static/werkzeug.css
+-rw-r--r--   0        0        0       50 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/werkzeug/theme.conf
+-rw-r--r--   0        0        0     4516 2024-04-29 16:44:54.000000 pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/versions.py
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 pallets_sphinx_themes-2.1.3/PKG-INFO
```

### Comparing `pallets_sphinx_themes-2.1.2/CHANGES.rst` & `pallets_sphinx_themes-2.1.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Version 2.1.3
+-------------
+
+Released 2024-04-29
+
+-   Allow Sphinx's parallel build feature. :issue:`88`
+
+
 Version 2.1.2
 -------------
 
 Released 2024-04-19
 
 -   Use modern packaging metadata with ``pyproject.toml`` instead of ``setup.cfg``.
 -   Use ``flit_core`` instead of ``setuptools`` as build backend.
```

### Comparing `pallets_sphinx_themes-2.1.2/LICENSE.txt` & `pallets_sphinx_themes-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/pyproject.toml` & `pallets_sphinx_themes-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Pallets-Sphinx-Themes"
-version = "2.1.2"
+version = "2.1.3"
 description = "Sphinx themes for Pallets and related projects."
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 maintainers = [{ name = "Pallets", email = "contact@palletsprojects.com" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Sphinx",
```

### Comparing `pallets_sphinx_themes-2.1.2/requirements/dev.txt` & `pallets_sphinx_themes-2.1.3/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/__init__.py` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/__init__.py`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/theme_check.py` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/theme_check.py`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/click/domain.py` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/click/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,14 +251,19 @@
 
 
 class ClickDomain(Domain):
     name = "click"
     label = "Click"
     directives = {"example": DeclareExampleDirective, "run": RunExampleDirective}
 
+    def merge_domaindata(self, docnames, otherdata):
+        # Needed to support parallel build.
+        # Not using self.data -- nothing to merge.
+        pass
+
 
 def delete_example_runner_state(app, doctree):
     """Close and remove the :class:`ExampleRunner` instance once the
     document has been read.
     """
     runner = getattr(doctree, "click_example_runner", None)
```

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/click/static/click.css` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/click/static/click.css`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/jinja/__init__.py` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/jinja/__init__.py`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/jinja/domain.py` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/jinja/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,10 +254,15 @@
     label = "Jinja"
     directives = {
         "filters": MappedFunctionsDirective,
         "tests": MappedFunctionsDirective,
         "nodes": NodesDirective,
     }
 
+    def merge_domaindata(self, docnames, otherdata):
+        # Needed to support parallel build.
+        # Not using self.data -- nothing to merge.
+        pass
+
 
 def setup(app):
     app.add_domain(JinjaDomain)
```

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/__init__.py` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/__init__.py`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/layout.html` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/layout.html`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/relations.html` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/relations.html`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/src/pallets_sphinx_themes/versions.py` & `pallets_sphinx_themes-2.1.3/src/pallets_sphinx_themes/versions.py`

 * *Files identical despite different names*

### Comparing `pallets_sphinx_themes-2.1.2/PKG-INFO` & `pallets_sphinx_themes-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pallets-Sphinx-Themes
-Version: 2.1.2
+Version: 2.1.3
 Summary: Sphinx themes for Pallets and related projects.
 Maintainer-email: Pallets <contact@palletsprojects.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

