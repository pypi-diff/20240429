# Comparing `tmp/coveralls-3.4.0a1.tar.gz` & `tmp/coveralls-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveralls-3.4.0a1.tar", max compression
+gzip compressed data, was "coveralls-4.0.0.tar", max compression
```

## Comparing `coveralls-3.4.0a1.tar` & `coveralls-4.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1080 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/LICENSE.rst
--rw-r--r--   0        0        0     3880 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/README.rst
--rw-r--r--   0        0        0      134 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/__init__.py
--rw-r--r--   0        0        0       62 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/__main__.py
--rw-r--r--   0        0        0    16232 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/api.py
--rw-r--r--   0        0        0     3434 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/cli.py
--rw-r--r--   0        0        0      336 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/exception.py
--rw-r--r--   0        0        0     4086 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/git.py
--rw-r--r--   0        0        0     7466 2024-04-26 16:43:14.938078 coveralls-3.4.0a1/coveralls/reporter.py
--rw-r--r--   0        0        0     1689 2024-04-26 16:43:14.942078 coveralls-3.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     5317 1970-01-01 00:00:00.000000 coveralls-3.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-29 14:26:08.785074 coveralls-4.0.0/LICENSE.rst
+-rw-r--r--   0        0        0     3880 2024-04-29 14:26:08.785074 coveralls-4.0.0/README.rst
+-rw-r--r--   0        0        0      134 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/__main__.py
+-rw-r--r--   0        0        0    16403 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/api.py
+-rw-r--r--   0        0        0     3434 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/cli.py
+-rw-r--r--   0        0        0      336 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/exception.py
+-rw-r--r--   0        0        0     4086 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/git.py
+-rw-r--r--   0        0        0     4367 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/reporter.py
+-rw-r--r--   0        0        0     1720 2024-04-29 14:26:08.789074 coveralls-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 coveralls-4.0.0/PKG-INFO
```

### Comparing `coveralls-3.4.0a1/LICENSE.rst` & `coveralls-4.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `coveralls-3.4.0a1/README.rst` & `coveralls-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `coveralls-3.4.0a1/coveralls/api.py` & `coveralls-4.0.0/coveralls/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import codecs
 import json
 import logging
 import os
-import random
 import re
-import sys
 
 import coverage
 import requests
 
 from .exception import CoverallsException
 from .git import git_info
 from .reporter import CoverallReporter
@@ -103,27 +101,42 @@
             or os.environ.get('CIRCLE_BUILD_NUM')
         )
         pr = (os.environ.get('CI_PULL_REQUEST') or '').split('/')[-1] or None
         job = os.environ.get('CIRCLE_NODE_INDEX')
         return 'circleci', job, number, pr
 
     def load_config_from_github(self):
+        # See https://github.com/lemurheavy/coveralls-public/issues/1710
+
         # Github tokens and standard Coveralls tokens are almost but not quite
         # the same -- forceibly using Github's flow seems to be more stable
         self.config['repo_token'] = os.environ.get('GITHUB_TOKEN')
 
         pr = None
         if os.environ.get('GITHUB_REF', '').startswith('refs/pull/'):
             pr = os.environ.get('GITHUB_REF', '//').split('/')[2]
 
-        # N.B. some users require this to be 'github' and some require it to
-        # be 'github-actions'. Defaulting to 'github-actions' as it seems more
-        # common -- users can specify the service name manually to override
-        # this.
-        return 'github-actions', None, os.environ.get('GITHUB_RUN_ID'), pr
+        # TODO: coveralls suggests using the RUN_ID for both these values:
+        # https://github.com/lemurheavy/coveralls-public/issues/1710#issuecomment-1539203555
+        # However, they also suggest following this successful config approach:
+        # https://github.com/lemurheavy/coveralls-public/issues/1710#issuecomment-1913696022
+        # which instead sets:
+        # COVERALLS_SERVICE_JOB_ID: $GITHUB_RUN_ID
+        # COVERALLS_SERVICE_NUMBER: $GITHUB_WORKFLOW-$GITHUB_RUN_NUMBER
+        # should we do the same?
+        job = os.environ.get('GITHUB_RUN_ID')
+        number = os.environ.get('GITHUB_RUN_ID')
+
+        # N.B. per Coveralls:
+        # > When you want to identify the repo at Coveralls by its
+        # > GITHUB_TOKEN, you should choose github, and when you want to
+        # > identify it by its Coveralls Repo Token, you should choose
+        # > github-action.
+        # https://github.com/lemurheavy/coveralls-public/issues/1710#issuecomment-1539203555
+        return 'github', job, number, pr
 
     @staticmethod
     def load_config_from_jenkins():
         pr = os.environ.get('CI_PULL_REQUEST', '').split('/')[-1] or None
         return 'jenkins', os.environ.get('BUILD_NUMBER'), None, pr
 
     @staticmethod
@@ -185,17 +198,14 @@
         if os.environ.get('APPVEYOR'):
             name, job, number, pr = self.load_config_from_appveyor()
         elif os.environ.get('BUILDKITE'):
             name, job, number, pr = self.load_config_from_buildkite()
         elif os.environ.get('CIRCLECI'):
             name, job, number, pr = self.load_config_from_circle()
         elif os.environ.get('GITHUB_ACTIONS'):
