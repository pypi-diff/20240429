# Comparing `tmp/python-criteria-0.4.0.tar.gz` & `tmp/python_criteria-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-criteria-0.4.0.tar", last modified: Wed Apr 10 10:38:10 2024, max compression
+gzip compressed data, was "python_criteria-0.5.0.tar", last modified: Sun Apr 28 23:48:54 2024, max compression
```

## Comparing `python-criteria-0.4.0.tar` & `python_criteria-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:38:10.188271 python-criteria-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:38:10.184271 python-criteria-0.4.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.devcontainer/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.devcontainer/postCreateCommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:38:10.184271 python-criteria-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:38:10.184271 python-criteria-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:38:10.184271 python-criteria-0.4.0/.husky/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:38:10.184271 python-criteria-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-10 10:38:06.000000 python-criteria-0.4.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-10 10:38:06.000000 python-criteria-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-10 10:38:10.188271 python-criteria-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 10:38:06.000000 python-criteria-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-10 10:38:06.000000 python-criteria-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:38:10.188271 python-criteria-0.4.0/python_criteria/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-10 10:38:06.000000 python-criteria-0.4.0/python_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-10 10:38:06.000000 python-criteria-0.4.0/python_criteria/clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 10:38:06.000000 python-criteria-0.4.0/python_criteria/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-10 10:38:06.000000 python-criteria-0.4.0/python_criteria/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-10 10:38:06.000000 python-criteria-0.4.0/python_criteria/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-10 10:38:06.000000 python-criteria-0.4.0/python_criteria/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:38:10.188271 python-criteria-0.4.0/python_criteria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-10 10:38:10.000000 python-criteria-0.4.0/python_criteria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-10 10:38:10.000000 python-criteria-0.4.0/python_criteria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:38:10.000000 python-criteria-0.4.0/python_criteria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 10:38:10.000000 python-criteria-0.4.0/python_criteria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:38:10.188271 python-criteria-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:48:54.216230 python_criteria-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:48:54.212230 python_criteria-0.5.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.devcontainer/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.devcontainer/postCreateCommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:48:54.212230 python_criteria-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:48:54.212230 python_criteria-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:48:54.212230 python_criteria-0.5.0/.husky/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:48:54.212230 python_criteria-0.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-28 23:48:50.000000 python_criteria-0.5.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-28 23:48:50.000000 python_criteria-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-28 23:48:54.216230 python_criteria-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-28 23:48:50.000000 python_criteria-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-28 23:48:50.000000 python_criteria-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:48:54.212230 python_criteria-0.5.0/python_criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-28 23:48:50.000000 python_criteria-0.5.0/python_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-28 23:48:50.000000 python_criteria-0.5.0/python_criteria/clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-28 23:48:50.000000 python_criteria-0.5.0/python_criteria/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-28 23:48:50.000000 python_criteria-0.5.0/python_criteria/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-28 23:48:50.000000 python_criteria-0.5.0/python_criteria/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-28 23:48:50.000000 python_criteria-0.5.0/python_criteria/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:48:54.216230 python_criteria-0.5.0/python_criteria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-28 23:48:54.000000 python_criteria-0.5.0/python_criteria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-28 23:48:54.000000 python_criteria-0.5.0/python_criteria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 23:48:54.000000 python_criteria-0.5.0/python_criteria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-28 23:48:54.000000 python_criteria-0.5.0/python_criteria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 23:48:54.216230 python_criteria-0.5.0/setup.cfg
```

### Comparing `python-criteria-0.4.0/.devcontainer/devcontainer.json` & `python_criteria-0.5.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/.devcontainer/docker-compose.yml` & `python_criteria-0.5.0/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/.github/workflows/python-publish.yml` & `python_criteria-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/.gitignore` & `python_criteria-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/.pylintrc` & `python_criteria-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/.vscode/tasks.json` & `python_criteria-0.5.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/LICENSE` & `python_criteria-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/pyproject.toml` & `python_criteria-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/python_criteria/clauses.py` & `python_criteria-0.5.0/python_criteria/clauses.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/python_criteria/filter.py` & `python_criteria-0.5.0/python_criteria/filter.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/python_criteria/sqlalchemy.py` & `python_criteria-0.5.0/python_criteria/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/python_criteria/visitor.py` & `python_criteria-0.5.0/python_criteria/visitor.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.4.0/python_criteria.egg-info/SOURCES.txt` & `python_criteria-0.5.0/python_criteria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

