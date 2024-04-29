# Comparing `tmp/edx-codejail-3.3.3.tar.gz` & `tmp/edx-codejail-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/edx-codejail-3.3.3.tar", last modified: Fri Feb 17 07:31:27 2023, max compression
+gzip compressed data, was "dist/edx-codejail-3.4.0.tar", last modified: Mon Apr 29 16:12:45 2024, max compression
```

## Comparing `edx-codejail-3.3.3.tar` & `edx-codejail-3.4.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/memory_stress.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/testing.txt
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/sandbox.in
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/testing.in
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/pip_tools.in
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/common_constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/tox.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/development.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/development.in
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/requirements/sandbox.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/sudoers-file/
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/sudoers-file/01-sandbox
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/codejail/
--rw-r--r--   0 runner    (1001) docker     (122)    10347 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/safe_exec.py
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/django_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     7184 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2873 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/subproc.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    13027 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/jail_code.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/django_integration_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/codejail/proxy_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/apparmor-profiles/
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/apparmor-profiles/home.sandbox.codejail_sandbox-python3.8.bin.python
--rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     8146 2023-02-17 07:31:18.000000 edx-codejail-3.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/edx_codejail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/edx_codejail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/edx_codejail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/edx_codejail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/edx_codejail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/edx_codejail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-17 07:31:27.000000 edx-codejail-3.3.3/edx_codejail.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/memory_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/testing.in
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/sandbox.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/development.in
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/sandbox.in
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/pip_tools.in
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/testing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/development.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/requirements/tox.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/edx_codejail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/edx_codejail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/edx_codejail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/edx_codejail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/edx_codejail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/edx_codejail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/edx_codejail.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/apparmor-profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/apparmor-profiles/home.sandbox.codejail_sandbox-python3.bin.python
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/sudoers-file/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/sudoers-file/01-sandbox-python-3.11
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/sudoers-file/01-sandbox-python-3.8
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:12:45.000000 edx-codejail-3.4.0/codejail/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/django_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/jail_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/django_integration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/safe_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/proxy_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-29 16:12:39.000000 edx-codejail-3.4.0/codejail/subproc.py
```

### Comparing `edx-codejail-3.3.3/requirements/testing.txt` & `edx-codejail-3.4.0/requirements/testing.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
-astroid==2.11.6           # via pylint
-attrs==21.4.0             # via pytest
-dill==0.3.5.1             # via pylint
-iniconfig==1.1.1          # via pytest
-isort==5.10.1             # via -r requirements/testing.in, pylint
-lazy-object-proxy==1.7.1  # via astroid
+astroid==3.1.0            # via pylint
+dill==0.3.8               # via pylint
+exceptiongroup==1.2.1     # via pytest
+iniconfig==2.0.0          # via pytest
+isort==5.13.2             # via -r requirements/testing.in, pylint
 mccabe==0.7.0             # via pylint
-packaging==21.3           # via pytest
-platformdirs==2.5.2       # via pylint
-pluggy==1.0.0             # via pytest
-py==1.11.0                # via pytest
-pycodestyle==2.8.0        # via -r requirements/testing.in
-pylint==2.14.3            # via -r requirements/testing.in
-pyparsing==3.0.9          # via packaging
-pytest==7.1.2             # via -r requirements/testing.in
+packaging==24.0           # via pytest
+platformdirs==4.2.1       # via pylint
+pluggy==1.5.0             # via pytest
+pycodestyle==2.11.1       # via -r requirements/testing.in
+pylint==3.1.0             # via -r requirements/testing.in
+pytest==8.1.1             # via -r requirements/testing.in
 tomli==2.0.1              # via pylint, pytest
-tomlkit==0.11.0           # via pylint
-typing-extensions==4.2.0  # via astroid, pylint
-wrapt==1.14.1             # via astroid
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
+tomlkit==0.12.4           # via pylint
+typing-extensions==4.11.0  # via astroid, pylint
```

### Comparing `edx-codejail-3.3.3/requirements/common_constraints.txt` & `edx-codejail-3.4.0/requirements/common_constraints.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,24 @@
 # Writing an issue against the offending project and linking to it here is good.
 #
 # Note: Changes to this file will automatically be used by other repos, referencing
 #  this file from Github directly. It does not require packaging in edx-lint.
 
 
 # using LTS django version
