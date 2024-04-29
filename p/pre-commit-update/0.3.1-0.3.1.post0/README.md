# Comparing `tmp/pre_commit_update-0.3.1.tar.gz` & `tmp/pre_commit_update-0.3.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_update-0.3.1.tar", max compression
+gzip compressed data, was "pre_commit_update-0.3.1.post0.tar", max compression
```

## Comparing `pre_commit_update-0.3.1.tar` & `pre_commit_update-0.3.1.post0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/LICENSE
--rw-r--r--   0        0        0     6594 2024-04-26 20:49:14.183951 pre_commit_update-0.3.1/README.md
--rw-r--r--   0        0        0     1675 2024-04-26 20:45:38.009532 pre_commit_update-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/__init__.py
--rw-r--r--   0        0        0     3167 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/cli.py
--rw-r--r--   0        0        0      229 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/__init__.py
--rw-r--r--   0        0        0      685 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/env.py
--rw-r--r--   0        0        0     3116 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/message.py
--rw-r--r--   0        0        0     4526 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/repo.py
--rw-r--r--   0        0        0      800 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/yaml.py
--rw-r--r--   0        0        0        0 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/py.typed
--rw-r--r--   0        0        0     2151 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/repo.py
--rw-r--r--   0        0        0      759 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/utils.py
--rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 pre_commit_update-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-04-26 21:16:03.414133 pre_commit_update-0.3.1.post0/LICENSE
+-rw-r--r--   0        0        0      367 2024-04-26 21:16:03.414133 pre_commit_update-0.3.1.post0/README.md
+-rw-r--r--   0        0        0     1665 2024-04-29 12:41:40.793796 pre_commit_update-0.3.1.post0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 15:53:44.498016 pre_commit_update-0.3.1.post0/src/pre_commit_update/__init__.py
+-rw-r--r--   0        0        0     3167 2024-04-26 21:16:03.414133 pre_commit_update-0.3.1.post0/src/pre_commit_update/cli.py
+-rw-r--r--   0        0        0      229 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/env.py
+-rw-r--r--   0        0        0     3116 2024-04-26 21:16:03.414133 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/message.py
+-rw-r--r--   0        0        0     5614 2024-04-26 21:16:03.417466 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/repo.py
+-rw-r--r--   0        0        0      800 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/yaml.py
+-rw-r--r--   0        0        0        0 2022-04-01 23:18:32.000000 pre_commit_update-0.3.1.post0/src/pre_commit_update/py.typed
+-rw-r--r--   0        0        0     2151 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/repo.py
+-rw-r--r--   0        0        0      759 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/utils.py
+-rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 pre_commit_update-0.3.1.post0/PKG-INFO
```

### Comparing `pre_commit_update-0.3.1/LICENSE` & `pre_commit_update-0.3.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1/pyproject.toml` & `pre_commit_update-0.3.1.post0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "pre-commit-update"
-version = "0.3.1"
+version = "0.3.1post0"
 description = "Simple CLI tool to check and update pre-commit hooks."
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = ["Vojko Pribudić <dmanthing@gmail.com>"]
-repository = "https://gitlab.com/vojko.pribudic.foss/pre-commit-update"
+repository = "https://gitlab.com/vojko.pribudic/pre-commit-update"
 readme = "README.md"
 license = "MIT"
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
@@ -27,16 +27,16 @@
 include = ["README.md", "LICENSE"]
 exclude = [
     ".gitignore",
     ".gitlab-ci.yml",
 ]
 
 [tool.poetry.urls]
-"Tracker" = "https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/issues"
-"Changelog" = "https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/releases"
+"Tracker" = "https://gitlab.com/vojko.pribudic/pre-commit-update/-/issues"
+"Changelog" = "https://gitlab.com/vojko.pribudic/pre-commit-update/-/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 click = ">=8.1"
 GitPython = ">=3.1"
 packaging = ">=23.2"
 pyproject-parser = ">=0.9"
```

### Comparing `pre_commit_update-0.3.1/src/pre_commit_update/cli.py` & `pre_commit_update-0.3.1.post0/src/pre_commit_update/cli.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1/src/pre_commit_update/managers/env.py` & `pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/env.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1/src/pre_commit_update/managers/message.py` & `pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/message.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1/src/pre_commit_update/managers/yaml.py` & `pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/yaml.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1/src/pre_commit_update/repo.py` & `pre_commit_update-0.3.1.post0/src/pre_commit_update/repo.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1/src/pre_commit_update/utils.py` & `pre_commit_update-0.3.1.post0/src/pre_commit_update/utils.py`

 * *Files identical despite different names*

