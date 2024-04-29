# Comparing `tmp/gcp-releasetool-2.0.0rc1.tar.gz` & `tmp/gcp-releasetool-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-releasetool-2.0.0rc1.tar", last modified: Wed Feb  7 01:47:58 2024, max compression
+gzip compressed data, was "gcp-releasetool-2.0.1.tar", last modified: Mon Apr 29 20:09:15 2024, max compression
```

## Comparing `gcp-releasetool-2.0.0rc1.tar` & `gcp-releasetool-2.0.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.932550 gcp-releasetool-2.0.0rc1/
--rw-rw-r--   0 root         (0)     1003    11358 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/LICENSE
--rw-rw-r--   0 root         (0)     1003       60 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003      787 2024-02-07 01:47:58.932550 gcp-releasetool-2.0.0rc1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2069 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.924549 gcp-releasetool-2.0.0rc1/autorelease/
--rw-rw-r--   0 root         (0)     1003        0 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/autorelease/__init__.py
--rw-rw-r--   0 root         (0)     1003     3438 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/autorelease/__main__.py
--rw-rw-r--   0 root         (0)     1003     3305 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/autorelease/common.py
--rw-rw-r--   0 root         (0)     1003     9001 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/autorelease/github.py
--rw-rw-r--   0 root         (0)     1003     3500 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/autorelease/kokoro.py
--rw-rw-r--   0 root         (0)     1003     1787 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/autorelease/reporter.py
--rw-rw-r--   0 root         (0)     1003     5246 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/autorelease/tag.py
--rw-rw-r--   0 root         (0)     1003    10355 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/autorelease/trigger.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.924549 gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/
--rw-r--r--   0 root         (0)     1003      787 2024-02-07 01:47:58.000000 gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1649 2024-02-07 01:47:58.000000 gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-02-07 01:47:58.000000 gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       59 2024-02-07 01:47:58.000000 gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003        1 2024-02-07 01:47:58.000000 gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      204 2024-02-07 01:47:58.000000 gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       37 2024-02-07 01:47:58.000000 gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.924549 gcp-releasetool-2.0.0rc1/protos/
--rw-rw-r--   0 root         (0)     1003        0 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/protos/__init__.py
--rw-rw-r--   0 root         (0)     1003     5134 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/protos/kokoro_api_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.924549 gcp-releasetool-2.0.0rc1/releasetool/
--rw-rw-r--   0 root         (0)     1003      638 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/__init__.py
--rw-rw-r--   0 root         (0)     1003     6772 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/__main__.py
--rw-rw-r--   0 root         (0)     1003     4296 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/circleci.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.928550 gcp-releasetool-2.0.0rc1/releasetool/commands/
--rw-rw-r--   0 root         (0)     1003        0 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/__init__.py
--rw-rw-r--   0 root         (0)     1003     6214 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/common.py
--rw-rw-r--   0 root         (0)     1003     6108 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/publish_reporter.py
--rw-rw-r--   0 root         (0)     1003     1958 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/publish_reporter.sh
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.928550 gcp-releasetool-2.0.0rc1/releasetool/commands/start/
--rw-rw-r--   0 root         (0)     1003        0 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/start/__init__.py
--rw-rw-r--   0 root         (0)     1003     8090 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/start/go.py
--rw-rw-r--   0 root         (0)     1003    13934 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/start/java.py
--rw-rw-r--   0 root         (0)     1003     7501 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/start/nodejs.py
--rw-rw-r--   0 root         (0)     1003     8303 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/start/python.py
--rw-rw-r--   0 root         (0)     1003     2268 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/start/python_tool.py
--rw-rw-r--   0 root         (0)     1003     8739 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/start/ruby.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.928550 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/
--rw-rw-r--   0 root         (0)     1003        0 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/__init__.py
--rw-rw-r--   0 root         (0)     1003     1138 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/cpp.py
--rw-rw-r--   0 root         (0)     1003     4833 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/dotnet.py
--rw-rw-r--   0 root         (0)     1003     1145 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/go.py
--rw-rw-r--   0 root         (0)     1003     3976 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/java.py
--rw-rw-r--   0 root         (0)     1003     7683 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/nodejs.py
--rw-rw-r--   0 root         (0)     1003     1874 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/php.py
--rw-rw-r--   0 root         (0)     1003     5849 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/python.py
--rw-rw-r--   0 root         (0)     1003     3475 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/python_tool.py
--rw-rw-r--   0 root         (0)     1003     8329 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/commands/tag/ruby.py
--rw-rw-r--   0 root         (0)     1003     2366 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/filehelpers.py
--rw-rw-r--   0 root         (0)     1003     4056 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/git.py
--rw-rw-r--   0 root         (0)     1003     9773 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/github.py
--rw-rw-r--   0 root         (0)     1003     1137 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/secrets.py
--rw-rw-r--   0 root         (0)     1003     1910 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/releasetool/update_check.py
--rw-r--r--   0 root         (0)     1003       38 2024-02-07 01:47:58.932550 gcp-releasetool-2.0.0rc1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2125 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 01:47:58.932550 gcp-releasetool-2.0.0rc1/tests/
--rw-rw-r--   0 root         (0)     1003        0 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003    65497 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/tests/common_test.py
--rw-rw-r--   0 root         (0)     1003     6890 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/tests/test_autorelease_tag.py
--rw-rw-r--   0 root         (0)     1003    15311 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/tests/test_autorelease_trigger.py
--rw-rw-r--   0 root         (0)     1003       34 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/tests/test_dummy.py
--rw-rw-r--   0 root         (0)     1003     1234 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/tests/test_github.py
--rw-rw-r--   0 root         (0)     1003     1715 2024-02-07 01:45:55.000000 gcp-releasetool-2.0.0rc1/tests/test_publish_reporter.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.280384 gcp-releasetool-2.0.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003       60 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003      784 2024-04-29 20:09:15.280384 gcp-releasetool-2.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2069 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.268382 gcp-releasetool-2.0.1/autorelease/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/autorelease/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3438 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/autorelease/__main__.py
+-rw-rw-r--   0 root         (0)     1003     3305 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/autorelease/common.py
+-rw-rw-r--   0 root         (0)     1003     9001 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/autorelease/github.py
+-rw-rw-r--   0 root         (0)     1003     3500 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/autorelease/kokoro.py
+-rw-rw-r--   0 root         (0)     1003     1787 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/autorelease/reporter.py
+-rw-rw-r--   0 root         (0)     1003     5246 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/autorelease/tag.py
+-rw-rw-r--   0 root         (0)     1003    10355 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/autorelease/trigger.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.272383 gcp-releasetool-2.0.1/gcp_releasetool.egg-info/
+-rw-r--r--   0 root         (0)     1003      784 2024-04-29 20:09:15.000000 gcp-releasetool-2.0.1/gcp_releasetool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1649 2024-04-29 20:09:15.000000 gcp-releasetool-2.0.1/gcp_releasetool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-29 20:09:15.000000 gcp-releasetool-2.0.1/gcp_releasetool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       59 2024-04-29 20:09:15.000000 gcp-releasetool-2.0.1/gcp_releasetool.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-29 20:09:15.000000 gcp-releasetool-2.0.1/gcp_releasetool.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      204 2024-04-29 20:09:15.000000 gcp-releasetool-2.0.1/gcp_releasetool.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       37 2024-04-29 20:09:15.000000 gcp-releasetool-2.0.1/gcp_releasetool.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.272383 gcp-releasetool-2.0.1/protos/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/protos/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5134 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/protos/kokoro_api_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.272383 gcp-releasetool-2.0.1/releasetool/
+-rw-rw-r--   0 root         (0)     1003      638 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6772 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/__main__.py
+-rw-rw-r--   0 root         (0)     1003     4296 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/circleci.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.272383 gcp-releasetool-2.0.1/releasetool/commands/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6173 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/common.py
+-rw-rw-r--   0 root         (0)     1003     6108 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/publish_reporter.py
+-rw-rw-r--   0 root         (0)     1003     1958 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/publish_reporter.sh
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.276383 gcp-releasetool-2.0.1/releasetool/commands/start/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/start/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8090 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/start/go.py
+-rw-rw-r--   0 root         (0)     1003    13934 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/start/java.py
+-rw-rw-r--   0 root         (0)     1003     7501 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/start/nodejs.py
+-rw-rw-r--   0 root         (0)     1003     8303 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/start/python.py
+-rw-rw-r--   0 root         (0)     1003     2268 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/start/python_tool.py
+-rw-rw-r--   0 root         (0)     1003     8739 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/start/ruby.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.276383 gcp-releasetool-2.0.1/releasetool/commands/tag/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1138 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/cpp.py
+-rw-rw-r--   0 root         (0)     1003     4833 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/dotnet.py
+-rw-rw-r--   0 root         (0)     1003     1145 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/go.py
+-rw-rw-r--   0 root         (0)     1003     3976 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/java.py
+-rw-rw-r--   0 root         (0)     1003     7683 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/nodejs.py
+-rw-rw-r--   0 root         (0)     1003     1879 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/php.py
+-rw-rw-r--   0 root         (0)     1003     5849 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/python.py
+-rw-rw-r--   0 root         (0)     1003     3475 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/python_tool.py
+-rw-rw-r--   0 root         (0)     1003     8329 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/commands/tag/ruby.py
+-rw-rw-r--   0 root         (0)     1003     2366 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/filehelpers.py
+-rw-rw-r--   0 root         (0)     1003     4056 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/git.py
+-rw-rw-r--   0 root         (0)     1003     9773 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/github.py
+-rw-rw-r--   0 root         (0)     1003     1137 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/secrets.py
+-rw-rw-r--   0 root         (0)     1003     1910 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/releasetool/update_check.py
+-rw-r--r--   0 root         (0)     1003       38 2024-04-29 20:09:15.280384 gcp-releasetool-2.0.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2122 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-29 20:09:15.280384 gcp-releasetool-2.0.1/tests/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003    65497 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/tests/common_test.py
+-rw-rw-r--   0 root         (0)     1003     6890 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/tests/test_autorelease_tag.py
+-rw-rw-r--   0 root         (0)     1003    15311 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/tests/test_autorelease_trigger.py
+-rw-rw-r--   0 root         (0)     1003       34 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/tests/test_dummy.py
+-rw-rw-r--   0 root         (0)     1003     1234 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/tests/test_github.py
+-rw-rw-r--   0 root         (0)     1003     1715 2024-04-29 20:07:18.000000 gcp-releasetool-2.0.1/tests/test_publish_reporter.py
```

### Comparing `gcp-releasetool-2.0.0rc1/LICENSE` & `gcp-releasetool-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/PKG-INFO` & `gcp-releasetool-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-releasetool
-Version: 2.0.0rc1
+Version: 2.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Google LLC
 Author-email: theaflowers@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gcp-releasetool-2.0.0rc1/README.md` & `gcp-releasetool-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/autorelease/__main__.py` & `gcp-releasetool-2.0.1/autorelease/__main__.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/autorelease/common.py` & `gcp-releasetool-2.0.1/autorelease/common.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/autorelease/github.py` & `gcp-releasetool-2.0.1/autorelease/github.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/autorelease/kokoro.py` & `gcp-releasetool-2.0.1/autorelease/kokoro.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/autorelease/reporter.py` & `gcp-releasetool-2.0.1/autorelease/reporter.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/autorelease/tag.py` & `gcp-releasetool-2.0.1/autorelease/tag.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/autorelease/trigger.py` & `gcp-releasetool-2.0.1/autorelease/trigger.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/PKG-INFO` & `gcp-releasetool-2.0.1/gcp_releasetool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-releasetool