-Django<4.0
+Django<5.0
 
 # elasticsearch>=7.14.0 includes breaking changes in it which caused issues in discovery upgrade process.
 # elastic search changelog: https://www.elastic.co/guide/en/enterprise-search/master/release-notes-7.14.0.html
 elasticsearch<7.14.0
 
-setuptools<60
-
 # django-simple-history>3.0.0 adds indexing and causes a lot of migrations to be affected
 django-simple-history==3.0.0
+
+# opentelemetry requires version 6.x at the moment:
+# https://github.com/open-telemetry/opentelemetry-python/issues/3570
+# Normally this could be added as a constraint in edx-django-utils, where we're
+# adding the opentelemetry dependency. However, when we compile pip-tools.txt,
+# that uses version 7.x, and then there's no undoing that when compiling base.txt.
+# So we need to pin it globally, for now.
+# Ticket for unpinning: https://github.com/openedx/edx-lint/issues/407
+importlib-metadata<7
```

### Comparing `edx-codejail-3.3.3/requirements/tox.txt` & `edx-codejail-3.4.0/requirements/tox.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
-distlib==0.3.4            # via virtualenv
-filelock==3.7.1           # via tox, virtualenv
-packaging==21.3           # via tox
-platformdirs==2.5.2       # via virtualenv
-pluggy==1.0.0             # via tox
-py==1.11.0                # via tox
-pyparsing==3.0.9          # via packaging
-six==1.16.0               # via tox, virtualenv
-toml==0.10.2              # via tox
-tox==3.25.0               # via -r requirements/tox.in
-virtualenv==20.14.1       # via tox
+cachetools==5.3.3         # via tox
+chardet==5.2.0            # via tox
+colorama==0.4.6           # via tox
+distlib==0.3.8            # via virtualenv
+filelock==3.13.4          # via tox, virtualenv
+packaging==24.0           # via pyproject-api, tox
+platformdirs==4.2.1       # via tox, virtualenv
+pluggy==1.5.0             # via tox
+pyproject-api==1.6.1      # via tox
+tomli==2.0.1              # via pyproject-api, tox
+tox==4.14.2               # via -r requirements/tox.in
+virtualenv==20.26.0       # via tox
```

### Comparing `edx-codejail-3.3.3/requirements/development.txt` & `edx-codejail-3.4.0/requirements/development.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
-astroid==2.11.6           # via -r requirements/testing.txt, pylint
-attrs==21.4.0             # via -r requirements/testing.txt, pytest
-dill==0.3.5.1             # via -r requirements/testing.txt, pylint
-iniconfig==1.1.1          # via -r requirements/testing.txt, pytest
-isort==5.10.1             # via -r requirements/testing.txt, pylint
-lazy-object-proxy==1.7.1  # via -r requirements/testing.txt, astroid
+astroid==3.1.0            # via -r requirements/testing.txt, pylint
+dill==0.3.8               # via -r requirements/testing.txt, pylint
+exceptiongroup==1.2.1     # via -r requirements/testing.txt, pytest
+iniconfig==2.0.0          # via -r requirements/testing.txt, pytest
+isort==5.13.2             # via -r requirements/testing.txt, pylint
 mccabe==0.7.0             # via -r requirements/testing.txt, pylint
-packaging==21.3           # via -r requirements/testing.txt, pytest
-platformdirs==2.5.2       # via -r requirements/testing.txt, pylint
-pluggy==1.0.0             # via -r requirements/testing.txt, pytest
-py==1.11.0                # via -r requirements/testing.txt, pytest
-pycodestyle==2.8.0        # via -r requirements/testing.txt
-pylint==2.14.3            # via -r requirements/testing.txt
-pyparsing==3.0.9          # via -r requirements/testing.txt, packaging
-pytest==7.1.2             # via -r requirements/testing.txt
+packaging==24.0           # via -r requirements/testing.txt, pytest
+platformdirs==4.2.1       # via -r requirements/testing.txt, pylint
+pluggy==1.5.0             # via -r requirements/testing.txt, pytest
+pycodestyle==2.11.1       # via -r requirements/testing.txt
+pylint==3.1.0             # via -r requirements/testing.txt
+pytest==8.1.1             # via -r requirements/testing.txt
 tomli==2.0.1              # via -r requirements/testing.txt, pylint, pytest
