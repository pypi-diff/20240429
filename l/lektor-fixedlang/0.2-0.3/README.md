# Comparing `tmp/lektor-fixedlang-0.2.tar.gz` & `tmp/lektor_fixedlang-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-fixedlang-0.2.tar", last modified: Thu Mar 14 14:04:33 2024, max compression
+gzip compressed data, was "lektor_fixedlang-0.3.tar", last modified: Mon Apr 29 12:53:29 2024, max compression
```

## Comparing `lektor-fixedlang-0.2.tar` & `lektor_fixedlang-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-03-14 14:04:33.263575 lektor-fixedlang-0.2/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1491 2024-02-21 13:50:36.000000 lektor-fixedlang-0.2/LICENSE.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)     4372 2024-03-14 14:04:33.263575 lektor-fixedlang-0.2/PKG-INFO
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1474 2024-03-14 14:04:10.000000 lektor-fixedlang-0.2/README.rst
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-03-14 14:04:33.263575 lektor-fixedlang-0.2/lektor_fixedlang.egg-info/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     4372 2024-03-14 14:04:33.000000 lektor-fixedlang-0.2/lektor_fixedlang.egg-info/PKG-INFO
--rw-r--r--   0 uyar      (1000) uyar      (1000)      323 2024-03-14 14:04:33.000000 lektor-fixedlang-0.2/lektor_fixedlang.egg-info/SOURCES.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2024-03-14 14:04:33.000000 lektor-fixedlang-0.2/lektor_fixedlang.egg-info/dependency_links.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       62 2024-03-14 14:04:33.000000 lektor-fixedlang-0.2/lektor_fixedlang.egg-info/entry_points.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       90 2024-03-14 14:04:33.000000 lektor-fixedlang-0.2/lektor_fixedlang.egg-info/requires.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       17 2024-03-14 14:04:33.000000 lektor-fixedlang-0.2/lektor_fixedlang.egg-info/top_level.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1686 2024-03-14 13:34:55.000000 lektor-fixedlang-0.2/lektor_fixedlang.py
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1931 2024-03-01 19:33:27.000000 lektor-fixedlang-0.2/pyproject.toml
--rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2024-03-14 14:04:33.263575 lektor-fixedlang-0.2/setup.cfg
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-03-14 14:04:33.263575 lektor-fixedlang-0.2/tests/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1677 2024-03-14 13:45:35.000000 lektor-fixedlang-0.2/tests/test_fixedlang.py
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-29 12:53:29.239700 lektor_fixedlang-0.3/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1491 2024-02-21 13:50:36.000000 lektor_fixedlang-0.3/LICENSE.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     4489 2024-04-29 12:53:29.239700 lektor_fixedlang-0.3/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1474 2024-03-14 14:04:10.000000 lektor_fixedlang-0.3/README.rst
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-29 12:53:29.239700 lektor_fixedlang-0.3/lektor_fixedlang.egg-info/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     4489 2024-04-29 12:53:29.000000 lektor_fixedlang-0.3/lektor_fixedlang.egg-info/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      323 2024-04-29 12:53:29.000000 lektor_fixedlang-0.3/lektor_fixedlang.egg-info/SOURCES.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2024-04-29 12:53:29.000000 lektor_fixedlang-0.3/lektor_fixedlang.egg-info/dependency_links.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       62 2024-04-29 12:53:29.000000 lektor_fixedlang-0.3/lektor_fixedlang.egg-info/entry_points.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      116 2024-04-29 12:53:29.000000 lektor_fixedlang-0.3/lektor_fixedlang.egg-info/requires.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       17 2024-04-29 12:53:29.000000 lektor_fixedlang-0.3/lektor_fixedlang.egg-info/top_level.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     2254 2024-04-29 12:52:28.000000 lektor_fixedlang-0.3/lektor_fixedlang.py
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     2119 2024-04-29 12:45:09.000000 lektor_fixedlang-0.3/pyproject.toml
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2024-04-29 12:53:29.239700 lektor_fixedlang-0.3/setup.cfg
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-29 12:53:29.239700 lektor_fixedlang-0.3/tests/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     3319 2024-04-29 12:49:34.000000 lektor_fixedlang-0.3/tests/test_fixedlang.py
```

### Comparing `lektor-fixedlang-0.2/LICENSE.txt` & `lektor_fixedlang-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lektor-fixedlang-0.2/PKG-INFO` & `lektor_fixedlang-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-fixedlang
-Version: 0.2
+Version: 0.3
 Summary: Set fixed languages for patterns in Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
 License: Copyright 2024 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -33,26 +33,29 @@
 Project-URL: repository, https://github.com/uyar/lektor-fixedlang
 Keywords: lektor,plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Lektor
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: lektor
+Requires-Dist: beautifulsoup4
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: style
 Requires-Dist: ruff; extra == "style"
 Provides-Extra: dev
 Requires-Dist: lektor-fixedlang[style,tests]; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: tox; extra == "dev"
