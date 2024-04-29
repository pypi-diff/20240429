# Comparing `tmp/across_burstcube-0.0.7.tar.gz` & `tmp/across_burstcube-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "across_burstcube-0.0.7.tar", last modified: Mon Apr 29 01:44:13 2024, max compression
+gzip compressed data, was "across_burstcube-0.4.tar", last modified: Fri Apr 19 18:58:37 2024, max compression
```

## Comparing `across_burstcube-0.0.7.tar` & `across_burstcube-0.4.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:13.214738 across_burstcube-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:13.210738 across_burstcube-0.0.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:13.210738 across_burstcube-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-29 01:44:13.214738 across_burstcube-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:13.214738 across_burstcube-0.0.7/across_burstcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-29 01:44:13.000000 across_burstcube-0.0.7/across_burstcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-29 01:44:13.000000 across_burstcube-0.0.7/across_burstcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 01:44:13.000000 across_burstcube-0.0.7/across_burstcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-29 01:44:13.000000 across_burstcube-0.0.7/across_burstcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 01:44:13.000000 across_burstcube-0.0.7/across_burstcube.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:13.210738 across_burstcube-0.0.7/across_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:13.210738 across_burstcube-0.0.7/across_client/across/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/across/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/across/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/across/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:13.210738 across_burstcube-0.0.7/across_client/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/base/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/base/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/base/daterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/base/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/base/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:13.210738 across_burstcube-0.0.7/across_client/burstcube/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/burstcube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/burstcube/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/burstcube/toorequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/across_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-29 01:44:02.000000 across_burstcube-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 01:44:13.214738 across_burstcube-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.469876 across_burstcube-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 18:58:32.000000 across_burstcube-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 18:58:32.000000 across_burstcube-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.469876 across_burstcube-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 18:58:32.000000 across_burstcube-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_burstcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/across/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/daterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/burstcube/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/fov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/toorequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 18:58:32.000000 across_burstcube-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:58:37.469876 across_burstcube-0.4/setup.cfg
```

### Comparing `across_burstcube-0.0.7/.github/ISSUE_TEMPLATE.md` & `across_burstcube-0.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.7/.github/PULL_REQUEST_TEMPLATE.md` & `across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.7/.github/workflows/deploy.yml` & `across_burstcube-0.4/.github/workflows/deploy.yml`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
       - name: Checkout the repository
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
           python-version: "3.11"
 
       - name: Git describe
         id: ghd
         uses: proudust/gh-describe@v2
 
@@ -30,15 +30,15 @@
           build
           --user
 
       - name: Build a binary wheel and a source tarball
         run: python3 -m build
 
       - name: Store the distribution packages
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
@@ -49,13 +49,13 @@
     environment:
       name: pypi
       url: https://pypi.org/p/across-burstcube  # Replace <package-name> with your PyPI project name
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v4
+        uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `across_burstcube-0.0.7/.github/workflows/pylint.yml` & `across_burstcube-0.4/.github/workflows/pylint.yml`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.9", "3.10", "3.11"]
     steps:
-    - uses: actions/checkout@v4
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v5
+      uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install flake8 mypy
     - name: Lint with flake8
```

### Comparing `across_burstcube-0.0.7/across_burstcube.egg-info/SOURCES.txt` & `across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,9 +21,11 @@
 across_client/base/__init__.py
 across_client/base/common.py
 across_client/base/coords.py
 across_client/base/daterange.py
 across_client/base/schema.py
 across_client/base/user.py
 across_client/burstcube/__init__.py
+across_client/burstcube/constants.py
+across_client/burstcube/fov.py
 across_client/burstcube/schema.py
 across_client/burstcube/toorequest.py
```

### Comparing `across_burstcube-0.0.7/across_client/base/common.py` & `across_burstcube-0.4/across_client/base/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,136 +1,36 @@
 import json
 import warnings
-from typing import Type
+from pathlib import PosixPath
+from typing import Any, Dict, Optional, Tuple, Type
 
 import requests
 
 from ..constants import API_URL
-from ..functions import _tablefy
-from .schema import BaseSchema, FileHolder
+from ..functions import tablefy
+from .schema import BaseSchema
 
 
 class ACROSSBase:
     """
-    Mixin class for ACROSS API classes that provides a representation
-    of the API data. Includes support for Jupyter notebooks.
+    Base class for ACROSS API Classes including common methods for all API classes.
     """
 