-tomlkit==0.11.0           # via -r requirements/testing.txt, pylint
-typing-extensions==4.2.0  # via -r requirements/testing.txt, astroid, pylint
-wrapt==1.14.1             # via -r requirements/testing.txt, astroid
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
+tomlkit==0.12.4           # via -r requirements/testing.txt, pylint
+typing-extensions==4.11.0  # via -r requirements/testing.txt, astroid, pylint
```

### Comparing `edx-codejail-3.3.3/PKG-INFO` & `edx-codejail-3.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-codejail
-Version: 3.3.3
+Version: 3.4.0
 Summary: CodeJail manages execution of untrusted code in secure sandboxes. It is designed primarily for Python execution, but can be used for other languages as well.
 Home-page: https://github.com/openedx/codejail
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Description: CodeJail
         ========
@@ -67,61 +67,65 @@
         
         To secure Python execution, you'll be creating a new virtualenv.  This means
         you'll have two: the main virtualenv for your project, and the new one for
         sandboxed Python code.
         
         Choose a place for the new virtualenv, call it **<SANDENV>**.  It will be
         automatically detected and used if you put it right alongside your existing
-        virtualenv, but with `-sandbox` appended.  So if your existing virtualenv is in
-        `/home/chris/ve/myproj`, make **<SANDENV>** be `/home/chris/ve/myproj-sandbox`.
+        virtualenv, but with ``-sandbox`` appended.  So if your existing virtualenv is in
+        ``/home/chris/ve/myproj``, make **<SANDENV>** be ``/home/chris/ve/myproj-sandbox``.
         
         The user running the LMS is **<SANDBOX_CALLER>**, for example, you on
-        your dev machine, or `www-data` on a server.
+        your dev machine, or ``www-data`` on a server.
         
         Other details here that depend on your configuration:
         
-        1. Create the new virtualenv::
+        1. Create the new virtualenv, using ``--copies`` so that there's a distinct Python executable to limit::
         
-            $ sudo virtualenv <SANDENV>
+            $ sudo python3.8 -m venv --copies <SANDENV>
+        
+           By default, the virtualenv would just symlink against the system Python, and apparmor's default configuration on some operating systems may prevent confinement from being appled to that.
         
         2. (Optional) If you have particular packages you want available to your
            sandboxed code, install them by activating the sandbox virtual env, and
            using pip to install them::
         
-            $ source <SANDENV>/bin/activate
-            $ pip install -r requirements/sandbox.txt
+            $ <SANDENV>/bin/pip install -r requirements/sandbox.txt
         
         3. Add a sandbox user::
         
             $ sudo addgroup sandbox
             $ sudo adduser --disabled-login sandbox --ingroup sandbox
         
         4. Let the web server run the sandboxed Python as sandbox.  Create the file
-           `/etc/sudoers.d/01-sandbox`::
+           ``/etc/sudoers.d/01-sandbox``::
         
             $ sudo visudo -f /etc/sudoers.d/01-sandbox
         
             <SANDBOX_CALLER> ALL=(sandbox) SETENV:NOPASSWD:<SANDENV>/bin/python
             <SANDBOX_CALLER> ALL=(sandbox) SETENV:NOPASSWD:/usr/bin/find
             <SANDBOX_CALLER> ALL=(ALL) NOPASSWD:/usr/bin/pkill
         
+           (Note that the ``find`` binary can run arbitrary code, so this is not a safe sudoers file for non-codejail purposes.)
+        
         5. Edit an AppArmor profile.  This is a text file specifying the limits on the
-           sandboxed Python executable.  The file must be in `/etc/apparmor.d` and must
+           sandboxed Python executable.  The file must be in ``/etc/apparmor.d`` and must
            be named based on the executable, with slashes replaced by dots.  For
