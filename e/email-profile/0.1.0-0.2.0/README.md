# Comparing `tmp/email_profile-0.1.0.tar.gz` & `tmp/email_profile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_profile-0.1.0.tar", last modified: Mon Apr 22 04:00:29 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `email_profile-0.1.0.tar` & `email_profile-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:00:29.216956 email_profile-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-22 04:00:25.000000 email_profile-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-22 04:00:29.216956 email_profile-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-22 04:00:25.000000 email_profile-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:00:29.216956 email_profile-0.1.0/email_profile/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-22 04:00:25.000000 email_profile-0.1.0/email_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 04:00:25.000000 email_profile-0.1.0/email_profile/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:00:29.216956 email_profile-0.1.0/email_profile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-22 04:00:29.000000 email_profile-0.1.0/email_profile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-22 04:00:29.000000 email_profile-0.1.0/email_profile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 04:00:29.000000 email_profile-0.1.0/email_profile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 04:00:29.000000 email_profile-0.1.0/email_profile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 04:00:29.000000 email_profile-0.1.0/email_profile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 04:00:29.000000 email_profile-0.1.0/email_profile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 04:00:29.216956 email_profile-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1710 2024-04-22 04:00:25.000000 email_profile-0.1.0/setup.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 email_profile-0.2.0/.env-example
+-rw-r--r--   0        0        0    52850 2020-02-02 00:00:00.000000 email_profile-0.2.0/_poetry.lock
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 email_profile-0.2.0/_pyproject-poetry.toml
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 email_profile-0.2.0/example.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 email_profile-0.2.0/requirements-dev.txt
+-rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 email_profile-0.2.0/setup.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 email_profile-0.2.0/tox.ini
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 email_profile-0.2.0/.github/workflows/python-app-code-quality.yml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 email_profile-0.2.0/.github/workflows/python-app-test.yml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 email_profile-0.2.0/.github/workflows/python-publish-pypi-test.yml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 email_profile-0.2.0/.github/workflows/python-publish-pypi.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/cli.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/core.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/data.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/message.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/utils.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/where.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/config/__init__.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/config/controller.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/config/database.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/models/__init__.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/models/attachment.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/models/email.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/models/mailbox.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/serializers/__init__.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 email_profile-0.2.0/email_profile/serializers/where.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/test_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/test_message.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/serializers/__init__.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/serializers/test_where.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/utils/__init__.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/utils/test_mailbox.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/utils/test_mode.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 email_profile-0.2.0/tests/email_profile/utils/test_status.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 email_profile-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 email_profile-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 email_profile-0.2.0/README.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 email_profile-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 email_profile-0.2.0/PKG-INFO
```

### Comparing `email_profile-0.1.0/LICENSE` & `email_profile-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `email_profile-0.1.0/email_profile/__init__.py` & `email_profile-0.2.0/email_profile/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 __author__ = 'Fernando Celmer <email@fernandocelmer.com>'
 __copyright__ = """MIT License
 
 Copyright (c) 2024 Email Profile
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -18,7 +18,11 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE."""
+
+from email_profile.core import Email
+
+__all__ = ['Email']
```

### Comparing `email_profile-0.1.0/setup.py` & `email_profile-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     version=__version__,
     author="Fernando Celmer",
     author_email="email@fernandocelmer.com",
     description="📩 Email Profile",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls = {
-    'Homepage': 'https://github.com/linux-profile/email-profile',
-    'Repository': 'https://github.com/linux-profile/email-profile',
-    'Documentation': 'https://github.com/linux-profile/email-profile/blob/master/README.md',
-    'Issues': 'https://github.com/linux-profile/email-profile/issues',
+        'Homepage': 'https://github.com/linux-profile/email-profile',
+        'Repository': 'https://github.com/linux-profile/email-profile',
+        'Documentation': 'https://github.com/linux-profile/email-profile/blob/master/README.md',
+        'Issues': 'https://github.com/linux-profile/email-profile/issues',
     },
     cmdclass={
         'install': CustomInstallCommand,
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         "Operating System :: OS Independent",
```