-    @property
-    def parameters(self) -> dict:
-        """
-        Return parameters as dict
-
-        Returns
-        -------
-        dict
-            Dictionary of parameters
-        """
-        if hasattr(self, "model_dump"):
-            return {k: v for k, v in self.model_dump().items() if v is not None}
-        else:
-            return {k: v for k, v in self.__dict__.items() if v is not None}
-
-    @property
-    def _table(self) -> tuple:
-        """
-        Table with head showing results of the API query.
-
-        Returns
-        -------
-        tuple
-            Tuple containing two lists, the header and the table data
-        """
-        if hasattr(self, "entries") and len(self.entries) > 0:
-            header = self.entries[0]._table[0]
-            table = [t._table[1][0] for t in self.entries]
-        else:
-            # Start with arguments
-            if hasattr(self, "_get_schema"):
-                _parameters = list(self.parameters.keys())
-            else:
-                _parameters = []
-            _parameters += list(self.parameters.keys())
-
-            _parameters
-            # Don't include api_token in table
-            try:
-                _parameters.pop(_parameters.index("api_token"))
-            except ValueError:
-                pass
-
-            # Removed repeated values
-            _parameters = list(set(_parameters))
-
-            header = [par for par in _parameters]
-            table = []
-            for row in _parameters:
-                value = getattr(self, row)
-                table.append(value)
-            table = [table]
-        return header, table
-
-    def _repr_html_(self) -> str:
-        """Return a HTML summary of the API data, for e.g. Jupyter.
-
-        Returns
-        -------
-        str
-            HTML summary of data
-        """
-        header, table = self._table
-
-        if len(table) > 0:
-            return _tablefy(table, header)
-        else:
-            return "No data"
-
-    def __repr__(self) -> str:
-        # print a string showing the API call and arguments with their values
-        # in a way that can be copied and pasted into a script
-        args = ",".join([f"{k}={v}" for k, v in self.parameters.items()])
-        return f"{self.__class__.__name__}({args})"
-
-
-class ACROSSEndPoint(ACROSSBase):
-    """
-    Base class for ACROSS API Classes including common methods for all API
-    endpoint classes.
-
-    Methods
-    -------
-    api_url(argdict)
-        URL for this API call.
-    get()
-        Perform a 'GET' submission to ACROSS API.
-    put()
-        Perform a 'PUT' submission to ACROSS API.
-    post()
-        Perform a 'POST' submission to ACROSS API.
-    delete()
-        Perform a 'DELETE' submission to ACROSS API.
-    validate_get()
-        Validate arguments for GET
-    validate_put()
-        Validate arguments for PUT
-    validate_post()
-        Validate arguments for POST
-    validate_del()
-        Validate arguments for DELETE
-
-    """
+    # Type hints
+    entries: list
 
     # API descriptors type hints
+    _schema: Type[BaseSchema]
     _get_schema: Type[BaseSchema]
     _put_schema: Type[BaseSchema]
     _post_schema: Type[BaseSchema]
     _del_schema: Type[BaseSchema]
 
     _mission: str
-    _api_name: str
+    _api_name: str = __name__
 
     def __getitem__(self, i):
         return self.entries[i]
 
     def api_url(self, argdict) -> str:
         """
         URL for this API call.
@@ -142,14 +42,51 @@
         """
         # If arguments has `id` in it, then put this in the path
         if "id" in argdict.keys() and argdict["id"] is not None:
             return f"{API_URL}{self._mission.lower()}/{self._api_name.lower()}/{argdict['id']}"
         return f"{API_URL}{self._mission.lower()}/{self._api_name.lower()}"
 
     @property
+    def schema(self) -> Any:
+        """Return pydantic schema for this API class
+
+        Returns
+        -------
+        object
+            Pydantic Schema
+        """
+        return self._schema.model_validate(self)
+
+    @property
+    def parameters(self) -> dict:
+        """
+        Return parameters as dict
+
+        Returns
+        -------
+        dict
+            Dictionary of parameters
+        """
+        return {k: v for k, v in self._schema.model_validate(self) if v is not None}
+
+    @parameters.setter
+    def parameters(self, params: dict):
+        """
+        Set API parameters from a given dict which is validated from self._schema
+
+        Parameters
+        ----------
+        params : dict
+            Dictionary of class parameters
+        """
+        for k, v in self._schema(**params):
+            if hasattr(self, k) and v is not None:
+                setattr(self, k, v)
+
+    @property
     def headers(self) -> dict:
         # If we have a api_token, then use this to authenticate
         if hasattr(self, "api_token"):
             headers = {"Authorization": f"Bearer {self.api_token}"}
         else:
             headers = {}
         return headers
