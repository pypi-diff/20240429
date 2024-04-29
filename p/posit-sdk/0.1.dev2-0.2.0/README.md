# Comparing `tmp/posit-sdk-0.1.dev2.tar.gz` & `tmp/posit_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posit-sdk-0.1.dev2.tar", last modified: Fri Mar 22 18:16:15 2024, max compression
+gzip compressed data, was "posit_sdk-0.2.0.tar", last modified: Mon Apr 29 16:18:22 2024, max compression
```

## Comparing `posit-sdk-0.1.dev2.tar` & `posit_sdk-0.2.0.tar`

### file list

```diff
@@ -1,104 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.410097 posit-sdk-0.1.dev2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.github/workflows/conventional-commits.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/examples/connect/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/examples/connect/dash/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/dash/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/dash/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/dash/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/examples/connect/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/fastapi/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/fastapi/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/fastapi/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/examples/connect/flask/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/flask/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/flask/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/flask/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/examples/connect/shiny-python/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/shiny-python/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/shiny-python/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/shiny-python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/examples/connect/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/streamlit/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/streamlit/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/examples/connect/streamlit/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.414096 posit-sdk-0.1.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.418096 posit-sdk-0.1.dev2/src/posit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-22 18:16:15.000000 posit-sdk-0.1.dev2/src/posit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.422097 posit-sdk-0.1.dev2/src/posit/connect/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/content.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.422097 posit-sdk-0.1.dev2/src/posit/connect/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/external/databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/me.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/src/posit/connect/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/src/posit_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-03-22 18:16:15.000000 posit-sdk-0.1.dev2/src/posit_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-22 18:16:15.000000 posit-sdk-0.1.dev2/src/posit_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:16:15.000000 posit-sdk-0.1.dev2/src/posit_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 18:16:15.000000 posit-sdk-0.1.dev2/src/posit_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 18:16:15.000000 posit-sdk-0.1.dev2/src/posit_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.414096 posit-sdk-0.1.dev2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.414096 posit-sdk-0.1.dev2/tests/posit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/tests/posit/connect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.414096 posit-sdk-0.1.dev2/tests/posit/connect/__api__/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/content/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066.json
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/content.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/user.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/users/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/users/a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6.json
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/users.json
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/users?page_number=1&page_size=500.json
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/users?page_number=2&page_size=500.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:15.426097 posit-sdk-0.1.dev2/tests/posit/connect/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/external/test_databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-03-22 18:16:00.000000 posit-sdk-0.1.dev2/tests/posit/connect/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.639304 posit_sdk-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.619304 posit_sdk-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.623304 posit_sdk-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.github/workflows/conventional-commits.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.623304 posit_sdk-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-29 16:18:22.639304 posit_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.627304 posit_sdk-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/0001-overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.627304 posit_sdk-0.2.0/examples/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.627304 posit_sdk-0.2.0/examples/connect/dash/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/dash/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/dash/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/dash/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.627304 posit_sdk-0.2.0/examples/connect/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/fastapi/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/fastapi/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.627304 posit_sdk-0.2.0/examples/connect/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/flask/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/flask/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/flask/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.627304 posit_sdk-0.2.0/examples/connect/shiny-python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/shiny-python/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/shiny-python/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/shiny-python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.627304 posit_sdk-0.2.0/examples/connect/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/streamlit/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/streamlit/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/examples/connect/streamlit/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:18:22.639304 posit_sdk-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.619304 posit_sdk-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.627304 posit_sdk-0.2.0/src/posit/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 16:18:22.000000 posit_sdk-0.2.0/src/posit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.631304 posit_sdk-0.2.0/src/posit/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16935 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.631304 posit_sdk-0.2.0/src/posit/connect/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/external/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/me.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.631304 posit_sdk-0.2.0/src/posit/connect/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/metrics/shiny_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/metrics/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/metrics/visits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/src/posit/connect/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.639304 posit_sdk-0.2.0/src/posit_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-29 16:18:22.000000 posit_sdk-0.2.0/src/posit_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-29 16:18:22.000000 posit_sdk-0.2.0/src/posit_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:18:22.000000 posit_sdk-0.2.0/src/posit_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 16:18:22.000000 posit_sdk-0.2.0/src/posit_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 16:18:22.000000 posit_sdk-0.2.0/src/posit_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.619304 posit_sdk-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.619304 posit_sdk-0.2.0/tests/posit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.619304 posit_sdk-0.2.0/tests/posit/connect/__api__/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.623304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles/101/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles/101/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles/101/download/bundle.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles/101.json
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/permissions/94.json
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.623304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/instrumentation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/instrumentation/content/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/instrumentation/content/visits?limit=500&next=23948901087.json
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/instrumentation/content/visits?limit=500.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/instrumentation/shiny/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/instrumentation/shiny/usage?limit=500&next=23948901087.json
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/instrumentation/shiny/usage?limit=500.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/tasks/jXhOhdm5OOSkGhJw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/user.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/users/a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/users?page_number=1&page_size=500.jsonc
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/__api__/v1/users?page_number=2&page_size=500.jsonc
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/external/test_databricks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:18:22.635304 posit_sdk-0.2.0/tests/posit/connect/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/metrics/test_shiny_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/metrics/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/metrics/test_visits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15612 2024-04-29 16:18:08.000000 posit_sdk-0.2.0/tests/posit/connect/test_users.py
```

### Comparing `posit-sdk-0.1.dev2/.github/workflows/conventional-commits.yaml` & `posit_sdk-0.2.0/.github/workflows/conventional-commits.yaml`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/.github/workflows/pull-request.yaml` & `posit_sdk-0.2.0/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/.gitignore` & `posit_sdk-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/CODE_OF_CONDUCT.md` & `posit_sdk-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/CONTRIBUTING.md` & `posit_sdk-0.2.0/CONTRIBUTING.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,53 +6,68 @@
 
 ## Prerequisites
 
 Before contributing to the `posit-sdk`, ensure that the following prerequisites are met:
 
 - Python >=3.8
 
+> [!TIP]
+> We recommend using virtual environments to maintain a clean and consistent development environment.
+
 ## Instructions
 
+> [!WARNING]
+> Executing `make` will utilize `pip` to install third-party packages in your activated Python environment. Please review the [`Makefile`](./Makefile) to verify behavior before executing any commands.
+
 1. Fork the repository and clone it to your local machine.
 1. Create a new branch for your feature or bug fix.
 1. Run `make` to run the default development workflow.
 1. Make your changes and test them thoroughly using `make test`
+1. Run `make fmt`, `make lint`, and `make fix` to verify adherence to the project style guide.
 1. Commit your changes and push them to your forked repository.
 1. Submit a pull request to the main repository.
 
-Please ensure that your code follows the project's coding conventions and style guidelines using the configured pre-commit hooks. Run `pre-commit install` install to configure this functionality on your machine.
-
-Also, make sure to include tests for any new functionality or bug fixes.
-
 ## Tooling
 
 Use the default make target to execute the full build pipeline. For details on specific targets, refer to the [Makefile](./Makefile).
 
+## Style Guide
+
+We use [Ruff](https://docs.astral.sh/ruff/) for linting and code formatting. All proposed changes must successfully pass the `make lint` rules prior to merging.
+
+Utilize `make fmt lint fix` to format and lint your changes.
+
+### (Optional) pre-commit
+
+This project is configured for [pre-commit](https://pre-commit.com). Once enabled, a `git commit` hook is created, which invokes `make fmt lint fix`.
+
+To enable pre-commit on your machine, run `pre-commit install`.
+
 ## Release
 
 ### Instructions
 
 To start a release create a semver compatible tag.
 
-_For this example, we will use the tag `v0.0.dev0`. This tag already exists, so you will not be able run the following commands verbatim._
+_For this example, we will use the tag `v0.1.0`. This tag already exists, so you will not be able run the following commands verbatim._
 
 **Step 1**
 
 Create a proper SemVer compatible tag. Consult the [SemVer specification](https://semver.org/spec/v2.0.0.html) if you are unsure what this means.
 
-`git tag v0.0.dev0`
+`git tag v0.1.0`
 
 **Step 2**
 
 Push the tag GitHub.
 
-`git push origin v0.0.dev0`
+`git push origin v0.1.0`
 
 This command will trigger the [Release GitHub Action](https://github.com/posit-dev/posit-sdk-py/actions/workflows/release.yaml).
 
 **Step 3**
 
 Once complete, the release will be available on [PyPI](https://pypi.org/project/posit-sdk).
 
 ### Pre-Releases
 
-Any tags denoted as a pre-release as defined by the [SemVer 2.0.0](https://semver.org/spec/v2.0.0.html) specification will be marked as such in GitHub. For example, the `v0.0.dev0` is a pre-release. Tag `v0.0.0` is a standard-release. Please consult the specification for additional information.
+Any tags denoted as a pre-release as defined by the [SemVer 2.0.0](https://semver.org/spec/v2.0.0.html) specification will be marked as such in GitHub. For example, the `v0.1.rc1` is a pre-release. Tag `v0.1.0` is a standard-release. Please consult the specification for additional information.
```

