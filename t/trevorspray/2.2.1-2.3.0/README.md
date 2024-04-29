# Comparing `tmp/trevorspray-2.2.1.tar.gz` & `tmp/trevorspray-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trevorspray-2.2.1.tar", max compression
+gzip compressed data, was "trevorspray-2.3.0.tar", max compression
```

## Comparing `trevorspray-2.2.1.tar` & `trevorspray-2.3.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    35149 2020-09-23 15:46:29.895512 trevorspray-2.2.1/LICENSE
--rw-r--r--   0        0        0      811 2023-09-15 23:03:11.651755 trevorspray-2.2.1/pyproject.toml
--rw-r--r--   0        0        0       24 2023-08-18 20:31:26.263403 trevorspray-2.2.1/trevorspray/__init__.py
--rwxr-xr-x   0        0        0     9988 2023-08-28 02:01:26.650869 trevorspray-2.2.1/trevorspray/cli.py
--rw-r--r--   0        0        0      173 2023-06-20 15:41:48.178620 trevorspray-2.2.1/trevorspray/lib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10274 2022-02-05 01:19:08.134611 trevorspray-2.2.1/trevorspray/lib/__pycache__/discover.cpython-310.pyc
--rw-r--r--   0        0        0    19396 2023-08-28 17:26:01.356809 trevorspray-2.2.1/trevorspray/lib/__pycache__/discover.cpython-311.pyc
--rw-r--r--   0        0        0    10380 2022-02-02 18:01:43.844552 trevorspray-2.2.1/trevorspray/lib/__pycache__/discover.cpython-39.pyc
--rw-r--r--   0        0        0      328 2022-02-05 00:51:49.874543 trevorspray-2.2.1/trevorspray/lib/__pycache__/errors.cpython-310.pyc
--rw-r--r--   0        0        0      412 2023-06-20 16:59:20.433427 trevorspray-2.2.1/trevorspray/lib/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0      324 2021-12-13 20:13:34.963665 trevorspray-2.2.1/trevorspray/lib/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     4148 2022-04-25 18:43:52.894020 trevorspray-2.2.1/trevorspray/lib/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0     6951 2023-06-20 16:59:20.403427 trevorspray-2.2.1/trevorspray/lib/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     3625 2022-01-25 19:23:44.701631 trevorspray-2.2.1/trevorspray/lib/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     8383 2022-04-29 20:12:15.812195 trevorspray-2.2.1/trevorspray/lib/__pycache__/proxy.cpython-310.pyc
--rw-r--r--   0        0        0    18352 2023-09-02 22:52:58.998530 trevorspray-2.2.1/trevorspray/lib/__pycache__/proxy.cpython-311.pyc
--rw-r--r--   0        0        0     7910 2022-02-02 20:58:01.961663 trevorspray-2.2.1/trevorspray/lib/__pycache__/proxy.cpython-39.pyc
--rw-r--r--   0        0        0     4880 2022-01-25 18:16:33.441462 trevorspray-2.2.1/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc
--rw-r--r--   0        0        0     6483 2022-04-25 18:43:53.020687 trevorspray-2.2.1/trevorspray/lib/__pycache__/trevor.cpython-310.pyc
--rw-r--r--   0        0        0    14020 2023-08-25 14:04:36.040936 trevorspray-2.2.1/trevorspray/lib/__pycache__/trevor.cpython-311.pyc
--rw-r--r--   0        0        0     6050 2022-02-02 18:57:32.781359 trevorspray-2.2.1/trevorspray/lib/__pycache__/trevor.cpython-39.pyc
--rw-r--r--   0        0        0     4672 2022-01-25 21:00:12.908541 trevorspray-2.2.1/trevorspray/lib/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0    12552 2023-08-28 02:01:14.440870 trevorspray-2.2.1/trevorspray/lib/discover.py
--rw-r--r--   0        0        0      638 2023-08-25 14:04:43.510943 trevorspray-2.2.1/trevorspray/lib/enumerators/__init__.py
--rw-r--r--   0        0        0      752 2022-02-05 00:51:49.937877 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1146 2023-08-25 14:04:53.974285 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      748 2022-02-01 21:14:34.331680 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2215 2022-04-25 18:43:53.024021 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc
--rw-r--r--   0        0        0     3719 2023-08-18 20:13:02.381756 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc
--rw-r--r--   0        0        0     2177 2022-01-31 20:34:18.741622 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc
--rw-r--r--   0        0        0     2057 2022-04-25 18:43:53.024021 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc
--rw-r--r--   0        0        0     2859 2023-08-18 20:13:02.381756 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc
--rw-r--r--   0        0        0     2020 2022-02-01 21:21:47.395032 trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc
--rw-r--r--   0        0        0     2476 2023-08-18 19:33:02.614220 trevorspray-2.2.1/trevorspray/lib/enumerators/onedrive.py
--rw-r--r--   0        0        0     1935 2023-08-18 19:36:08.034566 trevorspray-2.2.1/trevorspray/lib/enumerators/seamless_sso.py
--rw-r--r--   0        0        0       44 2023-06-20 16:20:18.948469 trevorspray-2.2.1/trevorspray/lib/errors.py
--rw-r--r--   0        0        0     4419 2023-06-20 16:20:19.028468 trevorspray-2.2.1/trevorspray/lib/logger.py
--rw-r--r--   0        0        0     1036 2022-02-05 00:51:49.937877 trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1705 2023-06-20 16:59:20.503430 trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1028 2022-01-27 17:15:46.627782 trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0    11619 2022-02-05 00:51:49.937877 trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc
--rw-r--r--   0        0        0    22339 2023-08-25 13:54:33.207064 trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc
--rw-r--r--   0        0        0    11403 2022-01-25 21:04:10.745217 trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc
--rw-r--r--   0        0        0      568 2023-06-20 16:20:18.965135 trevorspray-2.2.1/trevorspray/lib/looters/base.py
--rw-r--r--   0        0        0    16108 2023-08-24 17:51:46.694520 trevorspray-2.2.1/trevorspray/lib/looters/msol.py
--rw-r--r--   0        0        0    13059 2023-09-02 22:43:28.507420 trevorspray-2.2.1/trevorspray/lib/proxy.py
--rw-r--r--   0        0        0      655 2023-07-13 14:36:03.130817 trevorspray-2.2.1/trevorspray/lib/sprayers/__init__.py
--rw-r--r--   0        0        0      746 2022-02-05 00:51:49.874543 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1150 2023-08-18 20:13:01.188422 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      742 2022-02-01 21:14:34.305014 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3247 2022-02-07 14:54:28.512909 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc
--rw-r--r--   0        0        0     5635 2023-09-02 22:52:58.925188 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc
--rw-r--r--   0        0        0     3245 2022-02-03 20:11:00.807482 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc
--rw-r--r--   0        0        0     4879 2022-04-25 18:43:52.970687 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc
--rw-r--r--   0        0        0     9087 2023-06-20 16:59:20.456761 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc
--rw-r--r--   0        0        0     4800 2022-02-03 20:22:37.297511 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc
--rw-r--r--   0        0        0     3710 2023-09-07 15:52:18.961090 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/auth0.cpython-311.pyc
--rw-r--r--   0        0        0     3836 2022-02-07 14:54:28.479575 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     6909 2023-09-02 22:52:47.560602 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3843 2022-02-03 20:01:13.737457 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1289 2022-02-05 00:51:49.937877 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2023-06-20 16:59:20.503430 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc
--rw-r--r--   0        0        0     1271 2022-01-18 15:54:51.036838 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc
--rw-r--r--   0        0        0     6213 2023-08-18 20:13:01.251755 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/google.cpython-311.pyc
--rw-r--r--   0        0        0     3097 2023-09-07 15:52:18.961090 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/jumpcloud.cpython-311.pyc
--rw-r--r--   0        0        0     3743 2022-04-25 18:43:53.017354 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc
--rw-r--r--   0        0        0     5522 2023-06-20 16:59:20.496763 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc
--rw-r--r--   0        0        0     3688 2022-02-03 20:11:00.850815 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc
--rw-r--r--   0        0        0     2054 2022-02-07 14:54:28.512909 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc
--rw-r--r--   0        0        0     3386 2023-06-20 17:00:00.287891 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc
--rw-r--r--   0        0        0     2027 2022-02-03 21:46:45.294387 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc
--rw-r--r--   0        0        0     2842 2022-02-07 14:54:28.482909 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc
--rw-r--r--   0        0        0     4936 2023-09-02 22:52:47.560602 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-02-03 20:11:00.794149 trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc
--rw-r--r--   0        0        0     3793 2023-09-15 23:03:11.651755 trevorspray-2.2.1/trevorspray/lib/sprayers/adfs.py
--rw-r--r--   0        0        0     7408 2023-06-20 16:20:19.078468 trevorspray-2.2.1/trevorspray/lib/sprayers/anyconnect.py
--rw-r--r--   0        0        0     3040 2023-09-15 23:03:11.651755 trevorspray-2.2.1/trevorspray/lib/sprayers/auth0.py
--rw-r--r--   0        0        0     4144 2023-09-02 22:00:09.670026 trevorspray-2.2.1/trevorspray/lib/sprayers/base.py
--rw-r--r--   0        0        0     1297 2023-06-20 16:20:18.995135 trevorspray-2.2.1/trevorspray/lib/sprayers/example.py
--rw-r--r--   0        0        0     6025 2023-08-16 20:20:37.120725 trevorspray-2.2.1/trevorspray/lib/sprayers/google.py.bak
--rw-r--r--   0        0        0     2118 2023-09-15 23:03:11.651755 trevorspray-2.2.1/trevorspray/lib/sprayers/jumpcloud.py
--rw-r--r--   0        0        0     5046 2023-06-20 16:20:19.058468 trevorspray-2.2.1/trevorspray/lib/sprayers/msol.py
--rw-r--r--   0        0        0     2250 2023-06-20 16:59:57.761155 trevorspray-2.2.1/trevorspray/lib/sprayers/okta.py
--rw-r--r--   0        0        0     3295 2023-09-15 23:03:11.651755 trevorspray-2.2.1/trevorspray/lib/sprayers/owa.py
--rw-r--r--   0        0        0     8547 2023-08-25 14:04:10.670914 trevorspray-2.2.1/trevorspray/lib/trevor.py
--rw-r--r--   0        0        0       91 2023-06-20 16:20:19.031802 trevorspray-2.2.1/trevorspray/lib/util/__init__.py
--rw-r--r--   0        0        0      274 2022-02-05 00:51:49.824543 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      330 2023-06-20 16:59:20.406760 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      272 2022-01-31 18:58:32.148049 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5749 2022-04-25 18:43:52.897354 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc
--rw-r--r--   0        0        0    11469 2023-08-28 17:26:01.263476 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc
--rw-r--r--   0        0        0     5534 2022-02-02 15:07:49.377447 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc
--rw-r--r--   0        0        0     6610 2022-02-05 00:51:49.874543 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc
--rw-r--r--   0        0        0    10993 2023-08-25 13:54:33.137065 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc
--rw-r--r--   0        0        0     6644 2022-01-28 21:23:31.518382 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc
--rw-r--r--   0        0        0     1165 2022-01-31 16:20:46.034318 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc
--rw-r--r--   0        0        0     4855 2022-02-05 00:51:49.871210 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc
--rw-r--r--   0        0        0     9285 2023-08-25 14:05:17.534307 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc
--rw-r--r--   0        0        0     4807 2022-01-31 20:14:54.024908 trevorspray-2.2.1/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc
--rw-r--r--   0        0        0     5862 2023-08-28 02:00:36.284208 trevorspray-2.2.1/trevorspray/lib/util/misc.py
--rw-r--r--   0        0        0     7203 2023-08-18 20:31:22.106729 trevorspray-2.2.1/trevorspray/lib/util/ntlmdecoder.py
--rw-r--r--   0        0        0     4404 2023-08-25 14:05:14.534304 trevorspray-2.2.1/trevorspray/lib/util/threadpool.py
--rwxr-xr-x   0        0        0     2816 2020-10-15 19:54:12.675089 trevorspray-2.2.1/trevorspray/trevorproxy.py.bak
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 trevorspray-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-09-23 15:46:29.895512 trevorspray-2.3.0/LICENSE
+-rw-r--r--   0        0        0      811 2024-04-29 12:46:49.173234 trevorspray-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-08-18 20:31:26.263403 trevorspray-2.3.0/trevorspray/__init__.py
+-rwxr-xr-x   0        0        0     9968 2024-03-19 13:59:30.522292 trevorspray-2.3.0/trevorspray/cli.py
+-rw-r--r--   0        0        0      173 2023-06-20 15:41:48.178620 trevorspray-2.3.0/trevorspray/lib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10274 2022-02-05 01:19:08.134611 trevorspray-2.3.0/trevorspray/lib/__pycache__/discover.cpython-310.pyc
+-rw-r--r--   0        0        0    19396 2023-08-28 17:26:01.356809 trevorspray-2.3.0/trevorspray/lib/__pycache__/discover.cpython-311.pyc
+-rw-r--r--   0        0        0    10380 2022-02-02 18:01:43.844552 trevorspray-2.3.0/trevorspray/lib/__pycache__/discover.cpython-39.pyc
+-rw-r--r--   0        0        0      328 2022-02-05 00:51:49.874543 trevorspray-2.3.0/trevorspray/lib/__pycache__/errors.cpython-310.pyc
+-rw-r--r--   0        0        0      412 2023-06-20 16:59:20.433427 trevorspray-2.3.0/trevorspray/lib/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0      324 2021-12-13 20:13:34.963665 trevorspray-2.3.0/trevorspray/lib/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     4148 2022-04-25 18:43:52.894020 trevorspray-2.3.0/trevorspray/lib/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0     6951 2023-06-20 16:59:20.403427 trevorspray-2.3.0/trevorspray/lib/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     3625 2022-01-25 19:23:44.701631 trevorspray-2.3.0/trevorspray/lib/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     8383 2022-04-29 20:12:15.812195 trevorspray-2.3.0/trevorspray/lib/__pycache__/proxy.cpython-310.pyc
+-rw-r--r--   0        0        0    18352 2023-09-02 22:52:58.998530 trevorspray-2.3.0/trevorspray/lib/__pycache__/proxy.cpython-311.pyc
+-rw-r--r--   0        0        0     7910 2022-02-02 20:58:01.961663 trevorspray-2.3.0/trevorspray/lib/__pycache__/proxy.cpython-39.pyc
+-rw-r--r--   0        0        0     4880 2022-01-25 18:16:33.441462 trevorspray-2.3.0/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc
+-rw-r--r--   0        0        0     6483 2022-04-25 18:43:53.020687 trevorspray-2.3.0/trevorspray/lib/__pycache__/trevor.cpython-310.pyc
+-rw-r--r--   0        0        0    14020 2023-08-25 14:04:36.040936 trevorspray-2.3.0/trevorspray/lib/__pycache__/trevor.cpython-311.pyc
+-rw-r--r--   0        0        0     6050 2022-02-02 18:57:32.781359 trevorspray-2.3.0/trevorspray/lib/__pycache__/trevor.cpython-39.pyc
+-rw-r--r--   0        0        0     4672 2022-01-25 21:00:12.908541 trevorspray-2.3.0/trevorspray/lib/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0    12552 2023-08-28 02:01:14.440870 trevorspray-2.3.0/trevorspray/lib/discover.py
+-rw-r--r--   0        0        0      638 2023-08-25 14:04:43.510943 trevorspray-2.3.0/trevorspray/lib/enumerators/__init__.py
+-rw-r--r--   0        0        0      752 2022-02-05 00:51:49.937877 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1146 2023-08-25 14:04:53.974285 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      748 2022-02-01 21:14:34.331680 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2215 2022-04-25 18:43:53.024021 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc
+-rw-r--r--   0        0        0     3719 2023-08-18 20:13:02.381756 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc
+-rw-r--r--   0        0        0     2177 2022-01-31 20:34:18.741622 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc
+-rw-r--r--   0        0        0     2057 2022-04-25 18:43:53.024021 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc
+-rw-r--r--   0        0        0     2859 2023-08-18 20:13:02.381756 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc
+-rw-r--r--   0        0        0     2020 2022-02-01 21:21:47.395032 trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc
+-rw-r--r--   0        0        0     2476 2023-08-18 19:33:02.614220 trevorspray-2.3.0/trevorspray/lib/enumerators/onedrive.py
+-rw-r--r--   0        0        0     1935 2023-08-18 19:36:08.034566 trevorspray-2.3.0/trevorspray/lib/enumerators/seamless_sso.py
+-rw-r--r--   0        0        0       44 2023-06-20 16:20:18.948469 trevorspray-2.3.0/trevorspray/lib/errors.py
+-rw-r--r--   0        0        0     4419 2023-06-20 16:20:19.028468 trevorspray-2.3.0/trevorspray/lib/logger.py
+-rw-r--r--   0        0        0     1036 2022-02-05 00:51:49.937877 trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1705 2023-06-20 16:59:20.503430 trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1028 2022-01-27 17:15:46.627782 trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0    11619 2022-02-05 00:51:49.937877 trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc
+-rw-r--r--   0        0        0    22339 2023-08-25 13:54:33.207064 trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc
+-rw-r--r--   0        0        0    11403 2022-01-25 21:04:10.745217 trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc
+-rw-r--r--   0        0        0      568 2023-06-20 16:20:18.965135 trevorspray-2.3.0/trevorspray/lib/looters/base.py
+-rw-r--r--   0        0        0    16108 2023-08-24 17:51:46.694520 trevorspray-2.3.0/trevorspray/lib/looters/msol.py
+-rw-r--r--   0        0        0    13059 2023-09-02 22:43:28.507420 trevorspray-2.3.0/trevorspray/lib/proxy.py
+-rw-r--r--   0        0        0      655 2023-07-13 14:36:03.130817 trevorspray-2.3.0/trevorspray/lib/sprayers/__init__.py
+-rw-r--r--   0        0        0      746 2022-02-05 00:51:49.874543 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1150 2023-08-18 20:13:01.188422 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      742 2022-02-01 21:14:34.305014 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3247 2022-02-07 14:54:28.512909 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc
+-rw-r--r--   0        0        0     5639 2023-09-25 13:12:11.111840 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc
+-rw-r--r--   0        0        0     3245 2022-02-03 20:11:00.807482 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc
+-rw-r--r--   0        0        0     4879 2022-04-25 18:43:52.970687 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc
+-rw-r--r--   0        0        0     9087 2023-06-20 16:59:20.456761 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc
+-rw-r--r--   0        0        0     4800 2022-02-03 20:22:37.297511 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc
+-rw-r--r--   0        0        0     3710 2023-09-25 13:12:11.108507 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/auth0.cpython-311.pyc
+-rw-r--r--   0        0        0     3836 2022-02-07 14:54:28.479575 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     6909 2023-09-02 22:52:47.560602 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3843 2022-02-03 20:01:13.737457 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1289 2022-02-05 00:51:49.937877 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-06-20 16:59:20.503430 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc
+-rw-r--r--   0        0        0     1271 2022-01-18 15:54:51.036838 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc
+-rw-r--r--   0        0        0     6213 2023-08-18 20:13:01.251755 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0        0        0     3101 2023-09-25 13:12:11.108507 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/jumpcloud.cpython-311.pyc
+-rw-r--r--   0        0        0     3743 2022-04-25 18:43:53.017354 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc
+-rw-r--r--   0        0        0     5522 2023-06-20 16:59:20.496763 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc
+-rw-r--r--   0        0        0     3688 2022-02-03 20:11:00.850815 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc
+-rw-r--r--   0        0        0     2054 2022-02-07 14:54:28.512909 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc
+-rw-r--r--   0        0        0     3386 2023-06-20 17:00:00.287891 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc
+-rw-r--r--   0        0        0     2027 2022-02-03 21:46:45.294387 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc
+-rw-r--r--   0        0        0     2842 2022-02-07 14:54:28.482909 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc
+-rw-r--r--   0        0        0     4940 2023-09-25 13:12:11.085173 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-02-03 20:11:00.794149 trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc
+-rw-r--r--   0        0        0     3793 2023-09-15 23:03:11.651755 trevorspray-2.3.0/trevorspray/lib/sprayers/adfs.py
+-rw-r--r--   0        0        0     7408 2023-06-20 16:20:19.078468 trevorspray-2.3.0/trevorspray/lib/sprayers/anyconnect.py
+-rw-r--r--   0        0        0     3040 2023-09-15 23:03:11.651755 trevorspray-2.3.0/trevorspray/lib/sprayers/auth0.py
+-rw-r--r--   0        0        0     4144 2023-09-02 22:00:09.670026 trevorspray-2.3.0/trevorspray/lib/sprayers/base.py
+-rw-r--r--   0        0        0     1297 2023-06-20 16:20:18.995135 trevorspray-2.3.0/trevorspray/lib/sprayers/example.py
+-rw-r--r--   0        0        0     6025 2023-08-16 20:20:37.120725 trevorspray-2.3.0/trevorspray/lib/sprayers/google.py.bak
+-rw-r--r--   0        0        0     2118 2023-09-15 23:03:11.651755 trevorspray-2.3.0/trevorspray/lib/sprayers/jumpcloud.py
+-rw-r--r--   0        0        0     5228 2024-04-29 12:46:21.167970 trevorspray-2.3.0/trevorspray/lib/sprayers/msol.py
+-rw-r--r--   0        0        0     2250 2023-06-20 16:59:57.761155 trevorspray-2.3.0/trevorspray/lib/sprayers/okta.py
+-rw-r--r--   0        0        0     3295 2023-09-15 23:03:11.651755 trevorspray-2.3.0/trevorspray/lib/sprayers/owa.py
+-rw-r--r--   0        0        0     8547 2023-08-25 14:04:10.670914 trevorspray-2.3.0/trevorspray/lib/trevor.py
+-rw-r--r--   0        0        0       91 2023-06-20 16:20:19.031802 trevorspray-2.3.0/trevorspray/lib/util/__init__.py
+-rw-r--r--   0        0        0      274 2022-02-05 00:51:49.824543 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      330 2023-06-20 16:59:20.406760 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      272 2022-01-31 18:58:32.148049 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5749 2022-04-25 18:43:52.897354 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc
+-rw-r--r--   0        0        0    11469 2023-08-28 17:26:01.263476 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc
+-rw-r--r--   0        0        0     5534 2022-02-02 15:07:49.377447 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc
+-rw-r--r--   0        0        0     6610 2022-02-05 00:51:49.874543 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc
+-rw-r--r--   0        0        0    10993 2023-08-25 13:54:33.137065 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc
+-rw-r--r--   0        0        0     6644 2022-01-28 21:23:31.518382 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc
+-rw-r--r--   0        0        0     1165 2022-01-31 16:20:46.034318 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc
+-rw-r--r--   0        0        0     4855 2022-02-05 00:51:49.871210 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc
+-rw-r--r--   0        0        0     9285 2023-08-25 14:05:17.534307 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc
+-rw-r--r--   0        0        0     4807 2022-01-31 20:14:54.024908 trevorspray-2.3.0/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc
+-rw-r--r--   0        0        0     5862 2023-08-28 02:00:36.284208 trevorspray-2.3.0/trevorspray/lib/util/misc.py
+-rw-r--r--   0        0        0     7203 2023-08-18 20:31:22.106729 trevorspray-2.3.0/trevorspray/lib/util/ntlmdecoder.py
+-rw-r--r--   0        0        0     4404 2023-08-25 14:05:14.534304 trevorspray-2.3.0/trevorspray/lib/util/threadpool.py
+-rwxr-xr-x   0        0        0     2816 2020-10-15 19:54:12.675089 trevorspray-2.3.0/trevorspray/trevorproxy.py.bak
+-rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 trevorspray-2.3.0/PKG-INFO
```

### Comparing `trevorspray-2.2.1/LICENSE` & `trevorspray-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/pyproject.toml` & `trevorspray-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trevorspray"
-version = "2.2.1"
+version = "2.3.0"
 description = "A modular password sprayer with threading, SSH proxying, loot modules, and more"
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 repository = "https://github.com/blacklanternsecurity/TREVORspray"
 homepage = "https://github.com/blacklanternsecurity/TREVORspray"
 
 [tool.poetry.dependencies]