@@ -168,31 +105,26 @@
         ------
         HTTPError
             Raised if GET doesn't return a 200 response.
         """
         if self.validate_get():
             # Create an array of parameters from the schema
             get_params = {
-                key: value
-                for key, value in self._get_schema.model_validate(self)
-                if key in self._get_schema.model_fields
+                key: value for key, value in self._get_schema.model_validate(self)
             }
-
             # Do the GET request
             req = requests.get(
                 self.api_url(get_params),
                 params=get_params,
                 headers=self.headers,
                 timeout=60,
             )
-
             if req.status_code == 200:
                 # Parse, validate and record values from returned API JSON
-                assert hasattr(self, "model_validate")
-                for k, v in self.model_validate(req.json()):
+                for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
             elif req.status_code == 404:
                 """Handle 404 errors gracefully, by issuing a warning"""
                 warnings.warn(req.json()["detail"])
             else:
                 # Raise an exception if the HTML response was not 200
@@ -224,24 +156,23 @@
                 self.api_url(del_params),
                 params=del_params,
                 headers=self.headers,
                 timeout=60,
             )
             if req.status_code == 200:
                 # Parse, validate and record values from returned API JSON
-                assert hasattr(self, "model_validate")
-                for k, v in self.model_validate(req.json()):
+                for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
             else:
                 # Raise an exception if the HTML response was not 200
                 req.raise_for_status()
         return False
 
-    def put(self) -> bool:
+    def put(self, payload={}) -> bool:
         """
         Perform a 'PUT' submission to ACROSS API. Used for pushing/replacing
         information.
 
         Returns
         -------
         bool
@@ -250,14 +181,30 @@
         Raises
         ------
         HTTPError
             Raised if PUT doesn't return a 201 response.
         """
 
         if self.validate_put():
+            # Extract any files out of the arguments
+            files: Dict[str, Tuple[Optional[str], Any, str]] = {
+                key.replace("filename", "file"): (
+                    # Return either the existing filelike object, or open the file
+                    value.name,
+                    (
+                        getattr(self, key.replace("filename", "file"))
+                        if hasattr(self, key.replace("filename", "file"))
+                        else value.open("rb")
+                    ),
+                    "application/octet-stream",
+                )
+                for key, value in self._put_schema.model_validate(self)
+                if type(value) is PosixPath
+            }
+
             # Extract all POST parameters from the schema
             all_params = self._put_schema.model_validate(self).model_dump(
                 mode="json", exclude_none=True
             )
 
             # Extract query parameters
             put_params = {
@@ -267,41 +214,33 @@
             }
 
             # URL for this API call
             api_url = self.api_url(put_params)
             if "id" in put_params.keys():
                 put_params.pop("id")  # Remove id from query parameters
 
-            # Add any files and json data to files
-            files = dict()
+            # Add any json data to files
             for k in all_params:
-                if isinstance(getattr(self, k), FileHolder):
-                    files[k] = getattr(self, k).upload_file_tuple
-                elif isinstance(all_params[k], dict):
+                if isinstance(all_params[k], dict):
                     files[k] = (None, json.dumps(all_params[k]), "application/json")
 
             # Submit request
             req = requests.put(
                 api_url,
                 params=put_params,
                 headers=self.headers,
                 files=files,
                 timeout=60,
             )
 
             if req.status_code == 201:
                 # Parse, validate and record values from returned API JSON
-                assert hasattr(self, "model_validate")
-                for k, v in self.model_validate(req.json()):
+                for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
-            elif req.status_code == 304:
-                # No changes made
-                warnings.warn("Update identical to values on server. No changes made.")
-                return False
             else:
                 print("ERROR: ", req.status_code, req.json())
                 req.raise_for_status()
         return False
 
     def post(self) -> bool:
         """
