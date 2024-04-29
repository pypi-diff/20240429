# Comparing `tmp/zer1t0_aze-0.0.4.tar.gz` & `tmp/zer1t0_aze-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zer1t0_aze-0.0.4.tar", last modified: Sun Apr 28 17:47:31 2024, max compression
+gzip compressed data, was "zer1t0_aze-0.0.5.tar", last modified: Sun Apr 28 22:05:13 2024, max compression
```

## Comparing `zer1t0_aze-0.0.4.tar` & `zer1t0_aze-0.0.5.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     2002 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1582 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.432376 zer1t0_aze-0.0.4/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1136 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/arm_api.py
--rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_brute_passwords.py
--rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_brute_service_subdomains.py
--rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_brute_usernames.py
--rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_get_tenant_domains.py
--rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_get_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     1632 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_list_role_assignment.py
--rw-rw-r--   0 user      (1000) user      (1000)     9516 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_search_token_in_cache.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)       37 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/error.py
--rw-rw-r--   0 user      (1000) user      (1000)      444 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/profile.py
--rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)     1802 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/tokens.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/aze/version.py
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1353 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     2002 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     2436 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/SOURCES.txt
--rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-get-login-info
--rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-inspect-token
--rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-login-with-token
--rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-tenant-id
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/az-whoami
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.440376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.444376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_get_login_info.py
--rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_inspect_token.py
--rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_login_with_token.py
--rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_tenant_id.py
--rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_whoami.py
--rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/read_in.py
--rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/tenant.py
--rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.444376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dependency_links.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 17:47:31.448376 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/
--rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
--rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
--rw-rw-r--   0 user      (1000) user      (1000)      632 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-28 17:45:20.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-28 17:47:31.000000 zer1t0_aze-0.0.4/zer1t0_aze.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2181 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1761 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.309157 zer1t0_aze-0.0.5/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      767 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/arm_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_brute_add_app_secret.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9476 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_brute_passwords.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4079 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_brute_service_subdomains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2965 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_brute_usernames.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3253 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2794 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_get_tenant_domains.py
+-rw-rw-r--   0 user      (1000) user      (1000)      982 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_get_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1131 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_list_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_list_sp_app_role_assignment.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9596 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2434 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_search_token_in_cache.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/error.py
+-rw-rw-r--   0 user      (1000) user      (1000)      754 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/graph_api.py
+-rw-rw-r--   0 user      (1000) user      (1000)      817 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1700 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      679 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/request_az.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2768 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/tokens.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/aze/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1422 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    35125 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2181 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      751 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     2540 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)      107 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-get-login-info
+-rwxrwxr-x   0 user      (1000) user      (1000)      106 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-inspect-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      109 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-login-with-token
+-rwxrwxr-x   0 user      (1000) user      (1000)      102 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-tenant-id
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/az-whoami
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.317157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/
+-rw-rw-r--   0 user      (1000) user      (1000)      132 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3158 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      869 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     5617 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     8123 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1106 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      380 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_whoami.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     1063 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      695 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)      733 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     3319 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_get_login_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)      573 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_inspect_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10027 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_login_with_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)      895 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_tenant_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)      156 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_whoami.py
+-rw-rw-r--   0 user      (1000) user      (1000)      836 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/read_in.py
+-rw-rw-r--   0 user      (1000) user      (1000)      464 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/tenant.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.321157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      415 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      341 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      229 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dependency_links.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-28 22:05:13.325157 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/
+-rw-rw-r--   0 user      (1000) user      (1000)    19900 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz
+-rw-rw-r--   0 user      (1000) user      (1000)    21497 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl
+-rw-rw-r--   0 user      (1000) user      (1000)      764 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1141 2024-04-28 22:02:54.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-28 22:05:13.000000 zer1t0_aze-0.0.5/zer1t0_aze.egg-info/top_level.txt
```

### Comparing `zer1t0_aze-0.0.4/LICENSE` & `zer1t0_aze-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/PKG-INFO` & `zer1t0_aze-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.4
+Version: 0.0.5
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,27 +18,29 @@
 
 A python package intended to be used along with Azure Cli to expand its
 capabilities, even if many commands are completely independent from Azure Cli.
 
 
 ## Commands
 
-AZE includes the following commands, many of them do not require to be
-authenticated in Azure:
+AZE includes the following commands, many of them require to be
+authenticated (marked with Auth) in Azure:
 