```

### Comparing `trevorspray-2.2.1/trevorspray/cli.py` & `trevorspray-2.3.0/trevorspray/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,18 +253,17 @@
             os.environ["HTTP_PROXY"] = options.proxy
             os.environ["HTTPS_PROXY"] = options.proxy
 
         trevorproxy_logger = logging.getLogger("trevorproxy")
         trevorspray_logger = logging.getLogger("trevorspray")
         trevorproxy_logger.handlers = trevorspray_logger.handlers
 
-        if not (options.users and options.passwords):
-            if not options.recon:
-                log.error("Please specify --users and --passwords, or --recon")
-                sys.exit(2)
+        if not (options.users and options.passwords) and not options.recon:
+            log.error("Please specify --users and --passwords, or --recon")
+            sys.exit(2)
         if options.users:
             options.users = list(
                 util.files_to_list(options.users, lowercase=True).keys()
             )
         if options.passwords:
             options.passwords = list(util.files_to_list(options.passwords).keys())
```

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/discover.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/discover.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/discover.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/discover.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/discover.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/discover.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/logger.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/logger.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/logger.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/proxy.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/proxy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/proxy.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/proxy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/proxy.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/proxy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/trevor.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/trevor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/trevor.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/trevor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/trevor.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/trevor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/__pycache__/util.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/discover.py` & `trevorspray-2.3.0/trevorspray/lib/discover.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__init__.py` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__init__.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/__init__.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/onedrive.py` & `trevorspray-2.3.0/trevorspray/lib/enumerators/onedrive.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/enumerators/seamless_sso.py` & `trevorspray-2.3.0/trevorspray/lib/enumerators/seamless_sso.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/logger.py` & `trevorspray-2.3.0/trevorspray/lib/logger.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/looters/base.py` & `trevorspray-2.3.0/trevorspray/lib/looters/base.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/looters/msol.py` & `trevorspray-2.3.0/trevorspray/lib/looters/msol.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/proxy.py` & `trevorspray-2.3.0/trevorspray/lib/proxy.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__init__.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__init__.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/__init__.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4ab0f364 (Sat Sep  2 21:59:38 2023 UTC)
-files sz: 3780
+moddate:  0xafe20465 (Fri Sep 15 23:03:11 2023 UTC)
+files sz: 3793
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640364046c036d
@@ -405,122 +405,123 @@
             code
                argcount  : 4
                nlocals   : 7
                stacksize : 6
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
-                  00a00100000000000000000000000000000000000000007c017c02a60200
-                  00ab0200000000000000007d047405000000000000000000007c006a0300
-                  00000000000000a6010000ab0100000000000000007d0574090000000000
-                  00000000007c056a0500000000000000006401ac02a6020000ab02000000
-                  00000000007d0664037c06760072617c0167017c0664033c0000007c05a0
-                  060000000000000000000000000000000000000000740f00000000000000
-                  0000007c066401ac04a6020000ab020000000000000000ac05a6010000ab
-                  0100000000000000007d057411000000000000000000007c05a6010000ab
-                  0100000000000000007c045f030000000000000000741200000000000000
-                  000000a00a000000000000000000000000000000000000000064067c046a
-                  0300000000000000009b009d02a6010000ab01000000000000000001007c
-                  046a0300000000000000007c046a0b000000000000000064073c0000007c
-                  056a0c00000000000000009b0064087c056a0d00000000000000009b009d
-                  037c046a0b000000000000000064093c0000007c045300
+                  00a00100000000000000000000000000000000000000007c017c027c03a6
+                  030000ab0300000000000000007d047405000000000000000000007c006a
+                  030000000000000000a6010000ab0100000000000000007d057409000000
+                  000000000000007c056a0500000000000000006401ac02a6020000ab0200
+                  000000000000007d0664037c06760072617c0167017c0664033c0000007c
+                  05a0060000000000000000000000000000000000000000740f0000000000
+                  00000000007c066401ac04a6020000ab020000000000000000ac05a60100
+                  00ab0100000000000000007d057411000000000000000000007c05a60100
+                  00ab0100000000000000007c045f03000000000000000074120000000000
+                  0000000000a00a000000000000000000000000000000000000000064067c
+                  046a0300000000000000009b009d02a6010000ab01000000000000000001
+                  007c046a0300000000000000007c046a0b000000000000000064073c0000
+                  007c056a0c00000000000000009b0064087c056a0d00000000000000009b
+                  009d037c046a0b000000000000000064093c0000007c045300
                              0 COPY_FREE_VARS           1
                
                 57           2 RESUME                   0
                
                 58           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (create_request)
                             52 LOAD_FAST                1 (username)
                             54 LOAD_FAST                2 (password)
