# Comparing `tmp/jeeves_pr_stack-0.1.2.tar.gz` & `tmp/jeeves_pr_stack-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_pr_stack-0.1.2.tar", max compression
+gzip compressed data, was "jeeves_pr_stack-0.1.3.tar", max compression
```

## Comparing `jeeves_pr_stack-0.1.2.tar` & `jeeves_pr_stack-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1866 2023-09-09 13:22:17.066306 jeeves_pr_stack-0.1.2/README.md
--rw-r--r--   0        0        0       36 2023-09-07 11:49:27.494946 jeeves_pr_stack-0.1.2/jeeves_pr_stack/__init__.py
--rw-r--r--   0        0        0     6932 2024-02-02 09:50:30.069016 jeeves_pr_stack-0.1.2/jeeves_pr_stack/app.py
--rw-r--r--   0        0        0      606 2023-10-05 08:31:31.104154 jeeves_pr_stack-0.1.2/jeeves_pr_stack/errors.py
--rw-r--r--   0        0        0     3336 2023-09-27 21:50:07.566641 jeeves_pr_stack-0.1.2/jeeves_pr_stack/format.py
--rw-r--r--   0        0        0     2739 2024-02-02 09:50:30.069016 jeeves_pr_stack-0.1.2/jeeves_pr_stack/github.py
--rw-r--r--   0        0        0     4449 2024-02-02 09:50:30.069016 jeeves_pr_stack-0.1.2/jeeves_pr_stack/logic.py
--rw-r--r--   0        0        0     1929 2023-09-27 21:50:07.566641 jeeves_pr_stack-0.1.2/jeeves_pr_stack/models.py
--rw-r--r--   0        0        0      715 2024-02-02 09:50:38.081066 jeeves_pr_stack-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 jeeves_pr_stack-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1866 2024-04-29 09:56:59.403006 jeeves_pr_stack-0.1.3/README.md
+-rw-r--r--   0        0        0       36 2024-04-29 09:56:59.403006 jeeves_pr_stack-0.1.3/jeeves_pr_stack/__init__.py
+-rw-r--r--   0        0        0     6932 2024-04-29 09:56:59.403006 jeeves_pr_stack-0.1.3/jeeves_pr_stack/app.py
+-rw-r--r--   0        0        0      606 2024-04-29 09:56:59.403006 jeeves_pr_stack-0.1.3/jeeves_pr_stack/errors.py
+-rw-r--r--   0        0        0     3336 2024-04-29 09:56:59.403006 jeeves_pr_stack-0.1.3/jeeves_pr_stack/format.py
+-rw-r--r--   0        0        0     2802 2024-04-29 10:13:24.068537 jeeves_pr_stack-0.1.3/jeeves_pr_stack/github.py
+-rw-r--r--   0        0        0     4449 2024-04-29 09:56:59.403006 jeeves_pr_stack-0.1.3/jeeves_pr_stack/logic.py
+-rw-r--r--   0        0        0     1929 2024-04-29 09:56:59.403006 jeeves_pr_stack-0.1.3/jeeves_pr_stack/models.py
+-rw-r--r--   0        0        0      715 2024-04-29 10:13:24.068537 jeeves_pr_stack-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 jeeves_pr_stack-0.1.3/PKG-INFO
```

### Comparing `jeeves_pr_stack-0.1.2/README.md` & `jeeves_pr_stack-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jeeves_pr_stack-0.1.2/jeeves_pr_stack/app.py` & `jeeves_pr_stack-0.1.3/jeeves_pr_stack/app.py`

 * *Files identical despite different names*

### Comparing `jeeves_pr_stack-0.1.2/jeeves_pr_stack/errors.py` & `jeeves_pr_stack-0.1.3/jeeves_pr_stack/errors.py`

 * *Files identical despite different names*

### Comparing `jeeves_pr_stack-0.1.2/jeeves_pr_stack/format.py` & `jeeves_pr_stack-0.1.3/jeeves_pr_stack/format.py`

 * *Files identical despite different names*

### Comparing `jeeves_pr_stack-0.1.2/jeeves_pr_stack/github.py` & `jeeves_pr_stack-0.1.3/jeeves_pr_stack/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
     # This one is not informative
     raw_status_values.discard('SUCCESS')
 
     # No idea what to do with this one
     raw_status_values.discard('NEUTRAL')
 
+    # We do not care
+    raw_status_values.discard('SKIPPED')
+
     try:
         raw_status_values.remove('')
     except KeyError:
         pass   # noqa: WPS420
     else:
         return ChecksStatus.RUNNING
```

### Comparing `jeeves_pr_stack-0.1.2/jeeves_pr_stack/logic.py` & `jeeves_pr_stack-0.1.3/jeeves_pr_stack/logic.py`

 * *Files identical despite different names*

### Comparing `jeeves_pr_stack-0.1.2/jeeves_pr_stack/models.py` & `jeeves_pr_stack-0.1.3/jeeves_pr_stack/models.py`

 * *Files identical despite different names*

### Comparing `jeeves_pr_stack-0.1.2/pyproject.toml` & `jeeves_pr_stack-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jeeves-pr-stack"
-version = "0.1.2"
+version = "0.1.3"
 description = "Manage GitHub Pull Request stacks."
 authors = ["Anatoly Scherbakov <altaisoft@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `jeeves_pr_stack-0.1.2/PKG-INFO` & `jeeves_pr_stack-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: jeeves-pr-stack
-Version: 0.1.2
+Version: 0.1.3
 Summary: Manage GitHub Pull Request stacks.
 License: MIT
 Author: Anatoly Scherbakov
 Author-email: altaisoft@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jeeves-shell[all] (>=2.3.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Description-Content-Type: text/markdown
 
 # `jeeves-pr-stack`
 
 `jeeves-pr-stack` is a plugin for [jeeves](https://jeeves.sh) that helps manage stacks of GitHub pull requests. It aims to simplify the code review process by organizing pull requests that depend on each other.
```

