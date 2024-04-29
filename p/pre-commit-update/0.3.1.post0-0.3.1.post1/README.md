# Comparing `tmp/pre_commit_update-0.3.1.post0.tar.gz` & `tmp/pre_commit_update-0.3.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_update-0.3.1.post0.tar", max compression
+gzip compressed data, was "pre_commit_update-0.3.1.post1.tar", max compression
```

## Comparing `pre_commit_update-0.3.1.post0.tar` & `pre_commit_update-0.3.1.post1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-04-26 21:16:03.414133 pre_commit_update-0.3.1.post0/LICENSE
--rw-r--r--   0        0        0      367 2024-04-26 21:16:03.414133 pre_commit_update-0.3.1.post0/README.md
--rw-r--r--   0        0        0     1665 2024-04-29 12:41:40.793796 pre_commit_update-0.3.1.post0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 15:53:44.498016 pre_commit_update-0.3.1.post0/src/pre_commit_update/__init__.py
--rw-r--r--   0        0        0     3167 2024-04-26 21:16:03.414133 pre_commit_update-0.3.1.post0/src/pre_commit_update/cli.py
--rw-r--r--   0        0        0      229 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/__init__.py
--rw-r--r--   0        0        0      685 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/env.py
--rw-r--r--   0        0        0     3116 2024-04-26 21:16:03.414133 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/message.py
--rw-r--r--   0        0        0     5614 2024-04-26 21:16:03.417466 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/repo.py
--rw-r--r--   0        0        0      800 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/yaml.py
--rw-r--r--   0        0        0        0 2022-04-01 23:18:32.000000 pre_commit_update-0.3.1.post0/src/pre_commit_update/py.typed
--rw-r--r--   0        0        0     2151 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/repo.py
--rw-r--r--   0        0        0      759 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post0/src/pre_commit_update/utils.py
--rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 pre_commit_update-0.3.1.post0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-04-29 12:57:20.028245 pre_commit_update-0.3.1.post1/LICENSE
+-rw-r--r--   0        0        0      367 2024-04-29 12:57:20.028245 pre_commit_update-0.3.1.post1/README.md
+-rw-r--r--   0        0        0     1665 2024-04-29 13:09:15.955703 pre_commit_update-0.3.1.post1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 15:53:44.498016 pre_commit_update-0.3.1.post1/src/pre_commit_update/__init__.py
+-rw-r--r--   0        0        0     3167 2024-04-29 12:57:20.028245 pre_commit_update-0.3.1.post1/src/pre_commit_update/cli.py
+-rw-r--r--   0        0        0      229 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/env.py
+-rw-r--r--   0        0        0     3116 2024-04-29 12:57:20.028245 pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/message.py
+-rw-r--r--   0        0        0     5626 2024-04-29 13:08:59.715600 pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/repo.py
+-rw-r--r--   0        0        0      800 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/yaml.py
+-rw-r--r--   0        0        0        0 2022-04-01 23:18:32.000000 pre_commit_update-0.3.1.post1/src/pre_commit_update/py.typed
+-rw-r--r--   0        0        0     2151 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post1/src/pre_commit_update/repo.py
+-rw-r--r--   0        0        0      759 2024-04-18 17:00:48.849180 pre_commit_update-0.3.1.post1/src/pre_commit_update/utils.py
+-rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 pre_commit_update-0.3.1.post1/PKG-INFO
```

### Comparing `pre_commit_update-0.3.1.post0/LICENSE` & `pre_commit_update-0.3.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post0/pyproject.toml` & `pre_commit_update-0.3.1.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pre-commit-update"
-version = "0.3.1post0"
+version = "0.3.1post1"
 description = "Simple CLI tool to check and update pre-commit hooks."
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = ["Vojko Pribudić <dmanthing@gmail.com>"]
 repository = "https://gitlab.com/vojko.pribudic/pre-commit-update"
 readme = "README.md"
 license = "MIT"
 classifiers = [
```

### Comparing `pre_commit_update-0.3.1.post0/src/pre_commit_update/cli.py` & `pre_commit_update-0.3.1.post1/src/pre_commit_update/cli.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/env.py` & `pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/env.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/message.py` & `pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/message.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/repo.py` & `pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             if repo.current_version != repo.latest_version:
                 messages.add_to_update_message(
                     repo.name, repo.current_version, repo.latest_version
                 )
                 self._repos_data[i]["rev"] = repo.latest_version
                 continue
             if (
-                self._migration["repo_index"]
+                self._migration["repo_index"] is not None
                 and i == self._migration["repo_index"]
                 and repo.current_version == repo.latest_version
             ):
                 messages.add_to_update_message(
                     repo.name, self._migration["old_repo"], self._migration["new_repo"]
                 )
                 self._repos_data[i]["rev"] = repo.latest_version
```

### Comparing `pre_commit_update-0.3.1.post0/src/pre_commit_update/managers/yaml.py` & `pre_commit_update-0.3.1.post1/src/pre_commit_update/managers/yaml.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post0/src/pre_commit_update/repo.py` & `pre_commit_update-0.3.1.post1/src/pre_commit_update/repo.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post0/src/pre_commit_update/utils.py` & `pre_commit_update-0.3.1.post1/src/pre_commit_update/utils.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.1.post0/PKG-INFO` & `pre_commit_update-0.3.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pre-commit-update
-Version: 0.3.1.post0
+Version: 0.3.1.post1
 Summary: Simple CLI tool to check and update pre-commit hooks.
 Home-page: https://gitlab.com/vojko.pribudic/pre-commit-update
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pre-commit-update Version: 0.3.1.post0 Summary:
+Metadata-Version: 2.1 Name: pre-commit-update Version: 0.3.1.post1 Summary:
 Simple CLI tool to check and update pre-commit hooks. Home-page: https://
 gitlab.com/vojko.pribudic/pre-commit-update License: MIT Author: Vojko
 PribudiÄ Author-email: dmanthing@gmail.com Maintainer: Vojko PribudiÄ
 Maintainer-email: dmanthing@gmail.com Requires-Python: >=3.8 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Web
 Environment Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
```

