# Comparing `tmp/project_async-0.0.1rc74.post1.tar.gz` & `tmp/project_async-0.0.1rc76.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_async-0.0.1rc74.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "project_async-0.0.1rc76.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `project_async-0.0.1rc74.post1.tar` & `project_async-0.0.1rc76.post1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      340 2024-04-28 06:10:29.753233 project_async-0.0.1rc74.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-28 06:10:29.753233 project_async-0.0.1rc74.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      563 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      831 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1799 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.pypirc
--rw-r--r--   0        0        0       70 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.vscode/extensions.json
--rw-r--r--   0        0        0      459 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.vscode/launch.json
--rw-r--r--   0        0        0      821 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1071 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/LICENSE
--rw-r--r--   0        0        0     1889 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/README.md
--rw-r--r--   0        0        0      412 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/SUPPORT.md
--rw-r--r--   0        0        0     5925 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/pyproject.toml
--rw-r--r--   0        0        0      210 2024-04-28 06:10:46.157274 project_async-0.0.1rc74.post1/src/project_async/__init__.py
--rw-r--r--   0        0        0     1167 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/src/project_async/client.py
--rw-r--r--   0        0        0      270 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/src/project_async/errors.py
--rw-r--r--   0        0        0      810 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/src/project_async/model.py
--rw-r--r--   0        0        0      580 2024-04-28 06:10:29.757233 project_async-0.0.1rc74.post1/tests/test_client.py
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 project_async-0.0.1rc74.post1/PKG-INFO
+-rw-r--r--   0        0        0      340 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      563 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      831 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1799 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.pypirc
+-rw-r--r--   0        0        0       70 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      459 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      821 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1071 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/LICENSE
+-rw-r--r--   0        0        0     1889 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/README.md
+-rw-r--r--   0        0        0      412 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/SUPPORT.md
+-rw-r--r--   0        0        0     5925 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/pyproject.toml
+-rw-r--r--   0        0        0      210 2024-04-29 16:47:13.690792 project_async-0.0.1rc76.post1/src/project_async/__init__.py
+-rw-r--r--   0        0        0     1167 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/src/project_async/client.py
+-rw-r--r--   0        0        0      270 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/src/project_async/errors.py
+-rw-r--r--   0        0        0      810 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/src/project_async/model.py
+-rw-r--r--   0        0        0      580 2024-04-29 16:46:58.166844 project_async-0.0.1rc76.post1/tests/test_client.py
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 project_async-0.0.1rc76.post1/PKG-INFO
```

### Comparing `project_async-0.0.1rc74.post1/.devcontainer/devcontainer.json` & `project_async-0.0.1rc76.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/.github/dependabot.yml` & `project_async-0.0.1rc76.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/.github/workflows/CI.yml` & `project_async-0.0.1rc76.post1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/.github/workflows/schedule-update-actions.yml` & `project_async-0.0.1rc76.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/.gitignore` & `project_async-0.0.1rc76.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/.pre-commit-config.yaml` & `project_async-0.0.1rc76.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/.vscode/settings.json` & `project_async-0.0.1rc76.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/LICENSE` & `project_async-0.0.1rc76.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/README.md` & `project_async-0.0.1rc76.post1/README.md`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/pyproject.toml` & `project_async-0.0.1rc76.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 requires-python = ">=3.11"
 dependencies = ["aiohttp==3.9.5", "dataclasses-json==0.6.4"]
 dynamic = ['version']
 
 [project.optional-dependencies]
 dev = [
     "bandit[toml]==1.7.8",
-    "black==24.4.0",
+    "black==24.4.2",
     "check-manifest==0.49",
-    "flake8-bugbear==24.4.21",
+    "flake8-bugbear==24.4.26",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8",
     "flake8-pyproject",
     "isort==5.13.2",
     "pre-commit==3.7.0",
     "pylint==3.1.0",
     "pytest-cov==5.0.0",
     "pytest-mock<3.14.1",
     "pytest-runner",
-    "pytest==8.1.1",
+    "pytest==8.2.0",
     "pytest-github-actions-annotate-failures",
     "pytype",
     "shellcheck-py==0.10.0.1",
 ]
 
 [project.urls]
 Documentation = "https://github.com/albertomontesg/python-async-api-client/blob/main/README.md"
```

### Comparing `project_async-0.0.1rc74.post1/src/project_async/client.py` & `project_async-0.0.1rc76.post1/src/project_async/client.py`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/src/project_async/model.py` & `project_async-0.0.1rc76.post1/src/project_async/model.py`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/tests/test_client.py` & `project_async-0.0.1rc76.post1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `project_async-0.0.1rc74.post1/PKG-INFO` & `project_async-0.0.1rc76.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-async
-Version: 0.0.1rc74.post1
+Version: 0.0.1rc76.post1
 Summary: Sample Python Project for creating a new Python Async Client for a new API
 Author-email: Alberto Montes <al.montes.gomez@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp==3.9.5
 Requires-Dist: dataclasses-json==0.6.4
 Requires-Dist: bandit[toml]==1.7.8 ; extra == "dev"
-Requires-Dist: black==24.4.0 ; extra == "dev"
+Requires-Dist: black==24.4.2 ; extra == "dev"
 Requires-Dist: check-manifest==0.49 ; extra == "dev"
-Requires-Dist: flake8-bugbear==24.4.21 ; extra == "dev"
+Requires-Dist: flake8-bugbear==24.4.26 ; extra == "dev"
 Requires-Dist: flake8-docstrings ; extra == "dev"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: flake8-pyproject ; extra == "dev"
 Requires-Dist: isort==5.13.2 ; extra == "dev"
 Requires-Dist: pre-commit==3.7.0 ; extra == "dev"
 Requires-Dist: pylint==3.1.0 ; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "dev"
 Requires-Dist: pytest-mock<3.14.1 ; extra == "dev"
 Requires-Dist: pytest-runner ; extra == "dev"
-Requires-Dist: pytest==8.1.1 ; extra == "dev"
+Requires-Dist: pytest==8.2.0 ; extra == "dev"
 Requires-Dist: pytest-github-actions-annotate-failures ; extra == "dev"
 Requires-Dist: pytype ; extra == "dev"
 Requires-Dist: shellcheck-py==0.10.0.1 ; extra == "dev"
 Project-URL: Documentation, https://github.com/albertomontesg/python-async-api-client/blob/main/README.md
 Project-URL: Source, https://github.com/albertomontesg/python-async-api-client
 Project-URL: Tracker, https://github.com/albertomontesg/python-async-api-client/issues
 Provides-Extra: dev
```