### Comparing `posit-sdk-0.1.dev2/LICENSE` & `posit_sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/Makefile` & `posit_sdk-0.2.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 
 # Target for building the project, which will generate the distribution files in the `dist` directory.
 build:
 	$(PYTHON) -m build
 
 # Target for cleaning up generated files and directories
 clean:
+	rm -rf .coverage .mypy_cache .pytest_cache .ruff_cache *.egg-info build coverage.xml dist htmlcov coverage.xml
 	find . -name "*.egg-info" -exec rm -rf {} +
 	find . -name "*.pyc" -exec rm -f {} +
 	find . -name "__pycache__" -exec rm -rf {} +
 	find . -name "_version.py" -exec rm -rf {} +
-	rm -rf .coverage .mypy_cache .pytest_cache .ruff_cache *.egg-info build coverage.xml dist htmlcov coverage.xml
+	find . -type d -empty -delete
 
 # Target for generating coverage report
 cov:
 	$(PYTHON) -m coverage report
 
 # Target for generating HTML coverage report
 cov-html:
```

### Comparing `posit-sdk-0.1.dev2/PKG-INFO` & `posit_sdk-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posit-sdk
-Version: 0.1.dev2
+Version: 0.2.0
 Summary: Posit SDK for Python
 License: MIT License
         
         Copyright (c) 2024 posit-dev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,17 +23,18 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Source, https://github.com/posit-dev/posit-sdk-py
 Project-URL: Issues, https://github.com/posit-dev/posit-sdk-py/issues
 Keywords: posit,sdk
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests<3,>=2.31.0
@@ -48,21 +49,40 @@
 
 ```shell
 pip install posit-sdk
 ```
 
 ## Usage
 
+Establish server information and credentials using the following environment variables or when initializing a client. Then checkout some [examples](./examples/0001-overview.qmd) to get started.
+
+> [!CAUTION]
+> It is important to keep your API key safe and secure. Your API key grants access to your account and allows you to make authenticated requests to the Posit API. Treat your API key like a password and avoid sharing it with others. If you suspect that your API key has been compromised, regenerate a new one immediately to maintain the security of your account.
+
+### Option 1 (Preferred)
+
+```shell
+export CONNECT_API_KEY="my-secret-api-key"
+export CONNECT_SERVER="https://example.com/"
+```
+
+```python
+from posit.connect import Client
+
+with Client() as client:
+    print(client)
+```
+
+### Option 2
+
 ```python
 from posit.connect import Client
 
-# If CONNECT_API_KEY and CONNECT_SERVER are set in your environment,
-# they will be picked up, or you can pass them as arguments
-con = Client()
-con.users.find()
+with Client(api_key="my-secret-api-key", url="https://example.com") as client:
+    print(client)
 ```
 
 ## Contributing
 
 We welcome contributions to the Posit SDK for Python! If you would like to contribute, see the [CONTRIBUTING](CONTRIBUTING.md) guide for instructions.
 
 ## Issues
```

### Comparing `posit-sdk-0.1.dev2/examples/connect/dash/README.md` & `posit_sdk-0.2.0/examples/connect/dash/README.md`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/examples/connect/dash/app.py` & `posit_sdk-0.2.0/examples/connect/dash/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,20 @@
     Input("dummy", "children"),
 )
 def update_page(_):
     """
     Dash example application that shows user information and
     the first few rows from a table hosted in Databricks.
     """
-
-    session_token = flask.request.headers.get("Posit-Connect-User-Session-Token")
-    credentials_provider = viewer_credentials_provider(user_session_token=session_token)
+    session_token = flask.request.headers.get(
+        "Posit-Connect-User-Session-Token"
+    )
+    credentials_provider = viewer_credentials_provider(
+        user_session_token=session_token
+    )
 
     def get_greeting():
         cfg = Config(
             host=DATABRICKS_HOST_URL, credentials_provider=credentials_provider
         )
         databricks_user_info = CurrentUserAPI(ApiClient(cfg)).me()
         return f"Hello, {databricks_user_info.display_name}!"
```

### Comparing `posit-sdk-0.1.dev2/examples/connect/fastapi/README.md` & `posit_sdk-0.2.0/examples/connect/fastapi/README.md`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/examples/connect/fastapi/app.py` & `posit_sdk-0.2.0/examples/connect/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/examples/connect/flask/README.md` & `posit_sdk-0.2.0/examples/connect/flask/README.md`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/examples/connect/flask/app.py` & `posit_sdk-0.2.0/examples/connect/flask/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     """
     Flask example API that returns the first few rows from
     a table hosted in Databricks.
     """
     global rows
 
     session_token = request.headers.get("Posit-Connect-User-Session-Token")
-    credentials_provider = viewer_credentials_provider(user_session_token=session_token)
+    credentials_provider = viewer_credentials_provider(
+        user_session_token=session_token
+    )
 
     if rows is None:
         query = "SELECT * FROM samples.nyctaxi.trips LIMIT 10;"
 
         with sql.connect(
             server_hostname=DATABRICKS_HOST,
             http_path=SQL_HTTP_PATH,
```

### Comparing `posit-sdk-0.1.dev2/examples/connect/shiny-python/README.md` & `posit_sdk-0.2.0/examples/connect/shiny-python/README.md`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/examples/connect/shiny-python/app.py` & `posit_sdk-0.2.0/examples/connect/shiny-python/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,32 +20,37 @@
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     """
     Shiny for Python example application that shows user information and
     the first few rows from a table hosted in Databricks.
     """
-
-    session_token = session.http_conn.headers.get("Posit-Connect-User-Session-Token")
-    credentials_provider = viewer_credentials_provider(user_session_token=session_token)
+    session_token = session.http_conn.headers.get(
+        "Posit-Connect-User-Session-Token"
+    )
+    credentials_provider = viewer_credentials_provider(
+        user_session_token=session_token
+    )
 
     @render.data_frame
     def result():
         query = "SELECT * FROM samples.nyctaxi.trips LIMIT 10;"
 
         with sql.connect(
             server_hostname=DATABRICKS_HOST,
             http_path=SQL_HTTP_PATH,
             auth_type="databricks-oauth",
             credentials_provider=credentials_provider,
         ) as connection:
             with connection.cursor() as cursor:
                 cursor.execute(query)
                 rows = cursor.fetchall()
-                df = pd.DataFrame(rows, columns=[col[0] for col in cursor.description])
+                df = pd.DataFrame(
+                    rows, columns=[col[0] for col in cursor.description]
+                )
                 return df
 
     @render.text
     def text():
         cfg = Config(
             host=DATABRICKS_HOST_URL, credentials_provider=credentials_provider
         )
```

### Comparing `posit-sdk-0.1.dev2/examples/connect/streamlit/README.md` & `posit_sdk-0.2.0/examples/connect/streamlit/README.md`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/examples/connect/streamlit/app.py` & `posit_sdk-0.2.0/examples/connect/streamlit/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,25 @@
 import streamlit as st
 from streamlit.web.server.websocket_headers import _get_websocket_headers
 
 DATABRICKS_HOST = os.getenv("DATABRICKS_HOST")
 DATABRICKS_HOST_URL = f"https://{DATABRICKS_HOST}"
 SQL_HTTP_PATH = os.getenv("DATABRICKS_PATH")
 
-session_token = _get_websocket_headers().get("Posit-Connect-User-Session-Token")
+session_token = _get_websocket_headers().get(
+    "Posit-Connect-User-Session-Token"
+)
 
-credentials_provider = viewer_credentials_provider(user_session_token=session_token)
+credentials_provider = viewer_credentials_provider(
+    user_session_token=session_token
+)
 
-cfg = Config(host=DATABRICKS_HOST_URL, credentials_provider=credentials_provider)
+cfg = Config(
+    host=DATABRICKS_HOST_URL, credentials_provider=credentials_provider
+)
 databricks_user = CurrentUserAPI(ApiClient(cfg)).me()
 st.write(f"Hello, {databricks_user.display_name}!")
 
 with sql.connect(
     server_hostname=DATABRICKS_HOST,
     http_path=SQL_HTTP_PATH,
     auth_type="databricks-oauth",
```

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/README.md` & `posit_sdk-0.2.0/src/posit/connect/README.md`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/config.py` & `posit_sdk-0.2.0/src/posit/connect/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,59 @@
+"""Client configuration."""
+
 import os
 
 from typing import Optional
 
 from . import urls
 
 
 def _get_api_key() -> str:
-    """Gets the API key from the environment variable 'CONNECT_API_KEY'.
+    """Return the system configured api key.
+
+    Reads the environment variable 'CONNECT_API_KEY'.
 
-    Raises:
-        ValueError: if CONNECT_API_KEY is not set or invalid
+    Raises
+    ------
+        ValueError: If CONNECT_API_KEY is not set or invalid
 
-    Returns:
-        The API key
+    Returns
+    -------
+        str
     """
     value = os.environ.get("CONNECT_API_KEY")
     if not value:
         raise ValueError(
             "Invalid value for 'CONNECT_API_KEY': Must be a non-empty string."
         )
     return value
 
 
 def _get_url() -> str:
-    """Gets the endpoint from the environment variable 'CONNECT_SERVER'.
+    """Return the system configured url.
 