-           example, if your sandboxed Python is at `/home/chris/ve/myproj-sandbox/bin/python`,
-           then your AppArmor profile must be `/etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python`::
+           example, if your sandboxed Python is at ``/home/chris/ve/myproj-sandbox/bin/python``,
+           then your AppArmor profile must be ``/etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python``::
         
             $ sudo vim /etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python
         
             #include <tunables/global>
         
             <SANDENV>/bin/python {
                 #include <abstractions/base>
                 #include <abstractions/python>
         
+                <CODEJAIL_CHECKOUT>/** mr,
                 <SANDENV>/** mr,
                 # If you have code that the sandbox must be able to access, add lines
                 # pointing to those directories:
                 /the/path/to/your/sandbox-packages/** r,
         
                 /tmp/codejail-*/ rix,
                 /tmp/codejail-*/** wrix,
@@ -136,17 +140,19 @@
         Using CodeJail
         --------------
         
         If your CodeJail is properly configured to use safe_exec, try these
         commands at your Python terminal::
         
             import codejail.jail_code
-            codejail.jail_code.configure('python', '<SANDENV>/bin/python')
+            codejail.jail_code.configure('python', '<SANDENV>/bin/python', user='sandbox')
             import codejail.safe_exec
-            codejail.safe_exec.safe_exec("import os\nos.system('ls /etc')", {})
+            jailed_globals = {}
+            codejail.safe_exec.safe_exec("output=open('/etc/passwd').read()", jailed_globals)
+            print(jailed_globals)  # should be unreachable if codejail is working properly
         
         This should fail with an exception. 
         
         If you need to change the packages installed into your sandbox's virtualenv,
         you'll need to disable AppArmor, because your sandboxed Python doesn't have
         the rights to modify the files in its site-packages directory.
         
@@ -184,38 +190,43 @@
         
         Design
         ------
         
         CodeJail is general-purpose enough that it can be used in a variety of projects
         to run untrusted code.  It provides two layers:
         
-        * `jail_code.py` offers secure execution of subprocesses.  It does this by
+        * ``jail_code.py`` offers secure execution of subprocesses.  It does this by
           running the program in a subprocess managed by AppArmor.
         
-        * `safe_exec.py` offers specialized handling of Python execution, using
+        * ``safe_exec.py`` offers specialized handling of Python execution, using
           jail_code to provide the semantics of Python's exec statement.
         
         CodeJail runs programs under AppArmor.  AppArmor is an OS-provided feature to
         limit the resources programs can access. To run Python code with limited access
         to resources, we make a new virtualenv, then name that Python executable in an
         AppArmor profile, and restrict resources in that profile.  CodeJail will
         execute the provided Python program with that executable, and AppArmor will
         automatically limit the resources it can access.  CodeJail also uses setrlimit
         to limit the amount of CPU time and/or memory available to the process.
         
-        `CodeJail.jail_code` takes a program to run, files to copy into its
+        ``CodeJail.jail_code`` takes a program to run, files to copy into its
         environment, command-line arguments, and a stdin stream.  It creates a
         temporary directory, creates or copies the needed files, spawns a subprocess to
         run the code, and returns the output and exit status of the process.
         
-        `CodeJail.safe_exec` emulates Python's exec statement.  It takes a chunk of
+        ``CodeJail.safe_exec`` emulates Python's exec statement.  It takes a chunk of
         Python code, and runs it using jail_code, modifying the globals dictionary as a
         side-effect.  safe_exec does this by serializing the globals into and out of
         the subprocess as JSON.
         
+        Reporting Security Issues
+        -------------------------
+        
+        Please do not report security issues in public. Please email security@openedx.org.
+        
 Keywords: edx codejail
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `edx-codejail-3.3.3/LICENSE.txt` & `edx-codejail-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-codejail-3.3.3/codejail/safe_exec.py` & `edx-codejail-3.4.0/codejail/safe_exec.py`

 * *Files identical despite different names*

### Comparing `edx-codejail-3.3.3/codejail/django_integration.py` & `edx-codejail-3.4.0/codejail/django_integration.py`

 * *Files identical despite different names*

### Comparing `edx-codejail-3.3.3/codejail/proxy.py` & `edx-codejail-3.4.0/codejail/proxy.py`

 * *Files identical despite different names*

### Comparing `edx-codejail-3.3.3/codejail/subproc.py` & `edx-codejail-3.4.0/codejail/subproc.py`

 * *Files identical despite different names*

### Comparing `edx-codejail-3.3.3/codejail/util.py` & `edx-codejail-3.4.0/codejail/util.py`

 * *Files identical despite different names*

### Comparing `edx-codejail-3.3.3/codejail/jail_code.py` & `edx-codejail-3.4.0/codejail/jail_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,16 @@
         user = COMMANDS[command]['user']
         if user:
             # Run as the specified user
             cmd.extend(['sudo', '-u', user])
             rm_cmd.extend(['sudo', '-u', user])
 
         # Point TMPDIR at our temp directory.
+        # FIXME: This breaks command execution unless user param has been set.
+        #   Issue: https://github.com/openedx/codejail/issues/162
         cmd.extend(['TMPDIR=tmp'])
         # Start with the command line dictated by "python" or whatever.
         cmd.extend(COMMANDS[command]['cmdline_start'])
 
         # Add the code-specific command line pieces.
         cmd.extend(argv)
```

### Comparing `edx-codejail-3.3.3/codejail/django_integration_utils.py` & `edx-codejail-3.4.0/codejail/django_integration_utils.py`

 * *Files identical despite different names*

### Comparing `edx-codejail-3.3.3/setup.py` & `edx-codejail-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `edx-codejail-3.3.3/README.rst` & `edx-codejail-3.4.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -59,61 +59,65 @@
 
 To secure Python execution, you'll be creating a new virtualenv.  This means
 you'll have two: the main virtualenv for your project, and the new one for
 sandboxed Python code.
 
 Choose a place for the new virtualenv, call it **<SANDENV>**.  It will be
 automatically detected and used if you put it right alongside your existing
-virtualenv, but with `-sandbox` appended.  So if your existing virtualenv is in
-`/home/chris/ve/myproj`, make **<SANDENV>** be `/home/chris/ve/myproj-sandbox`.
+virtualenv, but with ``-sandbox`` appended.  So if your existing virtualenv is in
+``/home/chris/ve/myproj``, make **<SANDENV>** be ``/home/chris/ve/myproj-sandbox``.
 
 The user running the LMS is **<SANDBOX_CALLER>**, for example, you on
-your dev machine, or `www-data` on a server.
+your dev machine, or ``www-data`` on a server.
 
 Other details here that depend on your configuration:
 
-1. Create the new virtualenv::
+1. Create the new virtualenv, using ``--copies`` so that there's a distinct Python executable to limit::
 
-    $ sudo virtualenv <SANDENV>
+    $ sudo python3.8 -m venv --copies <SANDENV>
+
+   By default, the virtualenv would just symlink against the system Python, and apparmor's default configuration on some operating systems may prevent confinement from being appled to that.
 
 2. (Optional) If you have particular packages you want available to your
    sandboxed code, install them by activating the sandbox virtual env, and
    using pip to install them::
 
-    $ source <SANDENV>/bin/activate
-    $ pip install -r requirements/sandbox.txt
+    $ <SANDENV>/bin/pip install -r requirements/sandbox.txt
 
 3. Add a sandbox user::
 
     $ sudo addgroup sandbox
     $ sudo adduser --disabled-login sandbox --ingroup sandbox
 
 4. Let the web server run the sandboxed Python as sandbox.  Create the file
-   `/etc/sudoers.d/01-sandbox`::
+   ``/etc/sudoers.d/01-sandbox``::
 
     $ sudo visudo -f /etc/sudoers.d/01-sandbox
 
     <SANDBOX_CALLER> ALL=(sandbox) SETENV:NOPASSWD:<SANDENV>/bin/python
     <SANDBOX_CALLER> ALL=(sandbox) SETENV:NOPASSWD:/usr/bin/find
     <SANDBOX_CALLER> ALL=(ALL) NOPASSWD:/usr/bin/pkill
 
+   (Note that the ``find`` binary can run arbitrary code, so this is not a safe sudoers file for non-codejail purposes.)
+
 5. Edit an AppArmor profile.  This is a text file specifying the limits on the
-   sandboxed Python executable.  The file must be in `/etc/apparmor.d` and must
+   sandboxed Python executable.  The file must be in ``/etc/apparmor.d`` and must
    be named based on the executable, with slashes replaced by dots.  For
-   example, if your sandboxed Python is at `/home/chris/ve/myproj-sandbox/bin/python`,
-   then your AppArmor profile must be `/etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python`::
+   example, if your sandboxed Python is at ``/home/chris/ve/myproj-sandbox/bin/python``,
+   then your AppArmor profile must be ``/etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python``::
 
     $ sudo vim /etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python
 
     #include <tunables/global>
 
     <SANDENV>/bin/python {
         #include <abstractions/base>
         #include <abstractions/python>
 
+        <CODEJAIL_CHECKOUT>/** mr,
         <SANDENV>/** mr,
         # If you have code that the sandbox must be able to access, add lines
         # pointing to those directories:
         /the/path/to/your/sandbox-packages/** r,
 
         /tmp/codejail-*/ rix,
         /tmp/codejail-*/** wrix,
@@ -128,17 +132,19 @@
 Using CodeJail
 --------------
 
 If your CodeJail is properly configured to use safe_exec, try these
 commands at your Python terminal::
 
     import codejail.jail_code
-    codejail.jail_code.configure('python', '<SANDENV>/bin/python')
+    codejail.jail_code.configure('python', '<SANDENV>/bin/python', user='sandbox')
     import codejail.safe_exec
-    codejail.safe_exec.safe_exec("import os\nos.system('ls /etc')", {})
+    jailed_globals = {}
+    codejail.safe_exec.safe_exec("output=open('/etc/passwd').read()", jailed_globals)
+    print(jailed_globals)  # should be unreachable if codejail is working properly
 
 This should fail with an exception. 
 
 If you need to change the packages installed into your sandbox's virtualenv,
 you'll need to disable AppArmor, because your sandboxed Python doesn't have
 the rights to modify the files in its site-packages directory.
 
@@ -176,30 +182,35 @@
 
 Design
 ------
 
 CodeJail is general-purpose enough that it can be used in a variety of projects
 to run untrusted code.  It provides two layers:
 
-* `jail_code.py` offers secure execution of subprocesses.  It does this by
+* ``jail_code.py`` offers secure execution of subprocesses.  It does this by
   running the program in a subprocess managed by AppArmor.
 
-* `safe_exec.py` offers specialized handling of Python execution, using
+* ``safe_exec.py`` offers specialized handling of Python execution, using
   jail_code to provide the semantics of Python's exec statement.
 
 CodeJail runs programs under AppArmor.  AppArmor is an OS-provided feature to
 limit the resources programs can access. To run Python code with limited access
 to resources, we make a new virtualenv, then name that Python executable in an
 AppArmor profile, and restrict resources in that profile.  CodeJail will
 execute the provided Python program with that executable, and AppArmor will
 automatically limit the resources it can access.  CodeJail also uses setrlimit
 to limit the amount of CPU time and/or memory available to the process.
 
-`CodeJail.jail_code` takes a program to run, files to copy into its
+``CodeJail.jail_code`` takes a program to run, files to copy into its
 environment, command-line arguments, and a stdin stream.  It creates a
 temporary directory, creates or copies the needed files, spawns a subprocess to
 run the code, and returns the output and exit status of the process.
 
-`CodeJail.safe_exec` emulates Python's exec statement.  It takes a chunk of
+``CodeJail.safe_exec`` emulates Python's exec statement.  It takes a chunk of
 Python code, and runs it using jail_code, modifying the globals dictionary as a
 side-effect.  safe_exec does this by serializing the globals into and out of
 the subprocess as JSON.
+
+Reporting Security Issues
+-------------------------
+
+Please do not report security issues in public. Please email security@openedx.org.
```

### Comparing `edx-codejail-3.3.3/edx_codejail.egg-info/SOURCES.txt` & `edx-codejail-3.4.0/edx_codejail.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 memory_stress.py
 setup.cfg
 setup.py
-apparmor-profiles/home.sandbox.codejail_sandbox-python3.8.bin.python
+apparmor-profiles/home.sandbox.codejail_sandbox-python3.bin.python
 codejail/__init__.py
 codejail/django_integration.py
 codejail/django_integration_utils.py
 codejail/jail_code.py
 codejail/proxy.py
 codejail/proxy_main.py
 codejail/safe_exec.py
@@ -30,8 +30,9 @@
 requirements/pip_tools.txt
 requirements/sandbox.in
 requirements/sandbox.txt
 requirements/testing.in
 requirements/testing.txt
 requirements/tox.in
 requirements/tox.txt
-sudoers-file/01-sandbox
+sudoers-file/01-sandbox-python-3.11
+sudoers-file/01-sandbox-python-3.8
```

### Comparing `edx-codejail-3.3.3/edx_codejail.egg-info/PKG-INFO` & `edx-codejail-3.4.0/edx_codejail.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-codejail
-Version: 3.3.3
+Version: 3.4.0
 Summary: CodeJail manages execution of untrusted code in secure sandboxes. It is designed primarily for Python execution, but can be used for other languages as well.
 Home-page: https://github.com/openedx/codejail
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Description: CodeJail
         ========
@@ -67,61 +67,65 @@
         
         To secure Python execution, you'll be creating a new virtualenv.  This means
         you'll have two: the main virtualenv for your project, and the new one for
         sandboxed Python code.
         
         Choose a place for the new virtualenv, call it **<SANDENV>**.  It will be
         automatically detected and used if you put it right alongside your existing
-        virtualenv, but with `-sandbox` appended.  So if your existing virtualenv is in
-        `/home/chris/ve/myproj`, make **<SANDENV>** be `/home/chris/ve/myproj-sandbox`.
+        virtualenv, but with ``-sandbox`` appended.  So if your existing virtualenv is in
+        ``/home/chris/ve/myproj``, make **<SANDENV>** be ``/home/chris/ve/myproj-sandbox``.
         
         The user running the LMS is **<SANDBOX_CALLER>**, for example, you on
-        your dev machine, or `www-data` on a server.
+        your dev machine, or ``www-data`` on a server.
         
         Other details here that depend on your configuration:
         
-        1. Create the new virtualenv::
+        1. Create the new virtualenv, using ``--copies`` so that there's a distinct Python executable to limit::
         
-            $ sudo virtualenv <SANDENV>
+            $ sudo python3.8 -m venv --copies <SANDENV>
+        
+           By default, the virtualenv would just symlink against the system Python, and apparmor's default configuration on some operating systems may prevent confinement from being appled to that.
         
         2. (Optional) If you have particular packages you want available to your
            sandboxed code, install them by activating the sandbox virtual env, and
            using pip to install them::
         
-            $ source <SANDENV>/bin/activate
-            $ pip install -r requirements/sandbox.txt
+            $ <SANDENV>/bin/pip install -r requirements/sandbox.txt
         
         3. Add a sandbox user::
         
             $ sudo addgroup sandbox
             $ sudo adduser --disabled-login sandbox --ingroup sandbox
         
         4. Let the web server run the sandboxed Python as sandbox.  Create the file
-           `/etc/sudoers.d/01-sandbox`::
+           ``/etc/sudoers.d/01-sandbox``::
         
             $ sudo visudo -f /etc/sudoers.d/01-sandbox
         
             <SANDBOX_CALLER> ALL=(sandbox) SETENV:NOPASSWD:<SANDENV>/bin/python
             <SANDBOX_CALLER> ALL=(sandbox) SETENV:NOPASSWD:/usr/bin/find
             <SANDBOX_CALLER> ALL=(ALL) NOPASSWD:/usr/bin/pkill
         
+           (Note that the ``find`` binary can run arbitrary code, so this is not a safe sudoers file for non-codejail purposes.)
+        
         5. Edit an AppArmor profile.  This is a text file specifying the limits on the
-           sandboxed Python executable.  The file must be in `/etc/apparmor.d` and must
+           sandboxed Python executable.  The file must be in ``/etc/apparmor.d`` and must
            be named based on the executable, with slashes replaced by dots.  For
-           example, if your sandboxed Python is at `/home/chris/ve/myproj-sandbox/bin/python`,
-           then your AppArmor profile must be `/etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python`::
+           example, if your sandboxed Python is at ``/home/chris/ve/myproj-sandbox/bin/python``,
+           then your AppArmor profile must be ``/etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python``::
         
             $ sudo vim /etc/apparmor.d/home.chris.ve.myproj-sandbox.bin.python
         
             #include <tunables/global>
         
             <SANDENV>/bin/python {
                 #include <abstractions/base>
                 #include <abstractions/python>
         
+                <CODEJAIL_CHECKOUT>/** mr,
                 <SANDENV>/** mr,
                 # If you have code that the sandbox must be able to access, add lines
                 # pointing to those directories:
                 /the/path/to/your/sandbox-packages/** r,
         
                 /tmp/codejail-*/ rix,
                 /tmp/codejail-*/** wrix,
@@ -136,17 +140,19 @@
         Using CodeJail
         --------------
         
         If your CodeJail is properly configured to use safe_exec, try these
         commands at your Python terminal::
         
             import codejail.jail_code
-            codejail.jail_code.configure('python', '<SANDENV>/bin/python')
+            codejail.jail_code.configure('python', '<SANDENV>/bin/python', user='sandbox')
             import codejail.safe_exec
-            codejail.safe_exec.safe_exec("import os\nos.system('ls /etc')", {})
+            jailed_globals = {}
+            codejail.safe_exec.safe_exec("output=open('/etc/passwd').read()", jailed_globals)
+            print(jailed_globals)  # should be unreachable if codejail is working properly
         
         This should fail with an exception. 
         
         If you need to change the packages installed into your sandbox's virtualenv,
         you'll need to disable AppArmor, because your sandboxed Python doesn't have
         the rights to modify the files in its site-packages directory.
         
@@ -184,38 +190,43 @@
         
         Design
         ------
         
         CodeJail is general-purpose enough that it can be used in a variety of projects
         to run untrusted code.  It provides two layers:
         
-        * `jail_code.py` offers secure execution of subprocesses.  It does this by
+        * ``jail_code.py`` offers secure execution of subprocesses.  It does this by
           running the program in a subprocess managed by AppArmor.
         
-        * `safe_exec.py` offers specialized handling of Python execution, using
+        * ``safe_exec.py`` offers specialized handling of Python execution, using
           jail_code to provide the semantics of Python's exec statement.
         
         CodeJail runs programs under AppArmor.  AppArmor is an OS-provided feature to
         limit the resources programs can access. To run Python code with limited access
         to resources, we make a new virtualenv, then name that Python executable in an
         AppArmor profile, and restrict resources in that profile.  CodeJail will
         execute the provided Python program with that executable, and AppArmor will
         automatically limit the resources it can access.  CodeJail also uses setrlimit
         to limit the amount of CPU time and/or memory available to the process.
         
-        `CodeJail.jail_code` takes a program to run, files to copy into its
+        ``CodeJail.jail_code`` takes a program to run, files to copy into its
         environment, command-line arguments, and a stdin stream.  It creates a
         temporary directory, creates or copies the needed files, spawns a subprocess to
         run the code, and returns the output and exit status of the process.
         
-        `CodeJail.safe_exec` emulates Python's exec statement.  It takes a chunk of
+        ``CodeJail.safe_exec`` emulates Python's exec statement.  It takes a chunk of
         Python code, and runs it using jail_code, modifying the globals dictionary as a
         side-effect.  safe_exec does this by serializing the globals into and out of
         the subprocess as JSON.
         
+        Reporting Security Issues
+        -------------------------
+        
+        Please do not report security issues in public. Please email security@openedx.org.
+        
 Keywords: edx codejail
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