-                            56 PRECALL                  2
-                            60 CALL                     2
-                            70 STORE_FAST               4 (request)
-               
-                59          72 LOAD_GLOBAL              5 (NULL + urlparse)
-                            84 LOAD_FAST                0 (self)
-                            86 LOAD_ATTR                3 (url)
-                            96 PRECALL                  1
-                           100 CALL                     1
-                           110 STORE_FAST               5 (parsed_url)
-               
-                62         112 LOAD_GLOBAL              9 (NULL + parse_qs)
-                           124 LOAD_FAST                5 (parsed_url)
-                           126 LOAD_ATTR                5 (query)
-                           136 LOAD_CONST               1 (True)
-                           138 KW_NAMES                 2
-                           140 PRECALL                  2
-                           144 CALL                     2
-                           154 STORE_FAST               6 (query)
-               
-                63         156 LOAD_CONST               3 ('username')
-                           158 LOAD_FAST                6 (query)
-                           160 CONTAINS_OP              0
-                           162 POP_JUMP_FORWARD_IF_FALSE    97 (to 358)
-               
-                64         164 LOAD_FAST                1 (username)
-                           166 BUILD_LIST               1
-                           168 LOAD_FAST                6 (query)
-                           170 LOAD_CONST               3 ('username')
-                           172 STORE_SUBSCR
-               
-                65         176 LOAD_FAST                5 (parsed_url)
-                           178 LOAD_METHOD              6 (_replace)
-                           200 LOAD_GLOBAL             15 (NULL + urlencode)
-                           212 LOAD_FAST                6 (query)
-                           214 LOAD_CONST               1 (True)
-                           216 KW_NAMES                 4
-                           218 PRECALL                  2
-                           222 CALL                     2
-                           232 KW_NAMES                 5
-                           234 PRECALL                  1
-                           238 CALL                     1
-                           248 STORE_FAST               5 (parsed_url)
-               
-                66         250 LOAD_GLOBAL             17 (NULL + urlunparse)
-                           262 LOAD_FAST                5 (parsed_url)
-                           264 PRECALL                  1
-                           268 CALL                     1
-                           278 LOAD_FAST                4 (request)
-                           280 STORE_ATTR               3 (url)
-               
-                67         290 LOAD_GLOBAL             18 (log)
-                           302 LOAD_METHOD             10 (debug)
-                           324 LOAD_CONST               6 ('Replaced username in URL, new URL: ')
-                           326 LOAD_FAST                4 (request)
-                           328 LOAD_ATTR                3 (url)
-                           338 FORMAT_VALUE             0
-                           340 BUILD_STRING             2
-                           342 PRECALL                  1
-                           346 CALL                     1
-                           356 POP_TOP
-               
-                68     >>  358 LOAD_FAST                4 (request)
-                           360 LOAD_ATTR                3 (url)
-                           370 LOAD_FAST                4 (request)
-                           372 LOAD_ATTR               11 (headers)
-                           382 LOAD_CONST               7 ('Referrer')
-                           384 STORE_SUBSCR
-               
-                69         388 LOAD_FAST                5 (parsed_url)
-                           390 LOAD_ATTR               12 (scheme)
-                           400 FORMAT_VALUE             0
-                           402 LOAD_CONST               8 ('://')
-                           404 LOAD_FAST                5 (parsed_url)
-                           406 LOAD_ATTR               13 (netloc)
-                           416 FORMAT_VALUE             0
-                           418 BUILD_STRING             3
-                           420 LOAD_FAST                4 (request)
-                           422 LOAD_ATTR               11 (headers)
-                           432 LOAD_CONST               9 ('Origin')
-                           434 STORE_SUBSCR
+                            56 LOAD_FAST                3 (proxythread)
+                            58 PRECALL                  3
+                            62 CALL                     3
+                            72 STORE_FAST               4 (request)
+               
+                59          74 LOAD_GLOBAL              5 (NULL + urlparse)
+                            86 LOAD_FAST                0 (self)
+                            88 LOAD_ATTR                3 (url)
+                            98 PRECALL                  1
+                           102 CALL                     1
+                           112 STORE_FAST               5 (parsed_url)
+               
+                62         114 LOAD_GLOBAL              9 (NULL + parse_qs)
+                           126 LOAD_FAST                5 (parsed_url)
+                           128 LOAD_ATTR                5 (query)
+                           138 LOAD_CONST               1 (True)
+                           140 KW_NAMES                 2
+                           142 PRECALL                  2
+                           146 CALL                     2
+                           156 STORE_FAST               6 (query)
+               
+                63         158 LOAD_CONST               3 ('username')
+                           160 LOAD_FAST                6 (query)
+                           162 CONTAINS_OP              0
+                           164 POP_JUMP_FORWARD_IF_FALSE    97 (to 360)
+               
+                64         166 LOAD_FAST                1 (username)
+                           168 BUILD_LIST               1
+                           170 LOAD_FAST                6 (query)
+                           172 LOAD_CONST               3 ('username')
+                           174 STORE_SUBSCR
+               
+                65         178 LOAD_FAST                5 (parsed_url)
+                           180 LOAD_METHOD              6 (_replace)
+                           202 LOAD_GLOBAL             15 (NULL + urlencode)
+                           214 LOAD_FAST                6 (query)
+                           216 LOAD_CONST               1 (True)
+                           218 KW_NAMES                 4
+                           220 PRECALL                  2
+                           224 CALL                     2
+                           234 KW_NAMES                 5
+                           236 PRECALL                  1
+                           240 CALL                     1
+                           250 STORE_FAST               5 (parsed_url)
+               
+                66         252 LOAD_GLOBAL             17 (NULL + urlunparse)
+                           264 LOAD_FAST                5 (parsed_url)
+                           266 PRECALL                  1
+                           270 CALL                     1
+                           280 LOAD_FAST                4 (request)
+                           282 STORE_ATTR               3 (url)
+               
+                67         292 LOAD_GLOBAL             18 (log)
+                           304 LOAD_METHOD             10 (debug)
+                           326 LOAD_CONST               6 ('Replaced username in URL, new URL: ')
+                           328 LOAD_FAST                4 (request)
+                           330 LOAD_ATTR                3 (url)
+                           340 FORMAT_VALUE             0
+                           342 BUILD_STRING             2
+                           344 PRECALL                  1
+                           348 CALL                     1
+                           358 POP_TOP
+               
+                68     >>  360 LOAD_FAST                4 (request)
+                           362 LOAD_ATTR                3 (url)
+                           372 LOAD_FAST                4 (request)
+                           374 LOAD_ATTR               11 (headers)
+                           384 LOAD_CONST               7 ('Referrer')
+                           386 STORE_SUBSCR
+               
+                69         390 LOAD_FAST                5 (parsed_url)
+                           392 LOAD_ATTR               12 (scheme)
+                           402 FORMAT_VALUE             0
+                           404 LOAD_CONST               8 ('://')
+                           406 LOAD_FAST                5 (parsed_url)
+                           408 LOAD_ATTR               13 (netloc)
+                           418 FORMAT_VALUE             0
+                           420 BUILD_STRING             3
+                           422 LOAD_FAST                4 (request)
+                           424 LOAD_ATTR               11 (headers)
+                           434 LOAD_CONST               9 ('Origin')
+                           436 STORE_SUBSCR
                