-    The `requests` library uses 'endpoint' instead of 'server'. We will use 'endpoint' from here forward for consistency.
+    Reads the environment variable 'CONNECT_SERVER'.
 
-    Raises:
-        ValueError: if CONNECT_SERVER is not set or invalid.
+    Raises
+    ------
+        ValueError: If CONNECT_SERVER is not set or invalid
 
-    Returns:
-        The endpoint.
+    Returns
+    -------
+        str
     """
     value = os.environ.get("CONNECT_SERVER")
     if not value:
         raise ValueError(
             "Invalid value for 'CONNECT_SERVER': Must be a non-empty string."
         )
     return value
 
 
 class Config:
-    """Derived configuration properties"""
+    """Configuration object."""
 
     def __init__(
         self, api_key: Optional[str] = None, url: Optional[str] = None
     ) -> None:
         self.api_key = api_key or _get_api_key()
-        self.url = urls.server_to_api_url(url or _get_url())
-        urls.validate(self.url)
+        self.url = urls.create(url or _get_url())
```

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/external/databricks.py` & `posit_sdk-0.2.0/src/posit/connect/external/databricks.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 HeaderFactory = Callable[[], Dict[str, str]]
 
 
 # https://github.com/databricks/databricks-sdk-py/blob/v0.20.0/databricks/sdk/credentials_provider.py
 # https://github.com/databricks/databricks-sql-python/blob/v3.1.0/src/databricks/sql/auth/authenticators.py
 # In order to keep compatibility with the Databricks SDK
 class CredentialsProvider(abc.ABC):
-    """CredentialsProvider is the protocol (call-side interface)
-    for authenticating requests to Databricks REST APIs"""
+    """Protocol Databricks authentication.
+
+    A call-side interface for the Databricks Rest API.
+    """
 
     @abc.abstractmethod
     def auth_type(self) -> str:
         raise NotImplementedError
 
     @abc.abstractmethod
     def __call__(self, *args, **kwargs) -> HeaderFactory:
@@ -30,17 +32,17 @@
         self.user_session_token = user_session_token
 
     def auth_type(self) -> str:
         return "posit-oauth-integration"
 
     def __call__(self, *args, **kwargs) -> HeaderFactory:
         def inner() -> Dict[str, str]:
-            access_token = self.posit_oauth.get_credentials(self.user_session_token)[
-                "access_token"
-            ]
+            access_token = self.posit_oauth.get_credentials(
+                self.user_session_token
+            )["access_token"]
             return {"Authorization": f"Bearer {access_token}"}
 
         return inner
 
 
 # Use this environment variable to determine if the
 # client SDK was initialized from a piece of content running on a Connect server.
@@ -62,12 +64,14 @@
     # If the user-session-token wasn't provided and we're running on Connect then we raise an exception.
     # user_session_token is required to impersonate the viewer.
     if user_session_token is None:
         raise ValueError(
             "The user-session-token is required for viewer authentication."
         )
 
-    return PositOAuthIntegrationCredentialsProvider(client.oauth, user_session_token)
+    return PositOAuthIntegrationCredentialsProvider(
+        client.oauth, user_session_token
+    )
 
 
 def service_account_credentials_provider(client: Optional[Client] = None):
     raise NotImplementedError
```

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/hooks.py` & `posit_sdk-0.2.0/src/posit/connect/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,14 @@
     if response.status_code >= 400:
         try:
             data = response.json()
             error_code = data["code"]
             message = data["error"]
             http_status = response.status_code
             http_status_message = responses[http_status]
-            raise ClientError(error_code, message, http_status, http_status_message)
+            raise ClientError(
+                error_code, message, http_status, http_status_message
+            )
         except JSONDecodeError:
             # No JSON error message from Connect, so just raise
             response.raise_for_status()
     return response
```

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/me.py` & `posit_sdk-0.2.0/src/posit/connect/me.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,13 +10,14 @@
     """
     Gets the current user.
 
     Args:
         config (Config): The configuration object containing the URL.
         session (requests.Session): The session object used for making HTTP requests.
 
-    Returns:
+    Returns
+    -------
         User: The current user.
     """
-    url = urls.append_path(config.url, "v1/user")
+    url = urls.append(config.url, "v1/user")
     response = session.get(url)
     return User(config, session, **response.json())
```

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/oauth.py` & `posit_sdk-0.2.0/src/posit/connect/oauth.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,21 @@
     access_token: str
     issued_token_type: str
     token_type: str
 
 
 class OAuthIntegration:
     def __init__(self, config: Config, session: Session) -> None:
-        self.url = urls.append_path(config.url, "v1/oauth/integrations/credentials")
+        self.url = urls.append(config.url, "v1/oauth/integrations/credentials")
         self.config = config
         self.session = session
 
-    def get_credentials(self, user_session_token: Optional[str] = None) -> Credentials:
+    def get_credentials(
+        self, user_session_token: Optional[str] = None
+    ) -> Credentials:
         # craft a basic credential exchange request where the self.config.api_key owner
         # is requesting their own credentials
         data = dict()
         data["grant_type"] = "urn:ietf:params:oauth:grant-type:token-exchange"
         data["subject_token_type"] = "urn:posit:connect:api-key"
         data["subject_token"] = self.config.api_key
```

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/paginator.py` & `posit_sdk-0.2.0/src/posit/connect/paginator.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 
 @dataclass
 class Page:
     """
     Represents a page of results returned by the paginator.
 
-    Attributes:
+    Attributes
+    ----------
         current_page (int): The current page number.
         total (int): The total number of results.
         results (List[dict]): The list of results on the current page.
     """
 
     current_page: int
     total: int
@@ -28,40 +29,46 @@
     """
     A class for paginating through API results.
 
     Args:
         session (requests.Session): The session object to use for making API requests.
         url (str): The URL of the paginated API endpoint.
 
-    Attributes:
+    Attributes
+    ----------
         session (requests.Session): The session object to use for making API requests.
         url (str): The URL of the paginated API endpoint.
     """
 
-    def __init__(self, session: requests.Session, url: str) -> None:
+    def __init__(
+        self, session: requests.Session, url: str, params: dict = {}
+    ) -> None:
         self.session = session
         self.url = url
+        self.params = params
 
     def fetch_results(self) -> List[dict]:
         """
         Fetches and returns all the results from the paginated API endpoint.
 
-        Returns:
+        Returns
+        -------
             A list of dictionaries representing the fetched results.
         """
         results = []
         for page in self.fetch_pages():
             results.extend(page.results)
         return results
 
     def fetch_pages(self) -> Generator[Page, None, None]:
         """
         Fetches pages of results from the API.
 
-        Yields:
+        Yields
+        ------
             Page: A page of results from the API.
         """
         count = 0
         page_number = 1
         while True:
             page = self.fetch_page(page_number)
             page_number += 1
@@ -82,14 +89,19 @@
     def fetch_page(self, page_number: int) -> Page:
         """
         Fetches a specific page of data from the API.
 
         Args:
             page_number (int): The page number to fetch.
 
-        Returns:
+        Returns
+        -------
             Page: The fetched page object.
 
         """
-        params = {"page_number": page_number, "page_size": _MAX_PAGE_SIZE}
+        params = {
+            **self.params,
+            "page_number": page_number,
+            "page_size": _MAX_PAGE_SIZE,
+        }
         response = self.session.get(self.url, params=params)
         return Page(**response.json())
```

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/urls.py` & `posit_sdk-0.2.0/src/posit/connect/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,89 @@
 from __future__ import annotations
 
 import posixpath
 
 from urllib.parse import urlsplit, urlunsplit
 
+Url = str
 
-def server_to_api_url(url: str) -> str:
-    """
-    Fixes the given URL by appending '__api__' if it doesn't already end with it.
 
-    Args:
-        url (str): The URL to fix.
+def create(url: str) -> Url:
+    """Create a Url.
 
-    Returns:
-        str: The fixed URL.
-    """
-    url = url.rstrip("/")
-    if not url.endswith("__api__"):
-        return append_path(url, "__api__")
-    return url
+    Asserts that the Url is a proper Posit Connect endpoint. The path '__api__' is appended to the Url if it isn't already present.
 
+    Parameters
+    ----------
+    url : str
+        The original Url.
+
+    Returns
+    -------
+    Url
+        The validated and formatted Url.
+
+    Raises
+    ------
+    ValueError
+        The Url is missing a scheme.
+    ValueError
+        The Url is missing a network location (i.e., a domain name).
+
+    Examples
+    --------
+    >>> urls.create("http://example.com")
+    http://example.com/__api__
 
-def validate(url: str) -> None:
-    """
-    Check if the given URL is valid.
-
-    Args:
-        url (str): The URL to be validated.
+    >>> urls.create("http://example.com/__api__")
+    http://example.com/__api__
 
-    Returns:
-        bool: True if the URL is valid, False otherwise.
-
-    Raises:
-        ValueError: If the URL is missing a scheme or is not absolute.
     """
     split = urlsplit(url, allow_fragments=False)
     if not split.scheme:
         raise ValueError(
             f"url must specify a scheme (e.g., http://example.com/__api__): {url}"
         )
 
     if not split.netloc:
         raise ValueError(
             f"url must be absolute (e.g., http://example.com/__api__): {url}"
         )
 
