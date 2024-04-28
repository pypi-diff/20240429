# Comparing `tmp/cz_conventional_gitmoji-0.3.0.tar.gz` & `tmp/cz_conventional_gitmoji-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_conventional_gitmoji-0.3.0.tar", max compression
+gzip compressed data, was "cz_conventional_gitmoji-0.3.1.tar", max compression
```

## Comparing `cz_conventional_gitmoji-0.3.0.tar` & `cz_conventional_gitmoji-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2615 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/README.md
--rw-r--r--   0        0        0     2631 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/__init__.py
--rw-r--r--   0        0        0     1285 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/conventional_gitmojis_info.txt
--rw-r--r--   0        0        0    13466 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/main.py
--rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/py.typed
--rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/gitmojify/__init__.py
--rw-r--r--   0        0        0     1687 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/gitmojify/mojify.py
--rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/gitmojify/py.typed
--rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/__init__.py
--rw-r--r--   0        0        0     2701 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/gitmojis.py
--rw-r--r--   0        0        0      406 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/model.py
--rw-r--r--   0        0        0        0 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/py.typed
--rw-r--r--   0        0        0    10765 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/spec.py
--rw-r--r--   0        0        0      817 2024-04-17 20:13:25.142815 cz_conventional_gitmoji-0.3.0/src/shared/utils.py
--rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2625 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/README.md
+-rw-r--r--   0        0        0     2554 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/__init__.py
+-rw-r--r--   0        0        0     1285 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/conventional_gitmojis_info.txt
+-rw-r--r--   0        0        0    13467 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/main.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/py.typed
+-rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/gitmojify/__init__.py
+-rw-r--r--   0        0        0     1687 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/gitmojify/mojify.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/gitmojify/py.typed
+-rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/__init__.py
+-rw-r--r--   0        0        0     2701 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/gitmojis.py
+-rw-r--r--   0        0        0      406 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/model.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/py.typed
+-rw-r--r--   0        0        0    10765 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/spec.py
+-rw-r--r--   0        0        0      817 2024-04-28 22:58:29.670232 cz_conventional_gitmoji-0.3.1/src/shared/utils.py
+-rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 cz_conventional_gitmoji-0.3.1/PKG-INFO
```

### Comparing `cz_conventional_gitmoji-0.3.0/README.md` & `cz_conventional_gitmoji-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # cz-conventional-gitmoji
 
 A [commitizen](https://github.com/commitizen-tools/commitizen) plugin that combines [gitmoji](https://gitmoji.dev/) and [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/).
 
 ## Installation
 
-```bash
-poetry add cz-conventional-gitmoji
-```
-
-or with pip:
+With `pip` or any other package manager of your choice, the usual way:
 
 ```bash
 pip install cz-conventional-gitmoji
 ```
 
 ## Usage
```

### Comparing `cz_conventional_gitmoji-0.3.0/pyproject.toml` & `cz_conventional_gitmoji-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cz-conventional-gitmoji"
-version = "0.3.0"
+version = "0.3.1"
 description = "A commitizen plugin that combines gitmoji and conventional."
 authors = ["ljnsn <82611987+ljnsn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "shared", from = "src" },
   { include = "cz_gitmoji", from = "src" },
@@ -16,41 +16,38 @@
 cz_gitmoji = "cz_gitmoji.main:CommitizenGitmojiCz"
 
 [tool.poetry.scripts]
 gitmojify = "gitmojify.mojify:run"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-commitizen = "^3.2.2"
-attrs = "^23.1.0"
+commitizen = ">=3.2.2"
+attrs = ">=23.1.0"
 setuptools = { version = "*", python = ">=3.12" }
 
 [tool.poetry.group.dev.dependencies]
-black = ">=22.12,<24.0"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-coverage = { extras = ["toml"], version = "^7.0.1" }
-ruff = ">=0.0.246,<0.3.8"
-mypy = "^1.3.0"
+pytest = ">=7.2.0"
+pytest-cov = ">=4.0.0"
+coverage = { extras = ["toml"], version = ">=7.0.1" }
+ruff = ">=0.3.7"
+mypy = ">=1.3.0"
 pre-commit = ">=2.0"
 
 [tool.commitizen]
 name = "cz_gitmoji"
-version = "0.3.0"
+version = "0.3.1"
 bump_message = "🔖 bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 update_changelog_on_bump = true
 
-[tool.black]
-target-version = ["py37", "py38", "py39", "py310", "py311"]
-
 [tool.ruff]
 fix = true
 src = ["src", "test"]
+target-version = "py37"
 
 [tool.ruff.lint]
 ignore = [
   # Line too long
   "E501",
   # unable to detect undefined names
   "F403",
```

### Comparing `cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/conventional_gitmojis_info.txt` & `cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/conventional_gitmojis_info.txt`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.0/src/cz_gitmoji/main.py` & `cz_conventional_gitmoji-0.3.1/src/cz_gitmoji/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,23 +28,23 @@
     return required_validator(text, msg="Subject is required.")
 
 
 class CommitizenGitmojiCz(BaseCommitizen):
     # pattern to match messages for bumping
     # if none of these match, version will not be bumped (unless manually specified)
     bump_pattern = (
-        rf"^(BREAKING[\-\ ]CHANGE"
+        rf"^((BREAKING[\-\ ]CHANGE"
         rf"|{GJ_BOOM}? ?boom"
         rf"|{GJ_FEAT}? ?feat"
         rf"|{GJ_FIX}? ?fix"
         rf"|{GJ_HOTFIX}? ?hotfix"
         rf"|{GJ_REFACTOR}? +refactor"
         rf"|{GJ_PERF}? ?perf)"
         r"(\(.+\))?"  # scope
-        r"(!)?"  # breaking
+        r"!?):"  # breaking
     )
     # map types to SemVer
     bump_map = OrderedDict(
         (
             (r"^.+!$", MAJOR),
             (r"^BREAKING[\-\ ]CHANGE", MAJOR),
             (rf"^{GJ_BOOM}? ?boom", MAJOR),
```

### Comparing `cz_conventional_gitmoji-0.3.0/src/gitmojify/mojify.py` & `cz_conventional_gitmoji-0.3.1/src/gitmojify/mojify.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.0/src/shared/gitmojis.py` & `cz_conventional_gitmoji-0.3.1/src/shared/gitmojis.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.0/src/shared/spec.py` & `cz_conventional_gitmoji-0.3.1/src/shared/spec.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.0/src/shared/utils.py` & `cz_conventional_gitmoji-0.3.1/src/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cz_conventional_gitmoji-0.3.0/PKG-INFO` & `cz_conventional_gitmoji-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: cz-conventional-gitmoji
-Version: 0.3.0
+Version: 0.3.1
 Summary: A commitizen plugin that combines gitmoji and conventional.
 Home-page: https://github.com/ljnsn/cz-conventional-gitmoji
 License: MIT
 Author: ljnsn
 Author-email: 82611987+ljnsn@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: commitizen (>=3.2.2,<4.0.0)
+Requires-Dist: attrs (>=23.1.0)
+Requires-Dist: commitizen (>=3.2.2)
 Requires-Dist: setuptools ; python_version >= "3.12"
 Project-URL: Repository, https://github.com/ljnsn/cz-conventional-gitmoji
 Description-Content-Type: text/markdown
 
 # cz-conventional-gitmoji
 
 A [commitizen](https://github.com/commitizen-tools/commitizen) plugin that combines [gitmoji](https://gitmoji.dev/) and [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/).
 
 ## Installation
 
-```bash
-poetry add cz-conventional-gitmoji
-```
-
-or with pip:
+With `pip` or any other package manager of your choice, the usual way:
 
 ```bash
 pip install cz-conventional-gitmoji
 ```
 
 ## Usage
```