-                70         438 LOAD_FAST                4 (request)
-                           440 RETURN_VALUE
+                70         440 LOAD_FAST                4 (request)
+                           442 RETURN_VALUE
                consts
                   None
                   True
                   ('keep_blank_values',)
                   'username'
                   ('doseq',)
                   ('query',)
@@ -531,15 +532,15 @@
                names      ('super', 'create_request', 'urlparse', 'url', 'parse_qs', 'query', '_replace', 'urlencode', 'urlunparse', 'log', 'debug', 'headers', 'scheme', 'netloc')
                varnames   ('self', 'username', 'password', 'proxythread', 'request', 'parsed_url', 'query')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bls/Downloads/code/trevorspray/trevorspray/lib/sprayers/adfs.py'
                name       'create_request'
                firstlineno 57
-               lnotab 0x0401440128032c0108010c014a01280144011e013201
+               lnotab 0x0401460128032c0108010c014a01280144011e013201
             code
                argcount  : 2
                nlocals   : 12
                stacksize : 6
                flags     : 3
                code
                   0x970064017d0264007d0364007d0464027d057401000000000000000000
```

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/auth0.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/auth0.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x9ebcf464 (Sun Sep  3 17:04:30 2023 UTC)
-files sz: 3041
+moddate:  0xafe20465 (Fri Sep 15 23:03:11 2023 UTC)
+files sz: 3040
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640264036c026d035a0301
```

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/google.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/jumpcloud.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/jumpcloud.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x60bcf464 (Sun Sep  3 17:03:28 2023 UTC)
-files sz: 2105
+moddate:  0xafe20465 (Fri Sep 15 23:03:11 2023 UTC)
+files sz: 2118
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640264036c026d035a0301
@@ -128,183 +128,184 @@
             code
                argcount  : 4
                nlocals   : 11
                stacksize : 6
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
-                  00a00100000000000000000000000000000000000000007c017c02a60200
-                  00ab0200000000000000007d0464017d057405000000000000000000006a
-                  0300000000000000007c057c006a0400000000000000007c036a05000000
-                  0000000000ac02a6030000ab0300000000000000007d067c06a006000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  00a003000000000000000000000000000000000000000064036404a60200
-                  00ab0200000000000000007d077c066a070000000000000000a003000000
-                  000000000000000000000000000000000064056404a6020000ab02000000
-                  00000000007d087c077325741000000000000000000000a0090000000000
-                  00000000000000000000000000000064067c069b0064077c066a0a000000
-                  00000000009b009d04a6010000ab01000000000000000001007c08732574
-                  1000000000000000000000a0090000000000000000000000000000000000
-                  00000064087c069b0064077c066a0700000000000000009b009d04a60100
+                  00a00100000000000000000000000000000000000000007c017c027c03a6
+                  030000ab0300000000000000007d0464017d057405000000000000000000
+                  006a0300000000000000007c057c006a0400000000000000007c036a0500
+                  00000000000000ac02a6030000ab0300000000000000007d067c06a00600
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  000000a003000000000000000000000000000000000000000064036404a6
+                  020000ab0200000000000000007d077c066a070000000000000000a00300
+                  0000000000000000000000000000000000000064056404a6020000ab0200
+                  000000000000007d087c077325741000000000000000000000a009000000
+                  000000000000000000000000000000000064067c069b0064077c066a0a00
+                  000000000000009b009d04a6010000ab01000000000000000001007c0873
+                  25741000000000000000000000a009000000000000000000000000000000
+                  000000000064087c069b0064077c066a0700000000000000009b009d04a6
+                  010000ab0100000000000000000100741000000000000000000000a00b00
+                  0000000000000000000000000000000000000064097c079b009d02a60100
                   00ab0100000000000000000100741000000000000000000000a00b000000