+    url = url.rstrip("/")
+    if not url.endswith("__api__"):
+        url = append(url, "__api__")
+
+    return url
 
-def append_path(url: str, path: str) -> str:
-    """
-    Appends a path to a URL.
 
-    Args:
-        url (str): The original URL.
-        path (str): The path to append.
+def append(url: Url, path: str) -> Url:
+    """Append a path to a Url.
 
-    Returns:
-        str: The modified URL with the appended path.
+    Parameters
+    ----------
+    url : Url
+        A valid Url.
+    path : str
+        A valid Url path.
+
+    Returns
+    -------
+    Url
+        The original Url with the path appended to the end.
+
+    Examples
+    --------
+    >>> url = urls.create("http://example.com/__api__")
+    >>> urls.append(url, "path")
+    http://example.com/__api__/path
     """
-    # See https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlsplit
-    split = urlsplit(url, allow_fragments=False)
     # Removes leading '/' from path to avoid double slashes.
     path = path.lstrip("/")
-    # Prepend the path with the existing URL path.
+    # Removes trailing '/' from path to avoid double slashes.
+    path = path.rstrip("/")
+    # See https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlsplit
+    split = urlsplit(url, allow_fragments=False)
+    # Append the path to unmodified Url path.
     path = posixpath.join(split.path, path)
     # See https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlunsplit
     return urlunsplit((split.scheme, split.netloc, path, split.query, None))
```

### Comparing `posit-sdk-0.1.dev2/src/posit/connect/users.py` & `posit_sdk-0.2.0/src/posit/connect/users.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,35 +62,37 @@
         Locks the user account.
 
         .. warning:: You cannot unlock your own account. Once an account is locked, only an admin can unlock it.
 
         Args:
             force (bool, optional): If set to True, overrides lock protection allowing a user to lock their own account. Defaults to False.
 
-        Returns:
+        Returns
+        -------
             None
         """
         _me = me.get(self.config, self.session)
         if _me.guid == self.guid and not force:
             raise RuntimeError(
                 "You cannot lock your own account. Set force=True to override this behavior."
             )
-        url = urls.append_path(self.config.url, f"v1/users/{self.guid}/lock")
+        url = urls.append(self.config.url, f"v1/users/{self.guid}/lock")
         body = {"locked": True}
         self.session.post(url, json=body)
         super().update(locked=True)
 
     def unlock(self):
         """
         Unlocks the user account.
 
-        Returns:
+        Returns
+        -------
             None
         """
