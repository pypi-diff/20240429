# Comparing `tmp/git_gerrit_bridge-1.1.2.tar.gz` & `tmp/git_gerrit_bridge-1.2.0.tar.gz`

## Comparing `git_gerrit_bridge-1.1.2.tar` & `git_gerrit_bridge-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/__main__.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/checkout.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/clean.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/new.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/push.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/rebase.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/status.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/branch.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/change.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/changebase.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/gerrit.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/git.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/localchange.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/remotechange.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/version.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/README.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/__main__.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/cli/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/cli/checkout.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/cli/clean.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/cli/new.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/cli/push.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/cli/rebase.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/cli/status.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/cli/sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/branch.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/change.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/changebase.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/gerrit.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/git.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/localchange.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/remotechange.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/git_gerrit/utils/version.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/README.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.2.0/PKG-INFO
```

### Comparing `git_gerrit_bridge-1.1.2/.github/workflows/pypi-publish.yml` & `git_gerrit_bridge-1.2.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/cli/__init__.py` & `git_gerrit_bridge-1.2.0/git_gerrit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/cli/checkout.py` & `git_gerrit_bridge-1.2.0/git_gerrit/cli/checkout.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/cli/clean.py` & `git_gerrit_bridge-1.2.0/git_gerrit/cli/clean.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/cli/rebase.py` & `git_gerrit_bridge-1.2.0/git_gerrit/cli/rebase.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/cli/status.py` & `git_gerrit_bridge-1.2.0/git_gerrit/cli/status.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/cli/sync.py` & `git_gerrit_bridge-1.2.0/git_gerrit/cli/sync.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/utils/branch.py` & `git_gerrit_bridge-1.2.0/git_gerrit/utils/branch.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/utils/change.py` & `git_gerrit_bridge-1.2.0/git_gerrit/utils/change.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/utils/gerrit.py` & `git_gerrit_bridge-1.2.0/git_gerrit/utils/gerrit.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/utils/git.py` & `git_gerrit_bridge-1.2.0/git_gerrit/utils/git.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/utils/localchange.py` & `git_gerrit_bridge-1.2.0/git_gerrit/utils/localchange.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/utils/remotechange.py` & `git_gerrit_bridge-1.2.0/git_gerrit/utils/remotechange.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/git_gerrit/utils/version.py` & `git_gerrit_bridge-1.2.0/git_gerrit/utils/version.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/LICENSE.txt` & `git_gerrit_bridge-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/README.md` & `git_gerrit_bridge-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/pyproject.toml` & `git_gerrit_bridge-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.2/PKG-INFO` & `git_gerrit_bridge-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: git-gerrit-bridge
-Version: 1.1.2
+Version: 1.2.0
 Summary: Git subcommand to ease local branch management with gerrit.
 Project-URL: Documentation, https://github.com/Scheirle/git-gerrit-bridget#readme
 Project-URL: Issues, https://github.com/Scheirle/git-gerrit-bridge/issues
 Project-URL: Source, https://github.com/Scheirle/git-gerrit-bridge
 Author-email: Bernhard Scheirle <bernhard@scheirle.de>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.txt
```