-            # N.B. Github Actions fails if this is not set even when null.
-            # Other services fail if this is set to null. Sigh.
-            self.config['service_job_id'] = None
             name, job, number, pr = self.load_config_from_github()
         elif os.environ.get('JENKINS_HOME'):
             name, job, number, pr = self.load_config_from_jenkins()
         elif os.environ.get('TRAVIS'):
             self._token_required = False
             name, job, number, pr = self.load_config_from_travis()
         elif os.environ.get('SEMAPHORE'):
@@ -267,40 +277,26 @@
     def submit_report(self, json_string):
         endpoint = f'{self._coveralls_host.rstrip("/")}/api/v1/jobs'
         verify = not bool(os.environ.get('COVERALLS_SKIP_SSL_VERIFY'))
         response = requests.post(
             endpoint, files={'json_file': json_string}, verify=verify,
         )
 
-        # check and adjust/resubmit if submission looks like it failed due to
-        # resubmission (non-unique)
         if response.status_code == 422:
-            # attach a random value to ensure uniqueness
-            # TODO: an auto-incrementing integer might be easier to reason
-            # about if we could fetch the previous value
-            # N.B. Github Actions fails if this is not set to null.
-            # Other services fail if this is set to null. Sigh x2.
-            if os.environ.get('GITHUB_REPOSITORY'):
-                new_id = None
-            else:
-                new_id = '-'.join((
-                    self.config.get('service_job_id', '42'),
-                    str(random.randint(0, sys.maxsize)),
-                ))
-            print(f'resubmitting with id {new_id}')
-
-            self.config['service_job_id'] = new_id
-            self._data = None  # force create_report to use updated data
-            json_string = self.create_report()
-
-            response = requests.post(
-                endpoint,
-                files={'json_file': json_string},
-                verify=verify,
-            )
+            if self.config['service_name'].startswith('github'):
+                print(
+                    'Received 422 submitting job via Github Actions. By '
+                    'default, coveralls-python uses the "github" service '
+                    'name, which requires you to set the $GITHUB_TOKEN '
+                    'environment variable. If you want to use a '
+                    'COVERALLS_REPO_TOKEN instead, please manually override '
+                    '$COVERALLS_SERVICE_NAME to "github-actions". For more '
+                    'info, see https://coveralls-python.readthedocs.io/en'
+                    '/latest/usage/configuration.html#github-actions-support',
+                )
 
         try:
             response.raise_for_status()
             data = response.json()
         except Exception as e:
             raise CoverallsException(
                 f'Could not submit coverage: {e}',
```

### Comparing `coveralls-3.4.0a1/coveralls/cli.py` & `coveralls-4.0.0/coveralls/cli.py`

 * *Files identical despite different names*

### Comparing `coveralls-3.4.0a1/coveralls/git.py` & `coveralls-4.0.0/coveralls/git.py`

 * *Files identical despite different names*

### Comparing `coveralls-3.4.0a1/pyproject.toml` & `coveralls-4.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveralls"
-version = "3.4.0a1"
+version = "4.0.0"
 description = "Show coverage stats online via coveralls.io"
 readme = "README.rst"
 
 repository = "http://github.com/TheKevJames/coveralls-python"
 authors = ["Kevin James <coveralls-python@thekev.in>"]
 license = "MIT"
 
@@ -28,22 +28,22 @@
 
 [tool.poetry.scripts]
 coveralls = "coveralls.cli:main"
 python-coveralls = "coveralls.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
-coverage = ">=5.0,<7.5,!=6.0.*,!=6.1,!=6.1.1"
+coverage = { version = ">=5.0,<7.5,!=6.0.*,!=6.1,!=6.1.1", extras = ["toml"] }
 docopt = ">=0.6.1,<0.7.0"
 requests = ">=1.0.0,<3.0.0"
 
 pyyaml = { version = ">=3.10,<7.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
-pytest = "8.1.1"
+pytest = "8.2.0"
 responses = "0.25.0"
 
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "7.3.7", python = ">=3.9" }
```

### Comparing `coveralls-3.4.0a1/PKG-INFO` & `coveralls-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveralls
-Version: 3.4.0a1
+Version: 4.0.0
 Summary: Show coverage stats online via coveralls.io
 Home-page: http://github.com/TheKevJames/coveralls-python
 License: MIT
 Author: Kevin James
 Author-email: coveralls-python@thekev.in
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: yaml
-Requires-Dist: coverage (>=5.0,<7.5,!=6.0.*,!=6.1,!=6.1.1)
+Requires-Dist: coverage[toml] (>=5.0,<7.5,!=6.0.*,!=6.1,!=6.1.1)
 Requires-Dist: docopt (>=0.6.1,<0.7.0)
 Requires-Dist: pyyaml (>=3.10,<7.0) ; extra == "yaml"
 Requires-Dist: requests (>=1.0.0,<3.0.0)
 Project-URL: Changelog, https://github.com/TheKevJames/coveralls-python/blob/master/CHANGELOG.md
 Project-URL: Docs, https://coveralls-python.rtfd.io/
 Project-URL: Repository, http://github.com/TheKevJames/coveralls-python
 Description-Content-Type: text/x-rst
```