-Version: 2.0.0rc1
+Version: 2.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Google LLC
 Author-email: theaflowers@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gcp-releasetool-2.0.0rc1/gcp_releasetool.egg-info/SOURCES.txt` & `gcp-releasetool-2.0.1/gcp_releasetool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/protos/kokoro_api_pb2.py` & `gcp-releasetool-2.0.1/protos/kokoro_api_pb2.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/__init__.py` & `gcp-releasetool-2.0.1/releasetool/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/__main__.py` & `gcp-releasetool-2.0.1/releasetool/__main__.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/circleci.py` & `gcp-releasetool-2.0.1/releasetool/circleci.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/common.py` & `gcp-releasetool-2.0.1/releasetool/commands/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,19 +165,16 @@
     if release is not None and tag_sha == ctx.release_pr["merge_commit_sha"]:
         return True
     else:
         return False
 
 
 def publish_via_kokoro(ctx: TagContext) -> None:
-    kokoro_url = "https://fusion.corp.google.com/projectanalysis/current/KOKORO/"
-
-    ctx.fusion_url = parse.urljoin(
-        kokoro_url, parse.quote_plus(f"prod:{ctx.kokoro_job_name}")
-    )
+    kokoro_url = "https://fusion2.corp.google.com/ci;prev=s/kokoro/prod"
+    ctx.fusion_url = f"${kokoro_url}:${parse.quote_plus(ctx.kokoro_job_name)}"
 
     if ctx.interactive:
         pyperclip.copy(ctx.release_tag)
 
         click.secho(
             "> Trigger the Kokoro build with the commitish below to publish to PyPI. The commitish has been copied to the clipboard.",
             fg="cyan",
```

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/publish_reporter.py` & `gcp-releasetool-2.0.1/releasetool/commands/publish_reporter.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/publish_reporter.sh` & `gcp-releasetool-2.0.1/releasetool/commands/publish_reporter.sh`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/start/go.py` & `gcp-releasetool-2.0.1/releasetool/commands/start/go.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/start/java.py` & `gcp-releasetool-2.0.1/releasetool/commands/start/java.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/start/nodejs.py` & `gcp-releasetool-2.0.1/releasetool/commands/start/nodejs.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/start/python.py` & `gcp-releasetool-2.0.1/releasetool/commands/start/python.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/start/python_tool.py` & `gcp-releasetool-2.0.1/releasetool/commands/start/python_tool.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/start/ruby.py` & `gcp-releasetool-2.0.1/releasetool/commands/start/ruby.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/cpp.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/cpp.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/dotnet.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/dotnet.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/go.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/go.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/java.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/java.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/nodejs.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/nodejs.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/php.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/php.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Returns:
         The name of the Kokoro job to trigger or None if there is no job to trigger
     """
     repo_short_name = upstream_repo.split("/")[-1]
 
     if repo_short_name == "google-cloud-php":
-        return "cloud-devrel/client-libraries/php/google-cloud-php/docs"
+        return "cloud-devrel/client-libraries/php/google-cloud-php/docs/docs"
     else:
         return f"cloud-devrel/client-libraries/php/{upstream_repo}/release"
 
 
 def package_name(pull: dict) -> Union[str, None]:
     return None
```

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/python.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/python.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/python_tool.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/python_tool.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/commands/tag/ruby.py` & `gcp-releasetool-2.0.1/releasetool/commands/tag/ruby.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/filehelpers.py` & `gcp-releasetool-2.0.1/releasetool/filehelpers.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/git.py` & `gcp-releasetool-2.0.1/releasetool/git.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/github.py` & `gcp-releasetool-2.0.1/releasetool/github.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/secrets.py` & `gcp-releasetool-2.0.1/releasetool/secrets.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/releasetool/update_check.py` & `gcp-releasetool-2.0.1/releasetool/update_check.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/setup.py` & `gcp-releasetool-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 
 name = 'gcp-releasetool'
 description = ''
-version = "2.0.0rc1"
+version = "2.0.1"
 release_status = 'Development Status :: 3 - Alpha'
 dependencies = [
     "requests>=2.31.0",
     "attrs>=20.1.0",
     "click>=8.0.4, <8.1.0",
     "cryptography>=42",
     "google-auth>=2.22.0",
```

### Comparing `gcp-releasetool-2.0.0rc1/tests/common_test.py` & `gcp-releasetool-2.0.1/tests/common_test.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/tests/test_autorelease_tag.py` & `gcp-releasetool-2.0.1/tests/test_autorelease_tag.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/tests/test_autorelease_trigger.py` & `gcp-releasetool-2.0.1/tests/test_autorelease_trigger.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/tests/test_github.py` & `gcp-releasetool-2.0.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gcp-releasetool-2.0.0rc1/tests/test_publish_reporter.py` & `gcp-releasetool-2.0.1/tests/test_publish_reporter.py`

 * *Files identical despite different names*