@@ -315,47 +254,77 @@
 
         Raises
         ------
         HTTPError
             Raised if POST doesn't return a 201 response.
         """
         if self.validate_post():
+            # Extract any files out of the arguments
+            files: Dict[str, Tuple[Optional[str], Any, str]] = {
+                key: (
+                    PosixPath(getattr(self, key + "name")).name
+                    if getattr(self, key) is not None
+                    else "healpix_file.fits",
+                    open(getattr(self, key + "name"), "rb"),
+                    "application/octet-stream",
+                )
+                if getattr(self, key) is None
+                and getattr(self, key + "name") is not None
+                else (
+                    PosixPath(getattr(self, key).name).name
+                    if getattr(self, key) is not None
+                    else None,
+                    getattr(self, key),
+                    "application/octet-stream",
+                )
+                for key, value in self._post_schema.model_validate(self)
+                if "_file" in key
+            }
+
+            # If files are gzipped, then set the content type to
+            # application/x-gzip
+            for key in files:
+                filename = files[key][0]
+                if isinstance(filename, str):
+                    if ".gz" in filename:
+                        files[key] = (
+                            files[key][0],
+                            files[key][1],
+                            "application/x-gzip",
+                        )
+
             # Extract all POST parameters from the schema
             all_params = self._post_schema.model_validate(self).model_dump(
                 mode="json", exclude_none=True
             )
 
             # Extract query parameters
             post_params = {
                 k: all_params[k]
                 for k in all_params
                 if not isinstance(all_params[k], dict)
             }
 
-            # Add any files and json data to files
-            files = dict()
+            # Add any json data to files
             for k in all_params:
-                if isinstance(getattr(self, k), FileHolder):
-                    files[k] = getattr(self, k).upload_file_tuple
-                elif isinstance(all_params[k], dict):
+                if isinstance(all_params[k], dict):
                     files[k] = (None, json.dumps(all_params[k]), "application/json")
-
             # Submit request
             req = requests.post(
                 self.api_url(post_params),
                 params=post_params,
                 headers=self.headers,
                 files=files,
                 timeout=60,
             )
 
             if req.status_code == 201:
                 # Parse, validate and record values from returned API JSON
-                assert hasattr(self, "model_validate")
-                for k, v in self.model_validate(req.json()):
+                print(req.json())
+                for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
             elif req.status_code == 200:
                 warnings.warn(req.json()["detail"])
                 return False
             else:
                 # Raise an exception if the HTML response was not 200
@@ -414,15 +383,14 @@
         Returns
         -------
         bool
             Is it validated? True | False
         """
         if hasattr(self, "_post_schema"):
             self._post_schema.model_validate(self.__dict__)
-            # self._post_schema.model_validate(self)
         else:
             warnings.warn("POST not allowed for this class.")
             return False
         return True
 
     def validate_del(self) -> bool:
         """Validate if value to be POST matches Schema
@@ -434,7 +402,65 @@
         """
         if hasattr(self, "_del_schema"):
             self._del_schema.model_validate(self.__dict__)
         else:
             warnings.warn("DELETE not allowed for this class.")
             return False
         return True
+
+    @property
+    def _table(self) -> tuple:
+        """
+        Table with head showing results of the API query.
+
+        Returns
+        -------
+        tuple
+            Tuple containing two lists, the header and the table data
+        """
+        if hasattr(self, "entries") and len(self.entries) > 0:
+            header = self.entries[0]._table[0]
+            table = [t._table[1][0] for t in self.entries]
+        else:
+            # Start with arguments
+            if hasattr(self, "_get_schema"):
+                _parameters = list(self.parameters.keys())
+            else:
+                _parameters = []
+            _parameters += list(self.parameters.keys())
+            # Don't include client_id/client_secret in table
+            try:
+                _parameters.pop(_parameters.index("client_id"))
+                _parameters.pop(_parameters.index("client_secret"))
+            except ValueError:
+                pass
+
+            # Removed repeated values
+            _parameters = list(set(_parameters))
+
+            header = [par for par in _parameters]
+            table = []
+            for row in _parameters:
+                value = getattr(self, row)
+                table.append(value)
+            table = [table]
+        return header, table
+
+    def _repr_html_(self) -> str:
+        """Return a HTML summary of the API data, for e.g. Jupyter.
+
+        Returns
+        -------
+        str
+            HTML summary of data
+        """
+        header, table = self._table
+        if len(table) > 0:
+            return tablefy(table, header)
+        else:
+            return "No data"
+
+    def __repr__(self) -> str:
+        # print a string showing the API call and arguments with their values
+        # in a way that can be copied and pasted into a script
+        args = ",".join([f"{k}={v}" for k, v in self.parameters.items()])
+        return f"{self.__class__.__name__}({args})"
```

### Comparing `across_burstcube-0.0.7/across_client/base/coords.py` & `across_burstcube-0.4/across_client/base/coords.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     if type(coord) is Longitude or type(coord) is Latitude:
         return coord.value
     # Universal translator
     return float(coord)
 
 
 class ACROSSSkyCoord:
