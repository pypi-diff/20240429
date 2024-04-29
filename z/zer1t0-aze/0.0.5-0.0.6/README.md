# Comparing `tmp/zer1t0_aze-0.0.5.tar.gz` & `tmp/zer1t0_aze-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zer1t0_aze-0.0.5.tar", last modified: Sun Apr 28 22:05:13 2024, max compression
+gzip compressed data, was "zer1t0_aze-0.0.6.tar", last modified: Mon Apr 29 20:55:27 2024, max compression
```

## Comparing `zer1t0_aze-0.0.5.tar` & `zer1t0_aze-0.0.6.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     2181 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1761 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.309157 zer1t0_aze-0.0.5/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      767 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/arm_api.py
--rw-rw-r--   0 user      (1000) user      (1000)     1741 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_brute_add_app_secret.py
--rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_brute_passwords.py
--rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_brute_service_subdomains.py
--rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_brute_usernames.py
--rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_get_tenant_domains.py
--rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_get_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     1131 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_list_role_assignment.py
--rw-rw-r--   0 user      (1000) user      (1000)      800 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_list_sp_app_role_assignment.py
--rw-rw-r--   0 user      (1000) user      (1000)     9596 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_search_token_in_cache.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)       80 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/error.py
--rw-rw-r--   0 user      (1000) user      (1000)      754 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/graph_api.py
--rw-rw-r--   0 user      (1000) user      (1000)      817 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/profile.py
--rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      679 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/request_az.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)     2768 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/tokens.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/version.py
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1422 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     2181 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     2540 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/SOURCES.txt
--rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-get-login-info
--rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-inspect-token
--rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-login-with-token
--rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-tenant-id
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-whoami
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.317157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.321157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dependency_links.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/
--rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
--rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
--rw-rw-r--   0 user      (1000) user      (1000)      764 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 20:55:27.988486 zer1t0_aze-0.0.6/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2414 2024-04-29 20:55:27.984486 zer1t0_aze-0.0.6/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1994 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 20:55:27.968485 zer1t0_aze-0.0.6/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      767 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/arm_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_brute_add_app_secret.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3167 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_brute_blob_containers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_brute_passwords.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6861 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_brute_service_subdomains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_brute_usernames.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_get_tenant_domains.py
+-rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_get_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3369 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_list_blobs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1131 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_list_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_list_sp_app_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9596 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_search_token_in_cache.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)      754 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/graph_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1248 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/permutations.py
+-rw-rw-r--   0 user      (1000) user      (1000)      817 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      679 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/request_az.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2768 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/tokens.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/aze/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-29 20:55:27.988486 zer1t0_aze-0.0.6/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1475 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 20:55:27.984486 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2414 2024-04-29 20:55:27.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     2613 2024-04-29 20:55:27.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/az-get-login-info
+-rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/az-inspect-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/az-login-with-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/az-tenant-id
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/az-whoami
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 20:55:27.980486 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 20:55:27.984486 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/
+-rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 20:55:27.980486 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-29 20:55:27.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/dependency_links.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-29 20:55:27.984486 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/dist/
+-rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
+-rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
+-rw-rw-r--   0 user      (1000) user      (1000)      864 2024-04-29 20:55:27.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-29 20:55:27.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-29 20:52:26.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-29 20:55:27.000000 zer1t0_aze-0.0.6/zer1t0_aze.egg-info/top_level.txt
```

### Comparing `zer1t0_aze-0.0.5/LICENSE` & `zer1t0_aze-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/PKG-INFO` & `zer1t0_aze-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.5
+Version: 0.0.6
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,23 +26,25 @@
 authenticated (marked with Auth) in Azure:
 
 - **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains (No auth).