-                  000000000000000000000000000000000064097c079b009d02a6010000ab
-                  0100000000000000000100741000000000000000000000a00b0000000000
-                  000000000000000000000000000000640a7c089b009d02a6010000ab0100
-                  00000000000000010064057c0869017d097c09a00c000000000000000000
-                  00000000000000000000007c006a070000000000000000a6010000ab0100
-                  000000000000000100640b7c0769017d0a7c0aa00c000000000000000000
-                  00000000000000000000007c006a040000000000000000a6010000ab0100
-                  0000000000000001007c0a7c045f0400000000000000007c097c045f0700
-                  000000000000007c045300
+                  0000000000000000000000000000000000640a7c089b009d02a6010000ab
+                  010000000000000000010064057c0869017d097c09a00c00000000000000
+                  000000000000000000000000007c006a070000000000000000a6010000ab
+                  0100000000000000000100640b7c0769017d0a7c0aa00c00000000000000
+                  000000000000000000000000007c006a040000000000000000a6010000ab
+                  01000000000000000001007c0a7c045f0400000000000000007c097c045f
+                  0700000000000000007c045300
                              0 COPY_FREE_VARS           1
                
                 27           2 RESUME                   0
                
                 28           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (create_request)
                             52 LOAD_FAST                1 (username)
                             54 LOAD_FAST                2 (password)