-        url = urls.append_path(self.config.url, f"v1/users/{self.guid}/lock")
+        url = urls.append(self.config.url, f"v1/users/{self.guid}/lock")
         body = {"locked": False}
         self.session.post(url, json=body)
         super().update(locked=False)
 
     @overload
     def update(
         self,
@@ -106,99 +108,121 @@
         Args:
             email (str): The email address for the user.
             username (str): The username for the user.
             first_name (str): The first name for the user.
             last_name (str): The last name for the user.
             user_role (str): The role for the user.
 
-        Returns:
+        Returns
+        -------
             None
         """
         ...
 
     @overload
     def update(self, *args, **kwargs) -> None:
         """
         Update the user.
 
         Args:
             *args
             **kwargs
 
-        Returns:
+        Returns
+        -------
             None
         """
         ...
 
     def update(self, *args, **kwargs) -> None:
         """
         Update the user.
 
         Args:
             *args
             **kwargs
 
-        Returns:
+        Returns
+        -------
             None
         """
         body = dict(*args, **kwargs)
-        url = urls.append_path(self.config.url, f"v1/users/{self.guid}")
+        url = urls.append(self.config.url, f"v1/users/{self.guid}")
         response = self.session.put(url, json=body)
         super().update(**response.json())
 
 
-class Users(Resources[User]):
+class Users(Resources):
     def __init__(self, config: Config, session: requests.Session) -> None:
-        self.url = urls.append_path(config.url, "v1/users")
+        self.url = urls.append(config.url, "v1/users")
         self.config = config
         self.session = session
 
-    def find(self) -> List[User]:
-        paginator = Paginator(self.session, self.url)
+    @overload
+    def find(
+        self,
+        prefix: str = ...,
+        user_role: str = ...,
+        account_status: str = ...,
+    ) -> List[User]:
+        ...
+
+    @overload
+    def find(self, *args, **kwargs) -> List[User]:
+        ...
+
+    def find(self, *args, **kwargs):
+        params = dict(*args, **kwargs)
+        paginator = Paginator(self.session, self.url, params=params)
         results = paginator.fetch_results()
         return [
             User(
                 config=self.config,
                 session=self.session,
                 **user,
             )
             for user in results
         ]
 
-    def find_one(self) -> User | None:
-        paginator = Paginator(self.session, self.url)
+    @overload
+    def find_one(
+        self,
+        prefix: str = ...,
+        user_role: str = ...,
+        account_status: str = ...,
+    ) -> User | None:
+        ...
+
+    @overload
+    def find_one(self, *args, **kwargs) -> User | None:
+        ...
+
+    def find_one(self, *args, **kwargs) -> User | None:
+        params = dict(*args, **kwargs)
+        paginator = Paginator(self.session, self.url, params=params)
         pages = paginator.fetch_pages()
         results = (result for page in pages for result in page.results)
         users = (
             User(
                 config=self.config,
                 session=self.session,
                 **result,
             )
             for result in results
         )
         return next(users, None)
 
     def get(self, id: str) -> User:
-        url = urls.append_path(self.config.url, f"v1/users/{id}")
+        url = urls.append(self.config.url, f"v1/users/{id}")
         response = self.session.get(url)
         return User(
             config=self.config,
             session=self.session,
             **response.json(),
         )
 
-    def create(self) -> User:
-        raise NotImplementedError()
-
-    def update(self) -> User:
-        raise NotImplementedError()
-
-    def delete(self) -> None:
-        raise NotImplementedError()
-
     def count(self) -> int:
         response: requests.Response = self.session.get(
             self.url, params={"page_size": 1}
         )
         result: dict = response.json()
         return result["total"]
```

### Comparing `posit-sdk-0.1.dev2/src/posit_sdk.egg-info/PKG-INFO` & `posit_sdk-0.2.0/src/posit_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posit-sdk
-Version: 0.1.dev2
+Version: 0.2.0
 Summary: Posit SDK for Python
 License: MIT License
         
         Copyright (c) 2024 posit-dev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,17 +23,18 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Source, https://github.com/posit-dev/posit-sdk-py
 Project-URL: Issues, https://github.com/posit-dev/posit-sdk-py/issues
 Keywords: posit,sdk
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests<3,>=2.31.0
@@ -48,21 +49,40 @@
 
 ```shell
 pip install posit-sdk
 ```
 
 ## Usage
 
+Establish server information and credentials using the following environment variables or when initializing a client. Then checkout some [examples](./examples/0001-overview.qmd) to get started.
+
+> [!CAUTION]
+> It is important to keep your API key safe and secure. Your API key grants access to your account and allows you to make authenticated requests to the Posit API. Treat your API key like a password and avoid sharing it with others. If you suspect that your API key has been compromised, regenerate a new one immediately to maintain the security of your account.
+
+### Option 1 (Preferred)
+
+```shell
+export CONNECT_API_KEY="my-secret-api-key"
+export CONNECT_SERVER="https://example.com/"
+```
+
+```python
+from posit.connect import Client
+
+with Client() as client:
+    print(client)
+```
+
+### Option 2
+
 ```python
 from posit.connect import Client
 
-# If CONNECT_API_KEY and CONNECT_SERVER are set in your environment,
-# they will be picked up, or you can pass them as arguments
-con = Client()
-con.users.find()
+with Client(api_key="my-secret-api-key", url="https://example.com") as client:
+    print(client)
 ```
 
 ## Contributing
 
 We welcome contributions to the Posit SDK for Python! If you would like to contribute, see the [CONTRIBUTING](CONTRIBUTING.md) guide for instructions.
 
 ## Issues
```

### Comparing `posit-sdk-0.1.dev2/src/posit_sdk.egg-info/SOURCES.txt` & `posit_sdk-0.2.0/src/posit_sdk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 requirements.txt
 .github/workflows/conventional-commits.yaml
 .github/workflows/main.yaml
 .github/workflows/pull-request.yaml
 .github/workflows/release.yaml
 .vscode/launch.json
 .vscode/settings.json
+examples/0001-overview.qmd
 examples/__init__.py
 examples/connect/.gitignore
 examples/connect/dash/README.md
 examples/connect/dash/app.py
 examples/connect/dash/requirements.txt
 examples/connect/fastapi/README.md
 examples/connect/fastapi/app.py
@@ -34,45 +35,68 @@
 examples/connect/streamlit/app.py
 examples/connect/streamlit/requirements.txt
 src/posit/__init__.py
 src/posit/_version.py
 src/posit/connect/README.md
 src/posit/connect/__init__.py
 src/posit/connect/auth.py
+src/posit/connect/bundles.py
 src/posit/connect/client.py
 src/posit/connect/config.py
 src/posit/connect/content.py
+src/posit/connect/cursors.py
 src/posit/connect/errors.py
 src/posit/connect/hooks.py
 src/posit/connect/me.py
 src/posit/connect/oauth.py
 src/posit/connect/paginator.py
+src/posit/connect/permissions.py
 src/posit/connect/resources.py
+src/posit/connect/tasks.py
 src/posit/connect/urls.py
 src/posit/connect/users.py
 src/posit/connect/external/__init__.py
 src/posit/connect/external/databricks.py
+src/posit/connect/metrics/__init__.py
+src/posit/connect/metrics/shiny_usage.py
+src/posit/connect/metrics/usage.py
+src/posit/connect/metrics/visits.py
 src/posit_sdk.egg-info/PKG-INFO
 src/posit_sdk.egg-info/SOURCES.txt
 src/posit_sdk.egg-info/dependency_links.txt
 src/posit_sdk.egg-info/requires.txt
 src/posit_sdk.egg-info/top_level.txt
 tests/posit/connect/api.py
 tests/posit/connect/test_auth.py
+tests/posit/connect/test_bundles.py
 tests/posit/connect/test_client.py
 tests/posit/connect/test_config.py
 tests/posit/connect/test_content.py
 tests/posit/connect/test_errors.py
 tests/posit/connect/test_hooks.py
 tests/posit/connect/test_oauth.py
+tests/posit/connect/test_permissions.py
 tests/posit/connect/test_resources.py
+tests/posit/connect/test_tasks.py
 tests/posit/connect/test_urls.py
 tests/posit/connect/test_users.py
 tests/posit/connect/__api__/v1/content.json
 tests/posit/connect/__api__/v1/user.json
-tests/posit/connect/__api__/v1/users.json
-tests/posit/connect/__api__/v1/users?page_number=1&page_size=500.json
-tests/posit/connect/__api__/v1/users?page_number=2&page_size=500.json
+tests/posit/connect/__api__/v1/users?page_number=1&page_size=500.jsonc
+tests/posit/connect/__api__/v1/users?page_number=2&page_size=500.jsonc
 tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066.json
+tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles.json
+tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/permissions.json
+tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles/101.json
+tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/bundles/101/download/bundle.tar.gz
+tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066/permissions/94.json
+tests/posit/connect/__api__/v1/instrumentation/content/visits?limit=500&next=23948901087.json
+tests/posit/connect/__api__/v1/instrumentation/content/visits?limit=500.json
+tests/posit/connect/__api__/v1/instrumentation/shiny/usage?limit=500&next=23948901087.json
+tests/posit/connect/__api__/v1/instrumentation/shiny/usage?limit=500.json
+tests/posit/connect/__api__/v1/tasks/jXhOhdm5OOSkGhJw.json
 tests/posit/connect/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json
 tests/posit/connect/__api__/v1/users/a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6.json
-tests/posit/connect/external/test_databricks.py
+tests/posit/connect/external/test_databricks.py
+tests/posit/connect/metrics/test_shiny_usage.py
+tests/posit/connect/metrics/test_usage.py
+tests/posit/connect/metrics/test_visits.py
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066.json` & `posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content/f2f37341-e21d-3d80-c698-a935ad614066.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -87,8 +87,8 @@
 00000560: 223a 2022 6874 7470 733a 2f2f 636f 6e6e  ": "https://conn
 00000570: 6563 742e 6578 616d 706c 652f 636f 6e6e  ect.example/conn
 00000580: 6563 742f 232f 6170 7073 2f66 3266 3337  ect/#/apps/f2f37
 00000590: 3334 312d 6532 3164 2d33 6438 302d 6336  341-e21d-3d80-c6
 000005a0: 3938 2d61 3933 3561 6436 3134 3036 3622  98-a935ad614066"
 000005b0: 2c0a 2020 2020 2261 7070 5f72 6f6c 6522  ,.    "app_role"
 000005c0: 3a20 2276 6965 7765 7222 2c0a 2020 2020  : "viewer",.    
-000005d0: 2269 6422 3a20 2238 3237 3422 0a7d       "id": "8274".}
+000005d0: 2269 6422 3a20 2238 3237 3422 0a7d 0a    "id": "8274".}.
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/content.json` & `posit_sdk-0.2.0/tests/posit/connect/__api__/v1/content.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9700336700336699%*

 * *Differences: {'0': "{'owner': OrderedDict([('guid', 'a01792e3-2e67-402e-99af-be04a48da074'), ('username', "*

 * *      "'al'), ('first_name', 'Alice'), ('last_name', 'User')])}",*

 * * '1': "{'tags': [OrderedDict([('id', '7'), ('name', 'Performance'), ('parent_id', '5'), "*

 * *      "('created_time', '2019-10-08T19:45:23Z'), ('updated_time', '2019-10-08T19:45:23Z')]), "*

 * *      "OrderedDict([('id', '34'), ('name', 'Data'), ('parent_id', '3'), ('created_time', "*

 * *      "'2023-05-18T16:41:59Z'), ('updated_time', '2023-05-18T16:41:59Z')])] […]*

```diff
@@ -27,14 +27,20 @@
         "max_conns_per_process": null,
         "max_processes": null,
         "memory_limit": null,
         "memory_request": null,
         "min_processes": null,
         "name": "team-admin-dashboard",
         "nvidia_gpu_limit": null,
+        "owner": {
+            "first_name": "Alice",
+            "guid": "a01792e3-2e67-402e-99af-be04a48da074",
+            "last_name": "User",
+            "username": "al"
+        },
         "owner_guid": "a01792e3-2e67-402e-99af-be04a48da074",
         "parameterized": false,
         "py_environment_management": null,
         "py_version": null,
         "quarto_version": null,
         "r_environment_management": true,
         "r_version": "3.5.3",
@@ -72,25 +78,47 @@
         "max_conns_per_process": null,
         "max_processes": null,
         "memory_limit": null,
         "memory_request": null,
         "min_processes": null,
         "name": "Performance-Data-1671216053560",
         "nvidia_gpu_limit": null,
+        "owner": {
+            "first_name": "Bob",
+            "guid": "87c12c08-11cd-4de1-8da3-12a7579c4998",
+            "last_name": "Loblaw",
+            "username": "robert"
+        },
         "owner_guid": "87c12c08-11cd-4de1-8da3-12a7579c4998",
         "parameterized": false,
         "py_environment_management": true,
         "py_version": "3.9.17",
         "quarto_version": "1.3.340",
         "r_environment_management": null,
         "r_version": null,
         "read_timeout": null,
         "run_as": null,
         "run_as_current_user": false,
         "service_account_name": null,
+        "tags": [
+            {
+                "created_time": "2019-10-08T19:45:23Z",
+                "id": "7",
+                "name": "Performance",
+                "parent_id": "5",
+                "updated_time": "2019-10-08T19:45:23Z"
+            },
+            {
+                "created_time": "2023-05-18T16:41:59Z",
+                "id": "34",
+                "name": "Data",
+                "parent_id": "3",
+                "updated_time": "2023-05-18T16:41:59Z"
+            }
+        ],
         "title": "Performance Data"
     },
     {
         "access_type": "logged_in",
         "amd_gpu_limit": null,
         "app_mode": "python-streamlit",
         "app_role": "viewer",
@@ -117,14 +145,20 @@
         "max_conns_per_process": null,
         "max_processes": null,
         "memory_limit": null,
         "memory_request": null,
         "min_processes": null,
         "name": "My-Streamlit-app",
         "nvidia_gpu_limit": null,
+        "owner": {
+            "first_name": "Carlos",
+            "guid": "20a79ce3-6e87-4522-9faf-be24228800a4",
+            "last_name": "User",
+            "username": "carlos12"
+        },
         "owner_guid": "20a79ce3-6e87-4522-9faf-be24228800a4",
         "parameterized": false,
         "py_environment_management": true,
         "py_version": "3.9.17",
         "quarto_version": null,
         "r_environment_management": null,
         "r_version": null,
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/__api__/v1/users?page_number=1&page_size=500.json` & `posit_sdk-0.2.0/tests/posit/connect/__api__/v1/users?page_number=2&page_size=500.jsonc`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,45 @@
-00000000: 7b0a 2020 2020 2272 6573 756c 7473 223a  {.    "results":
-00000010: 205b 0a20 2020 2020 2020 207b 0a20 2020   [.        {.   
-00000020: 2020 2020 2020 2020 2022 656d 6169 6c22           "email"
-00000030: 3a20 2261 6c69 6365 4063 6f6e 6e65 6374  : "alice@connect
-00000040: 2e65 7861 6d70 6c65 222c 0a20 2020 2020  .example",.     
-00000050: 2020 2020 2020 2022 7573 6572 6e61 6d65         "username
-00000060: 223a 2022 616c 222c 0a20 2020 2020 2020  ": "al",.       
-00000070: 2020 2020 2022 6669 7273 745f 6e61 6d65       "first_name
-00000080: 223a 2022 416c 6963 6522 2c0a 2020 2020  ": "Alice",.    
-00000090: 2020 2020 2020 2020 226c 6173 745f 6e61          "last_na
-000000a0: 6d65 223a 2022 5573 6572 222c 0a20 2020  me": "User",.   
-000000b0: 2020 2020 2020 2020 2022 7573 6572 5f72           "user_r
-000000c0: 6f6c 6522 3a20 2270 7562 6c69 7368 6572  ole": "publisher
-000000d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000000e0: 6372 6561 7465 645f 7469 6d65 223a 2022  created_time": "
-000000f0: 3230 3137 2d30 382d 3038 5431 353a 3234  2017-08-08T15:24
-00000100: 3a33 325a 222c 0a20 2020 2020 2020 2020  :32Z",.         
-00000110: 2020 2022 7570 6461 7465 645f 7469 6d65     "updated_time
-00000120: 223a 2022 3230 3233 2d30 332d 3032 5432  ": "2023-03-02T2
-00000130: 303a 3235 3a30 365a 222c 0a20 2020 2020  0:25:06Z",.     
-00000140: 2020 2020 2020 2022 6163 7469 7665 5f74         "active_t
-00000150: 696d 6522 3a20 2232 3031 382d 3035 2d30  ime": "2018-05-0
-00000160: 3954 3136 3a35 383a 3435 5a22 2c0a 2020  9T16:58:45Z",.  
-00000170: 2020 2020 2020 2020 2020 2263 6f6e 6669            "confi
-00000180: 726d 6564 223a 2074 7275 652c 0a20 2020  rmed": true,.   
-00000190: 2020 2020 2020 2020 2022 6c6f 636b 6564           "locked
-000001a0: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
-000001b0: 2020 2020 2020 2267 7569 6422 3a20 2261        "guid": "a
-000001c0: 3031 3739 3265 332d 3265 3637 2d34 3032  01792e3-2e67-402
-000001d0: 652d 3939 6166 2d62 6530 3461 3438 6461  e-99af-be04a48da
-000001e0: 3037 3422 0a20 2020 2020 2020 207d 2c0a  074".        },.
-000001f0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000200: 2020 2020 2020 2265 6d61 696c 223a 2022        "email": "
-00000210: 626f 6240 636f 6e6e 6563 742e 6578 616d  bob@connect.exam
-00000220: 706c 6522 2c0a 2020 2020 2020 2020 2020  ple",.          
-00000230: 2020 2275 7365 726e 616d 6522 3a20 2272    "username": "r
-00000240: 6f62 6572 7422 2c0a 2020 2020 2020 2020  obert",.        
-00000250: 2020 2020 2266 6972 7374 5f6e 616d 6522      "first_name"
-00000260: 3a20 2242 6f62 222c 0a20 2020 2020 2020  : "Bob",.       
-00000270: 2020 2020 2022 6c61 7374 5f6e 616d 6522       "last_name"
-00000280: 3a20 224c 6f62 6c61 7722 2c0a 2020 2020  : "Loblaw",.    
-00000290: 2020 2020 2020 2020 2275 7365 725f 726f          "user_ro
-000002a0: 6c65 223a 2022 7075 626c 6973 6865 7222  le": "publisher"
-000002b0: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
-000002c0: 7265 6174 6564 5f74 696d 6522 3a20 2232  reated_time": "2
-000002d0: 3032 332d 3031 2d30 3654 3139 3a34 373a  023-01-06T19:47:
-000002e0: 3239 5a22 2c0a 2020 2020 2020 2020 2020  29Z",.          
-000002f0: 2020 2275 7064 6174 6564 5f74 696d 6522    "updated_time"
-00000300: 3a20 2232 3032 332d 3035 2d30 3554 3139  : "2023-05-05T19
-00000310: 3a30 383a 3435 5a22 2c0a 2020 2020 2020  :08:45Z",.      
-00000320: 2020 2020 2020 2261 6374 6976 655f 7469        "active_ti
-00000330: 6d65 223a 2022 3230 3233 2d30 352d 3035  me": "2023-05-05
-00000340: 5432 303a 3239 3a31 315a 222c 0a20 2020  T20:29:11Z",.   
-00000350: 2020 2020 2020 2020 2022 636f 6e66 6972           "confir
-00000360: 6d65 6422 3a20 7472 7565 2c0a 2020 2020  med": true,.    
-00000370: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
-00000380: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00000390: 2020 2020 2022 6775 6964 223a 2022 3837       "guid": "87
-000003a0: 6331 3263 3038 2d31 3163 642d 3464 6531  c12c08-11cd-4de1
-000003b0: 2d38 6461 332d 3132 6137 3537 3963 3439  -8da3-12a7579c49
-000003c0: 3938 220a 2020 2020 2020 2020 7d0a 2020  98".        }.  
-000003d0: 2020 5d2c 0a20 2020 2022 6375 7272 656e    ],.    "curren
-000003e0: 745f 7061 6765 223a 2031 2c0a 2020 2020  t_page": 1,.    
-000003f0: 2274 6f74 616c 223a 2033 0a7d            "total": 3.}
+00000000: 2f2f 2041 2073 7562 7365 7175 656e 7420  // A subsequent 
+00000010: 7369 6e67 6c65 2070 6167 6520 7265 7370  single page resp
+00000020: 6f6e 7365 2066 726f 6d20 7468 6520 272f  onse from the '/
+00000030: 7631 2f75 7365 7273 2720 656e 6470 6f69  v1/users' endpoi
+00000040: 6e74 2e0a 2f2f 0a2f 2f20 5468 6973 2066  nt..//.// This f
+00000050: 696c 6520 6973 2074 7970 6963 616c 6c79  ile is typically
+00000060: 2075 7365 6420 696e 2063 6f6e 6a75 6e63   used in conjunc
+00000070: 7469 6f6e 2077 6974 6820 7631 2f75 7365  tion with v1/use
+00000080: 7273 3f70 6167 655f 6e75 6d62 6572 3d31  rs?page_number=1
+00000090: 2670 6167 655f 7369 7a65 3d35 3030 2e6a  &page_size=500.j
+000000a0: 736f 6e63 0a0a 7b0a 2020 2020 2272 6573  sonc..{.    "res
+000000b0: 756c 7473 223a 205b 0a20 2020 2020 2020  ults": [.       
+000000c0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000000d0: 656d 6169 6c22 3a20 2263 6172 6c6f 7340  email": "carlos@
+000000e0: 636f 6e6e 6563 742e 6578 616d 706c 6522  connect.example"
+000000f0: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
+00000100: 7365 726e 616d 6522 3a20 2263 6172 6c6f  sername": "carlo
+00000110: 7331 3222 2c0a 2020 2020 2020 2020 2020  s12",.          
+00000120: 2020 2266 6972 7374 5f6e 616d 6522 3a20    "first_name": 
+00000130: 2243 6172 6c6f 7322 2c0a 2020 2020 2020  "Carlos",.      
+00000140: 2020 2020 2020 226c 6173 745f 6e61 6d65        "last_name
+00000150: 223a 2022 5573 6572 222c 0a20 2020 2020  ": "User",.     
+00000160: 2020 2020 2020 2022 7573 6572 5f72 6f6c         "user_rol
+00000170: 6522 3a20 2270 7562 6c69 7368 6572 222c  e": "publisher",
+00000180: 0a20 2020 2020 2020 2020 2020 2022 6372  .            "cr
+00000190: 6561 7465 645f 7469 6d65 223a 2022 3230  eated_time": "20
+000001a0: 3139 2d30 392d 3039 5431 353a 3234 3a33  19-09-09T15:24:3
+000001b0: 325a 222c 0a20 2020 2020 2020 2020 2020  2Z",.           
+000001c0: 2022 7570 6461 7465 645f 7469 6d65 223a   "updated_time":
+000001d0: 2022 3230 3232 2d30 332d 3032 5432 303a   "2022-03-02T20:
+000001e0: 3235 3a30 365a 222c 0a20 2020 2020 2020  25:06Z",.       
+000001f0: 2020 2020 2022 6163 7469 7665 5f74 696d       "active_tim
+00000200: 6522 3a20 2232 3032 302d 3035 2d31 3154  e": "2020-05-11T
+00000210: 3136 3a35 383a 3435 5a22 2c0a 2020 2020  16:58:45Z",.    
+00000220: 2020 2020 2020 2020 2263 6f6e 6669 726d          "confirm
+00000230: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+00000240: 2020 2020 2020 2022 6c6f 636b 6564 223a         "locked":
+00000250: 2066 616c 7365 2c0a 2020 2020 2020 2020   false,.        
+00000260: 2020 2020 2267 7569 6422 3a20 2232 3061      "guid": "20a
+00000270: 3739 6365 332d 3665 3837 2d34 3532 322d  79ce3-6e87-4522-
+00000280: 3966 6166 2d62 6532 3432 3238 3830 3061  9faf-be24228800a
+00000290: 3422 0a20 2020 2020 2020 207d 0a20 2020  4".        }.   
+000002a0: 205d 2c0a 2020 2020 2263 7572 7265 6e74   ],.    "current
+000002b0: 5f70 6167 6522 3a20 322c 0a20 2020 2022  _page": 2,.    "
+000002c0: 746f 7461 6c22 3a20 330a 7d0a            total": 3.}.
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/test_client.py` & `posit_sdk-0.2.0/tests/posit/connect/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,35 +96,43 @@
         )
 
     def test_get(self, MockSession):
         api_key = "foobar"
         url = "http://foo.bar/__api__"
         client = Client(api_key=api_key, url=url)
         client.get("/foo")
-        client.session.get.assert_called_once_with("http://foo.bar/__api__/foo")
+        client.session.get.assert_called_once_with(
+            "http://foo.bar/__api__/foo"
+        )
 
     def test_post(self, MockSession):
         api_key = "foobar"
         url = "http://foo.bar/__api__"
         client = Client(api_key=api_key, url=url)
         client.post("/foo")
-        client.session.post.assert_called_once_with("http://foo.bar/__api__/foo")
+        client.session.post.assert_called_once_with(
+            "http://foo.bar/__api__/foo"
+        )
 
     def test_put(self, MockSession):
         api_key = "foobar"
         url = "http://foo.bar/__api__"
         client = Client(api_key=api_key, url=url)
         client.put("/foo")
-        client.session.put.assert_called_once_with("http://foo.bar/__api__/foo")
+        client.session.put.assert_called_once_with(
+            "http://foo.bar/__api__/foo"
+        )
 
     def test_patch(self, MockSession):
         api_key = "foobar"
         url = "http://foo.bar/__api__"
         client = Client(api_key=api_key, url=url)
         client.patch("/foo")
-        client.session.patch.assert_called_once_with("http://foo.bar/__api__/foo")
+        client.session.patch.assert_called_once_with(
+            "http://foo.bar/__api__/foo"
+        )
 
     def test_delete(self, MockSession):
         api_key = "foobar"
         url = "http://foo.bar/__api__"
         client = Client(api_key=api_key, url=url)
         client.delete("/foo")
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/test_config.py` & `posit_sdk-0.2.0/tests/posit/connect/test_config.py`

 * *Files identical despite different names*

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/test_errors.py` & `posit_sdk-0.2.0/tests/posit/connect/test_errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 class TestClientError:
     def test(self):
         error_code = 0
         error_message = "foo"
         http_status = 404
         http_message = "Foo Bar"
         with pytest.raises(
-            ClientError, match=r"foo \(Error Code: 0, HTTP Status: 404 Foo Bar\)"
+            ClientError,
+            match=r"foo \(Error Code: 0, HTTP Status: 404 Foo Bar\)",
         ):
             raise ClientError(
                 error_code=error_code,
                 error_message=error_message,
                 http_status=http_status,
                 http_message=http_message,
             )
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/test_hooks.py` & `posit_sdk-0.2.0/tests/posit/connect/test_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 
 
 def test_response_client_error_with_json_payload():
     response = Response()
     response.status_code = 400
     response.raw = io.BytesIO(b'{"code":0,"error":"foobar"}')
     with pytest.raises(
-        ClientError, match=r"foobar \(Error Code: 0, HTTP Status: 400 Bad Request\)"
+        ClientError,
+        match=r"foobar \(Error Code: 0, HTTP Status: 400 Bad Request\)",
     ):
         handle_errors(response)
 
 
 def test_response_client_error_without_payload():
     response = Response()
     response.status_code = 404
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/test_oauth.py` & `posit_sdk-0.2.0/tests/posit/connect/test_oauth.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,8 +38,10 @@
                 "access_token": "sdk-user-token",
                 "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
                 "token_type": "Bearer",
             },
         )
         con = Client(api_key="12345", url="https://connect.example/")
         assert con.oauth.get_credentials()["access_token"] == "sdk-user-token"
-        assert con.oauth.get_credentials("cit")["access_token"] == "viewer-token"
+        assert (
+            con.oauth.get_credentials("cit")["access_token"] == "viewer-token"
+        )
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/test_resources.py` & `posit_sdk-0.2.0/tests/posit/connect/test_resources.py`

 * *Files 22% similar despite different names*

```diff
@@ -60,58 +60,7 @@
 
     def test_foo(self):
         k = "foo"
         v = "bar"
         d = dict({k: v})
         r = FakeResource(config, session, **d)
         assert r.foo == v
-
-
-class TestResources(Resources[Any]):
-    def create(self) -> Any:
-        return super().create()  # type: ignore [safe-super]
-
-    def delete(self) -> None:
-        return super().delete()  # type: ignore [safe-super]
-
-    def find(self) -> List[Any]:
-        return super().find()  # type: ignore [safe-super]
-
-    def find_one(self) -> Optional[Any]:
-        return super().find_one()  # type: ignore [safe-super]
-
-    def get(self) -> Any:
-        return super().get()  # type: ignore [safe-super]
-
-    def update(self) -> Any:
-        return super().update()  # type: ignore [safe-super]
-
-    def count(self) -> int:
-        return super().count()  # type: ignore [safe-super]
-
-    def test_create(self):
-        with pytest.raises(NotImplementedError):
-            self.create()
-
-    def test_delete(self):
-        with pytest.raises(NotImplementedError):
-            self.delete()
-
-    def test_find(self):
-        with pytest.raises(NotImplementedError):
-            self.find()
-
-    def test_find_one(self):
-        with pytest.raises(NotImplementedError):
-            self.find_one()
-
-    def test_get(self):
-        with pytest.raises(NotImplementedError):
-            self.get()
-
-    def test_update(self):
-        with pytest.raises(NotImplementedError):
-            self.update()
-
-    def test_count(self):
-        with pytest.raises(NotImplementedError):
-            self.count()
```

### Comparing `posit-sdk-0.1.dev2/tests/posit/connect/test_users.py` & `posit_sdk-0.2.0/tests/posit/connect/test_users.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from unittest.mock import Mock
 
-import pandas as pd
 import pytest
 import requests
 import responses
 
 from posit.connect.client import Client
 from posit.connect.users import User
 
 from .api import load_mock  # type: ignore
 
 session = Mock()
 url = Mock()
 
 
-class TestUser:
+class TestUserAttributes:
     def test_guid(self):
         user = User(session, url)
         assert hasattr(user, "guid")
         assert user.guid is None
         user = User(session, url, guid="test_guid")
         assert user.guid == "test_guid"
 
@@ -88,83 +87,101 @@
     def test_locked(self):
         user = User(session, url)
         assert hasattr(user, "locked")
         assert user.locked is None
         user = User(session, url, locked=False)
         assert user.locked is False
 
+
+class TestUserLock:
     @responses.activate
     def test_lock(self):
         responses.get(
             "https://connect.example/__api__/v1/users/a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6",
-            json=load_mock("v1/users/a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6.json"),
+            json=load_mock(
+                "v1/users/a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6.json"
+            ),
         )
         c = Client(api_key="12345", url="https://connect.example/")
         user = c.users.get("a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6")
         assert user.guid == "a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6"
 
         responses.get(
             "https://connect.example/__api__/v1/user",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
         responses.post(
             "https://connect.example/__api__/v1/users/a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6/lock",
             match=[responses.matchers.json_params_matcher({"locked": True})],
         )
         user.lock()
         assert user.locked
 
     @responses.activate
     def test_lock_self_true(self):
         responses.get(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
         c = Client(api_key="12345", url="https://connect.example/")
         user = c.users.get("20a79ce3-6e87-4522-9faf-be24228800a4")
         assert user.guid == "20a79ce3-6e87-4522-9faf-be24228800a4"
 
         responses.get(
             "https://connect.example/__api__/v1/user",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
         responses.post(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4/lock",
             match=[responses.matchers.json_params_matcher({"locked": True})],
         )
         user.lock(force=True)
         assert user.locked
 
     @responses.activate
     def test_lock_self_false(self):
         responses.get(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
         c = Client(api_key="12345", url="https://connect.example/")
         user = c.users.get("20a79ce3-6e87-4522-9faf-be24228800a4")
         assert user.guid == "20a79ce3-6e87-4522-9faf-be24228800a4"
 
         responses.get(
             "https://connect.example/__api__/v1/user",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
         responses.post(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4/lock",
             match=[responses.matchers.json_params_matcher({"locked": True})],
         )
         with pytest.raises(RuntimeError):
             user.lock(force=False)
         assert not user.locked
 
+
+class TestUserUnlock:
     @responses.activate
     def test_unlock(self):
         responses.get(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
         c = Client(api_key="12345", url="https://connect.example/")
         user = c.users.get("20a79ce3-6e87-4522-9faf-be24228800a4")
         assert user.guid == "20a79ce3-6e87-4522-9faf-be24228800a4"
 
         responses.post(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4/lock",
@@ -172,109 +189,20 @@
         )
         user.unlock()
         assert not user.locked
 
 
 class TestUsers:
     @responses.activate
-    def test_users_find(self):
-        responses.get(
-            "https://connect.example/__api__/v1/users",
-            match=[
-                responses.matchers.query_param_matcher(
-                    {"page_size": 500, "page_number": 1}
-                )
-            ],
-            json=load_mock("v1/users?page_number=1&page_size=500.json"),
-        )
-        responses.get(
-            "https://connect.example/__api__/v1/users",
-            match=[
-                responses.matchers.query_param_matcher(
-                    {"page_size": 500, "page_number": 2}
-                )
-            ],
-            json=load_mock("v1/users?page_number=2&page_size=500.json"),
-        )
-
-        con = Client(api_key="12345", url="https://connect.example/")
-        all_users = con.users.find()
-        assert len(all_users) == 3
-
-        df = pd.DataFrame(all_users)
-        assert isinstance(df, pd.DataFrame)
-        assert df.shape == (3, 11)
-        assert df.columns.to_list() == [
-            "email",
-            "username",
-            "first_name",
-            "last_name",
-            "user_role",
-            "created_time",
-            "updated_time",
-            "active_time",
-            "confirmed",
-            "locked",
-            "guid",
-        ]
-        assert df["username"].to_list() == ["al", "robert", "carlos12"]
-
-    @responses.activate
-    def test_users_find_one(self):
-        responses.get(
-            "https://connect.example/__api__/v1/users",
-            match=[
-                responses.matchers.query_param_matcher(
-                    {"page_size": 500, "page_number": 1}
-                )
-            ],
-            json=load_mock("v1/users?page_number=1&page_size=500.json"),
-        )
-        responses.get(
-            "https://connect.example/__api__/v1/users",
-            match=[
-                responses.matchers.query_param_matcher(
-                    {"page_size": 500, "page_number": 2}
-                )
-            ],
-            json=load_mock("v1/users?page_number=2&page_size=500.json"),
-        )
-
-        con = Client(api_key="12345", url="https://connect.example/")
-        c = con.users.find_one()
-        assert c.username == "al"
-
-    @responses.activate
-    def test_users_find_one_only_gets_necessary_pages(self):
-        responses.get(
-            "https://connect.example/__api__/v1/users",
-            json=load_mock("v1/users?page_number=1&page_size=500.json"),
-        )
-
-        con = Client(api_key="12345", url="https://connect.example/")
-        user = con.users.find_one()
-        assert user.username == "al"
-        assert len(responses.calls) == 1
-
-    @responses.activate
-    def test_users_find_one_finds_nothing(self):
-        responses.get(
-            "https://connect.example/__api__/v1/users",
-            json={"total": 0, "current_page": 1, "results": []},
-        )
-
-        con = Client(api_key="12345", url="https://connect.example/")
-        user = con.users.find_one()
-        assert user is None
-
-    @responses.activate
     def test_users_get(self):
         responses.get(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
 
         con = Client(api_key="12345", url="https://connect.example/")
         carlos = con.users.get("20a79ce3-6e87-4522-9faf-be24228800a4")
         assert carlos.username == "carlos12"
         assert carlos.first_name == "Carlos"
         assert carlos.created_time == "2019-09-09T15:24:32Z"
@@ -295,19 +223,25 @@
         assert carlos.username == "carlos12"
         assert carlos["some_new_field"] == "some_new_value"
 
     @responses.activate
     def test_user_update(self):
         responses.get(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
         patch_request = responses.put(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
-            match=[responses.matchers.json_params_matcher({"first_name": "Carlitos"})],
+            match=[
+                responses.matchers.json_params_matcher(
+                    {"first_name": "Carlitos"}
+                )
+            ],
             json={"first_name": "Carlitos"},
         )
 
         con = Client(api_key="12345", url="https://connect.example/")
         carlos = con.users.get("20a79ce3-6e87-4522-9faf-be24228800a4")
 
         assert patch_request.call_count == 0
@@ -318,15 +252,17 @@
         assert patch_request.call_count == 1
         assert carlos.first_name == "Carlitos"
 
     @responses.activate
     def test_user_update_server_error(self):
         responses.get(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
         responses.put(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
             status=500,
         )
 
         con = Client(api_key="12345", url="https://connect.example/")
@@ -334,15 +270,17 @@
         with pytest.raises(requests.HTTPError, match="500 Server Error"):
             carlos.update(first_name="Carlitos")
 
     @responses.activate
     def test_user_cant_setattr(self):
         responses.get(
             "https://connect.example/__api__/v1/users/20a79ce3-6e87-4522-9faf-be24228800a4",
-            json=load_mock("v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"),
+            json=load_mock(
+                "v1/users/20a79ce3-6e87-4522-9faf-be24228800a4.json"
+            ),
         )
 
         con = Client(api_key="12345", url="https://connect.example/")
         carlos = con.users.get("20a79ce3-6e87-4522-9faf-be24228800a4")
 
         with pytest.raises(
             AttributeError,
@@ -350,13 +288,148 @@
         ):
             carlos.first_name = "Carlitos"
 
     @responses.activate
     def test_count(self):
         responses.get(
             "https://connect.example/__api__/v1/users",
-            json=load_mock("v1/users.json"),
+            json=load_mock("v1/users?page_number=1&page_size=500.jsonc"),
             match=[responses.matchers.query_param_matcher({"page_size": 1})],
         )
         con = Client(api_key="12345", url="https://connect.example/")
         count = con.users.count()
-        assert count == 1
+        assert count == 3
+
+
+class TestUsersFindOne:
+    @responses.activate
+    def test_default(self):
+        # validate first result returned
+        responses.get(
+            "https://connect.example/__api__/v1/users",
+            json=load_mock("v1/users?page_number=1&page_size=500.jsonc"),
+        )
+        con = Client(api_key="12345", url="https://connect.example/")
+        user = con.users.find_one()
+        assert user.username == "al"
+        assert len(responses.calls) == 1
+
+    @responses.activate
+    def test_params(self):
+        mock_get = responses.get(
+            "https://connect.example/__api__/v1/users",
+            match=[
+                responses.matchers.query_param_matcher(
+                    {
+                        "page_size": 500,
+                        "page_number": 1,
+                        "key1": "value1",
+                        "key2": "value2",
+                        "key3": "value3",
+                    }
+                )
+            ],
+            json=load_mock("v1/users?page_number=1&page_size=500.jsonc"),
+        )
+        con = Client(api_key="12345", url="https://connect.example/")
+        con.users.find_one(key1="value1", key2="value2", key3="value3")
+        assert mock_get.call_count == 1
+
+    @responses.activate
+    def test_empty_results(self):
+        responses.get(
+            "https://connect.example/__api__/v1/users",
+            json={"total": 0, "current_page": 1, "results": []},
+        )
+
+        con = Client(api_key="12345", url="https://connect.example/")
+        user = con.users.find_one()
+        assert user is None
+
+
+class TestUsersFind:
+    @responses.activate
+    def test_default(self):
+        # validate response body is parsed and returned
+        responses.get(
+            "https://connect.example/__api__/v1/users",
+            match=[
+                responses.matchers.query_param_matcher(
+                    {"page_size": 500, "page_number": 1}
+                )
+            ],
+            json=load_mock("v1/users?page_number=1&page_size=500.jsonc"),
+        )
+        responses.get(
+            "https://connect.example/__api__/v1/users",
+            match=[
+                responses.matchers.query_param_matcher(
+                    {"page_size": 500, "page_number": 2}
+                )
+            ],
+            json=load_mock("v1/users?page_number=2&page_size=500.jsonc"),
+        )
+        con = Client(api_key="12345", url="https://connect.example/")
+        users = con.users.find()
+        assert len(users) == 3
+        assert users[0] == {
+            "email": "alice@connect.example",
+            "username": "al",
+            "first_name": "Alice",
+            "last_name": "User",
+            "user_role": "publisher",
+            "created_time": "2017-08-08T15:24:32Z",
+            "updated_time": "2023-03-02T20:25:06Z",
+            "active_time": "2018-05-09T16:58:45Z",
+            "confirmed": True,
+            "locked": False,
+            "guid": "a01792e3-2e67-402e-99af-be04a48da074",
+        }
+
+    @responses.activate
+    def test_params(self):
+        # validate input params are propagated to the query params
+        params = {"key1": "value1", "key2": "value2", "key3": "value3"}
+        responses.get(
+            "https://connect.example/__api__/v1/users",
+            match=[
+                responses.matchers.query_param_matcher(
+                    {
+                        "page_size": 500,
+                        "page_number": 1,
+                        "key1": "value1",
+                        "key2": "value2",
+                        "key3": "value3",
+                    }
+                )
+            ],
+            json=load_mock("v1/users?page_number=1&page_size=500.jsonc"),
+        )
+        responses.get(
+            "https://connect.example/__api__/v1/users",
+            match=[
+                responses.matchers.query_param_matcher(
+                    {
+                        "page_size": 500,
+                        "page_number": 2,
+                        "key1": "value1",
+                        "key2": "value2",
+                        "key3": "value3",
+                    }
+                )
+            ],
+            json=load_mock("v1/users?page_number=2&page_size=500.jsonc"),
+        )
+        con = Client(api_key="12345", url="https://connect.example/")
+        con.users.find_one(key1="value1", key2="value2", key3="value3")
+        responses.assert_call_count(
+            "https://connect.example/__api__/v1/users?key1=value1&key2=value2&key3=value3&page_number=1&page_size=500",
+            1,
+        )
+
+    @responses.activate
+    def test_params_not_dict_like(self):
+        # validate input params are propagated to the query params
+        con = Client(api_key="12345", url="https://connect.example/")
+        not_dict_like = "string"
+        with pytest.raises(ValueError):
+            con.users.find(not_dict_like)
```

