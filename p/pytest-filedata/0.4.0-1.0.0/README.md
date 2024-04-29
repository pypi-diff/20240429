# Comparing `tmp/pytest_filedata-0.4.0.tar.gz` & `tmp/pytest_filedata-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest_filedata-0.4.0.tar", last modified: Thu Jan 17 21:49:31 2019, max compression
+gzip compressed data, was "pytest_filedata-1.0.0.tar", max compression
```

## Comparing `pytest_filedata-0.4.0.tar` & `pytest_filedata-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,5 @@
-drwxrwxr-x   0 grizz    (699600003) grizz    (699600003)        0 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/
-drwxrwxr-x   0 grizz    (699600003) grizz    (699600003)        0 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/pytest_filedata.egg-info/
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)        1 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/pytest_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)       39 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/pytest_filedata.egg-info/entry_points.txt
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)       54 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/pytest_filedata.egg-info/requires.txt
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)       16 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/pytest_filedata.egg-info/top_level.txt
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)      546 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/pytest_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)        1 2018-01-01 03:03:25.000000 pytest_filedata-0.4.0/pytest_filedata.egg-info/zip-safe
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)     3286 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/pytest_filedata.egg-info/PKG-INFO
-drwxrwxr-x   0 grizz    (699600003) grizz    (699600003)        0 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/Ctl/
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)        5 2019-01-17 21:49:19.000000 pytest_filedata-0.4.0/Ctl/VERSION
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)       57 2019-01-17 21:29:20.000000 pytest_filedata-0.4.0/Ctl/requirements.txt
-drwxrwxr-x   0 grizz    (699600003) grizz    (699600003)        0 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/Ctl/tmp/
-drwxrwxr-x   0 grizz    (699600003) grizz    (699600003)        0 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/Ctl/tmp/git@github.com:20c/
-drwxrwxr-x   0 grizz    (699600003) grizz    (699600003)        0 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/Ctl/tmp/git@github.com:20c/pytest-filedata.git/
-drwxrwxr-x   0 grizz    (699600003) grizz    (699600003)        0 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/Ctl/tmp/git@github.com:20c/pytest-filedata.git/Ctl/
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)       57 2019-01-17 21:48:22.000000 pytest_filedata-0.4.0/Ctl/tmp/git@github.com:20c/pytest-filedata.git/Ctl/requirements.txt
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)       64 2019-01-17 21:48:22.000000 pytest_filedata-0.4.0/Ctl/tmp/git@github.com:20c/pytest-filedata.git/Ctl/requirements-test.txt
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)       64 2019-01-17 21:29:20.000000 pytest_filedata-0.4.0/Ctl/requirements-test.txt
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)      103 2019-01-17 21:38:34.000000 pytest_filedata-0.4.0/MANIFEST.in
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)      102 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/setup.cfg
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)     1517 2019-01-17 21:41:01.000000 pytest_filedata-0.4.0/setup.py
-drwxrwxr-x   0 grizz    (699600003) grizz    (699600003)        0 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/pytest_filedata/
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)     4403 2019-01-17 21:11:21.000000 pytest_filedata-0.4.0/pytest_filedata/__init__.py
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)     2020 2019-01-17 21:16:30.000000 pytest_filedata-0.4.0/README.md
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)     3286 2019-01-17 21:49:31.000000 pytest_filedata-0.4.0/PKG-INFO
--rw-rw-r--   0 grizz    (699600003) grizz    (699600003)    11358 2017-12-31 23:54:30.000000 pytest_filedata-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11358 2024-04-29 00:45:14.990386 pytest_filedata-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1872 2024-04-29 01:48:14.493049 pytest_filedata-1.0.0/README.md
+-rw-r--r--   0        0        0     1254 2024-04-29 01:53:51.401484 pytest_filedata-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4237 2024-04-29 01:48:14.496049 pytest_filedata-1.0.0/pytest_filedata/__init__.py
+-rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 pytest_filedata-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest_filedata-0.4.0/pytest_filedata/__init__.py` & `pytest_filedata-1.0.0/pytest_filedata/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-
-from future import standard_library
-standard_library.install_aliases()
-from builtins import map
-from builtins import object
 import collections
 from datetime import datetime
 import json
 import os
 import urllib.parse
 
 import requests_mock