-                            56 PRECALL                  2
-                            60 CALL                     2
-                            70 STORE_FAST               4 (request)
-               
-                30          72 LOAD_CONST               1 ('https://console.jumpcloud.com/userconsole/xsrf')
-                            74 STORE_FAST               5 (xsrf_url)
-               
-                31          76 LOAD_GLOBAL              5 (NULL + requests)
-                            88 LOAD_ATTR                3 (get)
-               
-                32          98 LOAD_FAST                5 (xsrf_url)
-                           100 LOAD_FAST                0 (self)
-                           102 LOAD_ATTR                4 (headers)
-                           112 LOAD_FAST                3 (proxythread)
-                           114 LOAD_ATTR                5 (proxy_arg)
-               
-                31         124 KW_NAMES                 2
-                           126 PRECALL                  3
-                           130 CALL                     3
-                           140 STORE_FAST               6 (xsrf_response)
-               
-                34         142 LOAD_FAST                6 (xsrf_response)
-                           144 LOAD_METHOD              6 (json)
-                           166 PRECALL                  0
-                           170 CALL                     0
-                           180 LOAD_METHOD              3 (get)
-                           202 LOAD_CONST               3 ('xsrf')
-                           204 LOAD_CONST               4 ('')
-                           206 PRECALL                  2
-                           210 CALL                     2
-                           220 STORE_FAST               7 (xsrf_token)
-               
-                35         222 LOAD_FAST                6 (xsrf_response)
-                           224 LOAD_ATTR                7 (cookies)
-                           234 LOAD_METHOD              3 (get)
-                           256 LOAD_CONST               5 ('_xsrf')
-                           258 LOAD_CONST               4 ('')
-                           260 PRECALL                  2
-                           264 CALL                     2
-                           274 STORE_FAST               8 (xsrf_cookie)
-               
-                36         276 LOAD_FAST                7 (xsrf_token)
-                           278 POP_JUMP_FORWARD_IF_TRUE    37 (to 354)
-               
-                37         280 LOAD_GLOBAL             16 (log)
-                           292 LOAD_METHOD              9 (warning)
-               
-                38         314 LOAD_CONST               6 ('Failed to obtain XSRF token: ')
-                           316 LOAD_FAST                6 (xsrf_response)
-                           318 FORMAT_VALUE             0
-                           320 LOAD_CONST               7 (':')
-                           322 LOAD_FAST                6 (xsrf_response)
-                           324 LOAD_ATTR               10 (text)
-                           334 FORMAT_VALUE             0
-                           336 BUILD_STRING             4
-               
-                37         338 PRECALL                  1
-                           342 CALL                     1
-                           352 POP_TOP
-               
-                40     >>  354 LOAD_FAST                8 (xsrf_cookie)
-                           356 POP_JUMP_FORWARD_IF_TRUE    37 (to 432)
-               
-                41         358 LOAD_GLOBAL             16 (log)
-                           370 LOAD_METHOD              9 (warning)
-               
-                42         392 LOAD_CONST               8 ('Failed to obtain XSRF cookie: ')
-                           394 LOAD_FAST                6 (xsrf_response)
-                           396 FORMAT_VALUE             0
-                           398 LOAD_CONST               7 (':')
-                           400 LOAD_FAST                6 (xsrf_response)
-                           402 LOAD_ATTR                7 (cookies)
-                           412 FORMAT_VALUE             0
-                           414 BUILD_STRING             4
-               
-                41         416 PRECALL                  1
-                           420 CALL                     1
-                           430 POP_TOP
-               
-                44     >>  432 LOAD_GLOBAL             16 (log)
-                           444 LOAD_METHOD             11 (debug)
-                           466 LOAD_CONST               9 ('Token: ')
-                           468 LOAD_FAST                7 (xsrf_token)
-                           470 FORMAT_VALUE             0
-                           472 BUILD_STRING             2
-                           474 PRECALL                  1
-                           478 CALL                     1
-                           488 POP_TOP
-               
-                45         490 LOAD_GLOBAL             16 (log)
-                           502 LOAD_METHOD             11 (debug)
-                           524 LOAD_CONST              10 ('Cookie: ')
-                           526 LOAD_FAST                8 (xsrf_cookie)
-                           528 FORMAT_VALUE             0
-                           530 BUILD_STRING             2
-                           532 PRECALL                  1
-                           536 CALL                     1
-                           546 POP_TOP
-               
-                46         548 LOAD_CONST               5 ('_xsrf')
-                           550 LOAD_FAST                8 (xsrf_cookie)
-                           552 BUILD_MAP                1
-                           554 STORE_FAST               9 (cookies)
-               
-                47         556 LOAD_FAST                9 (cookies)
-                           558 LOAD_METHOD             12 (update)
-                           580 LOAD_FAST                0 (self)
-                           582 LOAD_ATTR                7 (cookies)
-                           592 PRECALL                  1
-                           596 CALL                     1
-                           606 POP_TOP
-               
-                49         608 LOAD_CONST              11 ('X-Xsrftoken')
-                           610 LOAD_FAST                7 (xsrf_token)
-               
-                48         612 BUILD_MAP                1
-                           614 STORE_FAST              10 (headers)
-               
-                51         616 LOAD_FAST               10 (headers)
-                           618 LOAD_METHOD             12 (update)
-                           640 LOAD_FAST                0 (self)
-                           642 LOAD_ATTR                4 (headers)
-                           652 PRECALL                  1
-                           656 CALL                     1
-                           666 POP_TOP
-               
-                53         668 LOAD_FAST               10 (headers)
-                           670 LOAD_FAST                4 (request)
-                           672 STORE_ATTR               4 (headers)
-               
-                54         682 LOAD_FAST                9 (cookies)
-                           684 LOAD_FAST                4 (request)
-                           686 STORE_ATTR               7 (cookies)
+                            56 LOAD_FAST                3 (proxythread)
+                            58 PRECALL                  3
+                            62 CALL                     3
+                            72 STORE_FAST               4 (request)
+               
+                30          74 LOAD_CONST               1 ('https://console.jumpcloud.com/userconsole/xsrf')
+                            76 STORE_FAST               5 (xsrf_url)
+               
+                31          78 LOAD_GLOBAL              5 (NULL + requests)
+                            90 LOAD_ATTR                3 (get)
+               
+                32         100 LOAD_FAST                5 (xsrf_url)
+                           102 LOAD_FAST                0 (self)
+                           104 LOAD_ATTR                4 (headers)
+                           114 LOAD_FAST                3 (proxythread)
+                           116 LOAD_ATTR                5 (proxy_arg)
+               
+                31         126 KW_NAMES                 2
+                           128 PRECALL                  3
+                           132 CALL                     3
+                           142 STORE_FAST               6 (xsrf_response)
+               
+                34         144 LOAD_FAST                6 (xsrf_response)
+                           146 LOAD_METHOD              6 (json)
+                           168 PRECALL                  0
+                           172 CALL                     0
+                           182 LOAD_METHOD              3 (get)
+                           204 LOAD_CONST               3 ('xsrf')
+                           206 LOAD_CONST               4 ('')
+                           208 PRECALL                  2
+                           212 CALL                     2
+                           222 STORE_FAST               7 (xsrf_token)
+               
+                35         224 LOAD_FAST                6 (xsrf_response)
+                           226 LOAD_ATTR                7 (cookies)
+                           236 LOAD_METHOD              3 (get)
+                           258 LOAD_CONST               5 ('_xsrf')
+                           260 LOAD_CONST               4 ('')
+                           262 PRECALL                  2
+                           266 CALL                     2
+                           276 STORE_FAST               8 (xsrf_cookie)
+               
+                36         278 LOAD_FAST                7 (xsrf_token)
+                           280 POP_JUMP_FORWARD_IF_TRUE    37 (to 356)
+               
+                37         282 LOAD_GLOBAL             16 (log)
+                           294 LOAD_METHOD              9 (warning)
+               
+                38         316 LOAD_CONST               6 ('Failed to obtain XSRF token: ')
+                           318 LOAD_FAST                6 (xsrf_response)
+                           320 FORMAT_VALUE             0
+                           322 LOAD_CONST               7 (':')
+                           324 LOAD_FAST                6 (xsrf_response)
+                           326 LOAD_ATTR               10 (text)
+                           336 FORMAT_VALUE             0
+                           338 BUILD_STRING             4
+               
+                37         340 PRECALL                  1
+                           344 CALL                     1
+                           354 POP_TOP
+               
+                40     >>  356 LOAD_FAST                8 (xsrf_cookie)
+                           358 POP_JUMP_FORWARD_IF_TRUE    37 (to 434)
+               
+                41         360 LOAD_GLOBAL             16 (log)
+                           372 LOAD_METHOD              9 (warning)
+               
+                42         394 LOAD_CONST               8 ('Failed to obtain XSRF cookie: ')
+                           396 LOAD_FAST                6 (xsrf_response)
+                           398 FORMAT_VALUE             0
+                           400 LOAD_CONST               7 (':')
+                           402 LOAD_FAST                6 (xsrf_response)
+                           404 LOAD_ATTR                7 (cookies)
+                           414 FORMAT_VALUE             0
+                           416 BUILD_STRING             4
+               
+                41         418 PRECALL                  1
+                           422 CALL                     1
+                           432 POP_TOP
+               
+                44     >>  434 LOAD_GLOBAL             16 (log)
+                           446 LOAD_METHOD             11 (debug)
+                           468 LOAD_CONST               9 ('Token: ')
+                           470 LOAD_FAST                7 (xsrf_token)
+                           472 FORMAT_VALUE             0
+                           474 BUILD_STRING             2
+                           476 PRECALL                  1
+                           480 CALL                     1
+                           490 POP_TOP
+               
+                45         492 LOAD_GLOBAL             16 (log)
+                           504 LOAD_METHOD             11 (debug)
+                           526 LOAD_CONST              10 ('Cookie: ')
+                           528 LOAD_FAST                8 (xsrf_cookie)
+                           530 FORMAT_VALUE             0
+                           532 BUILD_STRING             2
+                           534 PRECALL                  1
+                           538 CALL                     1
+                           548 POP_TOP
+               
+                46         550 LOAD_CONST               5 ('_xsrf')
+                           552 LOAD_FAST                8 (xsrf_cookie)
+                           554 BUILD_MAP                1
+                           556 STORE_FAST               9 (cookies)
+               
+                47         558 LOAD_FAST                9 (cookies)
+                           560 LOAD_METHOD             12 (update)
+                           582 LOAD_FAST                0 (self)
+                           584 LOAD_ATTR                7 (cookies)
+                           594 PRECALL                  1
+                           598 CALL                     1
+                           608 POP_TOP
+               
+                49         610 LOAD_CONST              11 ('X-Xsrftoken')
+                           612 LOAD_FAST                7 (xsrf_token)
+               
+                48         614 BUILD_MAP                1
+                           616 STORE_FAST              10 (headers)
+               
+                51         618 LOAD_FAST               10 (headers)
+                           620 LOAD_METHOD             12 (update)
+                           642 LOAD_FAST                0 (self)
+                           644 LOAD_ATTR                4 (headers)
+                           654 PRECALL                  1
+                           658 CALL                     1
+                           668 POP_TOP
+               
+                53         670 LOAD_FAST               10 (headers)
+                           672 LOAD_FAST                4 (request)
+                           674 STORE_ATTR               4 (headers)
+               
+                54         684 LOAD_FAST                9 (cookies)
+                           686 LOAD_FAST                4 (request)
+                           688 STORE_ATTR               7 (cookies)
                