+- **az-brute-blob-containers**: Discover public containers in Azure blobs (No auth).
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
+- **az-list-blobs**: List blobs of container from URL (No auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
-- **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
-- **az-list-sp-app-role-assignment**: List App roles for a service principal.
+- **az-login-with-token**: Injects tokens directly into Azure Cli token cache.
+- **az-list-sp-app-role-assignment**: List App roles for a service principal (Auth).
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
-- **az-whoami**: Shorcut for "az ad signed-in-user show".
+- **az-whoami**: Shorcut for "az ad signed-in-user show" (Auth).
 
 ## Installation
 
 ```
 pip install zer1t0-aze
 ```
 
@@ -55,7 +57,8 @@
 ```
 
 ## Credits
 - [AADInternals](https://github.com/Gerenios/AADInternals)
 - [MicroBurst](https://github.com/NetSPI/MicroBurst)
 - [MSOLSpray](https://github.com/dafthack/MSOLSpray)
 - [o365creeper](https://github.com/LMGsec/o365creeper)
+- [OffensiveCloud](https://github.com/lutzenfried/OffensiveCloud)
```

### Comparing `zer1t0_aze-0.0.5/README.md` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: zer1t0-aze
+Version: 0.0.6
+Summary: Enhance azure cli
+Home-page: https://gitlab.com/Zer1t0/aze
+Author: Eloy Pérez González
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: msal_extensions
+Requires-Dist: dnspython
+
 # AZE (Azure Cli Enhacement)
 
 Extended utilities for azure management.
 
 A python package intended to be used along with Azure Cli to expand its
 capabilities, even if many commands are completely independent from Azure Cli.
 
@@ -12,23 +26,25 @@
 authenticated (marked with Auth) in Azure:
 
 - **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains (No auth).
+- **az-brute-blob-containers**: Discover public containers in Azure blobs (No auth).
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
+- **az-list-blobs**: List blobs of container from URL (No auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
-- **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
-- **az-list-sp-app-role-assignment**: List App roles for a service principal.
+- **az-login-with-token**: Injects tokens directly into Azure Cli token cache.
+- **az-list-sp-app-role-assignment**: List App roles for a service principal (Auth).
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
-- **az-whoami**: Shorcut for "az ad signed-in-user show".
+- **az-whoami**: Shorcut for "az ad signed-in-user show" (Auth).
 
 ## Installation
 
 ```
 pip install zer1t0-aze
 ```
 
@@ -41,7 +57,8 @@
 ```
 
 ## Credits
 - [AADInternals](https://github.com/Gerenios/AADInternals)
 - [MicroBurst](https://github.com/NetSPI/MicroBurst)
 - [MSOLSpray](https://github.com/dafthack/MSOLSpray)
 - [o365creeper](https://github.com/LMGsec/o365creeper)
+- [OffensiveCloud](https://github.com/lutzenfried/OffensiveCloud)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zer1t0_aze-0.0.5/aze/arm_api.py` & `zer1t0_aze-0.0.6/aze/arm_api.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_brute_add_app_secret.py` & `zer1t0_aze-0.0.6/aze/az_brute_add_app_secret.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_brute_passwords.py` & `zer1t0_aze-0.0.6/aze/az_brute_passwords.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_brute_usernames.py` & `zer1t0_aze-0.0.6/aze/az_brute_usernames.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_get_login_info.py` & `zer1t0_aze-0.0.6/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_get_tenant_domains.py` & `zer1t0_aze-0.0.6/aze/az_get_tenant_domains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_get_tenant_id.py` & `zer1t0_aze-0.0.6/aze/az_get_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_inspect_token.py` & `zer1t0_aze-0.0.6/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_list_role_assignment.py` & `zer1t0_aze-0.0.6/aze/az_list_role_assignment.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_list_sp_app_role_assignment.py` & `zer1t0_aze-0.0.6/aze/az_list_sp_app_role_assignment.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_login_with_token.py` & `zer1t0_aze-0.0.6/aze/az_login_with_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/az_search_token_in_cache.py` & `zer1t0_aze-0.0.6/aze/az_search_token_in_cache.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/graph_api.py` & `zer1t0_aze-0.0.6/aze/graph_api.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/profile.py` & `zer1t0_aze-0.0.6/aze/profile.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/read_in.py` & `zer1t0_aze-0.0.6/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/request_az.py` & `zer1t0_aze-0.0.6/aze/request_az.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/tokens.py` & `zer1t0_aze-0.0.6/aze/tokens.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/aze/utils.py` & `zer1t0_aze-0.0.6/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/setup.py` & `zer1t0_aze-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 
 
 scripts = [
     "az-brute-add-app-secret",
     "az-brute-passwords",
     "az-brute-usernames",
     "az-brute-service-subdomains",
+    "az-brute-blob-containers",
     "az-get-login-info",
     "az-get-tenant-domains",
     "az-get-tenant-id",
     "az-inspect-token",
+    "az-list-blobs",
     "az-list-subscriptions",
     "az-list-role-assignment",
     "az-list-sp-app-role-assignment",
     "az-login-with-token",
     "az-search-token-in-cache",
     "az-whoami",
 ]
```

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/LICENSE` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/PKG-INFO` & `zer1t0_aze-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: zer1t0-aze
-Version: 0.0.5
-Summary: Enhance azure cli
-Home-page: https://gitlab.com/Zer1t0/aze
-Author: Eloy Pérez González
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: msal_extensions
-Requires-Dist: dnspython
-
 # AZE (Azure Cli Enhacement)
 
 Extended utilities for azure management.
 
 A python package intended to be used along with Azure Cli to expand its
 capabilities, even if many commands are completely independent from Azure Cli.
 
@@ -26,23 +12,25 @@
 authenticated (marked with Auth) in Azure:
 
 - **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
   subdomains (No auth).
+- **az-brute-blob-containers**: Discover public containers in Azure blobs (No auth).
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
+- **az-list-blobs**: List blobs of container from URL (No auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
-- **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
-- **az-list-sp-app-role-assignment**: List App roles for a service principal.
+- **az-login-with-token**: Injects tokens directly into Azure Cli token cache.
+- **az-list-sp-app-role-assignment**: List App roles for a service principal (Auth).
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
-- **az-whoami**: Shorcut for "az ad signed-in-user show".
+- **az-whoami**: Shorcut for "az ad signed-in-user show" (Auth).
 
 ## Installation
 
 ```
 pip install zer1t0-aze
 ```
 
@@ -55,7 +43,8 @@
 ```
 
 ## Credits
 - [AADInternals](https://github.com/Gerenios/AADInternals)
 - [MicroBurst](https://github.com/NetSPI/MicroBurst)
 - [MSOLSpray](https://github.com/dafthack/MSOLSpray)
 - [o365creeper](https://github.com/LMGsec/o365creeper)
+- [OffensiveCloud](https://github.com/lutzenfried/OffensiveCloud)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/README.md` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/README.md`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/SOURCES.txt` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 aze/__init__.py
 aze/arm_api.py
 aze/az_brute_add_app_secret.py
+aze/az_brute_blob_containers.py
 aze/az_brute_passwords.py
 aze/az_brute_service_subdomains.py
 aze/az_brute_usernames.py
 aze/az_get_login_info.py
 aze/az_get_tenant_domains.py
 aze/az_get_tenant_id.py
 aze/az_inspect_token.py
+aze/az_list_blobs.py
 aze/az_list_role_assignment.py
 aze/az_list_sp_app_role_assignment.py
 aze/az_login_with_token.py
 aze/az_search_token_in_cache.py
 aze/az_whoami.py
 aze/error.py
 aze/graph_api.py
+aze/permutations.py
 aze/profile.py
 aze/read_in.py
 aze/request_az.py
 aze/tenant.py
 aze/tokens.py
 aze/utils.py
 aze/version.py
```

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_get_login_info.py` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_inspect_token.py` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_login_with_token.py` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_login_with_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_tenant_id.py` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/az_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/read_in.py` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/utils.py` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/entry_points.txt` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [console_scripts]
 az-brute-add-app-secret = aze.az_brute_add_app_secret:main
+az-brute-blob-containers = aze.az_brute_blob_containers:main
 az-brute-passwords = aze.az_brute_passwords:main
 az-brute-service-subdomains = aze.az_brute_service_subdomains:main
 az-brute-usernames = aze.az_brute_usernames:main
 az-get-login-info = aze.az_get_login_info:main
 az-get-tenant-domains = aze.az_get_tenant_domains:main
 az-get-tenant-id = aze.az_get_tenant_id:main
 az-inspect-token = aze.az_inspect_token:main
+az-list-blobs = aze.az_list_blobs:main
 az-list-role-assignment = aze.az_list_role_assignment:main
 az-list-sp-app-role-assignment = aze.az_list_sp_app_role_assignment:main
 az-list-subscriptions = aze.az_list_subscriptions:main
 az-login-with-token = aze.az_login_with_token:main
 az-search-token-in-cache = aze.az_search_token_in_cache:main
 az-whoami = aze.az_whoami:main
```

### Comparing `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/setup.py` & `zer1t0_aze-0.0.6/zer1t0_aze.egg-info/setup.py`

 * *Files identical despite different names*