+- **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
-  subdomains.
+  subdomains (No auth).
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
+- **az-list-sp-app-role-assignment**: List App roles for a service principal.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
 pip install zer1t0-aze
```

### Comparing `zer1t0_aze-0.0.4/README.md` & `zer1t0_aze-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 
 A python package intended to be used along with Azure Cli to expand its
 capabilities, even if many commands are completely independent from Azure Cli.
 
 
 ## Commands
 
-AZE includes the following commands, many of them do not require to be
-authenticated in Azure:
+AZE includes the following commands, many of them require to be
+authenticated (marked with Auth) in Azure:
 
+- **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
-  subdomains.
+  subdomains (No auth).
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
+- **az-list-sp-app-role-assignment**: List App roles for a service principal.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
 pip install zer1t0-aze
```

### Comparing `zer1t0_aze-0.0.4/aze/az_brute_passwords.py` & `zer1t0_aze-0.0.5/aze/az_brute_passwords.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/az_brute_service_subdomains.py` & `zer1t0_aze-0.0.5/aze/az_brute_service_subdomains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/az_brute_usernames.py` & `zer1t0_aze-0.0.5/aze/az_brute_usernames.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/az_get_login_info.py` & `zer1t0_aze-0.0.5/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/az_get_tenant_domains.py` & `zer1t0_aze-0.0.5/aze/az_get_tenant_domains.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/az_get_tenant_id.py` & `zer1t0_aze-0.0.5/aze/az_get_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/az_inspect_token.py` & `zer1t0_aze-0.0.5/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/az_login_with_token.py` & `zer1t0_aze-0.0.5/aze/az_login_with_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,17 +249,19 @@
 
     @property
     def endpoint(self):
         endpoint = self._info["aud"]
 
         # Seems that management.azure.com is the new endpoint
         # but still not used by Azure Cli, so we replace it
-        # for the old endpoint to make it compatible
-        if endpoint == "https://management.azure.com/":
-            return "https://management.core.windows.net/"
+        # with the old endpoint to make it compatible
+        if endpoint.startswith("https://management.azure.com"):
+            endpoint = "https://management.core.windows.net/"
+        if not endpoint.endswith("/"):
+            endpoint += "/"
         return endpoint
 
 
     @property
     def tenant_id(self):
         return self._info["tid"]
```

### Comparing `zer1t0_aze-0.0.4/aze/az_search_token_in_cache.py` & `zer1t0_aze-0.0.5/aze/az_search_token_in_cache.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/read_in.py` & `zer1t0_aze-0.0.5/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/aze/tokens.py` & `zer1t0_aze-0.0.5/aze/tokens.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,54 @@
 
 from msal_extensions import FilePersistenceWithDataProtection,\
     KeychainPersistence, LibsecretPersistence, FilePersistence,\
     PersistedTokenCache
 import os
+from .error import AzeError
 
 CredentialType = PersistedTokenCache.CredentialType
 
 # class CredentialType:
 #         ACCESS_TOKEN = "AccessToken"
 #         REFRESH_TOKEN = "RefreshToken"
 #         ACCOUNT = "Account"  # Not exactly a credential type, but we put it here
 #         ID_TOKEN = "IdToken"
 #         APP_METADATA = "AppMetadata"
 
+def search_token_for_subscription(subscription, scopes, token_cache=None):
+    token_cache = token_cache or load_token_cache()
+
+    accounts = search_token_in_cache(
+        CredentialType.ACCOUNT,
+        query={
+            "username": subscription["user"]["name"],
+            "realm": subscription["tenantId"],
+        },
+        token_cache=token_cache,
+    )
+    if not accounts:
+        raise AzeError("Unable to find account for subscription")
+
+    account = accounts[0]
+
+    access_tokens = search_token_in_cache(
+        CredentialType.ACCESS_TOKEN,
+        query={"home_account_id": account["home_account_id"]},
+        scopes=scopes,
+        token_cache=token_cache,
+    )
+
+    if not access_tokens:
+        raise AzeError(
+            "Unable to find Access Token for account '{}' with scope '{}'".format(
+                account["home_account_id"],
+                ", ".join(scopes),
+        ))
+
+    return access_tokens[0]
 
 def search_token_in_cache(
         token_type,
         query=None,
         scopes=None,
         token_cache=None
 ):