-                55         696 LOAD_FAST                4 (request)
-                           698 RETURN_VALUE
+                55         698 LOAD_FAST                4 (request)
+                           700 RETURN_VALUE
                consts
                   None
                   'https://console.jumpcloud.com/userconsole/xsrf'
                   ('headers', 'proxies')
                   'xsrf'
                   ''
                   '_xsrf'
@@ -318,15 +319,15 @@
                varnames   ('self', 'username', 'password', 'proxythread', 'request', 'xsrf_url', 'xsrf_response', 'xsrf_token', 'xsrf_cookie', 'cookies', 'headers')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bls/Downloads/code/trevorspray/trevorspray/lib/sprayers/jumpcloud.py'
                name       'create_request'
                firstlineno 27
                lnotab
-                  0x04014402040116011aff1203500136010401220118ff10030401220118
+                  0x04014602040116011aff1203500136010401220118ff10030401220118
                   ff10033a013a010801340204ff040334020e010e01
             code
                argcount  : 2
                nlocals   : 7
                stacksize : 5
                flags     : 3
                code
```

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x43b0f364 (Sat Sep  2 21:59:31 2023 UTC)
-files sz: 3282
+moddate:  0xafe20465 (Fri Sep 15 23:03:11 2023 UTC)
+files sz: 3295
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640264036c016d025a020100640064046c036d
@@ -417,68 +417,69 @@
                lnotab
                   0x0201220102ff1003220102ff1003220102ff10033401220102ff10040e
                   0116016202340118013c01500148015c020e013e0216010e01440232014a
                   04220102ff10030e0244010e013402
             code
                argcount  : 4
                nlocals   : 5
-               stacksize : 4
+               stacksize : 5
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
-                  00a00100000000000000000000000000000000000000007c017c02a60200
-                  00ab0200000000000000007d047c006a020000000000000000720a7c017c
-                  0266027c045f0300000000000000006e157409000000000000000000007c
-                  017c02a6020000ab0200000000000000007c045f0300000000000000007c
-                  045300
+                  00a00100000000000000000000000000000000000000007c017c027c03a6
+                  030000ab0300000000000000007d047c006a020000000000000000720a7c
+                  017c0266027c045f0300000000000000006e157409000000000000000000
+                  007c017c02a6020000ab0200000000000000007c045f0300000000000000
+                  007c045300
                              0 COPY_FREE_VARS           1
                
                 66           2 RESUME                   0
                
                 71           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (create_request)
                             52 LOAD_FAST                1 (username)
                             54 LOAD_FAST                2 (password)
-                            56 PRECALL                  2
-                            60 CALL                     2
-                            70 STORE_FAST               4 (r)
-               
-                72          72 LOAD_FAST                0 (self)
-                            74 LOAD_ATTR                2 (o365)
-                            84 POP_JUMP_FORWARD_IF_FALSE    10 (to 106)
-               
-                73          86 LOAD_FAST                1 (username)
-                            88 LOAD_FAST                2 (password)
-                            90 BUILD_TUPLE              2
-                            92 LOAD_FAST                4 (r)
-                            94 STORE_ATTR               3 (auth)
-                           104 JUMP_FORWARD            21 (to 148)
-               
-                75     >>  106 LOAD_GLOBAL              9 (NULL + HttpNtlmAuth)
-                           118 LOAD_FAST                1 (username)
-                           120 LOAD_FAST                2 (password)
-                           122 PRECALL                  2
-                           126 CALL                     2
-                           136 LOAD_FAST                4 (r)
-                           138 STORE_ATTR               3 (auth)
+                            56 LOAD_FAST                3 (proxythread)
+                            58 PRECALL                  3
+                            62 CALL                     3
+                            72 STORE_FAST               4 (r)
+               
+                72          74 LOAD_FAST                0 (self)
+                            76 LOAD_ATTR                2 (o365)
+                            86 POP_JUMP_FORWARD_IF_FALSE    10 (to 108)
+               
+                73          88 LOAD_FAST                1 (username)
+                            90 LOAD_FAST                2 (password)
+                            92 BUILD_TUPLE              2
+                            94 LOAD_FAST                4 (r)
+                            96 STORE_ATTR               3 (auth)
+                           106 JUMP_FORWARD            21 (to 150)
+               
+                75     >>  108 LOAD_GLOBAL              9 (NULL + HttpNtlmAuth)
+                           120 LOAD_FAST                1 (username)
+                           122 LOAD_FAST                2 (password)
+                           124 PRECALL                  2
+                           128 CALL                     2
+                           138 LOAD_FAST                4 (r)
+                           140 STORE_ATTR               3 (auth)
                
-                76     >>  148 LOAD_FAST                4 (r)
-                           150 RETURN_VALUE
+                76     >>  150 LOAD_FAST                4 (r)
+                           152 RETURN_VALUE
                consts
                   '\n        Returns request.Request() object\n        '
                names      ('super', 'create_request', 'o365', 'auth', 'HttpNtlmAuth')
                varnames   ('self', 'username', 'password', 'proxythread', 'r')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/bls/Downloads/code/trevorspray/trevorspray/lib/sprayers/owa.py'
                name       'create_request'
                firstlineno 66
-               lnotab 0x040544010e0114022a01
+               lnotab 0x040546010e0114022a01
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 7
                flags     : 3
                code
                   0x970064017d0264017d0364017d04740100000000000000000000740300
```

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/adfs.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/adfs.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/anyconnect.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/anyconnect.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/auth0.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/auth0.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/base.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/base.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/example.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/example.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/google.py.bak` & `trevorspray-2.3.0/trevorspray/lib/sprayers/google.py.bak`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/jumpcloud.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/jumpcloud.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/msol.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/msol.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,18 +90,23 @@
                 valid = True
                 msg = f"AADSTS530031: Valid credential, but access policy does not allow token issuance."
 
             elif "AADSTS50034" in error:
                 exists = False
                 msg = f"AADSTS50034: User does not exist."
 
-            elif "AADSTS50079" in error or "AADSTS50076" in error:
+            elif "AADSTS50076" in error:
                 valid = True
                 # Microsoft MFA response
-                msg = f"AADSTS50079: The response indicates MFA (Microsoft) is in use."
+                msg = f"AADSTS50076: The response indicates MFA (Microsoft) is in use."
+
+            elif "AADSTS50079" in error:
+                valid = True
+                # Microsoft MFA response
+                msg = f"AADSTS50079: The response indicates MFA (Microsoft) must be onboarded!"
 
             elif "AADSTS50055" in error:
                 valid = True
                 # User password is expired
                 msg = f"AADSTS50055: The user's password is expired."
 
             elif "AADSTS50131" in error:
```

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/okta.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/okta.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/sprayers/owa.py` & `trevorspray-2.3.0/trevorspray/lib/sprayers/owa.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/trevor.py` & `trevorspray-2.3.0/trevorspray/lib/trevor.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc` & `trevorspray-2.3.0/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/misc.py` & `trevorspray-2.3.0/trevorspray/lib/util/misc.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/ntlmdecoder.py` & `trevorspray-2.3.0/trevorspray/lib/util/ntlmdecoder.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/lib/util/threadpool.py` & `trevorspray-2.3.0/trevorspray/lib/util/threadpool.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/trevorspray/trevorproxy.py.bak` & `trevorspray-2.3.0/trevorspray/trevorproxy.py.bak`

 * *Files identical despite different names*

### Comparing `trevorspray-2.2.1/PKG-INFO` & `trevorspray-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: trevorspray
-Version: 2.2.1
+Version: 2.3.0
 Summary: A modular password sprayer with threading, SSH proxying, loot modules, and more
 Home-page: https://github.com/blacklanternsecurity/TREVORspray
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PySocks (>=1.7.1,<2.0.0)
 Requires-Dist: Pygments (>=2.10.0,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: exchangelib (>=4.6.1,<5.0.0)
 Requires-Dist: mechanicalsoup (>=1.3.0,<2.0.0)
 Requires-Dist: sh (>=1.14.2,<2.0.0)
 Requires-Dist: tldextract (>=3.1.2,<4.0.0)
```