+    ra: float
+    dec: float
+
     @property
     def skycoord(self) -> SkyCoord:
         """Returns a string representation of the skycoord."""
         if self.ra is None or self.dec is None:
             return None
         else:
             return SkyCoord(self.ra, self.dec, unit="deg")
```

### Comparing `across_burstcube-0.0.7/across_client/base/daterange.py` & `across_burstcube-0.4/across_client/base/daterange.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.7/across_client/burstcube/schema.py` & `across_burstcube-0.4/across_client/burstcube/schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from datetime import datetime
 from enum import Enum
-from typing import Any, Optional
+from io import IOBase
+from typing import List, Optional
 
-from pydantic import ConfigDict, model_validator
+from pydantic import ConfigDict  # type: ignore
 
-from ..base.common import ACROSSBase
-from ..base.schema import (
-    BaseSchema,
-    FileHolder,
-    OptionalDateRangeSchema,
-    OptionalPositionSchema,
-)
+from ..base.schema import BaseSchema, OptionalDateRangeSchema, OptionalPositionSchema
 
 
 class TOOReason(str, Enum):
     """
     Reasons for rejecting TOO observations
 
     Attributes
@@ -68,49 +63,51 @@
     declined = "Declined"
     approved = "Approved"
     executed = "Executed"
     deleted = "Deleted"
     other = "Other"
 
 
-class BurstCubeTriggerInfo(BaseSchema, ACROSSBase):
+class BurstCubeTriggerInfo(BaseSchema):
     """
     Metadata schema for the BurstCube Target of Opportunity (TOO) request. Note
     that this schema is not strictly defined, keys are only suggested, and
     additional keys can be added as needed.
-
-    Attributes
-    ----------
-    trigger_name : Optional[str]
-        The name of the trigger.
-    trigger_mission : Optional[str]
-        The mission that triggered the TOO request.
-    trigger_instrument : Optional[str]
-        The instrument that triggered the TOO request.
-    trigger_id : Optional[str]
-        The ID of the trigger.
-    trigger_duration : Optional[float]
-        The duration of the trigger.
-    classification : Optional[str]
-        The classification of the trigger.
-    justification : Optional[str]
-        Textual justification for the TOO request.
     """
 
     trigger_name: Optional[str] = None
     trigger_mission: Optional[str] = None
     trigger_instrument: Optional[str] = None
     trigger_id: Optional[str] = None
     trigger_duration: Optional[float] = None
     classification: Optional[str] = None
     justification: Optional[str] = None
 
     model_config = ConfigDict(extra="allow")
 
 
+class BurstCubeTOOSchema(OptionalPositionSchema):
+    """
+    Schema describing a BurstCube TOO Request.
+    """
+
+    id: Optional[int] = None
+    created_by: str
+    created_on: datetime
+    modified_by: Optional[str] = None
+    modified_on: Optional[datetime] = None
+    trigger_time: datetime
+    trigger_info: BurstCubeTriggerInfo
+    exposure: int
+    offset: int
+    reject_reason: TOOReason = TOOReason.none
+    status: TOOStatus = TOOStatus.requested
+    too_info: str = ""
+
+
 class BurstCubeTOODelSchema(BaseSchema):
     """
     Schema for BurstCubeTOO DELETE API call.
 
     Attributes
     ----------
     id