```

### Comparing `zer1t0_aze-0.0.4/aze/utils.py` & `zer1t0_aze-0.0.5/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/setup.py` & `zer1t0_aze-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 with open(version_file) as fi:
     vs = {}
     exec(fi.read(), vs)
     __version__ = vs["__version__"]
 
 
 scripts = [
+    "az-brute-add-app-secret",
     "az-brute-passwords",
     "az-brute-usernames",
     "az-brute-service-subdomains",
     "az-get-login-info",
     "az-get-tenant-domains",
     "az-get-tenant-id",
     "az-inspect-token",
     "az-list-subscriptions",
     "az-list-role-assignment",
+    "az-list-sp-app-role-assignment",
     "az-login-with-token",
     "az-search-token-in-cache",
     "az-whoami",
 ]
 
 console_scripts = [
     "{} = {}.{}:main".format(script, name, script.replace("-", "_"))
```

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/LICENSE` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/LICENSE`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/PKG-INFO` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zer1t0-aze
-Version: 0.0.4
+Version: 0.0.5
 Summary: Enhance azure cli
 Home-page: https://gitlab.com/Zer1t0/aze
 Author: Eloy Pérez González
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,27 +18,29 @@
 
 A python package intended to be used along with Azure Cli to expand its
 capabilities, even if many commands are completely independent from Azure Cli.
 
 
 ## Commands
 
-AZE includes the following commands, many of them do not require to be
-authenticated in Azure:
+AZE includes the following commands, many of them require to be
+authenticated (marked with Auth) in Azure:
 
+- **az-brute-add-app-secret**: Try to add a secret to all applications (Auth).
 - **az-brute-usernames**: Validates if a email is Microsoft managed (No auth).
 - **az-brute-passwords**: Validate Azure credentials (No auth).
 - **az-brute-service-subdomains**: Check if any Azure service is using the given
-  subdomains.
+  subdomains (No auth).
 - **az-get-login-info**: Retrieve login information about an Azure domain (No auth).
 - **az-get-tenant-domains**: Discover the domains associated with a tenant (No auth).
 - **az-get-tenant-id**: Retrieves the tenant id from tenant domain (No auth).
 - **az-inspect-token**: Show access token (jwt) payload in json format (No auth).
 - **az-list-role-assignment**: List roles without requiring a graph access token (Auth).
 - **az-login-with-token**: Adds tokens directly into Azure Cli token cache.
+- **az-list-sp-app-role-assignment**: List App roles for a service principal.
 - **az-search-token-in-cache**: Retrieve items from token cache based on the filters.
 - **az-whoami**: Shorcut for "az ad signed-in-user show".
 
 ## Installation
 
 ```
 pip install zer1t0-aze
```

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/README.md` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/README.md`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/SOURCES.txt` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 aze/__init__.py
 aze/arm_api.py
+aze/az_brute_add_app_secret.py
 aze/az_brute_passwords.py
 aze/az_brute_service_subdomains.py
 aze/az_brute_usernames.py
 aze/az_get_login_info.py
 aze/az_get_tenant_domains.py
 aze/az_get_tenant_id.py
 aze/az_inspect_token.py
 aze/az_list_role_assignment.py
+aze/az_list_sp_app_role_assignment.py
 aze/az_login_with_token.py
 aze/az_search_token_in_cache.py
 aze/az_whoami.py
 aze/error.py
+aze/graph_api.py
 aze/profile.py
 aze/read_in.py
+aze/request_az.py
 aze/tenant.py
 aze/tokens.py
 aze/utils.py
 aze/version.py
 zer1t0_aze.egg-info/LICENSE
 zer1t0_aze.egg-info/MANIFEST.in
 zer1t0_aze.egg-info/PKG-INFO
```

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_get_login_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_inspect_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_login.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_login_with_token.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/az_tenant_id.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/read_in.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/tenant.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_get_login_info.py` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_get_login_info.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_inspect_token.py` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_inspect_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_login_with_token.py` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_login_with_token.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/az_tenant_id.py` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/az_tenant_id.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/read_in.py` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/read_in.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/aze/utils.py` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/aze/utils.py`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/zer1t0-aze-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/dist/zer1t0_aze-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `zer1t0_aze-0.0.4/zer1t0_aze.egg-info/setup.py` & `zer1t0_aze-0.0.5/zer1t0_aze.egg-info/setup.py`

 * *Files identical despite different names*