```

### Comparing `lektor-fixedlang-0.2/README.rst` & `lektor_fixedlang-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `lektor-fixedlang-0.2/lektor_fixedlang.egg-info/PKG-INFO` & `lektor_fixedlang-0.3/lektor_fixedlang.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-fixedlang
-Version: 0.2
+Version: 0.3
 Summary: Set fixed languages for patterns in Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
 License: Copyright 2024 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -33,26 +33,29 @@
 Project-URL: repository, https://github.com/uyar/lektor-fixedlang
 Keywords: lektor,plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Lektor
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: lektor
+Requires-Dist: beautifulsoup4
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: style
 Requires-Dist: ruff; extra == "style"
 Provides-Extra: dev
 Requires-Dist: lektor-fixedlang[style,tests]; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: tox; extra == "dev"
```

### Comparing `lektor-fixedlang-0.2/lektor_fixedlang.py` & `lektor_fixedlang-0.3/lektor_fixedlang.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,70 @@
 # Copyright (C) 2024 H. Turgut Uyar <uyar@tekir.org>
 #
 # lektor-fixedlang is released under the BSD license.
 # Read the included LICENSE.txt file for details.
 
-__version__ = "0.2"
+__version__ = "0.3"
 
 import re
-from collections import defaultdict
 from pathlib import Path
 
+from bs4 import BeautifulSoup
 from lektor.db import Page
 from lektor.pluginsystem import Plugin
+from lektor.reporter import reporter
+
+
+def inherited_lang(node):
+    lang = None
+    for parent in node.parents:
+        lang = parent.attrs.get("lang")
+        if lang is not None:
+            break
+    return lang
 
 
 class FixedLangPlugin(Plugin):
     name = "fixedlang"
     description = "Set fixed language for specific patterns."
 
     def on_setup_env(self, **extra):
         config = self.get_config()
-        self.patterns = defaultdict(dict)
+        self.patterns = []
         for tag in config.sections():
             for pattern, lang in config.section_as_dict(tag).items():
-                self.patterns[pattern].update({"lang": lang, "tag": tag})
+                self.patterns.append((re.compile(f'({pattern})'), lang, tag))
         self.processed = set()
 
+    def on_before_build_all(self, builder, **extra):
+        reporter.report_generic("Starting setting fixed languages")
+
     def on_after_build(self, builder, build_state, source, prog, **extra):
-        if isinstance(source, Page):
-            artifact = prog.primary_artifact
-            if artifact is None:
-                return
-            filename = artifact.dst_filename
-            if filename in self.processed:
-                return
-            dst_file = Path(filename)
-            content = dst_file.read_text()
-            modified = False
-            for pattern, lang_tag in self.patterns.items():
-                if re.search(pattern, content, flags=re.IGNORECASE):
-                    content = re.sub(
-                        f'({pattern})',
-                        '<%(tag)s lang="%(lang)s">\\1</%(tag)s>' % lang_tag,
-                        content,
-                    )
-                    modified = True
-            if modified:
-                dst_file.write_text(content)
-            self.processed.add(filename)
+        if not isinstance(source, Page):
+            return
+        artifact = prog.primary_artifact
+        if artifact is None:
+            return
+        filename = artifact.dst_filename
+        if filename in self.processed:
+            return
+        dst_file = Path(filename)
+        content = dst_file.read_text()
+        modified = False
+        soup = BeautifulSoup(content, "html.parser")
+        for (compiled, lang, tag) in self.patterns:
+            for node in soup.find_all(string=compiled):
+                if lang == inherited_lang(node):
+                    continue
+                markup = compiled.sub(
+                    f'<{tag} lang="{lang}">\\1</{tag}>',
+                    node.string,
+                )
+                subsoup = BeautifulSoup(markup, "html.parser")
+                node.replace_with(subsoup)
+                modified = True
+        if modified:
+            dst_file.write_text(str(soup))
+        self.processed.add(filename)
+
+    def on_after_build_all(self, builder, **extra):
+        reporter.report_generic("Finished setting fixed languages")
```

### Comparing `lektor-fixedlang-0.2/pyproject.toml` & `lektor_fixedlang-0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [project]
 name = "lektor-fixedlang"
-version = "0.2"
+version = "0.3"
 description = "Set fixed languages for patterns in Lektor."
 readme = "README.rst"
 
 authors = [{name = "H. Turgut Uyar", email = "uyar@tekir.org"}]
 license = {file = "LICENSE.txt"}
 
 keywords = ["lektor", "plugin"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Framework :: Lektor",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
+    "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: Site Management",
 ]
 
 requires-python = "~=3.8"
-dependencies = ["lektor"]
+dependencies = ["lektor", "beautifulsoup4"]
 
 [project.optional-dependencies]
-tests = ["pytest"]
+tests = ["pytest", "pytest-cov"]
 style = ["ruff"]
 dev = [
     "lektor-fixedlang[tests,style]",
     "build",
     "twine",
     "tox",
 ]
@@ -40,14 +41,21 @@
 
 [project.urls]
 repository = "https://github.com/uyar/lektor-fixedlang"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
+[tool.coverage.run]
+source = ["lektor_fixedlang.py"]
+
+[tool.coverage.report]
+show_missing = true
+skip_covered = true
+
 [tool.ruff]
 line-length = 79
 
 [tool.ruff.lint]
 select = ["A", "E", "F", "I", "T", "W"]
 
 [tool.ruff.lint.per-file-ignores]
```