@@ -125,34 +122,15 @@
     Schema to submit a TOO request for BurstCube.
     """
 
     trigger_time: datetime
     trigger_info: BurstCubeTriggerInfo
     exposure: int = 200
     offset: int = -50
-    healpix_file: Optional[FileHolder] = None
-
-    @model_validator(mode="before")
-    @classmethod
-    def check_filename(cls, data: Any) -> Any:
-        if isinstance(data, dict):
-            if data["healpix_file"] is None and data["healpix_filename"] is not None:
-                data["healpix_file"] = FileHolder(filename=data["healpix_filename"])
-            elif (
-                data["healpix_file"] is not None
-                and data["healpix_filename"] is not None
-            ):
-                data["healpix_file"].filename = data["healpix_filename"]
-        else:
-            if data.healpix_file is None and data.healpix_filename is not None:
-                data.healpix_file = FileHolder(filename=data.healpix_filename)
-            elif data.healpix_file is not None and data.healpix_filename is not None:
-                data.healpix_file.filename = data.healpix_filename
-
-        return data
+    healpix_file: Optional[IOBase] = None
 
 
 class BurstCubeTOOGetSchema(BaseSchema):
     """
     Schema for BurstCubeTOO GET request.
     """
 
@@ -166,18 +144,26 @@
 
     id: int
     trigger_time: datetime
     trigger_info: BurstCubeTriggerInfo
     exposure: int = 200
     offset: int = -50
     status: TOOStatus
-    healpix_file: Optional[FileHolder] = None
+    healpix_file: Optional[IOBase] = None
 
 
 class BurstCubeTOORequestsGetSchema(OptionalDateRangeSchema):
     """
     Schema for GET requests to retrieve BurstCube Target of Opportunity (TOO) requests.
     """
 
     duration: Optional[float] = None
     limit: Optional[int] = None
     offset: Optional[int] = None
+
+
+class BurstCubeTOORequestsSchema(BaseSchema):
+    """
+    Schema for BurstCube TOO requests.
+    """
+
+    entries: List[BurstCubeTOOSchema]
```

### Comparing `across_burstcube-0.0.7/across_client/functions.py` & `across_burstcube-0.4/across_client/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import re
 import warnings
-from datetime import date, datetime, timezone
+from datetime import date, datetime, timedelta, timezone
 from typing import Optional, Union
 
+import astropy.units as u  # type: ignore
 import numpy as np
-from astropy.time import Time  # type: ignore
+from astropy.time import Time, TimeDelta  # type: ignore
+from astropy.units import Quantity
 from dateutil import parser
 
 
-def _tablefy(table: list, header: Optional[list] = None) -> str:
+def tablefy(table: list, header: Optional[list] = None) -> str:
     """Simple HTML table generator
 
     Parameters
     ----------
     table : list
         Data for table
     header : list, optional
@@ -44,15 +46,58 @@
 
 # Regex for matching date, time and datetime strings
 DATE_REGEX = r"^[0-2]\d{3}-(0?[1-9]|1[012])-([0][1-9]|[1-2][0-9]|3[0-1])?$"
 ISO8601_REGEX = r"^([\+-]?\d{4}(?!\d{2}\b))((-?)((0[1-9]|1[0-2])(\3([12]\d|0[1-9]|3[01]))?|W([0-4]\d|5[0-2])(-?[1-7])?|(00[1-9]|0[1-9]\d|[12]\d{2}|3([0-5]\d|6[1-6])))([T\s]((([01]\d|2[0-3])((:?)[0-5]\d)?|24\:?00)([\.,]\d+(?!:))?)?(\17[0-5]\d([\.,]\d+)?)?([zZ]|([\+-])([01]\d|2[0-3]):?([0-5]\d)?)?)?)?$"
 DATETIME_REGEX = r"^[0-2]\d{3}-(0?[1-9]|1[012])-([0][1-9]|[1-2][0-9]|3[0-1])[\sT]([0-9]:|[0-1][0-9]:|2[0-3]:)[0-5][0-9]:[0-5][0-9]+(\.\d+)?$"
 
 
-def _convert_to_dt(value: Union[str, date, datetime, Time]) -> Optional[datetime]:
+def convert_timedelta(
+    length: Union[str, float, timedelta, TimeDelta, Quantity, None], units=u.day
+) -> timedelta:
+    """Convert various timedelta formats to swiftdatetime or datetime
+
+    Parameters
+    ----------
+    length : Union[str, float, timedelta, TimeDelta, Quantity, None]
+        Value to be converted.
+    units : astropy.units.Quantity, optional
+        Unit to use if float/int given. Default is days.
+
+    Returns
+    -------
+    datetime.timedelta
+        Returned timedelta object.
+
+    Raises
+    ------
+    TypeError
+        Raised if incorrect format is given for conversion.
+    """
+
+    if units == u.day:
+        divisor = 86400.0
+    else:
+        divisor = 1.0
+    if type(length) is Quantity:
+        length = length.to(u.day).value
+    elif type(length) is timedelta:
+        length = length.total_seconds() / divisor
+    elif type(length) is TimeDelta:
+        length = length.to_datetime().total_seconds() / divisor  # type: ignore
+    else:
+        try:
+            length = float(length)  # type: ignore
+        except ValueError:
+            raise TypeError(
+                f"Length of time should be given as a datetime.timedelta, astropy TimeDelta, astropy quantity or as a number of {units}"
+            )
+    return timedelta(days=length)  # type: ignore
+
+
+def convert_to_dt(value: Union[str, date, datetime, Time]) -> Optional[datetime]:
     """Convert various date formats to datetime
 
     Parameters
     ----------
     value : Union[str, date, datetime, Time]
         Value to be converted.
```