@@ -22,25 +17,24 @@
     """
     global test_dir
     test_dir = base_dir
 
 
 def json_hook(data):
     date_keys = (
-        'last_change',
-        'last_reboot',
-        'last_reconfiguration',
-        )
+        "last_change",
+        "last_reboot",
+        "last_reconfiguration",
+    )
     for key in date_keys:
         if key in data:
             data[key] = datetime.strptime(data[key], "%Y-%m-%dT%H:%M:%S")
     return data
 
 
-
 class JSONEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, datetime):
             return o.isoformat()
 
         return json.JSONEncoder.default(self, o)
 
@@ -53,28 +47,29 @@
     return json.load(fobj, object_hook=json_hook)
 
 
 def loads(data):
     return json.loads(data, object_hook=json_hook)
 
 
-class FileTestData(object):
-    """ object to hold file test data """
+class FileTestData:
+    """object to hold file test data"""
+
     def __init__(self, inp=None, exp=None, name=None, path=None):
         self.input = inp
         self.expected = exp
         self.name = name
         self.path = path
 
     def dumps(self, data):
-        """ dump data in configured output method """
+        """dump data in configured output method"""
         return dumps(data)
 
     def loads(self, data):
-        """ load data in configured output method """
+        """load data in configured output method"""
         return loads(data)
 
 
 def get_test_files(dirname):
     """
     Gets a list of files in directory specified by name.
     """
@@ -85,73 +80,74 @@
 
 
 def get_data(name):
     """
     Gets data from fixture name.
     """
     data = collections.OrderedDict()
-    dirname = os.path.join(test_dir, *name.split('_'))
+    dirname = os.path.join(test_dir, *name.split("_"))
 
     if not os.path.isdir(dirname):
-        raise ValueError("data directory '{}' does not exist".format(dirname))
+        raise ValueError(f"data directory '{dirname}' does not exist")
 
     for each in get_test_files(dirname):
         if os.path.isdir(each):
             continue
 
         fname = os.path.basename(each)
-        if fname.startswith('.'):
+        if fname.startswith("."):
             continue
 
         test_name, ext = os.path.splitext(fname)
         data.setdefault(test_name, FileTestData(name=test_name, path=dirname))
 
         # could setattr
         attr = ext[1:]
-        if ext == '.expected':
+        if ext == ".expected":
             with open(each) as fobj:
                 data[test_name].expected = json.load(fobj, object_hook=json_hook)
         else:
             with open(each) as fobj:
                 setattr(data[test_name], attr, fobj.read())
 
     return data
 
 
-class RequestsData(object):
+class RequestsData:
     """
     class to use test data from requests
     """
+
     def __init__(self, prefix, real_http=False):
         self.prefix = prefix
         adapter = requests_mock.Adapter()
         adapter.register_uri(requests_mock.ANY, requests_mock.ANY, text=self.callback)
         self.mocker = requests_mock.Mocker(adapter=adapter, real_http=real_http)
 
     def callback(self, request, context):
         path = urllib.parse.urlparse(request.url).path
-        path = os.path.join(test_dir, 'data', self.prefix, path.lstrip('/'))
+        path = os.path.join(test_dir, "data", self.prefix, path.lstrip("/"))
 
         files = get_test_files(path)
 
         if len(files) > 1:
             raise NotImplementedError("Currently there must be only one response file")
 
         if len(files) == 0:
             # dir not found, check for file.input
-            fname = path + '.input'
+            fname = path + ".input"
             if not os.path.exists(fname):
-                raise ValueError("failed to find data for {}".format(path))
+                raise ValueError(f"failed to find data for {path}")
 
         else:
             fname = files[0]
 
         try:
             # file extension is status code
-            context.status_code = int(os.path.splitext(fname)[1].lstrip('.'))
+            context.status_code = int(os.path.splitext(fname)[1].lstrip("."))
 
         except ValueError:
             context.status_code = 200
 
         with open(fname) as fobj:
             return fobj.read()
```

### Comparing `pytest_filedata-0.4.0/README.md` & `pytest_filedata-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 # pytest filedata
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-filedata.svg?maxAge=3600)](https://pypi.python.org/pypi/pytest-filedata)
 [![PyPI](https://img.shields.io/pypi/pyversions/pytest-filedata.svg?maxAge=3600)](https://pypi.python.org/pypi/pytest-filedata)
 [![Travis CI](https://img.shields.io/travis/20c/pytest-filedata.svg?maxAge=3600)](https://travis-ci.org/20c/pytest-filedata)
 [![Code Health](https://landscape.io/github/20c/pytest-filedata/master/landscape.svg?style=flat)](https://landscape.io/github/20c/pytest-filedata/master)
 [![Codecov](https://img.shields.io/codecov/c/github/20c/pytest-filedata/master.svg?maxAge=3600)](https://codecov.io/github/20c/pytest-filedata)
-[![Requires.io](https://img.shields.io/requires/github/20c/pytest-filedata.svg?maxAge=3600)](https://requires.io/github/20c/pytest-filedata/requirements)
 
-easily load test data from files
+Easily load test data from files
 
 ### Introduction
 
 This was created to save the tediousness of working with sets of data for
 testing inside the test files.
 
 ### Installing
@@ -37,18 +36,18 @@
             data = pytest_filedata.get_data(fixture)
             metafunc.parametrize(fixture, list(data.values()), ids=list(data.keys()))
 ```
 
 
 ### License
 
-Copyright 2016 20C, LLC
+Copyright 2016-2024 20C, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this softare except in compliance with the License.
+you may not use this software except in compliance with the License.
 You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `pytest_filedata-0.4.0/LICENSE` & `pytest_filedata-1.0.0/LICENSE`

 * *Files identical despite different names*

