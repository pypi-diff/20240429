# Comparing `tmp/json-spec-0.9.8.tar.gz` & `tmp/json-spec-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-spec-0.9.8.tar", last modified: Thu Jul 24 12:58:38 2014, max compression
+gzip compressed data, was "dist/json-spec-0.9.9.tar", last modified: Wed Aug 13 14:01:55 2014, max compression
```

## Comparing `json-spec-0.9.8.tar` & `json-spec-0.9.9.tar`

### file list

```diff
@@ -1,582 +1,3427 @@
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       79 2014-06-08 13:14:34.000000 json-spec-0.9.8/.coveragerc
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      111 2014-07-17 03:32:17.000000 json-spec-0.9.8/.gitmodules
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      179 2014-07-17 09:49:47.000000 json-spec-0.9.8/.travis.yml
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      126 2014-07-24 12:58:37.000000 json-spec-0.9.8/AUTHORS
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2131 2014-07-24 12:58:37.000000 json-spec-0.9.8/ChangeLog
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3165 2014-06-10 14:39:26.000000 json-spec-0.9.8/CONTRIBUTING.rst
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/docs/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      171 2014-06-04 11:18:59.000000 json-spec-0.9.8/docs/authors.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1170 2014-07-23 13:23:03.000000 json-spec-0.9.8/docs/cli.rst
--rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)     8598 2014-07-24 12:49:21.000000 json-spec-0.9.8/docs/conf.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       32 2014-06-02 06:54:20.000000 json-spec-0.9.8/docs/contributing.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       51 2014-06-10 12:14:08.000000 json-spec-0.9.8/docs/history.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2231 2014-07-23 13:23:03.000000 json-spec-0.9.8/docs/index.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      362 2014-06-10 14:03:00.000000 json-spec-0.9.8/docs/installation.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     6466 2014-06-02 06:54:20.000000 json-spec-0.9.8/docs/make.bat
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     6777 2014-06-02 06:54:20.000000 json-spec-0.9.8/docs/Makefile
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3866 2014-06-10 12:07:29.000000 json-spec-0.9.8/docs/operations.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3165 2014-07-18 09:56:13.000000 json-spec-0.9.8/docs/pointer.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2546 2014-06-10 12:02:55.000000 json-spec-0.9.8/docs/reference.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       35 2014-07-23 13:29:04.000000 json-spec-0.9.8/docs/requirements.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4243 2014-07-18 10:15:51.000000 json-spec-0.9.8/docs/validators.rst
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/examples/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      325 2014-06-02 06:59:41.000000 json-spec-0.9.8/examples/basic.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1311 2014-06-02 15:32:59.000000 json-spec-0.9.8/examples/simple.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      793 2014-07-16 16:38:08.000000 json-spec-0.9.8/examples/test.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       99 2014-06-02 06:54:20.000000 json-spec-0.9.8/HISTORY.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1476 2014-06-04 11:18:59.000000 json-spec-0.9.8/LICENSE
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      288 2014-06-09 12:06:15.000000 json-spec-0.9.8/MANIFEST.in
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5414 2014-07-24 12:58:38.000000 json-spec-0.9.8/PKG-INFO
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)        0 2014-06-10 11:52:21.000000 json-spec-0.9.8/pytest.ini
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3405 2014-07-23 13:23:03.000000 json-spec-0.9.8/README.rst
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       29 2014-07-17 09:54:23.000000 json-spec-0.9.8/requirements-py27.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       29 2014-07-17 09:54:19.000000 json-spec-0.9.8/requirements-py32.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       29 2014-07-17 09:54:18.000000 json-spec-0.9.8/requirements-pypy.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)        4 2014-07-17 09:36:42.000000 json-spec-0.9.8/requirements.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2204 2014-07-24 12:58:38.000000 json-spec-0.9.8/setup.cfg
--rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)      281 2014-07-23 13:23:03.000000 json-spec-0.9.8/setup.py
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/json_spec.egg-info/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)        1 2014-07-24 12:58:37.000000 json-spec-0.9.8/src/json_spec.egg-info/dependency_links.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      871 2014-07-24 12:58:37.000000 json-spec-0.9.8/src/json_spec.egg-info/entry_points.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)        1 2014-06-09 09:45:21.000000 json-spec-0.9.8/src/json_spec.egg-info/not-zip-safe
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5414 2014-07-24 12:58:37.000000 json-spec-0.9.8/src/json_spec.egg-info/PKG-INFO
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4132 2014-06-10 14:39:26.000000 json-spec-0.9.8/src/json_spec.egg-info/PKG-INFO 2
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      103 2014-07-24 12:58:37.000000 json-spec-0.9.8/src/json_spec.egg-info/requires.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)    23853 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/json_spec.egg-info/SOURCES.txt
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)        9 2014-07-24 12:58:37.000000 json-spec-0.9.8/src/json_spec.egg-info/top_level.txt
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/
--rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)       35 2014-06-09 09:37:06.000000 json-spec-0.9.8/src/jsonspec/__init__.py
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/cli/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3780 2014-07-24 12:56:47.000000 json-spec-0.9.8/src/jsonspec/cli/__init__.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1756 2014-07-23 13:23:03.000000 json-spec-0.9.8/src/jsonspec/cli/parsers.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      677 2014-07-17 11:19:49.000000 json-spec-0.9.8/src/jsonspec/driver.py
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/misc/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)        0 2014-06-09 10:06:11.000000 json-spec-0.9.8/src/jsonspec/misc/__init__.py
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      638 2014-06-08 15:04:49.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/address.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1102 2014-06-08 14:45:08.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/calendar.json
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1791 2014-06-08 15:04:58.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/card.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      897 2014-06-08 14:50:47.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/hyper-schema.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      394 2014-06-08 14:57:43.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/json-ref.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      394 2014-06-08 14:56:15.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/links.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2476 2014-06-08 14:53:02.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/schema.json
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-04/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4816 2014-06-08 14:44:30.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-04/hyper-schema.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4375 2014-06-08 14:43:08.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/draft-04/schema.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      184 2014-06-08 14:44:58.000000 json-spec-0.9.8/src/jsonspec/misc/schemas/geo.json
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/operations/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2384 2014-06-10 11:50:29.000000 json-spec-0.9.8/src/jsonspec/operations/__init__.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     6389 2014-07-17 10:34:28.000000 json-spec-0.9.8/src/jsonspec/operations/bases.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      258 2014-06-10 10:59:26.000000 json-spec-0.9.8/src/jsonspec/operations/exceptions.py
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/pointer/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1042 2014-07-23 13:23:03.000000 json-spec-0.9.8/src/jsonspec/pointer/__init__.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     7571 2014-07-23 13:23:03.000000 json-spec-0.9.8/src/jsonspec/pointer/bases.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1591 2014-07-23 13:23:03.000000 json-spec-0.9.8/src/jsonspec/pointer/exceptions.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1859 2014-07-16 07:02:29.000000 json-spec-0.9.8/src/jsonspec/pointer/stages.py
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/reference/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1660 2014-06-10 12:35:57.000000 json-spec-0.9.8/src/jsonspec/reference/__init__.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3015 2014-07-17 03:32:17.000000 json-spec-0.9.8/src/jsonspec/reference/bases.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      256 2014-06-09 10:05:56.000000 json-spec-0.9.8/src/jsonspec/reference/exceptions.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4663 2014-07-17 10:30:17.000000 json-spec-0.9.8/src/jsonspec/reference/providers.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      910 2014-06-09 10:05:49.000000 json-spec-0.9.8/src/jsonspec/reference/util.py
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/src/jsonspec/validators/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1278 2014-07-23 07:21:19.000000 json-spec-0.9.8/src/jsonspec/validators/__init__.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2461 2014-07-24 12:47:00.000000 json-spec-0.9.8/src/jsonspec/validators/bases.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)    26433 2014-07-24 12:47:00.000000 json-spec-0.9.8/src/jsonspec/validators/draft03.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)    25855 2014-07-24 12:47:00.000000 json-spec-0.9.8/src/jsonspec/validators/draft04.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2208 2014-07-24 12:47:00.000000 json-spec-0.9.8/src/jsonspec/validators/exceptions.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3884 2014-07-17 15:59:07.000000 json-spec-0.9.8/src/jsonspec/validators/factorize.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3849 2014-07-17 10:02:03.000000 json-spec-0.9.8/src/jsonspec/validators/formats.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      348 2014-07-24 12:47:00.000000 json-spec-0.9.8/src/jsonspec/validators/pointer_util.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     7628 2014-07-24 12:46:53.000000 json-spec-0.9.8/src/jsonspec/validators/util.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)        6 2014-06-10 13:58:06.000000 json-spec-0.9.8/test-requirements.txt
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3178 2014-07-24 09:07:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13747.767380
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3184 2014-07-24 09:07:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13750.659383
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3196 2014-07-24 09:07:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13751.870161
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3202 2014-07-24 09:07:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13754.725564
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-07-24 09:07:18.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13757.87138
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3172 2014-07-24 09:07:18.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13759.913660
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3172 2014-07-24 09:07:18.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13760.814424
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3180 2014-07-24 09:07:18.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13763.284703
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3182 2014-07-24 09:07:19.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13765.696865
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3182 2014-07-24 09:07:19.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13766.217187
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3122 2014-07-24 09:07:19.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13767.563441
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3116 2014-07-24 09:07:19.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13772.315171
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4574 2014-07-24 09:07:20.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13774.53270
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4532 2014-07-24 09:07:20.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13776.480507
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3178 2014-07-24 09:13:03.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13848.148603
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3184 2014-07-24 09:13:03.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13851.883200
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3196 2014-07-24 09:13:03.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13852.658197
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3202 2014-07-24 09:13:03.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13855.981187
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-07-24 09:13:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13858.162103
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3172 2014-07-24 09:13:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13860.756322
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3172 2014-07-24 09:13:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13861.558717
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3180 2014-07-24 09:13:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13864.839483
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3182 2014-07-24 09:13:05.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13866.711117
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3182 2014-07-24 09:13:05.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13867.481307
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3122 2014-07-24 09:13:05.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13868.292406
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3116 2014-07-24 09:13:05.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13873.16479
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4572 2014-07-24 09:13:05.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13875.755524
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4532 2014-07-24 09:13:06.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13877.538157
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:54:47.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2890.971498
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:54:47.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2893.380811
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:54:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2894.793495
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:55:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2928.597283
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:55:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2931.192801
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:55:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2932.217942
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:55:18.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2936.233109
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:55:18.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2940.212753
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:56:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2955.883132
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:56:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2958.989772
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:56:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2959.860425
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:56:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2963.816177
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:56:04.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2965.224896
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:56:52.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2982.986653
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:56:52.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2985.374311
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:56:52.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2986.865546
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:56:52.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2990.591765
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:56:53.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2992.165742
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:56:53.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2995.662249
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:56:53.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2998.744678
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:57:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3037.34254
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:57:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3040.245703
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 08:57:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3041.402808
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 08:57:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3044.851117
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:57:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3045.205944
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:57:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3049.367076
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:57:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3051.497611
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:57:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3054.349643
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:57:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3057.398766
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:58:54.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3085.965903
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:58:54.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3088.825419
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 08:58:55.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3089.232615
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 08:58:55.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3092.436248
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:58:55.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3095.904202
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:58:55.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3097.390316
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:58:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3100.97279
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:58:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3103.875510
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:58:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3105.771180
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:58:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3106.253758
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:58:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3107.994561
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:16.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3120.464422
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:59:16.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3125.43493
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 08:59:16.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3126.120944
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 08:59:16.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3129.405140
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:59:16.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3132.21149
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:59:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3134.760557
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:59:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3135.702900
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:59:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3138.345249
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3140.618324
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:17.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3141.304302
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:59:18.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3142.803594
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 08:59:18.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3147.599067
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:53.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3158.411930
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:59:53.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3161.934483
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 08:59:53.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3162.638446
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 08:59:53.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3165.30416
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:59:54.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3170.833718
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:59:54.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3172.319935
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:59:54.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3173.761134
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:59:54.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3176.720397
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:55.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3178.85727
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:55.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3179.868910
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:59:55.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3180.240143
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 08:59:55.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3185.704742
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:09.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3196.399093
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:00:09.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3199.588691
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:00:10.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3200.680544
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:00:10.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3203.440856
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:00:10.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3206.290324
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:10.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3208.564692
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:10.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3209.81838
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:00:11.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3212.832848
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:11.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3214.644239
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:11.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3215.524698
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:00:11.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3216.42847
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:00:12.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3221.533410
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3234.388312
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:00:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3239.775417
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:00:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3240.557245
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:00:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3243.788730
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:00:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3246.569653
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3248.843454
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3249.165956
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:00:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3252.306359
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3254.372835
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3255.163085
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:00:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3256.990053
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:00:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3261.351666
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3270.227618
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:00:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3273.65115
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:00:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3274.237674
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:00:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3277.19176
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:00:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3280.898598
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3282.817350
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3283.45632
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:00:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3286.420993
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3288.53949
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3289.352556
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:00:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3290.992008
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:00:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3295.184522
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:03:42.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3371.384759
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:03:42.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3374.818857
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:03:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3375.499649
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:03:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3378.68842
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:03:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3381.949045
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:03:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3383.803880
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:03:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3384.450316
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:03:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3387.830297
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:03:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3389.699913
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:03:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3390.518846
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:03:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3391.881649
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:03:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3396.541112
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:04:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3441.966418
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:04:45.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3444.746082
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:04:45.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3445.389212
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:04:45.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3448.669825
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:04:45.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3451.277331
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:04:45.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3453.289143
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:04:46.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3454.270660
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:04:46.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3457.246427
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:04:46.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3459.861391
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:04:46.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3460.34642
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:04:46.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3461.488045
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:04:47.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3466.73300
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:22.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3486.358902
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:05:22.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3489.33416
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:05:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3490.359594
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:05:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3493.956052
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:05:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3496.412731
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:05:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3498.678016
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:05:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3499.653310
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:05:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3502.596799
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3504.746277
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3506.628550
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:05:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3507.403336
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:05:25.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3512.572538
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:42.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3529.610576
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:05:42.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3532.775761
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:05:42.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3533.315530
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:05:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3536.588954
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:05:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3539.967848
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:05:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3541.22712
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:05:43.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3542.763221
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:05:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3545.825074
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3547.736530
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3548.135588
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:05:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3549.508720
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:05:44.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3554.240623
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 09:22:22.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3972.942596
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:22:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3975.159309
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 09:22:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3976.791534
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 09:22:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3979.772513
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:22:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3982.279342
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 09:22:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3984.468176
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 09:22:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3985.566692
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 09:22:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3988.692617
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 09:22:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3990.65022
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 09:22:24.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3991.162196
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 09:22:25.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3992.692482
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 09:22:25.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3997.506601
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2699 2014-07-23 09:22:25.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3999.467478
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2699 2014-07-23 09:22:25.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4001.122983
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:22:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4386.103901
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:22:56.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4389.898871
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:22:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4390.632899
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:22:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4393.470355
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:22:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4396.156602
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:22:57.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4398.335494
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:22:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4399.783461
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:22:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4402.386347
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:22:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4404.323159
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:22:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4405.955599
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:22:58.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4406.891161
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:22:59.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4411.478689
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:22:59.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4413.968975
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:22:59.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4415.419854
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:24:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4426.141710
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:24:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4429.937892
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:24:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4430.821441
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:24:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4433.89739
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:24:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4436.770096
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:24:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4438.411035
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:24:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4439.293733
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:24:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4442.287569
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:24:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4444.159726
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:24:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4445.710963
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:24:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4446.450598
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:24:51.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4451.294775
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:24:51.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4453.638786
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:24:51.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4455.38743
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:26:12.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4467.379476
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:26:12.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4470.341302
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:26:12.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4471.812343
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:26:12.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4474.991156
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:26:12.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4477.375084
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:26:13.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4479.626998
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:26:13.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4480.740785
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:26:13.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4483.230982
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:26:13.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4485.229894
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:26:13.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4486.698391
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:26:14.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4487.369377
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:26:14.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4492.927826
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:26:14.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4494.717195
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:26:14.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4496.17482
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:26:39.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4504.364378
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:26:40.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4507.352679
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:26:40.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4508.176855
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:26:40.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4511.298714
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:26:40.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4514.641365
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:26:40.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4516.977717
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:26:41.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4517.350469
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:26:41.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4520.675089
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:26:41.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4522.387199
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:26:41.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4523.690505
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:26:41.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4524.889767
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:26:42.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4529.248185
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4271 2014-07-23 10:26:42.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4531.237339
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4261 2014-07-23 10:26:42.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4533.707872
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:34:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4743.717641
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:34:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4746.324090
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:34:48.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4747.508813
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:34:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4750.992548
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:34:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4753.754804
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:34:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4755.405723
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:34:49.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4756.396775
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:34:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4759.88261
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:34:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4761.575275
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:34:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4762.161881
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:34:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4763.893870
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:34:50.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4768.149540
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4271 2014-07-23 10:34:51.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4770.671103
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4261 2014-07-23 10:34:51.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4772.827193
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3065 2014-07-23 12:08:20.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5664.515422
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-23 12:08:20.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5667.105989
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3083 2014-07-23 12:08:20.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5668.35343
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3089 2014-07-23 12:08:20.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5671.860490
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3057 2014-07-23 12:08:21.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5674.189043
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-23 12:08:21.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5676.535254
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-23 12:08:21.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5677.102839
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-23 12:08:21.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5680.286131
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-23 12:08:21.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5682.664259
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-23 12:08:22.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5683.977639
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3009 2014-07-23 12:08:22.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5684.172089
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3003 2014-07-23 12:08:22.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5689.710149
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4384 2014-07-23 12:08:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5691.525107
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4374 2014-07-23 12:08:23.000000 json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5693.536998
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:22:02.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10951.421015
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:22:02.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10954.428544
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:22:02.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10955.515651
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:22:02.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10958.374497
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:22:02.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10961.951865
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:22:03.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10963.11090
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:22:03.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10964.235322
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:22:03.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10967.915676
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:22:03.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10969.453178
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:22:04.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10970.375256
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:22:04.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10971.286286
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:22:04.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10976.971196
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4542 2014-07-24 00:22:04.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10978.682256
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4524 2014-07-24 00:22:05.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10980.206840
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:22:50.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10991.289358
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:22:50.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10994.686238
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:22:51.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10995.496508
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:22:51.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10998.373400
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:22:51.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11001.427568
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:22:51.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11003.479443
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:22:51.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11004.275617
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:22:52.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11007.407176
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:22:52.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11009.692787
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:22:52.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11010.861199
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:22:52.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11011.548903
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:22:53.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11016.713601
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4542 2014-07-24 00:22:53.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11018.425276
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4524 2014-07-24 00:22:53.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11020.717207
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:23:08.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11027.481779
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:23:09.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11030.193078
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:23:09.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11031.558282
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:23:09.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11034.934266
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:23:09.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11037.482667
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:23:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11039.92172
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:23:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11040.580421
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:23:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11043.250772
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:23:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11045.419672
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:23:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11046.638359
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:23:11.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11047.919858
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:23:11.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11052.713388
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4542 2014-07-24 00:23:11.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11054.765457
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4524 2014-07-24 00:23:12.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11056.624922
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:23:55.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11079.32142
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:23:55.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11082.563451
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:23:55.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11083.791770
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:23:55.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11086.862515
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:23:55.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11089.653131
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:23:56.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11091.118511
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:23:56.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11092.423477
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:23:56.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11095.250029
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:23:56.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11097.571002
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:23:57.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11098.347740
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:23:57.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11099.987225
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:23:57.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11104.426307
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4539 2014-07-24 00:23:57.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11106.955388
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4521 2014-07-24 00:23:58.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11108.581593
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:27:09.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11214.938510
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:27:09.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11217.646151
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:27:09.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11218.439338
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:27:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11221.32430
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:27:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11224.576114
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:27:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11226.149202
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:27:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11227.460050
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:27:10.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11230.552639
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:27:11.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11232.351813
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:27:11.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11233.166456
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:27:11.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11234.465792
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:27:11.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11239.469005
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4539 2014-07-24 00:27:12.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11241.207429
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4521 2014-07-24 00:27:12.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11243.420688
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:27:32.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11254.37161
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:27:32.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11257.983127
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:27:32.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11258.865944
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:27:32.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11261.611179
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:27:32.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11264.878658
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:27:33.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11266.494999
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:27:33.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11267.165792
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:27:33.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11270.547077
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:27:33.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11272.5829
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:27:33.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11273.209790
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:27:34.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11274.892427
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:27:34.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11279.813165
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4539 2014-07-24 00:27:34.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11281.103429
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4521 2014-07-24 00:27:34.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11283.214539
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:31:45.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11335.350941
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:31:45.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11338.635226
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:31:45.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11339.166257
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:31:46.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11342.330369
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:31:46.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11345.410963
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:31:46.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11347.612141
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:31:46.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11348.579233
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:31:47.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11351.410803
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:31:47.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11353.363743
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:31:47.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11354.83605
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:31:47.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11355.869925
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:31:47.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11360.730957
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4539 2014-07-24 00:31:48.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11362.913135
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4521 2014-07-24 00:31:48.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11364.590973
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:49:40.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11441.798921
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:49:41.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11444.13221
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:49:41.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11445.542803
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:49:41.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11448.769610
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:49:41.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11451.89753
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:49:41.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11453.504155
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:49:42.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11454.962200
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:49:42.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11457.969910
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:49:42.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11459.197891
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:49:42.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11460.131903
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:49:43.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11461.163111
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:49:43.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11466.694589
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4166 2014-07-24 00:49:43.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11468.116318
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4166 2014-07-24 00:49:43.000000 json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11470.200781
--rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)      651 2014-07-23 13:23:03.000000 json-spec-0.9.8/tests/__init__.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      177 2014-06-13 07:51:45.000000 json-spec-0.9.8/tests/conftest.py
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/fixtures/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      129 2014-06-03 18:13:12.000000 json-spec-0.9.8/tests/fixtures/first.data1.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      276 2014-06-03 18:13:34.000000 json-spec-0.9.8/tests/fixtures/first.data2.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      720 2014-06-03 18:07:17.000000 json-spec-0.9.8/tests/fixtures/first.schema.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1354 2014-06-11 09:17:02.000000 json-spec-0.9.8/tests/fixtures/five.schema.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      402 2014-06-03 18:18:54.000000 json-spec-0.9.8/tests/fixtures/four.base.schema.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      660 2014-06-03 18:17:56.000000 json-spec-0.9.8/tests/fixtures/four.data.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3583 2014-06-11 16:43:11.000000 json-spec-0.9.8/tests/fixtures/four.entry.schema.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      272 2014-06-03 18:15:19.000000 json-spec-0.9.8/tests/fixtures/second.data1.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      788 2014-06-03 18:14:36.000000 json-spec-0.9.8/tests/fixtures/second.schema.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      145 2014-06-03 18:16:50.000000 json-spec-0.9.8/tests/fixtures/three.data1.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      173 2014-06-03 18:17:15.000000 json-spec-0.9.8/tests/fixtures/three.data2.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1270 2014-06-03 18:16:09.000000 json-spec-0.9.8/tests/fixtures/three.schema.json
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       39 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/.git
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)        5 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/.gitignore
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       98 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/.travis.yml
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/bin/
--rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)     9059 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/bin/jsonschema_suite
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1057 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/LICENSE
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3612 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/README.md
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/remotes/
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/remotes/folder/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       25 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/remotes/folder/folderInteger.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)       25 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/remotes/integer.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      110 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/remotes/subSchemas.json
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/tests/
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/tests/draft3/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2257 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/additionalItems.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2194 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/additionalProperties.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2989 2014-07-17 16:15:08.000000 json-spec-0.9.8/tests/suite/tests/draft3/dependencies.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1936 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/disallow.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1544 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/divisibleBy.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1964 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/enum.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2591 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/extends.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1136 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/items.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1063 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/maximum.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      706 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/maxItems.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      895 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/maxLength.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1063 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/minimum.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      693 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/minItems.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      886 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/minLength.json
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/tests/draft3/optional/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1663 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/optional/bignum.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     6577 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/optional/format.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      463 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/optional/jsregex.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      384 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/optional/zeroTerminatedFloats.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      582 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/pattern.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/patternProperties.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2881 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/properties.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3922 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/ref.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1961 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/refRemote.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1282 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/required.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)    13225 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/type.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2613 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft3/uniqueItems.json
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/tests/draft4/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2282 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/additionalItems.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2194 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/additionalProperties.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3025 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/allOf.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1608 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/anyOf.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      854 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/definitions.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3139 2014-07-16 10:16:27.000000 json-spec-0.9.8/tests/suite/tests/draft4/dependencies.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1975 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/enum.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1136 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/items.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1063 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/maximum.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      706 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/maxItems.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      896 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/maxLength.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      759 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/maxProperties.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1063 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/minimum.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      693 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/minItems.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      886 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/minLength.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      725 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/minProperties.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1525 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/multipleOf.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2266 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/not.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1607 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/oneOf.json
-drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-07-24 12:58:38.000000 json-spec-0.9.8/tests/suite/tests/draft4/optional/
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1663 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/optional/bignum.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4434 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/optional/format.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      384 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/optional/zeroTerminatedFloats.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      582 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/pattern.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/patternProperties.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2881 2014-07-16 09:33:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/properties.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3903 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/ref.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1961 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/refRemote.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      923 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/required.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     9306 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/type.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2613 2014-07-16 07:17:37.000000 json-spec-0.9.8/tests/suite/tests/draft4/uniqueItems.json
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1921 2014-07-23 17:05:35.000000 json-spec-0.9.8/tests/test_cli.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2075 2014-07-23 08:45:50.000000 json-spec-0.9.8/tests/test_draft03.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1969 2014-07-18 07:28:07.000000 json-spec-0.9.8/tests/test_draft04.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      949 2014-06-11 16:43:11.000000 json-spec-0.9.8/tests/test_errors.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2688 2014-07-24 12:47:00.000000 json-spec-0.9.8/tests/test_errors2.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5047 2014-07-23 08:34:25.000000 json-spec-0.9.8/tests/test_operations.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5220 2014-07-16 07:02:29.000000 json-spec-0.9.8/tests/test_pointer.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      977 2014-07-16 10:52:54.000000 json-spec-0.9.8/tests/test_provider.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1726 2014-06-11 16:43:12.000000 json-spec-0.9.8/tests/test_reference.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1814 2014-06-12 06:54:29.000000 json-spec-0.9.8/tests/test_util.py
--rw-r--r--   0 xavierbarbosa   (501) staff       (20)      454 2014-07-17 10:00:02.000000 json-spec-0.9.8/tox.ini
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       79 2014-06-08 13:14:34.000000 json-spec-0.9.9/.coveragerc
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      111 2014-07-17 03:32:17.000000 json-spec-0.9.9/.gitmodules
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      179 2014-07-17 09:49:47.000000 json-spec-0.9.9/.travis.yml
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      126 2014-08-13 14:01:50.000000 json-spec-0.9.9/AUTHORS
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2232 2014-08-13 14:01:50.000000 json-spec-0.9.9/ChangeLog
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3165 2014-06-10 14:39:26.000000 json-spec-0.9.9/CONTRIBUTING.rst
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/docs/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      171 2014-06-04 11:18:59.000000 json-spec-0.9.9/docs/authors.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4892 2014-08-13 13:55:23.000000 json-spec-0.9.9/docs/cli.rst
+-rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)     8663 2014-07-28 21:44:49.000000 json-spec-0.9.9/docs/conf.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       32 2014-06-02 06:54:20.000000 json-spec-0.9.9/docs/contributing.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       51 2014-06-10 12:14:08.000000 json-spec-0.9.9/docs/history.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2326 2014-08-13 13:55:23.000000 json-spec-0.9.9/docs/index.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      362 2014-06-10 14:03:00.000000 json-spec-0.9.9/docs/installation.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     6466 2014-06-02 06:54:20.000000 json-spec-0.9.9/docs/make.bat
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     6777 2014-06-02 06:54:20.000000 json-spec-0.9.9/docs/Makefile
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3866 2014-06-10 12:07:29.000000 json-spec-0.9.9/docs/operations.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3165 2014-07-18 09:56:13.000000 json-spec-0.9.9/docs/pointer.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2546 2014-06-10 12:02:55.000000 json-spec-0.9.9/docs/reference.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       35 2014-07-23 13:29:04.000000 json-spec-0.9.9/docs/requirements.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4207 2014-08-13 13:55:23.000000 json-spec-0.9.9/docs/validators.rst
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/examples/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      325 2014-06-02 06:59:41.000000 json-spec-0.9.9/examples/basic.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1311 2014-06-02 15:32:59.000000 json-spec-0.9.9/examples/simple.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      793 2014-07-16 16:38:08.000000 json-spec-0.9.9/examples/test.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       99 2014-06-02 06:54:20.000000 json-spec-0.9.9/HISTORY.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1476 2014-06-04 11:18:59.000000 json-spec-0.9.9/LICENSE
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      288 2014-06-09 12:06:15.000000 json-spec-0.9.9/MANIFEST.in
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5417 2014-08-13 14:01:55.000000 json-spec-0.9.9/PKG-INFO
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)        0 2014-06-10 11:52:21.000000 json-spec-0.9.9/pytest.ini
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3408 2014-08-13 14:00:28.000000 json-spec-0.9.9/README.rst
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       29 2014-07-28 21:33:29.000000 json-spec-0.9.9/requirements-py27.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       29 2014-07-28 21:33:29.000000 json-spec-0.9.9/requirements-py32.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       29 2014-07-28 21:33:29.000000 json-spec-0.9.9/requirements-pypy.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)        4 2014-07-28 21:15:19.000000 json-spec-0.9.9/requirements.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2459 2014-08-13 14:01:55.000000 json-spec-0.9.9/setup.cfg
+-rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)      281 2014-07-23 13:23:03.000000 json-spec-0.9.9/setup.py
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/json_spec.egg-info/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)        1 2014-08-13 14:01:50.000000 json-spec-0.9.9/src/json_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1119 2014-08-13 14:01:50.000000 json-spec-0.9.9/src/json_spec.egg-info/entry_points.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)        1 2014-06-09 09:45:21.000000 json-spec-0.9.9/src/json_spec.egg-info/not-zip-safe
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5417 2014-08-13 14:01:50.000000 json-spec-0.9.9/src/json_spec.egg-info/PKG-INFO
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4132 2014-06-10 14:39:26.000000 json-spec-0.9.9/src/json_spec.egg-info/PKG-INFO 2
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      103 2014-08-13 14:01:50.000000 json-spec-0.9.9/src/json_spec.egg-info/requires.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)   153032 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/json_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)        9 2014-08-13 14:01:50.000000 json-spec-0.9.9/src/json_spec.egg-info/top_level.txt
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/
+-rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)       35 2014-06-09 09:37:06.000000 json-spec-0.9.9/src/jsonspec/__init__.py
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/cli/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)    15550 2014-08-13 13:55:23.000000 json-spec-0.9.9/src/jsonspec/cli/__init__.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      677 2014-07-17 11:19:49.000000 json-spec-0.9.9/src/jsonspec/driver.py
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/misc/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)        0 2014-06-09 10:06:11.000000 json-spec-0.9.9/src/jsonspec/misc/__init__.py
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      638 2014-06-08 15:04:49.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/address.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1102 2014-06-08 14:45:08.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/calendar.json
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1791 2014-06-08 15:04:58.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/card.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      897 2014-06-08 14:50:47.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/hyper-schema.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      394 2014-06-08 14:57:43.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/json-ref.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      394 2014-06-08 14:56:15.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/links.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2476 2014-06-08 14:53:02.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/schema.json
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-04/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4816 2014-06-08 14:44:30.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-04/hyper-schema.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4375 2014-06-08 14:43:08.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/draft-04/schema.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      184 2014-06-08 14:44:58.000000 json-spec-0.9.9/src/jsonspec/misc/schemas/geo.json
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/operations/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2424 2014-08-13 13:55:09.000000 json-spec-0.9.9/src/jsonspec/operations/__init__.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     6429 2014-08-13 13:55:09.000000 json-spec-0.9.9/src/jsonspec/operations/bases.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      298 2014-08-13 13:55:09.000000 json-spec-0.9.9/src/jsonspec/operations/exceptions.py
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/pointer/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1042 2014-07-23 13:23:03.000000 json-spec-0.9.9/src/jsonspec/pointer/__init__.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     7571 2014-08-04 21:11:51.000000 json-spec-0.9.9/src/jsonspec/pointer/bases.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1591 2014-07-23 13:23:03.000000 json-spec-0.9.9/src/jsonspec/pointer/exceptions.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1859 2014-07-16 07:02:29.000000 json-spec-0.9.9/src/jsonspec/pointer/stages.py
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/reference/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1660 2014-06-10 12:35:57.000000 json-spec-0.9.9/src/jsonspec/reference/__init__.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3015 2014-07-17 03:32:17.000000 json-spec-0.9.9/src/jsonspec/reference/bases.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      256 2014-06-09 10:05:56.000000 json-spec-0.9.9/src/jsonspec/reference/exceptions.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4663 2014-08-06 07:06:40.000000 json-spec-0.9.9/src/jsonspec/reference/providers.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      910 2014-06-09 10:05:49.000000 json-spec-0.9.9/src/jsonspec/reference/util.py
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/src/jsonspec/validators/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1254 2014-07-28 21:34:10.000000 json-spec-0.9.9/src/jsonspec/validators/__init__.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2485 2014-07-28 21:34:10.000000 json-spec-0.9.9/src/jsonspec/validators/bases.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)    26473 2014-07-28 21:34:10.000000 json-spec-0.9.9/src/jsonspec/validators/draft03.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)    25895 2014-08-13 13:55:23.000000 json-spec-0.9.9/src/jsonspec/validators/draft04.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1935 2014-07-28 21:34:10.000000 json-spec-0.9.9/src/jsonspec/validators/exceptions.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3884 2014-07-17 15:59:07.000000 json-spec-0.9.9/src/jsonspec/validators/factorize.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3889 2014-07-28 21:34:10.000000 json-spec-0.9.9/src/jsonspec/validators/formats.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      388 2014-07-28 21:34:10.000000 json-spec-0.9.9/src/jsonspec/validators/pointer_util.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     7668 2014-07-28 21:34:10.000000 json-spec-0.9.9/src/jsonspec/validators/util.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)        6 2014-06-10 13:58:06.000000 json-spec-0.9.9/test-requirements.txt
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3178 2014-07-24 09:07:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13747.767380
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3184 2014-07-24 09:07:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13750.659383
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3196 2014-07-24 09:07:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13751.870161
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3202 2014-07-24 09:07:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13754.725564
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-07-24 09:07:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13757.87138
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3172 2014-07-24 09:07:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13759.913660
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3172 2014-07-24 09:07:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13760.814424
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3180 2014-07-24 09:07:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13763.284703
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3182 2014-07-24 09:07:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13765.696865
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3182 2014-07-24 09:07:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13766.217187
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3122 2014-07-24 09:07:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13767.563441
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3116 2014-07-24 09:07:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13772.315171
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4574 2014-07-24 09:07:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13774.53270
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4532 2014-07-24 09:07:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13776.480507
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3178 2014-07-24 09:13:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13848.148603
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3184 2014-07-24 09:13:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13851.883200
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3196 2014-07-24 09:13:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13852.658197
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3202 2014-07-24 09:13:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13855.981187
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-07-24 09:13:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13858.162103
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3172 2014-07-24 09:13:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13860.756322
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3172 2014-07-24 09:13:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13861.558717
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3180 2014-07-24 09:13:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13864.839483
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3182 2014-07-24 09:13:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13866.711117
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3182 2014-07-24 09:13:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13867.481307
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3122 2014-07-24 09:13:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13868.292406
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3116 2014-07-24 09:13:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13873.16479
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4572 2014-07-24 09:13:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13875.755524
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4532 2014-07-24 09:13:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13877.538157
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:35:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16342.147102
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:35:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16347.755810
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:35:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16350.705549
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:35:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16355.704674
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:35:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16360.153967
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:35:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16364.702492
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:35:59.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16367.887786
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:35:59.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16372.346985
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:36:00.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16376.681847
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:36:00.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16379.515453
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-13 12:36:00.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16382.567432
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-13 12:36:01.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16389.164255
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:36:01.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16393.979325
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:36:01.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16397.653708
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:37:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16419.152209
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16424.693528
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:37:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16427.907972
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16432.942195
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16437.201526
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16441.364426
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16444.138120
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16449.255351
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16453.230289
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16456.384401
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-13 12:37:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16459.585097
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-13 12:37:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16466.696883
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16470.315990
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:37:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16474.422276
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:38:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16488.825309
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16493.278265
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:38:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16496.584920
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16501.211211
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16506.411088
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16510.976513
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16513.457611
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16518.244099
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16522.532611
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16525.958325
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-13 12:38:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16528.460443
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-13 12:38:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16535.461421
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16539.550730
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:21.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16543.942621
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:38:40.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16554.946403
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:40.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16559.641521
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:38:41.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16562.252884
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:41.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16567.720760
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:41.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16572.548668
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16576.385557
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16579.54659
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16584.775958
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16588.205667
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16591.687369
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-13 12:38:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16594.247842
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-13 12:38:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16601.112614
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16605.128784
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:38:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16609.295376
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:39:02.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16624.341194
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16629.531467
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:39:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16634.579906
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16639.901383
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16644.31571
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16648.111213
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16651.298002
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16656.259216
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16660.374826
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16663.719250
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-13 12:39:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16666.564762
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-13 12:39:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16673.170290
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:07.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16677.287819
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:39:07.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16681.742251
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:40:35.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16704.120277
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:35.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16709.16048
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-13 12:40:36.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16712.340029
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:36.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16717.1029
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:36.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16722.714226
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:37.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16726.233081
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:37.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16729.345855
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:37.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16734.972963
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:38.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16738.578714
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:38.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16741.941897
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-13 12:40:39.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16744.793537
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-13 12:40:39.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16751.943051
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:39.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16755.689468
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-13 12:40:40.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16759.959887
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-13 12:41:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16804.705554
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16809.975895
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-13 12:41:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16812.459276
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16817.372220
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16822.195639
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16826.196123
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16829.643526
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16834.761615
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16838.388910
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16841.511018
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3382 2014-08-13 12:41:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16844.492538
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-13 12:41:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16851.316690
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16855.571300
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:41:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16859.692725
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-13 12:44:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16910.15315
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:44:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16915.833968
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-13 12:44:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16918.311714
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:44:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16923.120845
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:44:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16928.477651
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:44:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16932.428228
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:44:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16935.469966
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:44:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16940.210845
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:44:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16944.76695
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:44:19.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16947.688527
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3382 2014-08-13 12:44:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16950.916457
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-13 12:44:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16957.96220
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3419 2014-08-13 12:44:21.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16961.446842
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3419 2014-08-13 12:44:21.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16965.44174
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-13 12:46:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16993.977798
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:46:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.16998.453765
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-13 12:46:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17001.992738
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:46:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17006.433027
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:46:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17011.92856
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:46:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17015.767454
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:46:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17018.865485
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:46:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17023.547155
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:46:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17027.590767
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 12:46:07.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17030.574762
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3382 2014-08-13 12:46:07.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17033.460256
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-13 12:46:07.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17040.67895
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3419 2014-08-13 12:46:08.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17044.913172
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3419 2014-08-13 12:46:08.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17048.930833
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-13 12:46:59.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17087.488856
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:46:59.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17092.747616
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-13 12:47:00.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17097.72962
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:47:00.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17102.786151
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:47:01.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17107.30772
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:47:01.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17111.731146
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:47:01.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17114.539669
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:47:02.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17119.776889
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:47:02.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17123.810809
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:47:02.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17126.185214
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3385 2014-08-13 12:47:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17129.396958
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:47:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17136.37569
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3422 2014-08-13 12:47:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17140.25416
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3422 2014-08-13 12:47:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17144.340898
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-13 12:48:02.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17153.273125
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:48:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17158.371022
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-13 12:48:03.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17161.136502
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:48:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17166.674756
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:48:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17171.704177
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:48:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17175.22596
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:48:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17178.903312
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:48:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17183.623916
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:48:05.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17187.730707
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-13 12:48:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17190.291420
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3385 2014-08-13 12:48:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17193.799206
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3389 2014-08-13 12:48:06.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17200.464418
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3422 2014-08-13 12:48:07.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17204.435078
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3422 2014-08-13 12:48:07.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17208.364618
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3697 2014-08-13 13:01:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17468.487862
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 13:01:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17473.191129
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3714 2014-08-13 13:01:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17476.174784
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 13:01:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17481.926486
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 13:01:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17486.24513
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 13:01:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17490.805327
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3687 2014-08-13 13:01:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17493.206647
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 13:01:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17498.491363
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 13:01:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17502.422575
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3696 2014-08-13 13:01:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17505.373449
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3396 2014-08-13 13:01:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17508.945265
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-13 13:01:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17515.628875
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3416 2014-08-13 13:01:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17519.460132
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3416 2014-08-13 13:01:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17523.156591
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3700 2014-08-13 13:02:32.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17537.40360
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3704 2014-08-13 13:02:33.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17542.554801
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3717 2014-08-13 13:02:33.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17545.1533
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3721 2014-08-13 13:02:33.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17550.119478
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3690 2014-08-13 13:02:34.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17555.992431
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3692 2014-08-13 13:02:34.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17559.285002
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3690 2014-08-13 13:02:34.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17562.761903
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3699 2014-08-13 13:02:35.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17567.633812
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3701 2014-08-13 13:02:35.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17571.809780
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3699 2014-08-13 13:02:36.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17574.789940
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-13 13:02:36.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17577.746647
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3430 2014-08-13 13:02:36.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17584.685704
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5165 2014-08-13 13:02:37.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17588.870959
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5110 2014-08-13 13:02:37.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17592.349893
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3700 2014-08-13 13:02:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17599.607988
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3704 2014-08-13 13:02:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17604.102275
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3717 2014-08-13 13:02:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17607.411412
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3721 2014-08-13 13:02:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17612.527405
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3690 2014-08-13 13:02:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17617.188956
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3692 2014-08-13 13:02:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17621.35604
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3690 2014-08-13 13:02:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17624.67785
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3699 2014-08-13 13:02:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17629.621426
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3701 2014-08-13 13:02:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17633.721488
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3699 2014-08-13 13:02:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17636.662068
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-13 13:02:46.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17639.466967
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3430 2014-08-13 13:02:46.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17646.715311
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5165 2014-08-13 13:02:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17650.499381
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5110 2014-08-13 13:02:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17654.75815
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3700 2014-08-13 13:03:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17741.76097
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3704 2014-08-13 13:03:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17746.119811
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3717 2014-08-13 13:03:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17749.346292
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3721 2014-08-13 13:03:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17754.370928
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3690 2014-08-13 13:03:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17759.727479
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3692 2014-08-13 13:03:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17763.295330
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3690 2014-08-13 13:03:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17766.185441
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3699 2014-08-13 13:03:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17771.405993
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3701 2014-08-13 13:03:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17775.514960
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3699 2014-08-13 13:03:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17778.656993
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-13 13:03:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17781.51293
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3430 2014-08-13 13:03:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17788.885827
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5165 2014-08-13 13:03:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17792.468352
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5110 2014-08-13 13:03:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17796.529184
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:29.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17810.15144
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:29.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17813.831388
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:29.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17814.269414
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:29.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17817.901538
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:29.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17820.740896
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:30.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17822.600391
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:30.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17823.279010
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:30.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17826.436818
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:30.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17828.681763
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:30.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17829.522658
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:31.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17830.130825
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:31.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17835.411851
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:31.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17837.23281
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:31.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17839.398704
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17853.428228
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17856.615953
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17857.606072
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17860.941927
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17863.499864
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17865.91705
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17866.354745
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17869.804107
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17871.483132
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17872.513643
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17873.169010
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17878.702248
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17880.692442
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2975 2014-08-13 13:04:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17882.555987
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17900.50934
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17905.231657
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17908.91352
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17913.839138
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17918.205346
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17922.748316
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17925.602254
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17930.50311
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17934.137044
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17937.166588
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17940.685436
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17947.333673
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17951.204734
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:05:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17955.981670
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:06:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17963.498994
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:06:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17968.394551
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:06:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17971.747548
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:06:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17976.148478
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:06:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17981.94968
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3232 2014-08-13 13:06:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.17985.61732
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3698 2014-08-13 13:06:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18001.217402
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3702 2014-08-13 13:06:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18006.237508
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3715 2014-08-13 13:06:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18009.84480
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3719 2014-08-13 13:06:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18014.636007
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3688 2014-08-13 13:06:25.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18019.566603
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3690 2014-08-13 13:06:25.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18023.809496
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3688 2014-08-13 13:06:25.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18026.613156
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3697 2014-08-13 13:06:26.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18031.898925
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3699 2014-08-13 13:06:26.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18035.387591
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3697 2014-08-13 13:06:27.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18038.856626
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3397 2014-08-13 13:06:27.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18041.631419
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3428 2014-08-13 13:06:27.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18048.32637
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5163 2014-08-13 13:06:28.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18052.503888
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5108 2014-08-13 13:06:28.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18056.250918
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3698 2014-08-13 13:07:30.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18074.708734
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3702 2014-08-13 13:07:30.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18079.762678
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3715 2014-08-13 13:07:30.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18082.205308
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3719 2014-08-13 13:07:31.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18087.25409
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3688 2014-08-13 13:07:31.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18092.545251
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3690 2014-08-13 13:07:31.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18096.668442
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3688 2014-08-13 13:07:32.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18099.298146
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3697 2014-08-13 13:07:32.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18104.451211
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3699 2014-08-13 13:07:33.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18108.953008
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3697 2014-08-13 13:07:33.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18111.666565
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3397 2014-08-13 13:07:33.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18114.638821
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3428 2014-08-13 13:07:34.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18121.412452
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5163 2014-08-13 13:07:34.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18125.551702
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5108 2014-08-13 13:07:34.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.18129.593028
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:54:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2890.971498
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:54:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2893.380811
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:54:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2894.793495
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:55:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2928.597283
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:55:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2931.192801
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:55:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2932.217942
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:55:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2936.233109
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:55:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2940.212753
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:56:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2955.883132
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:56:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2958.989772
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:56:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2959.860425
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:56:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2963.816177
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:56:04.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2965.224896
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:56:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2982.986653
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:56:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2985.374311
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:56:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2986.865546
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:56:52.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2990.591765
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:56:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2992.165742
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:56:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2995.662249
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:56:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2998.744678
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:57:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3037.34254
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:57:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3040.245703
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 08:57:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3041.402808
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 08:57:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3044.851117
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:57:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3045.205944
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:57:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3049.367076
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:57:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3051.497611
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:57:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3054.349643
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:57:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3057.398766
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:58:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3085.965903
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:58:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3088.825419
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 08:58:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3089.232615
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 08:58:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3092.436248
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:58:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3095.904202
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:58:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3097.390316
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:58:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3100.97279
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:58:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3103.875510
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:58:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3105.771180
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:58:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3106.253758
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:58:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3107.994561
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3120.464422
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:59:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3125.43493
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 08:59:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3126.120944
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 08:59:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3129.405140
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:59:16.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3132.21149
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:59:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3134.760557
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:59:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3135.702900
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:59:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3138.345249
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3140.618324
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:17.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3141.304302
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:59:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3142.803594
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 08:59:18.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3147.599067
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3158.411930
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 08:59:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3161.934483
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 08:59:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3162.638446
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 08:59:53.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3165.30416
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 08:59:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3170.833718
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:59:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3172.319935
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 08:59:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3173.761134
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 08:59:54.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3176.720397
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3178.85727
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 08:59:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3179.868910
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 08:59:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3180.240143
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 08:59:55.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3185.704742
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:09.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3196.399093
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:00:09.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3199.588691
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:00:10.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3200.680544
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:00:10.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3203.440856
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:00:10.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3206.290324
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:10.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3208.564692
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:10.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3209.81838
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:00:11.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3212.832848
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:11.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3214.644239
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:11.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3215.524698
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:00:11.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3216.42847
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:00:12.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3221.533410
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3234.388312
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:00:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3239.775417
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:00:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3240.557245
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:00:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3243.788730
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:00:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3246.569653
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3248.843454
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3249.165956
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:00:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3252.306359
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3254.372835
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3255.163085
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:00:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3256.990053
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:00:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3261.351666
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3270.227618
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:00:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3273.65115
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:00:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3274.237674
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:00:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3277.19176
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:00:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3280.898598
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3282.817350
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:00:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3283.45632
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:00:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3286.420993
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3288.53949
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:00:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3289.352556
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:00:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3290.992008
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:00:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3295.184522
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:03:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3371.384759
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:03:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3374.818857
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:03:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3375.499649
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:03:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3378.68842
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:03:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3381.949045
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:03:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3383.803880
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:03:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3384.450316
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:03:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3387.830297
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:03:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3389.699913
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:03:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3390.518846
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:03:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3391.881649
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:03:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3396.541112
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:04:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3441.966418
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:04:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3444.746082
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:04:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3445.389212
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:04:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3448.669825
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:04:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3451.277331
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:04:45.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3453.289143
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:04:46.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3454.270660
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:04:46.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3457.246427
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:04:46.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3459.861391
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:04:46.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3460.34642
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:04:46.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3461.488045
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:04:47.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3466.73300
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:22.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3486.358902
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:05:22.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3489.33416
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:05:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3490.359594
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:05:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3493.956052
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:05:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3496.412731
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:05:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3498.678016
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:05:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3499.653310
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:05:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3502.596799
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3504.746277
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3506.628550
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:05:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3507.403336
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:05:25.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3512.572538
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3529.610576
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2950 2014-07-23 09:05:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3532.775761
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:05:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3533.315530
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2964 2014-07-23 09:05:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3536.588954
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2936 2014-07-23 09:05:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3539.967848
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:05:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3541.22712
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2938 2014-07-23 09:05:43.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3542.763221
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2942 2014-07-23 09:05:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3545.825074
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3547.736530
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:05:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3548.135588
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2884 2014-07-23 09:05:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3549.508720
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2878 2014-07-23 09:05:44.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3554.240623
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 09:22:22.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3972.942596
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 09:22:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3975.159309
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 09:22:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3976.791534
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 09:22:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3979.772513
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 09:22:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3982.279342
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 09:22:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3984.468176
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 09:22:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3985.566692
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 09:22:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3988.692617
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 09:22:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3990.65022
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 09:22:24.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3991.162196
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 09:22:25.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3992.692482
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 09:22:25.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3997.506601
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2699 2014-07-23 09:22:25.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3999.467478
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2699 2014-07-23 09:22:25.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4001.122983
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:22:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4386.103901
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:22:56.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4389.898871
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:22:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4390.632899
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:22:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4393.470355
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:22:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4396.156602
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:22:57.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4398.335494
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:22:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4399.783461
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:22:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4402.386347
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:22:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4404.323159
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:22:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4405.955599
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:22:58.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4406.891161
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:22:59.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4411.478689
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:22:59.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4413.968975
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:22:59.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4415.419854
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:24:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4426.141710
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:24:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4429.937892
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:24:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4430.821441
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:24:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4433.89739
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:24:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4436.770096
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:24:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4438.411035
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:24:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4439.293733
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:24:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4442.287569
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:24:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4444.159726
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:24:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4445.710963
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:24:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4446.450598
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:24:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4451.294775
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:24:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4453.638786
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:24:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4455.38743
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:26:12.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4467.379476
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:26:12.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4470.341302
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:26:12.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4471.812343
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:26:12.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4474.991156
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:26:12.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4477.375084
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:26:13.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4479.626998
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:26:13.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4480.740785
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:26:13.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4483.230982
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:26:13.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4485.229894
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:26:13.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4486.698391
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:26:14.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4487.369377
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:26:14.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4492.927826
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:26:14.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4494.717195
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3629 2014-07-23 10:26:14.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4496.17482
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:26:39.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4504.364378
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:26:40.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4507.352679
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:26:40.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4508.176855
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:26:40.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4511.298714
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:26:40.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4514.641365
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:26:40.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4516.977717
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:26:41.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4517.350469
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:26:41.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4520.675089
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:26:41.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4522.387199
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:26:41.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4523.690505
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:26:41.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4524.889767
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:26:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4529.248185
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4271 2014-07-23 10:26:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4531.237339
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4261 2014-07-23 10:26:42.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4533.707872
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2952 2014-07-23 10:34:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4743.717641
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2958 2014-07-23 10:34:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4746.324090
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2970 2014-07-23 10:34:48.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4747.508813
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2976 2014-07-23 10:34:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4750.992548
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2944 2014-07-23 10:34:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4753.754804
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:34:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4755.405723
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2946 2014-07-23 10:34:49.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4756.396775
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2954 2014-07-23 10:34:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4759.88261
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:34:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4761.575275
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2956 2014-07-23 10:34:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4762.161881
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2896 2014-07-23 10:34:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4763.893870
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2890 2014-07-23 10:34:50.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4768.149540
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4271 2014-07-23 10:34:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4770.671103
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4261 2014-07-23 10:34:51.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4772.827193
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3065 2014-07-23 12:08:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5664.515422
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-23 12:08:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5667.105989
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3083 2014-07-23 12:08:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5668.35343
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3089 2014-07-23 12:08:20.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5671.860490
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3057 2014-07-23 12:08:21.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5674.189043
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-23 12:08:21.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5676.535254
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-23 12:08:21.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5677.102839
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-23 12:08:21.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5680.286131
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-23 12:08:21.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5682.664259
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-23 12:08:22.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5683.977639
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3009 2014-07-23 12:08:22.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5684.172089
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3003 2014-07-23 12:08:22.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5689.710149
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4384 2014-07-23 12:08:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5691.525107
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4374 2014-07-23 12:08:23.000000 json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5693.536998
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:22:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10951.421015
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:22:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10954.428544
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:22:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10955.515651
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:22:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10958.374497
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:22:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10961.951865
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:22:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10963.11090
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:22:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10964.235322
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:22:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10967.915676
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:22:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10969.453178
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:22:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10970.375256
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:22:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10971.286286
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:22:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10976.971196
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4542 2014-07-24 00:22:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10978.682256
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4524 2014-07-24 00:22:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10980.206840
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:22:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10991.289358
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:22:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10994.686238
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:22:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10995.496508
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:22:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10998.373400
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:22:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11001.427568
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:22:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11003.479443
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:22:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11004.275617
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:22:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11007.407176
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:22:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11009.692787
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:22:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11010.861199
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:22:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11011.548903
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:22:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11016.713601
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4542 2014-07-24 00:22:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11018.425276
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4524 2014-07-24 00:22:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11020.717207
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:23:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11027.481779
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:23:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11030.193078
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:23:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11031.558282
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:23:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11034.934266
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:23:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11037.482667
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:23:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11039.92172
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:23:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11040.580421
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:23:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11043.250772
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:23:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11045.419672
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:23:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11046.638359
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:23:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11047.919858
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:23:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11052.713388
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4542 2014-07-24 00:23:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11054.765457
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4524 2014-07-24 00:23:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11056.624922
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:23:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11079.32142
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:23:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11082.563451
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:23:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11083.791770
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:23:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11086.862515
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:23:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11089.653131
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:23:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11091.118511
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:23:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11092.423477
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:23:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11095.250029
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:23:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11097.571002
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:23:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11098.347740
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:23:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11099.987225
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:23:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11104.426307
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4539 2014-07-24 00:23:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11106.955388
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4521 2014-07-24 00:23:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11108.581593
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:27:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11214.938510
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:27:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11217.646151
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:27:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11218.439338
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11221.32430
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11224.576114
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11226.149202
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11227.460050
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11230.552639
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:27:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11232.351813
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:27:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11233.166456
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:27:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11234.465792
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:27:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11239.469005
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4539 2014-07-24 00:27:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11241.207429
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4521 2014-07-24 00:27:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11243.420688
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:27:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11254.37161
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:27:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11257.983127
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:27:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11258.865944
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:27:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11261.611179
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:27:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11264.878658
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:27:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11266.494999
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:27:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11267.165792
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:27:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11270.547077
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:27:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11272.5829
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:27:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11273.209790
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:27:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11274.892427
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:27:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11279.813165
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4539 2014-07-24 00:27:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11281.103429
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4521 2014-07-24 00:27:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11283.214539
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:31:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11335.350941
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:31:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11338.635226
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:31:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11339.166257
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:31:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11342.330369
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:31:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11345.410963
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:31:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11347.612141
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:31:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11348.579233
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:31:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11351.410803
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:31:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11353.363743
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:31:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11354.83605
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:31:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11355.869925
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:31:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11360.730957
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4539 2014-07-24 00:31:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11362.913135
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4521 2014-07-24 00:31:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11364.590973
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3067 2014-07-24 00:49:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11441.798921
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3073 2014-07-24 00:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11444.13221
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3085 2014-07-24 00:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11445.542803
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3091 2014-07-24 00:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11448.769610
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3059 2014-07-24 00:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11451.89753
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11453.504155
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3061 2014-07-24 00:49:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11454.962200
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3069 2014-07-24 00:49:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11457.969910
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:49:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11459.197891
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3071 2014-07-24 00:49:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11460.131903
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3011 2014-07-24 00:49:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11461.163111
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3005 2014-07-24 00:49:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11466.694589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4166 2014-07-24 00:49:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11468.116318
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4166 2014-07-24 00:49:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11470.200781
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 19:48:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76531.987341
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 19:48:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76534.671371
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 19:48:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76535.953358
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 19:48:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76538.849973
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 19:48:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76541.806996
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:48:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76543.948647
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:48:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76544.562740
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 19:48:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76548.357570
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:48:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76552.315188
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:48:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76553.63037
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 19:48:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76555.174268
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 19:48:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76560.914983
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 19:48:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76562.261894
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 19:48:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76564.205793
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 19:49:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76572.512196
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 19:49:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76575.107734
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 19:49:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76576.720494
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 19:49:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76579.670884
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 19:49:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76582.707987
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:49:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76584.306150
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:49:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76585.276386
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 19:49:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76588.441141
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:49:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76590.713066
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:49:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76591.566981
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 19:49:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76592.848812
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 19:49:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76597.786889
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 19:49:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76599.948038
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 19:49:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76601.424123
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 19:49:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76608.855398
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 19:49:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76611.476339
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 19:49:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76612.297276
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 19:49:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76615.799785
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 19:49:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76618.549995
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:49:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76620.68416
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:49:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76621.323572
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 19:49:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76624.507424
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:49:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76627.782083
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:49:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76628.224213
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 19:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76629.945965
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 19:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76634.158353
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 19:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76636.301706
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 19:49:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76638.160009
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 19:49:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76639.267996
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-04 19:49:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76640.550259
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 19:49:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76647.390000
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 19:49:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76650.99694
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 19:49:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76651.458620
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 19:49:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76654.328841
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 19:49:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76657.771696
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:49:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76659.991065
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:49:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76660.768644
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 19:49:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76663.461228
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:49:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76665.117039
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:49:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76666.453420
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 19:49:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76667.669832
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 19:49:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76672.241417
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 19:49:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76674.419823
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 19:49:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76676.304715
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 19:50:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76677.687437
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-04 19:50:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76678.574353
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 19:50:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76685.393006
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 19:50:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76688.58525
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 19:50:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76689.639287
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 19:50:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76692.602330
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 19:50:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76695.877756
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:50:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76697.687943
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 19:50:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76698.168523
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 19:50:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76701.571689
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:50:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76703.323978
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 19:50:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76704.635837
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 19:50:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76705.227041
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 19:50:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76710.56047
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 19:50:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76712.287580
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 19:50:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76714.898011
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 19:50:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76715.105663
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-04 19:50:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76716.342401
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 20:11:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76736.405226
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 20:11:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76739.383154
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 20:11:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76740.76928
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 20:11:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76743.366407
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 20:11:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76746.540854
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:11:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76748.973375
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:11:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76749.848434
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 20:11:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76752.102983
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:11:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76754.497658
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:11:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76755.148069
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 20:11:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76756.312450
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 20:11:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76761.844048
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 20:11:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76763.944419
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 20:11:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76765.523070
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 20:11:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76766.852687
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-04 20:11:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76767.706264
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 20:12:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76775.262097
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 20:12:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76778.485343
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 20:12:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76779.449440
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 20:12:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76782.42254
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 20:12:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76785.476687
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:12:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76787.233126
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:12:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76788.623544
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 20:12:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76791.545440
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:12:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76793.570826
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:12:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76794.244797
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 20:12:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76795.287112
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 20:12:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76800.761082
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 20:12:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76802.634061
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 20:12:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76804.802509
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 20:12:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76805.587393
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-04 20:12:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76806.106067
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 20:12:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76813.399592
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 20:12:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76816.508956
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 20:12:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76817.517399
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 20:12:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76820.720155
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 20:12:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76823.986067
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:12:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76825.605767
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:12:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76826.627359
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 20:12:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76829.991165
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:12:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76831.821970
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:12:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76832.326662
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 20:12:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76834.889294
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 20:12:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76839.416239
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 20:12:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76841.483047
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 20:12:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76843.208769
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 20:12:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76845.624470
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-04 20:12:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76846.200236
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 20:46:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76900.809557
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 20:46:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76903.429179
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 20:46:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76904.369713
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 20:46:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76907.789088
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 20:46:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76910.270687
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:46:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76912.219850
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:46:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76913.552101
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 20:46:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76916.609337
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:46:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76918.551734
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:46:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76919.543862
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 20:46:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76920.822430
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 20:46:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76925.122399
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 20:46:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76927.762858
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 20:46:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76929.960915
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-04 20:46:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76930.416166
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3306 2014-08-04 20:46:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76931.42823
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 20:49:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76944.877285
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 20:49:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76947.351982
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 20:49:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76948.975332
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 20:49:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76951.463826
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 20:49:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76954.553363
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:49:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76956.411476
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 20:49:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76957.151793
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 20:49:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76960.276076
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:49:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76962.327696
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 20:49:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76963.931368
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 20:49:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76964.241905
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 20:49:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76969.467626
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 20:49:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76971.140829
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 20:49:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76973.693731
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 20:49:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76974.986274
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 20:49:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.76975.36411
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:00:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77006.789589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:00:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77009.970643
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:00:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77010.393728
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:00:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77013.111130
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:00:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77016.730017
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:00:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77018.682858
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:00:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77019.33507
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:00:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77022.842005
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:00:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77024.595952
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:00:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77025.875844
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:00:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77026.546457
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:00:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77031.683375
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 21:00:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77033.787338
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:00:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77035.834761
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:00:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77036.232361
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3306 2014-08-04 21:00:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77037.876812
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:01:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77045.94093
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:01:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77048.965334
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:01:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77049.430357
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:01:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77052.637127
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:01:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77055.292369
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:01:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77057.515152
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:01:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77058.866943
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:01:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77061.457164
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:01:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77063.851455
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:01:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77064.903430
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:01:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77065.156077
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:01:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77070.615966
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 21:01:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77072.487897
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:01:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77074.209954
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:01:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77075.1074
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3306 2014-08-04 21:01:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77076.352223
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:01:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77083.35515
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:01:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77086.305467
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:01:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77087.236085
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:01:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77090.998862
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:01:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77093.699192
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:01:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77095.812398
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:01:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77096.530852
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:01:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77099.909111
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:01:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77101.509235
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:01:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77102.739052
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:01:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77103.561549
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:01:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77108.832333
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 21:01:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77110.897965
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:01:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77112.375315
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:01:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77113.805421
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3306 2014-08-04 21:01:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77114.817397
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:02:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77121.792426
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:02:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77124.392244
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:02:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77125.193291
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:02:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77128.291112
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:02:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77131.955609
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:02:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77133.722561
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:02:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77134.811665
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:02:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77137.830648
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:02:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77139.905457
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:02:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77140.58606
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:02:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77141.340505
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:02:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77146.117327
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4713 2014-08-04 21:02:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77148.876134
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:02:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77150.86508
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:02:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77151.492396
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3306 2014-08-04 21:02:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77152.333930
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:03:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77159.839201
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:03:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77162.240598
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:03:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77163.921984
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:03:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77166.420580
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:03:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77169.498861
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:03:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77171.846582
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:03:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77172.430198
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:03:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77175.897383
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:03:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77177.390300
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:03:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77178.47040
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:03:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77179.638662
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:03:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77184.622232
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4714 2014-08-04 21:03:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77186.453108
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:03:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77188.589364
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:03:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77189.17809
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3308 2014-08-04 21:03:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77190.75607
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:04:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77209.811677
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:04:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77212.348955
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:04:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77213.962200
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:04:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77216.146096
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:04:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77219.559744
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:04:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77221.697741
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:04:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77222.872532
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:04:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77225.98063
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:04:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77227.395529
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:04:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77228.785106
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:04:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77229.893919
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:05:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77234.301435
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:05:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77236.762584
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:05:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77238.148301
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:05:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77239.127033
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3310 2014-08-04 21:05:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77240.228010
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:07:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77248.943424
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:07:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77251.116870
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:07:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77252.665125
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:07:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77255.963876
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:07:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77258.514514
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:07:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77260.629401
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:07:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77261.650102
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:07:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77264.23512
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:07:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77266.777401
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:07:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77267.195279
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:07:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77268.128532
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:07:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77273.398524
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:07:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77275.329638
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:07:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77277.493343
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:07:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77278.60788
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3300 2014-08-04 21:07:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77279.353182
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:07:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77287.227104
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:07:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77290.338972
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:07:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77291.453153
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:07:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77294.941765
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:07:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77297.553796
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:07:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77299.879120
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:07:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77300.801792
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:07:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77303.329796
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:07:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77305.26762
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:07:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77306.533025
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:07:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77307.8809
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:07:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77312.631753
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:07:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77314.621093
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:07:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77316.785430
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:07:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77317.542750
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3310 2014-08-04 21:07:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77318.804564
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:07:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77325.909615
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:07:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77328.314659
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:07:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77329.79709
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:07:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77332.931787
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:07:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77335.970555
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:07:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77337.522883
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:07:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77338.358318
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:07:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77341.917320
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:07:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77343.88912
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:07:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77344.402047
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:07:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77345.957684
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:07:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77350.484291
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:07:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77352.419972
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:07:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77354.601224
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:07:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77355.646264
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3310 2014-08-04 21:07:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77356.521977
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3226 2014-08-04 21:08:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77363.663692
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3235 2014-08-04 21:08:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77366.347544
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3244 2014-08-04 21:08:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77367.605902
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3253 2014-08-04 21:08:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77370.511077
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:08:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77373.198979
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:08:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77375.51378
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:08:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77376.97794
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:08:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77379.307745
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:08:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77381.495566
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:08:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77382.217509
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:08:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77383.994820
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:08:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77388.851031
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:08:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77390.194479
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:08:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77392.887613
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:08:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77393.785148
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3312 2014-08-04 21:08:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77394.556941
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3226 2014-08-04 21:08:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77401.210110
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3235 2014-08-04 21:08:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77404.587487
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3244 2014-08-04 21:08:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77405.251105
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3253 2014-08-04 21:08:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77408.990420
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:08:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77411.96957
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:08:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77413.738158
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:08:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77414.285182
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:08:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77417.21939
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:08:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77419.62720
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:08:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77420.487420
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:08:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77421.253882
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:08:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77426.137116
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:08:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77428.535290
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:08:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77430.602002
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:08:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77431.893586
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3312 2014-08-04 21:08:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77432.220550
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:09:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77439.532728
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:09:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77442.927344
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:09:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77443.639099
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:09:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77446.450262
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:09:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77449.10477
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:09:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77451.55175
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:09:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77452.351056
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:09:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77455.36732
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:09:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77457.547807
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:09:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77458.225964
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:09:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77459.623526
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:09:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77464.4631
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:09:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77466.546606
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:09:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77468.720151
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:09:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77469.843043
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3310 2014-08-04 21:09:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77470.352888
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3226 2014-08-04 21:09:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77479.399950
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3235 2014-08-04 21:09:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77482.819142
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3244 2014-08-04 21:09:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77483.427638
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3253 2014-08-04 21:09:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77486.632776
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:09:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77489.420047
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:09:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77491.177322
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:09:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77492.754417
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:09:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77495.526559
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:09:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77497.128897
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:09:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77498.424542
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:09:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77499.400557
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:09:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77504.678106
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:09:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77506.19166
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:09:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77508.833778
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:09:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77509.5900
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3310 2014-08-04 21:09:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77510.402090
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3226 2014-08-04 21:10:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77518.459183
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3235 2014-08-04 21:10:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77521.9237
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3244 2014-08-04 21:10:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77522.614090
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3253 2014-08-04 21:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77525.368312
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77528.735619
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77530.420599
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77531.729709
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77534.434829
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:10:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77536.53507
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:10:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77537.819817
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:10:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77538.650125
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:10:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77543.774584
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:10:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77545.856368
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:10:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77547.921797
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:10:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77548.340979
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3310 2014-08-04 21:10:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77549.628617
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:11:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77566.305338
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:11:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77569.634340
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:11:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77570.847064
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:11:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77573.170370
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:11:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77576.419285
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:11:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77578.474526
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:11:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77579.968099
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:11:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77582.7377
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:11:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77584.584753
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:11:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77585.685494
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:11:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77586.795443
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:11:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77591.637788
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4715 2014-08-04 21:11:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77593.23127
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:11:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77595.160196
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:11:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77596.994389
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3310 2014-08-04 21:11:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77597.827271
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:13:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77622.678446
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:13:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77625.959794
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:13:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77626.814606
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:13:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77629.213212
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:13:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77632.738639
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:13:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77634.805276
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:13:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77635.289855
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:13:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77638.539493
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:13:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77640.214640
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:13:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77641.314105
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:13:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77642.668238
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:13:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77647.498317
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 21:13:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77649.819529
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:13:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77651.822981
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:13:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77652.507072
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3288 2014-08-04 21:13:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77653.144854
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:16:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77665.341564
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:16:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77668.131647
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:16:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77669.2559
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:16:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77672.339435
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:16:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77675.781465
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:16:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77677.874362
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:16:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77678.594566
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:16:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77681.700245
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:16:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77683.81321
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:16:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77684.795436
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:16:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77685.319515
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:16:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77690.80626
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 21:16:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77692.290093
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:16:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77694.901939
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:16:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77695.485612
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3288 2014-08-04 21:16:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77696.842775
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:16:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77704.922172
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:16:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77707.610747
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:16:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77708.313003
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:16:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77711.353649
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:16:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77714.303671
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:16:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77716.610822
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:16:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77717.820863
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:16:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77720.319455
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:16:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77722.406845
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:16:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77723.964417
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:16:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77724.923242
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:16:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77729.464021
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4713 2014-08-04 21:16:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77731.592033
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:16:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77733.829587
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:16:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77734.949499
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3288 2014-08-04 21:16:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77735.627502
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:17:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77742.414007
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:17:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77745.740150
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:17:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77746.142921
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:17:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77749.160494
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:17:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77752.564927
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:17:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77754.849303
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:17:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77755.504460
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:17:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77758.732395
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:17:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77760.215176
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:17:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77761.37536
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:17:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77762.755516
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:17:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77767.746328
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 21:17:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77769.79981
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:17:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77771.959352
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:17:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77772.717856
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3288 2014-08-04 21:17:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77773.83388
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:18:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77787.877292
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:18:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77790.315709
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:18:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77791.918217
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:18:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77794.258857
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:18:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77797.912377
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:18:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77799.84788
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:18:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77800.285794
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:18:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77803.176264
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:18:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77805.181940
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:18:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77806.80095
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:18:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77807.59838
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:18:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77812.158468
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 21:18:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77814.394917
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:18:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77816.512467
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:18:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77817.784575
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3225 2014-08-04 21:18:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77824.23113
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-04 21:18:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77827.335103
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3243 2014-08-04 21:18:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77828.975980
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3252 2014-08-04 21:18:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77831.231088
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3220 2014-08-04 21:18:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77834.85955
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:18:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77836.322972
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3223 2014-08-04 21:18:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77837.485170
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3230 2014-08-04 21:18:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77840.745305
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:18:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77842.391255
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3233 2014-08-04 21:18:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77843.859037
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3179 2014-08-04 21:18:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77844.820331
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3166 2014-08-04 21:18:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77849.908516
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4712 2014-08-04 21:18:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77851.64900
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4657 2014-08-04 21:18:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77853.965354
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-04 21:18:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77854.560246
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-04 21:18:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.77855.825136
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:05:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78062.797560
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:05:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78065.367144
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:05:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78066.71356
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:05:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78069.453272
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:05:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78072.838236
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:05:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78074.718869
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:05:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78075.723021
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:05:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78078.220464
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:05:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78080.900671
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:05:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78081.992328
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:05:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78082.862639
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:05:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78087.530581
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:05:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78089.68709
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:05:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78091.220743
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:05:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78092.200525
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:05:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78093.887527
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:05:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78101.946299
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:05:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78104.681480
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:05:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78105.980096
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:05:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78108.349891
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:05:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78111.407425
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:05:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78113.904857
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:05:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78114.201448
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:05:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78117.702746
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:05:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78119.916322
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:05:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78120.651605
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:05:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78121.743342
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:05:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78126.701574
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:05:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78128.941283
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:05:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78130.902752
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:05:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78131.661063
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:05:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78132.978307
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:05:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78133.111424
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:05:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78134.206711
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:07:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78152.413807
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:07:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78155.426709
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:07:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78156.432235
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:07:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78159.817881
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:07:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78162.698918
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:07:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78164.502616
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:07:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78165.75590
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:07:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78168.582142
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:07:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78170.544153
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:07:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78171.293607
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:07:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78172.449674
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:07:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78177.995290
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:07:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78179.628291
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:07:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78181.773741
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:07:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78182.543287
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:07:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78183.975266
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:07:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78184.436437
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:07:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78185.513108
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-05 01:07:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78186.608450
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:07:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78187.687654
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:08:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78207.718756
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:08:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78210.149811
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:08:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78211.172881
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:08:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78214.6482
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:08:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78217.489064
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:08:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78219.708516
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:08:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78220.638324
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:08:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78223.514730
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:08:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78225.44406
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:08:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78226.308897
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:08:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78227.652844
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:08:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78232.672734
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78234.484079
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78236.497964
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78237.185180
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78238.410192
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:08:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78239.456769
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:08:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78240.211687
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:08:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78241.525879
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:08:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78242.250444
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:12:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78257.19951
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:12:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78260.972248
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:12:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78261.389281
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:12:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78264.848565
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:12:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78267.665511
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:12:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78269.990522
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:12:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78270.786097
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:12:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78273.350560
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:12:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78275.779773
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:12:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78276.70799
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:12:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78277.761475
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:12:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78282.479469
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:12:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78284.72318
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:12:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78286.729225
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:12:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78287.808301
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:12:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78288.85076
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:12:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78289.622638
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:12:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78290.645491
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:12:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78291.850459
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:12:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78292.511034
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3215 2014-08-05 01:12:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78293.717303
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3215 2014-08-05 01:12:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78294.472814
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:13:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78310.351688
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:13:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78313.49114
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:13:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78314.666962
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:13:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78317.903166
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:13:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78320.247925
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:13:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78322.110892
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:13:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78323.366698
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:13:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78326.132060
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:13:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78328.841965
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:13:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78329.635235
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:13:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78330.833060
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:13:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78335.725243
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:13:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78337.780279
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:13:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78339.352546
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:13:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78340.671959
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:13:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78341.244088
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:13:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78342.48248
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:13:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78343.86667
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:13:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78344.692042
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:13:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78345.288362
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3250 2014-08-05 01:13:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78346.752133
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3250 2014-08-05 01:13:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78347.969933
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:14:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78362.273248
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:14:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78365.55433
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:14:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78366.709925
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:14:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78369.610346
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:14:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78372.741329
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:14:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78374.73576
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:14:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78375.118606
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:14:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78378.546058
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:14:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78380.433021
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:14:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78381.181667
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:14:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78382.717847
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:14:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78387.980062
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:14:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78389.827864
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:14:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78391.151646
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:14:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78392.884866
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:14:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78393.48504
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:14:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78394.500366
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:14:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78395.367335
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:14:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78396.328018
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:14:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78397.597015
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3333 2014-08-05 01:14:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78398.265948
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:14:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78399.296829
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:16:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78408.896474
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:16:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78411.674533
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:16:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78412.92442
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:16:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78415.674624
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:16:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78418.570984
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:16:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78420.509499
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:16:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78421.258071
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:16:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78424.918524
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:16:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78426.490483
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:16:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78428.471379
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:16:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78429.640277
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:16:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78434.147800
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4717 2014-08-05 01:16:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78436.749893
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:16:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78438.882681
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:16:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78439.39593
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:16:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78440.783559
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:16:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78441.387242
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:16:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78442.879507
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:16:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78443.820525
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:16:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78444.195776
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3333 2014-08-05 01:16:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78445.445928
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:16:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78446.366346
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:16:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78456.996545
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:16:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78459.57275
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:16:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78460.649747
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:16:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78463.448599
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78466.509813
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78468.999586
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78469.101042
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78472.709347
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78474.157298
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:16:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78475.793677
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:16:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78476.428944
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:16:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78481.807218
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4718 2014-08-05 01:16:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78483.371721
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:16:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78485.932964
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:16:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78486.803547
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:16:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78487.607008
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:16:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78488.153668
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:16:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78489.733447
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:16:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78490.999111
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:16:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78491.640311
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3333 2014-08-05 01:16:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78492.950267
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 01:16:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78493.46725
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:21:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78504.494207
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:21:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78507.650310
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:21:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78508.718636
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:21:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78511.317482
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:21:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78514.452102
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:21:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78516.434821
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:21:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78517.137022
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:21:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78520.444690
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:21:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78522.350000
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:21:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78523.570389
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:21:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78524.833601
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:21:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78529.528505
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4718 2014-08-05 01:21:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78531.924390
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:21:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78533.297543
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:21:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78534.458329
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:21:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78535.501314
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:21:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78536.190978
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:21:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78537.625214
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:21:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78538.866629
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:21:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78539.319313
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3333 2014-08-05 01:21:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78540.360612
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 01:21:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78541.879248
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:22:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78549.506939
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:22:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78552.337141
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:22:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78553.29506
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:22:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78556.747173
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:22:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78559.976195
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:22:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78561.963260
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:22:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78562.584652
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:22:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78565.561243
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:22:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78567.599231
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:22:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78568.273285
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:22:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78569.83914
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:22:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78574.809960
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4718 2014-08-05 01:22:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78576.919744
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:22:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78578.49828
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:22:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78579.135029
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:22:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78580.201843
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:22:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78581.922569
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:22:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78582.754012
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:22:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78583.387015
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:22:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78584.827008
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3333 2014-08-05 01:22:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78585.679473
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 01:22:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78586.916717
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:23:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78595.455563
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:23:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78598.247788
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:23:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78599.293588
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:23:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78602.483863
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:23:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78605.167289
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:23:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78607.671662
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:23:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78608.5029
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:23:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78611.690846
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:23:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78613.34168
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:23:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78614.217738
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:23:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78615.165087
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:23:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78620.91678
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4718 2014-08-05 01:23:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78622.328089
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:23:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78624.525035
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:23:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78625.631917
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:23:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78626.964724
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:23:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78627.3045
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:23:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78628.679514
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:23:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78629.81457
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:23:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78630.551272
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3333 2014-08-05 01:23:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78631.799331
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 01:23:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78632.763580
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:24:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78639.194376
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:24:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78642.193762
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:24:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78643.329083
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:24:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78646.207894
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:24:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78649.866533
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:24:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78651.660804
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:24:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78652.774991
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:24:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78655.231462
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:24:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78657.902087
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:24:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78658.681124
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:24:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78659.266671
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:24:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78664.129944
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4719 2014-08-05 01:24:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78666.207162
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:24:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78668.478198
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:24:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78669.686841
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:24:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78670.211530
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:24:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78671.318390
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:24:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78672.609692
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:24:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78673.68159
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:24:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78674.917386
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3333 2014-08-05 01:24:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78675.722136
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 01:24:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78676.601133
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:24:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78687.116281
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:24:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78690.66176
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:24:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78691.882212
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:24:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78694.233135
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:24:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78697.254288
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:24:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78699.203189
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:24:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78700.66727
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:24:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78703.94058
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:24:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78705.866247
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:24:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78706.719751
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:24:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78707.308436
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:24:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78712.963421
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4719 2014-08-05 01:24:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78714.294875
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:24:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78716.474627
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:24:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78717.684470
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:24:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78718.362811
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:24:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78719.848044
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:24:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78720.188046
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:24:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78721.464967
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:24:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78722.695914
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 01:24:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78723.474423
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3373 2014-08-05 01:24:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78724.873340
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:25:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78731.606434
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:25:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78734.853364
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:25:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78735.897937
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78738.849351
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78741.664165
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78743.287986
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78744.349201
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78747.958034
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:25:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78749.36093
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:25:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78750.221999
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:25:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78751.651594
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:25:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78756.959512
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4719 2014-08-05 01:25:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78758.734550
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:25:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78760.858655
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:25:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78761.841092
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:25:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78762.344225
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:25:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78763.976016
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:25:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78764.109855
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:25:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78765.943404
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:25:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78766.587497
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 01:25:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78767.569801
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3373 2014-08-05 01:25:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78768.520263
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:26:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78782.353767
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:26:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78785.928551
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:26:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78786.490900
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:26:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78789.425614
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:26:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78792.665027
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:26:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78794.745663
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:26:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78795.452459
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:26:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78798.684121
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:26:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78800.780457
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:26:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78801.738635
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:26:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78802.3103
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:26:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78807.808939
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4719 2014-08-05 01:26:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78809.302727
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:26:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78811.840948
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:26:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78812.342881
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:26:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78813.318583
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:26:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78814.494980
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:26:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78815.291137
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:26:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78816.576568
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:26:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78817.485607
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-05 01:26:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78818.69582
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 01:26:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78819.260077
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:27:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78827.390838
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:27:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78830.941389
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:27:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78831.953990
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:27:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78834.874728
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:27:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78837.171265
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:27:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78839.40613
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:27:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78840.328943
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:27:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78843.274517
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:27:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78845.496085
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:27:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78846.386014
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:27:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78847.998393
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:27:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78852.61478
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:27:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78854.507794
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:27:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78856.505240
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:27:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78857.999287
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:27:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78858.76310
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:27:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78859.128472
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:27:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78860.240239
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:27:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78861.355751
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:27:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78862.766439
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:27:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78863.95876
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:27:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78864.701396
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:28:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78875.914138
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:28:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78878.289021
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:28:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78879.339556
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:28:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78882.18492
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:28:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78885.217941
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:28:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78887.711511
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:28:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78888.599344
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:28:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78891.857137
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:28:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78893.605038
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:28:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78894.575771
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:28:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78895.345230
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:28:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78900.786381
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:28:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78902.246391
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:28:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78904.574974
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:28:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78905.305874
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:28:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78906.109695
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:28:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78907.117630
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:28:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78908.622805
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:28:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78909.859843
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:28:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78910.860475
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:28:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78911.780175
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:28:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78912.822371
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:28:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78920.173191
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:28:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78923.832685
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:28:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78924.120449
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:28:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78927.553920
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:28:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78930.896267
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:28:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78932.616571
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:28:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78933.362793
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:28:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78936.685644
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:28:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78938.792110
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:28:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78939.186058
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:28:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78940.301676
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:28:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78945.995997
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:28:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78947.149491
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:28:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78949.807746
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:28:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78950.622669
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:28:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78951.688665
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:28:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78952.241696
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:28:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78953.442988
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:28:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78954.360744
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:28:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78955.233192
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:28:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78956.766752
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:28:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78957.811417
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3215 2014-08-05 01:28:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78958.766067
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3215 2014-08-05 01:28:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78959.168017
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:30:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78975.224041
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:30:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78978.171030
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:30:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78979.909821
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:30:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78982.634527
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:30:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78985.748130
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:30:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78988.622579
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:30:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78989.608482
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:30:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78992.370118
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:30:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78994.88881
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:30:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78995.227106
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:30:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.78998.364150
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:30:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79004.666462
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:30:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79006.917018
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:30:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79008.409798
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:30:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79009.42809
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:30:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79010.515503
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:30:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79011.351686
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:30:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79012.205050
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:30:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79013.342202
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:30:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79014.185511
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:30:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79015.345188
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:30:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79016.3680
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3332 2014-08-05 01:30:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79017.729189
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:30:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79018.459693
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:30:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79028.93663
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:30:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79031.31458
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:30:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79032.240368
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:30:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79035.747671
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:30:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79038.667246
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:30:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79040.330464
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:30:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79041.256573
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:30:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79044.373085
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:30:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79046.58662
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:30:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79047.585025
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:30:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79048.279287
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:30:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79053.703629
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:30:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79055.228713
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:30:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79057.831746
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:30:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79058.421687
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:30:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79059.803309
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:30:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79060.610334
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:30:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79061.130437
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:31:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79062.299519
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:31:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79063.57819
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:31:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79064.129131
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:31:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79065.695983
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3332 2014-08-05 01:31:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79066.552618
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:31:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79067.652931
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3229 2014-08-05 01:33:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79108.266356
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3238 2014-08-05 01:33:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79111.962980
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3247 2014-08-05 01:33:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79112.949847
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3256 2014-08-05 01:33:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79115.18316
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3224 2014-08-05 01:33:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79118.862790
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:33:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79120.546120
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3227 2014-08-05 01:33:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79121.184457
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3234 2014-08-05 01:33:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79124.239310
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:33:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79126.971714
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3237 2014-08-05 01:33:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79127.553972
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3183 2014-08-05 01:33:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79128.40600
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3170 2014-08-05 01:33:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79133.402855
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4716 2014-08-05 01:33:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79135.217101
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4661 2014-08-05 01:33:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79137.273101
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 01:33:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79138.220265
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3340 2014-08-05 01:33:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79139.838340
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 01:33:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79140.743119
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:33:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79141.562134
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:33:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79142.9624
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:33:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79143.854574
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:33:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79144.498100
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:33:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79145.816795
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3332 2014-08-05 01:33:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79146.621569
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:33:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79147.896374
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-05 01:37:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79274.36617
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-05 01:37:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79277.513600
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3356 2014-08-05 01:37:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79278.570408
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 01:37:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79281.690406
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3333 2014-08-05 01:37:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79284.201855
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:37:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79286.339041
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 01:37:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79287.199
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 01:37:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79290.312101
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3346 2014-08-05 01:37:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79292.338823
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3346 2014-08-05 01:37:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79293.191979
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3292 2014-08-05 01:37:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79294.591299
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3279 2014-08-05 01:37:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79299.257111
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4826 2014-08-05 01:37:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79301.554220
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4770 2014-08-05 01:37:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79303.563058
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3451 2014-08-05 01:37:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79304.626515
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3449 2014-08-05 01:37:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79305.967917
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3438 2014-08-05 01:37:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79306.277770
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3422 2014-08-05 01:37:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79307.980580
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3445 2014-08-05 01:37:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79308.277131
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3439 2014-08-05 01:37:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79309.277685
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3445 2014-08-05 01:37:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79310.805013
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3477 2014-08-05 01:37:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79311.572336
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3441 2014-08-05 01:37:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79312.587360
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 01:37:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79313.327586
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3346 2014-08-05 01:39:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79347.87245
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 01:39:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79350.180507
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3364 2014-08-05 01:39:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79351.626775
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3373 2014-08-05 01:39:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79354.147317
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3341 2014-08-05 01:39:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79357.936958
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-05 01:39:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79359.171270
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3344 2014-08-05 01:39:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79360.922657
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 01:39:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79363.781920
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 01:40:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79365.550676
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 01:40:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79366.400848
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3300 2014-08-05 01:40:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79367.64114
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3287 2014-08-05 01:40:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79372.905985
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4844 2014-08-05 01:40:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79374.431163
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4787 2014-08-05 01:40:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79376.269831
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:40:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79377.521288
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 01:40:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79378.706605
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3446 2014-08-05 01:40:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79379.743976
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3430 2014-08-05 01:40:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79380.257924
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3453 2014-08-05 01:40:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79381.727539
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3447 2014-08-05 01:40:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79382.762556
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3453 2014-08-05 01:40:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79383.814291
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 01:40:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79384.407875
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3449 2014-08-05 01:40:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79385.610015
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 01:40:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79386.220386
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3353 2014-08-05 01:46:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79456.985373
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3362 2014-08-05 01:46:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79459.477636
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 01:46:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79460.898476
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 01:46:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79463.122789
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-05 01:46:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79466.662443
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 01:47:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79468.759716
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 01:47:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79469.976661
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3359 2014-08-05 01:47:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79472.858811
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3362 2014-08-05 01:47:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79474.501257
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3362 2014-08-05 01:47:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79475.189046
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3308 2014-08-05 01:47:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79476.957606
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3295 2014-08-05 01:47:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79481.541708
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4850 2014-08-05 01:47:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79483.977552
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4793 2014-08-05 01:47:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79485.314113
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3465 2014-08-05 01:47:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79486.981682
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:47:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79487.489338
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3452 2014-08-05 01:47:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79488.681622
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3436 2014-08-05 01:47:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79489.602191
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:47:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79490.581167
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3453 2014-08-05 01:47:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79491.66390
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:47:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79492.782661
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3491 2014-08-05 01:47:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79493.961323
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3455 2014-08-05 01:47:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79494.822458
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 01:47:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79495.382383
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 01:53:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79603.627441
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 01:53:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79606.926972
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 01:53:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79607.912108
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 01:53:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79610.952195
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3257 2014-08-05 01:53:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79613.319265
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3359 2014-08-05 01:53:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79621.623473
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:53:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79624.255323
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3378 2014-08-05 01:53:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79625.341458
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3387 2014-08-05 01:53:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79628.175354
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 01:53:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79631.847040
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 01:53:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79633.606912
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 01:53:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79634.757806
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 01:53:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79637.619576
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:53:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79639.807092
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:53:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79640.478130
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:53:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79641.926014
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3300 2014-08-05 01:53:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79646.163392
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 01:53:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79648.371005
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 01:53:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79650.761310
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:53:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79651.951873
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3330 2014-08-05 01:53:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79652.246834
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 01:53:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79653.122163
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 01:53:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79654.569999
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:53:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79655.251868
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 01:53:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79656.502314
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:54:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79658.352875
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 01:54:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79659.532025
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:54:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79660.438802
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 01:54:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79661.963037
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3359 2014-08-05 01:54:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79668.209348
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:54:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79671.253811
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3378 2014-08-05 01:54:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79672.466254
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3387 2014-08-05 01:54:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79675.256312
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 01:54:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79678.853749
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 01:54:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79680.269270
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 01:54:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79681.462950
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 01:54:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79684.557996
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:54:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79686.24490
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:54:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79687.138859
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:54:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79688.133890
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3300 2014-08-05 01:54:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79693.587447
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 01:54:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79695.742947
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 01:54:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79697.419714
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-05 01:54:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79698.433020
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3338 2014-08-05 01:54:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79699.876323
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 01:54:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79700.904649
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 01:54:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79701.948756
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:54:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79702.834649
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 01:54:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79703.507110
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:54:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79704.508754
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 01:54:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79705.410828
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:54:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79706.159965
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 01:54:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79707.134080
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3359 2014-08-05 01:54:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79717.91332
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:54:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79720.163025
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3378 2014-08-05 01:54:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79721.151572
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3387 2014-08-05 01:54:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79724.694266
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 01:54:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79727.233797
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 01:54:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79729.639811
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 01:54:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79730.151494
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 01:54:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79733.727150
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:54:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79735.997651
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 01:54:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79736.983670
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 01:54:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79737.118785
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3300 2014-08-05 01:54:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79742.406441
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 01:54:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79744.734689
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 01:54:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79746.452610
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 01:54:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79747.297876
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 01:54:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79748.487665
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 01:54:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79749.15873
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 01:54:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79750.206003
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:54:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79751.973102
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 01:54:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79752.810750
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:54:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79753.383422
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 01:54:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79754.387445
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:54:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79755.833203
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 01:54:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79756.57642
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 01:55:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79763.501390
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:55:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79766.252134
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 01:55:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79767.85440
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 01:55:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79770.706711
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 01:55:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79773.241006
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:55:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79775.560810
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:55:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79776.538554
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 01:55:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79779.151441
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:55:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79781.500238
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:55:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79782.301301
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 01:55:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79783.701209
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 01:55:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79788.269307
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 01:55:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79790.322594
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 01:55:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79792.956414
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 01:55:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79793.9376
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3487 2014-08-05 01:55:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79794.301486
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 01:55:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79795.168096
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 01:55:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79796.501870
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:55:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79797.529921
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 01:55:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79798.678057
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:55:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79799.120222
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 01:55:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79800.381602
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:55:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79801.705363
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 01:55:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79802.691995
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 01:57:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79812.848395
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:57:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79815.471836
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 01:57:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79816.858098
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 01:57:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79819.253439
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 01:57:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79822.457720
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:57:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79824.529779
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:57:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79825.473780
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 01:57:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79828.641343
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:57:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79830.106935
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:57:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79831.375494
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 01:57:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79832.900439
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 01:57:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79837.237402
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 01:57:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79839.348538
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 01:57:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79841.640061
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 01:57:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79842.554909
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3487 2014-08-05 01:57:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79843.72325
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 01:57:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79846.398130
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 01:57:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79847.9889
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:57:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79848.360353
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 01:57:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79849.699861
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:57:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79850.328376
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 01:57:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79851.469257
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:57:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79852.114398
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 01:57:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79853.657496
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 01:58:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79864.685315
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:58:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79867.241969
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 01:58:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79868.196452
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 01:58:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79871.51267
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 01:58:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79874.452435
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:58:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79876.105025
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:58:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79877.513424
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 01:58:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79880.403992
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:58:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79882.793192
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:58:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79883.828726
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 01:58:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79884.174899
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 01:58:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79889.27723
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 01:58:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79891.241074
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 01:58:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79893.635906
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 01:58:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79894.859363
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3487 2014-08-05 01:58:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79895.281038
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 01:58:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79898.186097
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 01:58:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79899.627834
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:58:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79900.897250
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 01:58:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79901.253479
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:58:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79902.300876
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 01:58:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79903.999244
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:58:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79904.820000
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 01:58:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79905.730458
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 01:59:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79913.27226
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:59:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79916.858275
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 01:59:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79917.258924
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 01:59:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79920.558114
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 01:59:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79923.564438
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:59:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79925.134171
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 01:59:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79926.994622
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 01:59:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79929.248888
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:59:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79931.454292
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 01:59:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79932.325908
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 01:59:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79933.896793
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 01:59:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79938.870821
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 01:59:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79940.545026
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 01:59:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79942.867845
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 01:59:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79943.283159
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3487 2014-08-05 01:59:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79944.113918
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 01:59:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79947.765757
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 01:59:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79948.132178
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:59:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79949.835180
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 01:59:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79950.37488
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 01:59:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79951.752497
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 01:59:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79952.503695
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 01:59:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79953.609191
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 01:59:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79954.793179
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:02:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79975.985019
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:02:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79978.660762
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 02:02:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79979.415345
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 02:02:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79982.932191
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:02:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79985.915043
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:02:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79987.12047
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:02:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79988.637934
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 02:02:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79991.814339
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:02:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79993.875187
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:02:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79994.140804
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:02:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.79995.657060
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:02:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80000.798783
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 02:02:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80002.727362
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 02:02:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80004.57492
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 02:02:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80005.154740
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3487 2014-08-05 02:02:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80006.681863
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:02:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80007.103340
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 02:02:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80008.816625
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:02:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80009.159636
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 02:02:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80010.591324
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:02:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80011.205500
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 02:02:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80012.424572
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 02:02:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80013.188322
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 02:02:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80014.604130
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:04:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80035.691469
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:04:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80038.967759
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 02:04:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80039.375960
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 02:04:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80042.773225
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:04:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80045.752023
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:04:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80047.588094
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:04:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80048.569097
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 02:04:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80051.87482
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:04:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80053.234641
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:04:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80054.813991
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:04:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80055.872864
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:04:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80060.873061
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 02:04:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80062.449035
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 02:04:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80064.107608
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 02:04:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80065.258342
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3487 2014-08-05 02:04:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80066.782917
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:04:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80067.233809
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 02:04:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80068.166945
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:04:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80069.192322
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 02:04:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80070.116311
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:04:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80071.605773
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 02:04:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80072.242168
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 02:04:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80073.56101
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 02:04:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80074.689289
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:06:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80096.484189
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80099.494421
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 02:06:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80100.633876
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 02:06:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80103.369775
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:06:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80106.740659
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:06:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80108.359280
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:06:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80109.234737
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 02:06:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80112.940975
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80114.719326
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80115.665611
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:06:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80116.277962
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:06:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80121.714466
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 02:06:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80123.628838
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 02:06:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80125.773715
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 02:06:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80126.253914
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3487 2014-08-05 02:06:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80127.723387
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:06:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80128.266446
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 02:06:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80129.753815
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:06:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80130.891354
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 02:06:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80131.769816
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:06:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80132.571639
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 02:06:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80133.429189
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 02:06:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80134.504108
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 02:06:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80135.420294
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:06:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80149.223931
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80152.262226
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 02:06:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80153.981771
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 02:06:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80156.527269
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:06:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80159.195357
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:06:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80161.887532
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:06:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80162.424526
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 02:06:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80165.33084
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80167.51773
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80168.767555
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:06:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80169.847930
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:06:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80174.501114
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 02:06:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80176.591550
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 02:06:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80178.110964
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:06:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80179.643369
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 02:06:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80180.517569
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:06:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80181.355198
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 02:06:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80182.490722
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:06:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80183.569177
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 02:06:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80184.737479
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 02:06:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80185.696491
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 02:06:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80186.777679
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:06:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80191.866217
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80194.897295
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 02:06:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80195.201511
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 02:06:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80198.570474
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:06:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80201.259713
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:06:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80203.504927
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:06:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80204.181707
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3366 2014-08-05 02:06:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80207.936394
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80209.984563
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:06:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80210.341656
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:06:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80211.688001
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:06:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80216.923204
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4854 2014-08-05 02:06:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80218.108014
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4797 2014-08-05 02:06:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80220.301786
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:06:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80221.353770
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3440 2014-08-05 02:06:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80222.100962
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:06:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80223.442373
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3457 2014-08-05 02:06:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80224.307724
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:06:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80225.237897
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 02:06:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80226.75508
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 02:06:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80227.556024
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 02:06:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80228.60450
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 02:08:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80276.724076
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:08:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80279.560033
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:08:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80280.92529
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3376 2014-08-05 02:08:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80283.102105
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3346 2014-08-05 02:08:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80288.242943
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3349 2014-08-05 02:08:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80290.589031
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-05 02:08:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80291.764375
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 02:08:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80294.610239
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 02:08:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80296.534697
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3356 2014-08-05 02:08:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80297.342929
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3302 2014-08-05 02:08:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80298.255625
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3290 2014-08-05 02:08:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80303.813874
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4836 2014-08-05 02:08:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80305.536598
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4783 2014-08-05 02:08:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80307.253872
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3449 2014-08-05 02:08:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80308.424623
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3435 2014-08-05 02:08:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80309.952771
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:08:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80310.806827
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3452 2014-08-05 02:08:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80311.529302
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:08:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80312.834585
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3490 2014-08-05 02:08:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80313.658519
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3452 2014-08-05 02:08:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80314.478226
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3480 2014-08-05 02:08:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80315.653869
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3353 2014-08-05 02:09:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80349.251116
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3362 2014-08-05 02:09:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80352.103920
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 02:09:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80353.128974
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:09:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80356.380507
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-05 02:09:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80359.423577
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 02:09:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80361.395492
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3350 2014-08-05 02:09:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80362.832664
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:09:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80365.27545
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3361 2014-08-05 02:09:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80367.65709
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:09:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80368.432080
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3306 2014-08-05 02:09:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80369.345294
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3294 2014-08-05 02:09:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80374.100560
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4840 2014-08-05 02:09:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80376.211377
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4785 2014-08-05 02:09:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80378.247962
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3453 2014-08-05 02:09:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80379.507679
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3437 2014-08-05 02:09:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80380.182577
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 02:09:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80381.250387
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3454 2014-08-05 02:09:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80382.850361
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 02:09:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80383.781259
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3492 2014-08-05 02:09:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80384.930574
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:09:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80385.627079
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3482 2014-08-05 02:09:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80386.272853
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 02:10:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80441.375589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80444.99281
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80445.618895
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80448.489641
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80451.156701
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3292 2014-08-05 02:10:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80453.909146
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-05 02:10:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80454.49609
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80457.273934
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3292 2014-08-05 02:10:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80459.412192
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:10:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80460.429669
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3304 2014-08-05 02:10:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80461.602442
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80466.954111
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4077 2014-08-05 02:10:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80468.249098
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4077 2014-08-05 02:10:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80472.213419
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3451 2014-08-05 02:10:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80473.136440
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3435 2014-08-05 02:10:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80474.870761
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 02:10:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80480.570559
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80483.656331
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:10:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80484.353402
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80487.805821
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80491.713599
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3292 2014-08-05 02:10:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80493.541791
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-05 02:10:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80494.927887
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80497.713249
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3292 2014-08-05 02:10:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80499.279186
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:10:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80500.757027
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3304 2014-08-05 02:10:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80501.550877
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:10:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80506.765585
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4077 2014-08-05 02:10:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80508.538656
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4077 2014-08-05 02:10:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80510.80779
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3451 2014-08-05 02:10:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80511.292149
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3435 2014-08-05 02:10:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80512.643279
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 02:10:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80513.79849
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3452 2014-08-05 02:10:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80514.6080
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 02:10:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80515.604548
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3490 2014-08-05 02:10:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80516.594647
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3454 2014-08-05 02:10:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80517.241333
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3480 2014-08-05 02:10:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80518.521653
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3353 2014-08-05 02:11:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80531.637176
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3362 2014-08-05 02:11:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80534.356587
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 02:11:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80535.680799
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:11:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80538.719066
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-05 02:11:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80541.299420
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 02:11:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80543.612158
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3350 2014-08-05 02:11:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80544.847300
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:11:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80547.338705
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3361 2014-08-05 02:11:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80549.748780
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:11:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80550.638027
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3306 2014-08-05 02:11:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80551.884195
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3294 2014-08-05 02:11:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80556.215930
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4840 2014-08-05 02:11:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80558.869246
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4785 2014-08-05 02:11:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80560.363458
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3453 2014-08-05 02:11:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80561.930363
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3437 2014-08-05 02:11:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80562.248633
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 02:11:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80563.381953
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3454 2014-08-05 02:11:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80564.48856
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 02:11:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80565.926821
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3492 2014-08-05 02:11:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80566.315562
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 02:11:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80567.704812
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3482 2014-08-05 02:11:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80568.279835
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3351 2014-08-05 02:11:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80583.554024
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 02:11:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80586.52898
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:11:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80587.135818
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3375 2014-08-05 02:11:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80590.763992
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 02:11:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80593.856902
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3346 2014-08-05 02:11:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80595.802253
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3348 2014-08-05 02:11:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80596.402068
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3353 2014-08-05 02:11:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80599.546648
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3356 2014-08-05 02:11:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80601.23450
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:11:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80602.682467
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3304 2014-08-05 02:11:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80603.667114
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3289 2014-08-05 02:11:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80608.154089
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4835 2014-08-05 02:11:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80610.876997
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4780 2014-08-05 02:11:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80612.917250
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3451 2014-08-05 02:11:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80613.544986
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3435 2014-08-05 02:11:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80614.266257
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 02:11:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80615.618420
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3452 2014-08-05 02:11:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80616.68467
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 02:11:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80617.186561
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3490 2014-08-05 02:11:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80618.772798
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3454 2014-08-05 02:11:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80619.562266
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3480 2014-08-05 02:11:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80620.165499
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:16:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80645.109507
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3376 2014-08-05 02:16:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80648.546077
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3385 2014-08-05 02:16:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80649.276653
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3394 2014-08-05 02:16:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80652.440826
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3362 2014-08-05 02:16:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80655.51428
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 02:16:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80657.671387
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 02:16:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80658.263501
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:16:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80661.943365
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3375 2014-08-05 02:16:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80663.940048
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3375 2014-08-05 02:16:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80664.848425
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3322 2014-08-05 02:16:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80665.675100
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3309 2014-08-05 02:16:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80670.495661
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4865 2014-08-05 02:16:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80672.266343
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4808 2014-08-05 02:16:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80674.585287
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:16:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80675.856562
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3451 2014-08-05 02:16:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80676.6728
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3474 2014-08-05 02:16:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80677.63451
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3468 2014-08-05 02:16:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80678.897371
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3474 2014-08-05 02:16:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80679.546254
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3506 2014-08-05 02:16:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80680.678738
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3470 2014-08-05 02:16:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80681.285807
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3496 2014-08-05 02:16:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80682.665566
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 02:16:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80691.777781
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3374 2014-08-05 02:16:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80694.513433
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3384 2014-08-05 02:16:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80695.820347
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-05 02:16:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80698.487696
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:16:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80701.565659
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 02:16:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80703.549891
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 02:16:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80704.762896
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 02:16:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80707.881257
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3374 2014-08-05 02:16:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80709.988573
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3374 2014-08-05 02:16:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80710.483919
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3320 2014-08-05 02:16:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80711.448396
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3307 2014-08-05 02:16:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80716.253398
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4863 2014-08-05 02:16:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80718.726500
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4806 2014-08-05 02:16:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80720.65114
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3483 2014-08-05 02:16:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80721.232299
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80722.590398
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-05 02:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80723.779826
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3466 2014-08-05 02:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80724.403773
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-05 02:16:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80725.473482
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3504 2014-08-05 02:16:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80726.308115
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3468 2014-08-05 02:16:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80727.260869
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3494 2014-08-05 02:16:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80728.562924
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:20:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80740.588883
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:20:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80743.58774
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3378 2014-08-05 02:20:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80744.30451
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3387 2014-08-05 02:20:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80747.805271
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:20:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80750.481081
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:20:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80752.967098
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:20:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80753.172148
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 02:20:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80756.529041
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 02:20:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80758.519825
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 02:20:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80759.395553
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:20:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80760.609530
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:20:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80765.263902
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4847 2014-08-05 02:20:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80767.206674
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4792 2014-08-05 02:20:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80769.93011
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3478 2014-08-05 02:20:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80770.74941
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3462 2014-08-05 02:20:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80771.956452
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:20:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80772.697008
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3461 2014-08-05 02:20:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80773.501622
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:20:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80774.237231
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3499 2014-08-05 02:20:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80775.813021
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:20:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80776.583675
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 02:20:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80777.224641
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:21:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80789.464704
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:21:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80792.991196
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3378 2014-08-05 02:21:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80793.138801
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3387 2014-08-05 02:21:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80796.358056
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:21:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80799.957602
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:21:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80801.241397
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:21:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80802.335444
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 02:21:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80805.148490
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 02:21:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80807.207493
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 02:21:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80808.285791
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:21:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80809.469190
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:21:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80814.47850
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4847 2014-08-05 02:21:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80816.583893
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4792 2014-08-05 02:21:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80818.917286
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:21:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80819.445741
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3461 2014-08-05 02:21:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80820.771433
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:21:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80821.630099
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3499 2014-08-05 02:21:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80822.177839
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:21:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80823.309510
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 02:21:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80824.398600
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:21:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80832.500517
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:21:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80835.356906
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3378 2014-08-05 02:21:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80836.953577
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3387 2014-08-05 02:21:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80839.148254
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:21:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80842.549669
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:21:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80844.482334
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:21:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80845.582157
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 02:21:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80848.573085
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 02:21:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80850.933379
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 02:21:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80851.310727
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:21:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80852.559234
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:21:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80857.448718
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4847 2014-08-05 02:21:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80859.737477
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4792 2014-08-05 02:21:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80861.9985
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:21:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80862.789442
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3461 2014-08-05 02:21:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80863.731701
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:21:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80864.478638
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3499 2014-08-05 02:21:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80865.353669
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:21:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80866.263806
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 02:21:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80867.818049
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:22:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80872.996406
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 02:22:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80875.765074
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3378 2014-08-05 02:22:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80876.518753
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3387 2014-08-05 02:22:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80879.700135
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3355 2014-08-05 02:22:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80882.89185
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:22:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80884.992274
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3358 2014-08-05 02:22:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80885.265255
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-08-05 02:22:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80888.282319
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 02:22:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80890.112106
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3368 2014-08-05 02:22:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80891.172552
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3314 2014-08-05 02:22:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80892.951920
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3301 2014-08-05 02:22:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80897.699741
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4847 2014-08-05 02:22:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80899.777416
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4792 2014-08-05 02:22:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80901.23786
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:22:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80902.89172
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3461 2014-08-05 02:22:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80903.967328
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 02:22:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80904.789423
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3499 2014-08-05 02:22:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80905.331766
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3463 2014-08-05 02:22:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80906.344771
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 02:22:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80907.742353
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:25:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80955.774200
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:25:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80958.420642
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:25:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80959.335575
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 02:25:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80962.607794
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80965.715087
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80967.649995
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80968.594823
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 02:25:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80971.169880
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:25:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80973.181805
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:25:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80974.458757
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3326 2014-08-05 02:25:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80975.248005
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 02:25:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80980.598501
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4859 2014-08-05 02:25:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80982.622123
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4804 2014-08-05 02:25:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80984.163945
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:25:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80985.11857
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 02:25:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80986.787831
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:25:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80987.631629
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3511 2014-08-05 02:25:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80988.984787
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 02:25:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80989.465056
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3501 2014-08-05 02:25:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80990.676857
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:25:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.80998.57137
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:25:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81001.831530
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:25:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81002.433895
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 02:25:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81005.386133
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:25:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81008.761213
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:25:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81010.376224
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:25:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81011.937131
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 02:25:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81014.332251
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:25:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81016.104090
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:25:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81017.344925
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3326 2014-08-05 02:25:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81018.147549
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 02:25:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81023.439195
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4859 2014-08-05 02:25:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81025.406600
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4804 2014-08-05 02:25:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81027.825212
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:25:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81028.502383
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 02:25:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81029.808745
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:25:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81030.49356
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3511 2014-08-05 02:25:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81031.620326
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 02:25:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81032.981034
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3501 2014-08-05 02:25:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81033.811285
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:27:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81052.7524
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:27:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81055.340930
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:27:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81056.975610
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 02:27:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81059.650571
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:27:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81062.150130
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:27:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81064.448255
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:27:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81065.303253
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 02:27:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81068.573356
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:27:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81070.662801
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:27:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81071.255461
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3326 2014-08-05 02:27:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81072.778482
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 02:27:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81077.557622
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4859 2014-08-05 02:27:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81079.287858
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4804 2014-08-05 02:27:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81081.8101
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81082.834121
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 02:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81083.288508
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81084.9468
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3511 2014-08-05 02:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81085.980442
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 02:27:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81086.729105
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3501 2014-08-05 02:27:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81087.439402
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:28:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81099.761275
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:28:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81102.128753
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:28:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81103.307680
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 02:28:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81106.268142
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:28:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81109.594940
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:28:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81111.505387
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:28:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81112.322780
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 02:28:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81115.857651
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:28:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81117.260018
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:28:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81118.914623
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3326 2014-08-05 02:28:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81119.784816
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 02:28:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81124.156786
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4859 2014-08-05 02:28:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81126.625039
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4804 2014-08-05 02:28:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81128.658821
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:28:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81129.583892
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 02:28:14.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81130.450774
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:28:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81131.638381
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3511 2014-08-05 02:28:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81132.739323
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 02:28:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81133.563184
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3501 2014-08-05 02:28:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81134.400536
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:29:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81150.357855
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:29:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81153.244930
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:29:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81154.747227
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 02:29:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81157.562400
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:29:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81160.149982
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:29:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81162.462737
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:29:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81163.590243
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 02:29:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81166.352856
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:29:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81168.105371
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:29:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81169.683054
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3326 2014-08-05 02:29:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81170.893874
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 02:29:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81175.180117
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4859 2014-08-05 02:29:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81177.659852
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4804 2014-08-05 02:29:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81179.995197
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:29:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81180.46734
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 02:29:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81181.621220
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:29:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81182.862447
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3511 2014-08-05 02:29:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81183.696139
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 02:29:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81184.448244
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3501 2014-08-05 02:29:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81185.517739
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:29:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81192.112560
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:29:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81195.708601
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:29:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81196.958452
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 02:29:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81199.422899
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:29:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81202.558716
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:29:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81204.765502
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:29:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81205.724936
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 02:29:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81208.533130
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:29:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81210.834687
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:29:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81211.926262
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3326 2014-08-05 02:29:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81212.52794
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 02:29:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81217.946173
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4859 2014-08-05 02:29:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81219.283330
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4804 2014-08-05 02:29:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81221.200758
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:29:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81222.515215
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 02:29:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81223.950056
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:29:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81224.862593
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3511 2014-08-05 02:29:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81225.536419
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 02:29:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81226.773675
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3501 2014-08-05 02:29:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81227.525316
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:29:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81234.216239
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:29:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81237.329488
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:29:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81238.107612
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 02:29:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81241.804207
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:29:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81244.493109
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:29:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81246.36116
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:29:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81247.125062
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 02:29:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81250.640261
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:29:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81252.298048
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:29:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81253.817165
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3326 2014-08-05 02:29:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81254.71410
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 02:29:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81259.203237
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4859 2014-08-05 02:29:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81261.547477
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4804 2014-08-05 02:29:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81263.183964
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:29:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81264.342642
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 02:29:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81265.786264
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:29:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81266.359723
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3511 2014-08-05 02:29:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81267.621646
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 02:29:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81268.839686
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3501 2014-08-05 02:29:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81269.914407
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3372 2014-08-05 02:30:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81281.626764
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:30:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81284.882027
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:30:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81285.769222
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 02:30:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81288.182377
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3367 2014-08-05 02:30:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81291.836993
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:30:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81293.500793
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:30:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81294.824757
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 02:30:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81297.922155
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:30:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81299.924978
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 02:30:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81300.251357
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3326 2014-08-05 02:30:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81301.861974
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3313 2014-08-05 02:30:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81306.776219
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4859 2014-08-05 02:30:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81308.144495
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4804 2014-08-05 02:30:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81310.509669
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 02:30:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81311.849858
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3511 2014-08-05 02:30:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81312.276841
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 02:30:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81313.730515
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3501 2014-08-05 02:30:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81314.762260
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3381 2014-08-05 02:35:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81340.934538
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:35:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81343.876288
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 02:35:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81344.631360
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 02:35:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81347.958292
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3376 2014-08-05 02:35:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81350.966185
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 02:35:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81352.740304
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3379 2014-08-05 02:35:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81353.340560
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3387 2014-08-05 02:35:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81356.669514
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:35:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81358.33102
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3390 2014-08-05 02:35:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81359.372173
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3336 2014-08-05 02:35:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81360.993326
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3323 2014-08-05 02:35:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81365.382961
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4879 2014-08-05 02:35:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81367.298178
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4822 2014-08-05 02:35:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81369.8589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3488 2014-08-05 02:35:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81370.679181
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3520 2014-08-05 02:35:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81371.299020
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3484 2014-08-05 02:35:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81372.840057
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3510 2014-08-05 02:35:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81373.219943
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3402 2014-08-05 02:38:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81394.468320
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:38:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81397.818745
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-05 02:38:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81398.242729
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3430 2014-08-05 02:38:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81401.587673
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3397 2014-08-05 02:38:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81404.328170
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 02:38:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81406.226815
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 02:38:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81407.992049
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3408 2014-08-05 02:38:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81410.775640
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:38:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81412.382020
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:38:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81413.599632
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3356 2014-08-05 02:38:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81414.725162
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 02:38:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81419.710395
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4889 2014-08-05 02:38:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81421.478774
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4832 2014-08-05 02:38:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81423.773407
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3516 2014-08-05 02:38:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81424.676235
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3522 2014-08-05 02:38:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81425.717018
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3494 2014-08-05 02:38:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81426.728591
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3520 2014-08-05 02:38:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81427.725681
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 02:42:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81482.907909
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:42:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81485.946043
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:42:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81486.651940
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3434 2014-08-05 02:42:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81489.92617
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 02:42:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81492.788929
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 02:42:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81494.515973
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 02:42:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81495.666996
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-05 02:42:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81498.789243
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:42:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81500.581439
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:42:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81501.623693
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:42:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81502.625182
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-05 02:42:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81507.104582
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4893 2014-08-05 02:42:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81509.514589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4836 2014-08-05 02:42:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81511.448345
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3526 2014-08-05 02:42:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81512.610458
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3558 2014-08-05 02:42:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81513.546162
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3498 2014-08-05 02:42:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81514.978076
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3524 2014-08-05 02:42:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81515.758551
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 02:43:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81522.719250
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81525.597587
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:43:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81526.540328
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3434 2014-08-05 02:43:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81529.306589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 02:43:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81532.968882
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 02:43:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81534.120898
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 02:43:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81535.462883
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-05 02:43:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81538.590286
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81540.23764
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81541.843258
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:43:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81542.817220
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-05 02:43:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81547.372264
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4893 2014-08-05 02:43:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81549.933583
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4836 2014-08-05 02:43:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81551.374077
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3498 2014-08-05 02:43:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81552.846059
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3524 2014-08-05 02:43:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81553.854339
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 02:43:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81560.483514
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81563.442958
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:43:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81564.217861
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3434 2014-08-05 02:43:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81567.75372
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 02:43:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81570.135879
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 02:43:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81572.546605
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 02:43:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81573.111419
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-05 02:43:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81576.367296
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81578.853609
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81579.532290
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:43:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81580.26793
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-05 02:43:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81585.917832
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4893 2014-08-05 02:43:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81587.164326
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4836 2014-08-05 02:43:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81589.137853
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3498 2014-08-05 02:43:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81590.832317
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3524 2014-08-05 02:43:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81591.353608
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 02:43:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81596.104856
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81599.110406
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:43:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81600.191355
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3434 2014-08-05 02:43:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81603.215280
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 02:43:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81606.216619
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 02:43:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81608.566446
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 02:43:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81609.303238
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-05 02:43:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81612.641249
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81614.58376
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3415 2014-08-05 02:43:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81615.883586
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3360 2014-08-05 02:43:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81616.205111
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-05 02:43:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81621.314120
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4893 2014-08-05 02:43:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81623.878150
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4836 2014-08-05 02:43:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81625.227715
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3498 2014-08-05 02:43:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81626.833746
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3524 2014-08-05 02:43:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81627.721010
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3416 2014-08-05 02:45:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81638.291009
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81641.59704
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3435 2014-08-05 02:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81642.488917
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3444 2014-08-05 02:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81645.400143
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81648.892007
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3414 2014-08-05 02:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81650.51414
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3414 2014-08-05 02:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81651.164199
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3422 2014-08-05 02:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81654.940845
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81656.717979
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81657.965039
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:45:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81658.815754
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 02:45:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81663.159894
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4903 2014-08-05 02:45:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81665.339329
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4846 2014-08-05 02:45:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81667.79172
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3532 2014-08-05 02:45:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81668.127189
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3558 2014-08-05 02:45:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81669.717847
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3416 2014-08-05 02:45:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81674.708283
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:45:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81677.732257
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3435 2014-08-05 02:45:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81678.756906
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3444 2014-08-05 02:45:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81681.177015
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:45:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81685.441728
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3414 2014-08-05 02:45:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81687.200589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3414 2014-08-05 02:45:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81688.791032
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3422 2014-08-05 02:45:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81691.205596
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:45:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81693.822971
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3425 2014-08-05 02:45:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81694.320033
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3370 2014-08-05 02:45:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81695.436394
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3357 2014-08-05 02:45:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81700.952695
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4903 2014-08-05 02:45:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81702.491576
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4846 2014-08-05 02:45:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81704.228429
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3532 2014-08-05 02:45:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81705.425745
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3558 2014-08-05 02:45:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81706.493113
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3402 2014-08-05 02:47:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81735.657208
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:47:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81738.841552
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-05 02:47:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81739.238039
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3430 2014-08-05 02:47:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81742.773061
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3397 2014-08-05 02:47:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81745.903923
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 02:47:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81747.278348
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 02:47:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81748.453569
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3408 2014-08-05 02:47:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81751.73753
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:47:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81753.594679
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:47:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81754.701667
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3356 2014-08-05 02:47:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81755.803757
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 02:47:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81760.242054
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4889 2014-08-05 02:47:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81762.675520
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4832 2014-08-05 02:47:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81764.785175
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3402 2014-08-05 02:47:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81770.694634
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:47:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81773.63439
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-05 02:47:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81774.149008
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3430 2014-08-05 02:47:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81777.802410
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3397 2014-08-05 02:47:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81780.121557
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 02:47:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81782.708733
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 02:47:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81783.286657
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3408 2014-08-05 02:47:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81786.692029
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:47:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81788.48276
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 02:47:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81789.283369
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3356 2014-08-05 02:47:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81790.317181
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 02:47:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81795.115225
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4889 2014-08-05 02:47:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81797.498503
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4832 2014-08-05 02:47:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.81799.457124
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 03:00:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82009.304961
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:00:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82012.134216
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3329 2014-08-05 03:00:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82013.101062
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:00:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82016.583636
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:00:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82019.207711
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3337 2014-08-05 03:00:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82021.404246
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 03:00:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82022.568676
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:00:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82025.132943
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3337 2014-08-05 03:00:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82027.745743
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 03:00:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82028.972926
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 03:00:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82029.299972
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:00:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82034.872545
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4118 2014-08-05 03:00:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82036.945625
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4118 2014-08-05 03:00:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82038.872424
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3405 2014-08-05 03:01:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82084.316854
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 03:01:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82087.107673
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3424 2014-08-05 03:01:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82088.471238
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3430 2014-08-05 03:01:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82091.245390
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3397 2014-08-05 03:01:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82094.366948
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 03:01:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82096.856638
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3399 2014-08-05 03:01:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82097.630882
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3408 2014-08-05 03:01:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82100.67556
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3410 2014-08-05 03:01:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82102.672948
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3410 2014-08-05 03:01:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82103.876366
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3347 2014-08-05 03:01:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82104.243444
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3339 2014-08-05 03:01:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82109.278114
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4886 2014-08-05 03:01:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82111.159048
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4829 2014-08-05 03:01:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82113.126646
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82130.177895
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82133.843728
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82134.888790
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82137.534865
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82140.324695
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82142.971102
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82143.500417
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82146.505831
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82148.768794
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82149.681912
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82150.700698
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3315 2014-08-05 03:03:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82155.423697
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 03:03:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82157.714035
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4826 2014-08-05 03:03:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82159.162718
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3408 2014-08-05 03:03:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82167.265271
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3414 2014-08-05 03:03:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82170.799651
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3427 2014-08-05 03:03:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82171.300458
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3433 2014-08-05 03:03:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82174.593132
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 03:03:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82177.618185
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3402 2014-08-05 03:03:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82179.96281
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3402 2014-08-05 03:03:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82180.411420
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-05 03:03:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82183.153584
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3413 2014-08-05 03:03:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82185.502197
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3413 2014-08-05 03:03:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82186.607289
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3350 2014-08-05 03:04:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82187.321815
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3342 2014-08-05 03:04:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82192.293589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 03:04:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82194.845248
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4826 2014-08-05 03:04:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82196.555778
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 03:05:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82211.615339
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3407 2014-08-05 03:05:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82214.149321
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3420 2014-08-05 03:05:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82215.792924
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3426 2014-08-05 03:05:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82218.504966
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-05 03:05:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82221.117275
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:05:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82223.474556
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:05:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82224.734511
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 03:05:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82227.432349
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:05:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82229.736370
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:05:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82230.91792
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 03:05:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82231.208821
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:05:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82236.966839
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 03:05:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82238.729043
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4826 2014-08-05 03:05:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82240.428413
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 03:05:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82245.877019
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3407 2014-08-05 03:05:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82248.329528
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3420 2014-08-05 03:05:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82249.373870
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3426 2014-08-05 03:05:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82252.533695
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-05 03:05:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82255.77783
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:05:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82258.541690
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:05:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82259.805446
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 03:05:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82262.613351
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:05:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82264.466240
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:05:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82265.118118
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 03:05:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82266.757902
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:05:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82271.963330
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 03:05:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82273.415142
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4826 2014-08-05 03:05:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82275.196120
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 03:08:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82349.819414
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3407 2014-08-05 03:08:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82352.584442
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3420 2014-08-05 03:08:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82353.797747
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3426 2014-08-05 03:08:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82356.488877
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-05 03:08:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82359.867147
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82361.966694
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82362.668941
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 03:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82365.975863
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82367.280974
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:08:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82368.714810
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 03:08:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82369.192747
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:08:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82374.32338
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4436 2014-08-05 03:08:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82376.808987
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4436 2014-08-05 03:08:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82378.670885
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 03:09:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82386.42934
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3407 2014-08-05 03:09:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82389.429786
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3420 2014-08-05 03:09:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82390.820060
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3426 2014-08-05 03:09:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82393.137502
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-05 03:09:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82396.48041
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:09:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82398.274833
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:09:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82399.235616
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 03:09:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82402.101842
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:09:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82404.678361
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:09:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82405.866233
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 03:09:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82406.616330
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:09:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82411.864805
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 03:09:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82413.677870
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4826 2014-08-05 03:09:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82415.37781
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3401 2014-08-05 03:09:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82420.871882
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3407 2014-08-05 03:09:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82423.625217
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3420 2014-08-05 03:09:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82424.212817
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3426 2014-08-05 03:09:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82427.821576
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3393 2014-08-05 03:09:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82430.759710
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:09:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82432.591736
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 03:09:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82433.249760
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3404 2014-08-05 03:09:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82436.570526
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:09:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82438.469106
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-05 03:09:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82439.930487
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3343 2014-08-05 03:09:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82440.25148
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3335 2014-08-05 03:09:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82445.681180
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 03:09:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82447.258248
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4826 2014-08-05 03:09:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82449.982121
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3429 2014-08-05 07:46:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82879.488415
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3435 2014-08-05 07:46:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82882.104892
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3448 2014-08-05 07:46:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82883.729161
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3454 2014-08-05 07:46:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82886.129636
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3421 2014-08-05 07:46:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82889.359648
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3423 2014-08-05 07:46:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82891.914163
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3423 2014-08-05 07:46:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82892.208111
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3432 2014-08-05 07:46:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82895.860954
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3434 2014-08-05 07:46:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82897.483920
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3434 2014-08-05 07:46:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82898.945735
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3371 2014-08-05 07:46:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82899.576328
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 07:46:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82904.842176
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4904 2014-08-05 07:46:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82906.634652
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4847 2014-08-05 07:46:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82908.342674
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 07:50:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82923.399881
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-05 07:50:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82926.126556
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3380 2014-08-05 07:50:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82927.576
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-05 07:50:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82930.998942
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-05 07:50:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82933.383048
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 07:50:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82935.943905
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 07:50:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82936.386936
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-05 07:50:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82939.619776
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 07:50:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82941.47493
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 07:50:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82942.167976
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3385 2014-08-05 07:50:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82943.215655
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 07:50:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82948.95641
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4904 2014-08-05 07:50:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82950.152520
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4847 2014-08-05 07:50:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82952.300855
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3455 2014-08-05 07:50:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82960.499220
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3461 2014-08-05 07:50:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82963.255461
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3474 2014-08-05 07:50:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82964.228622
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3480 2014-08-05 07:50:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82967.446398
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3447 2014-08-05 07:50:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82970.708625
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3449 2014-08-05 07:50:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82972.12527
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3449 2014-08-05 07:50:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82973.841330
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 07:50:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82976.102541
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 07:50:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82978.164544
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 07:50:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82979.240305
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3385 2014-08-05 07:50:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82980.546007
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3377 2014-08-05 07:50:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82985.930299
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4904 2014-08-05 07:50:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82987.566959
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4847 2014-08-05 07:50:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82989.534926
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3464 2014-08-05 07:54:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.82999.263047
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3470 2014-08-05 07:54:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83002.390219
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3483 2014-08-05 07:54:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83003.533581
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 07:54:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83006.536128
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 07:54:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83009.385435
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 07:54:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83011.363048
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 07:54:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83012.59739
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 07:54:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83015.596684
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3469 2014-08-05 07:54:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83017.662449
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3469 2014-08-05 07:54:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83018.7612
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3394 2014-08-05 07:54:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83019.457876
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-05 07:54:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83024.982650
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4940 2014-08-05 07:54:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83026.123993
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 07:54:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83028.685956
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3464 2014-08-05 07:54:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83033.629783
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3470 2014-08-05 07:54:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83036.16243
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3483 2014-08-05 07:54:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83037.758879
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 07:54:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83040.875802
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 07:54:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83043.111050
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 07:54:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83045.556259
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 07:54:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83046.445892
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 07:54:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83049.237470
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3469 2014-08-05 07:54:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83051.470874
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3469 2014-08-05 07:54:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83052.771447
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3394 2014-08-05 07:54:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83053.783331
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-05 07:54:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83058.688542
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4940 2014-08-05 07:54:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83060.509307
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 07:54:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83063.262521
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3456 2014-08-05 07:55:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83074.392822
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3462 2014-08-05 07:55:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83077.325474
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 07:55:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83078.597819
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 07:55:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83081.739454
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3448 2014-08-05 07:55:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83084.621062
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3450 2014-08-05 07:55:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83086.770920
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3450 2014-08-05 07:55:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83087.26533
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3459 2014-08-05 07:55:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83090.20106
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3461 2014-08-05 07:55:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83092.318645
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3461 2014-08-05 07:55:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83093.631271
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3386 2014-08-05 07:55:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83094.576328
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3378 2014-08-05 07:55:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83099.337843
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4932 2014-08-05 07:55:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83101.289025
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4875 2014-08-05 07:55:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83103.446020
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3466 2014-08-05 07:58:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83162.76257
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-05 07:58:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83165.389139
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 07:58:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83166.499579
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3491 2014-08-05 07:58:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83169.684437
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 07:58:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83172.364321
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 07:58:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83174.630623
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 07:58:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83175.480130
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3469 2014-08-05 07:58:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83178.449224
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3471 2014-08-05 07:58:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83180.291072
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3471 2014-08-05 07:58:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83181.332191
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3396 2014-08-05 07:58:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83182.370321
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 07:58:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83187.189587
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4940 2014-08-05 07:58:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83189.580918
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 07:58:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83191.122454
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3466 2014-08-05 07:58:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83200.897493
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-05 07:58:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83203.168137
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3485 2014-08-05 07:58:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83204.377730
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3491 2014-08-05 07:58:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83207.909535
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3458 2014-08-05 07:58:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83210.316877
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 07:58:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83212.752062
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3460 2014-08-05 07:58:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83213.565193
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3469 2014-08-05 07:58:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83216.360928
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3471 2014-08-05 07:58:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83218.452780
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3471 2014-08-05 07:58:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83219.761553
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3396 2014-08-05 07:58:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83220.759956
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-05 07:58:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83225.859863
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4940 2014-08-05 07:58:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83227.66629
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4883 2014-08-05 07:58:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83229.776748
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3470 2014-08-05 07:59:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83238.754028
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-05 07:59:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83241.9433
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-05 07:59:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83242.213823
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3495 2014-08-05 07:59:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83245.811685
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3462 2014-08-05 07:59:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83248.19868
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3464 2014-08-05 07:59:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83250.660495
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3464 2014-08-05 07:59:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83251.742320
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 07:59:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83254.180190
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 07:59:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83256.399480
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 07:59:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83257.834299
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3400 2014-08-05 08:00:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83258.166627
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3392 2014-08-05 08:00:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83263.794743
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4945 2014-08-05 08:00:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83265.294474
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4888 2014-08-05 08:00:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.83267.650726
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-05 20:34:00.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85505.997473
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3479 2014-08-05 20:34:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85508.479899
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3492 2014-08-05 20:34:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85509.136619
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3498 2014-08-05 20:34:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85512.489331
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3465 2014-08-05 20:34:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85515.610150
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 20:34:01.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85517.476047
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3467 2014-08-05 20:34:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85518.635672
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-05 20:34:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85521.980721
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3478 2014-08-05 20:34:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85523.44357
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3478 2014-08-05 20:34:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85524.300504
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3403 2014-08-05 20:34:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85525.528381
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3395 2014-08-05 20:34:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85530.315674
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4948 2014-08-05 20:34:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85532.962023
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4891 2014-08-05 20:34:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85535.795507
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85602.52129
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85605.528997
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85606.603162
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85609.543473
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85612.126403
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85614.64773
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85615.413487
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85618.212058
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85620.457834
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85621.107538
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85622.611206
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3354 2014-08-05 20:36:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85627.694655
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4140 2014-08-05 20:36:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85629.930977
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4140 2014-08-05 20:36:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85631.597889
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-05 20:36:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85639.357217
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 20:36:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85642.553464
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3494 2014-08-05 20:36:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85643.414680
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 20:36:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85646.972839
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 20:36:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85649.584462
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 20:36:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85651.679830
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3469 2014-08-05 20:36:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85652.652466
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 20:36:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85655.418920
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 20:36:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85657.676553
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3480 2014-08-05 20:36:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85658.739425
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3405 2014-08-05 20:36:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85659.796849
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3363 2014-08-05 20:36:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85664.197661
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4158 2014-08-05 20:36:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85666.369515
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4158 2014-08-05 20:36:53.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85668.767057
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:40:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85685.24354
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:40:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85688.286895
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:40:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85689.465997
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:40:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85692.71556
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:40:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85695.735673
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:40:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85697.904129
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:40:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85698.915521
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:40:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85701.8533
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:40:07.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85703.553117
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:40:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85704.225489
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:40:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85705.695552
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:40:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85710.565895
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4170 2014-08-05 20:40:08.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85712.162197
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4170 2014-08-05 20:40:09.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85714.325231
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:42:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85722.160948
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:42:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85725.216777
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:42:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85726.927553
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:42:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85729.261432
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:42:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85732.855246
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:42:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85734.984496
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:42:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85735.117041
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:42:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85738.323270
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:42:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85740.639783
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:42:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85741.473085
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:42:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85742.498493
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:42:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85747.508706
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4170 2014-08-05 20:42:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85749.989042
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4170 2014-08-05 20:42:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85751.393776
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:45:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85759.283197
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:45:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85762.511148
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:45:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85763.803426
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85766.193892
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85769.757349
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85771.948267
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85772.745593
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:45:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85775.577421
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85777.124552
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85778.700803
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85779.80230
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:45:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85784.291989
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4170 2014-08-05 20:45:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85786.162278
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4170 2014-08-05 20:45:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85788.504699
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:47:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85800.722731
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:47:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85803.456580
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:47:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85804.63240
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:47:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85807.684638
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:47:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85810.396176
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:47:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85812.965112
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:47:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85813.725197
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:47:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85816.204570
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:47:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85818.126269
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:47:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85819.785993
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:47:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85820.244144
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:47:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85825.60234
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4170 2014-08-05 20:47:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85827.706924
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4170 2014-08-05 20:47:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85829.388651
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:48:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85837.570543
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:10.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85840.168300
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:48:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85841.817425
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85844.246091
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85847.616518
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:11.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85849.666051
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85850.500775
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85853.512458
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85855.602034
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85856.442952
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:48:12.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85857.417187
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85862.578231
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:48:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85864.50496
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:48:13.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85866.968446
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:48:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85873.524453
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85876.700936
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:48:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85877.506329
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85880.633721
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85883.967079
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85885.931352
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85886.961322
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85889.495987
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85891.250647
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85892.97682
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:48:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85893.614096
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:48:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85898.948006
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:48:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85900.811277
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:48:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85902.815564
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:52:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85921.489783
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85924.331235
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:52:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85925.524965
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85928.889747
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85931.152046
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85933.737323
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85934.964525
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85937.417717
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85939.216063
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85940.259431
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:52:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85941.36174
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:52:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85946.825274
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:52:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85948.511391
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:52:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85950.549162
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:54:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85961.539725
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85964.680476
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:54:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85965.372506
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85968.390292
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85971.724297
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85973.712217
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85974.460603
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85977.643888
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85979.423625
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85980.992609
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:54:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85981.850216
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:54:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85986.607856
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:54:32.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85988.625157
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:54:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.85990.998079
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-05 20:56:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86002.132707
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86005.409184
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-05 20:56:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86006.701488
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86009.995768
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86012.383195
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86014.760859
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86015.825616
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86018.217915
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86020.694654
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86021.734735
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-05 20:56:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86022.757323
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-05 20:56:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86027.143648
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:56:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86029.180098
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-05 20:56:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86031.415860
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-06 06:49:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86573.519648
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-06 06:49:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86576.646372
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-06 06:49:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86577.913652
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3508 2014-08-06 06:49:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86580.937361
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-06 06:49:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86583.508648
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-06 06:49:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86585.267872
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-06 06:49:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86586.867303
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3486 2014-08-06 06:49:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86589.670621
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3486 2014-08-06 06:49:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86591.832581
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3486 2014-08-06 06:49:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86592.925099
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-06 06:49:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86593.491560
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-06 06:49:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86598.989327
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4956 2014-08-06 06:49:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86600.797620
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4899 2014-08-06 06:49:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86602.227364
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3481 2014-08-06 07:03:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86648.485228
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3489 2014-08-06 07:03:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86651.839932
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3500 2014-08-06 07:03:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86652.269795
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3508 2014-08-06 07:03:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86655.693427
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-06 07:03:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86658.718305
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-06 07:03:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86660.62228
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3475 2014-08-06 07:03:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86661.918767
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3486 2014-08-06 07:03:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86664.89444
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3486 2014-08-06 07:03:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86666.378970
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3486 2014-08-06 07:03:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86667.714386
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3369 2014-08-06 07:03:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86668.602550
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-06 07:03:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86673.449969
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4956 2014-08-06 07:03:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86675.889595
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4899 2014-08-06 07:03:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86677.280452
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:17:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86923.392915
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3506 2014-08-06 07:17:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86926.667456
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:17:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86927.772573
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3525 2014-08-06 07:17:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86930.724648
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3492 2014-08-06 07:17:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86933.860766
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3492 2014-08-06 07:17:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86935.752617
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3492 2014-08-06 07:17:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86936.498640
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3503 2014-08-06 07:17:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86939.198662
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3503 2014-08-06 07:17:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86941.989036
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3503 2014-08-06 07:17:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86942.684793
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3384 2014-08-06 07:17:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86943.730401
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:17:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86948.175495
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4973 2014-08-06 07:17:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86950.672617
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4916 2014-08-06 07:17:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86952.524745
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:18:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86962.447534
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:18:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86965.995928
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:18:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86966.396142
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:18:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86969.787589
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:18:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86972.366138
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:18:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86974.560366
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:18:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86975.732166
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:18:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86978.902322
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:18:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86980.416431
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:18:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86981.246845
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3384 2014-08-06 07:18:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86982.754648
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:18:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86987.16563
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:18:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86989.611120
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:18:59.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.86991.381570
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:19:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87001.358967
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:19:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87004.404069
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:19:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87005.24122
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:19:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87008.471005
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:19:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87011.198668
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:19:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87013.560657
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:19:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87014.213403
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:19:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87017.815978
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:19:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87019.965412
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:19:41.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87020.758503
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3384 2014-08-06 07:19:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87021.846292
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:19:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87026.930836
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:19:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87028.118642
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:19:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87030.917730
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:20:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87037.646263
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87040.742860
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3388 2014-08-06 07:20:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87041.373624
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87044.251913
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87047.896189
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87049.848883
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:20:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87050.914389
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:29.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87053.793526
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87055.101435
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:20:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87056.315415
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3384 2014-08-06 07:20:30.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87057.639265
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87062.210320
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:20:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87064.427440
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:20:31.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87066.323812
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3410 2014-08-06 07:20:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87075.69027
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87078.135872
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3410 2014-08-06 07:20:54.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87079.241595
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87082.462333
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87085.473387
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:55.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87087.425706
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:20:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87088.336204
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87091.276722
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:56.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87093.912054
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:20:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87094.429276
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3384 2014-08-06 07:20:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87095.612955
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:20:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87100.169515
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:20:57.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87102.930768
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:20:58.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87104.646395
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3410 2014-08-06 07:21:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87113.862965
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:21:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87116.299254
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3410 2014-08-06 07:21:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87117.139391
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:21:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87120.141534
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:21:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87123.379586
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:21:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87125.900872
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:21:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87126.637111
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:21:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87129.874789
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:21:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87131.607613
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:21:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87132.485955
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3384 2014-08-06 07:21:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87133.746093
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:21:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87138.600049
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:21:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87140.186671
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:21:52.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87142.628812
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3410 2014-08-06 07:22:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87149.715498
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:22:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87152.846760
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3410 2014-08-06 07:22:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87153.870417
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:22:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87156.866511
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:22:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87159.207025
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:22:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87161.263530
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:22:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87162.687021
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:22:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87165.546480
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:22:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87167.424969
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3412 2014-08-06 07:22:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87168.90662
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3384 2014-08-06 07:22:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87169.288350
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3406 2014-08-06 07:22:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87174.805803
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:22:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87176.237575
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4196 2014-08-06 07:22:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87178.474813
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3484 2014-08-06 07:23:33.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87207.126963
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:23:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87210.608103
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3503 2014-08-06 07:23:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87211.601812
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:23:34.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87214.181155
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:23:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87217.225398
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:23:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87219.535872
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-06 07:23:35.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87220.108620
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:23:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87223.575364
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:23:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87225.313758
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3483 2014-08-06 07:23:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87226.14399
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3383 2014-08-06 07:23:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87227.790732
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:23:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87232.163649
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-06 07:23:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87234.275118
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-06 07:23:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87236.42871
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3484 2014-08-06 07:24:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87248.131520
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:24:24.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87251.88050
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3503 2014-08-06 07:24:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87252.371653
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:24:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87255.65079
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:24:25.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87258.761414
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:24:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87260.617392
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-06 07:24:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87261.635279
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:24:26.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87264.665275
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:24:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87266.665162
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3483 2014-08-06 07:24:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87267.540063
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3383 2014-08-06 07:24:27.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87268.461612
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:24:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87273.20926
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-06 07:24:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87275.580822
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4195 2014-08-06 07:24:28.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87277.715072
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3484 2014-08-06 07:25:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87284.1188
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:25:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87287.5386
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3503 2014-08-06 07:25:02.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87288.451620
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:25:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87291.242095
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:25:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87294.650716
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:25:03.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87296.297873
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-06 07:25:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87297.357640
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:25:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87300.489083
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:25:04.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87302.96375
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3483 2014-08-06 07:25:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87303.274697
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3383 2014-08-06 07:25:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87304.971102
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:25:05.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87309.191161
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4671 2014-08-06 07:25:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87311.31988
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4671 2014-08-06 07:25:06.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87313.867529
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3484 2014-08-06 07:26:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87322.674843
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-06 07:26:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87325.308536
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3506 2014-08-06 07:26:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87326.516354
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-06 07:26:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87329.812317
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-06 07:26:20.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87332.475390
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-06 07:26:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87334.226569
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-06 07:26:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87335.330581
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-06 07:26:21.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87338.704995
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-06 07:26:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87340.488965
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3486 2014-08-06 07:26:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87341.776864
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3383 2014-08-06 07:26:22.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87342.846885
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3476 2014-08-06 07:26:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87347.110954
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4671 2014-08-06 07:26:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87349.722401
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4671 2014-08-06 07:26:23.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87351.628690
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3484 2014-08-06 07:26:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87359.850870
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:26:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87362.635225
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3503 2014-08-06 07:26:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87363.149826
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:26:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87366.591505
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:26:48.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87369.898400
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:26:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87371.513680
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-06 07:26:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87372.800649
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:26:49.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87375.561291
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:26:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87377.628022
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3483 2014-08-06 07:26:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87378.498062
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3383 2014-08-06 07:26:50.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87379.466287
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:26:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87384.680055
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4671 2014-08-06 07:26:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87386.515295
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4671 2014-08-06 07:26:51.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87388.809405
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3484 2014-08-06 07:27:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87397.18221
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:27:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87400.988415
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3503 2014-08-06 07:27:36.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87401.620303
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:27:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87404.88671
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:27:37.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87407.596387
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:27:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87409.418052
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3472 2014-08-06 07:27:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87410.528449
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:27:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87413.22222
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:27:38.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87415.670112
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3483 2014-08-06 07:27:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87416.789084
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3383 2014-08-06 07:27:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87417.379473
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3473 2014-08-06 07:27:39.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87422.280115
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4671 2014-08-06 07:27:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87424.948402
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4671 2014-08-06 07:27:40.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87426.997550
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-06 07:54:15.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87880.761129
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3519 2014-08-06 07:54:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87883.704245
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3411 2014-08-06 07:54:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87884.929377
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3538 2014-08-06 07:54:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87887.816193
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3505 2014-08-06 07:54:16.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87890.86308
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3505 2014-08-06 07:54:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87892.79382
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3505 2014-08-06 07:54:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87893.585446
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3516 2014-08-06 07:54:17.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87896.646428
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3516 2014-08-06 07:54:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87898.87972
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3516 2014-08-06 07:54:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87899.493493
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3403 2014-08-06 07:54:18.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87900.361887
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3407 2014-08-06 07:54:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87905.743335
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4976 2014-08-06 07:54:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87907.135220
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4919 2014-08-06 07:54:19.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87909.46399
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3413 2014-08-06 07:56:42.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87920.58239
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3521 2014-08-06 07:56:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87923.880896
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3413 2014-08-06 07:56:43.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87924.470678
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3540 2014-08-06 07:56:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87927.719300
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3507 2014-08-06 07:56:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87930.280258
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3507 2014-08-06 07:56:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87932.465332
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3507 2014-08-06 07:56:44.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87933.567050
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3518 2014-08-06 07:56:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87936.875242
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3518 2014-08-06 07:56:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87938.398790
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3518 2014-08-06 07:56:45.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87939.763685
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3403 2014-08-06 07:56:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87940.273967
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3409 2014-08-06 07:56:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87945.687483
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4978 2014-08-06 07:56:46.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87947.186541
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4921 2014-08-06 07:56:47.000000 json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.87949.428452
+-rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)      651 2014-07-23 13:23:03.000000 json-spec-0.9.9/tests/__init__.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      177 2014-06-13 07:51:45.000000 json-spec-0.9.9/tests/conftest.py
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/fixtures/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      129 2014-06-03 18:13:12.000000 json-spec-0.9.9/tests/fixtures/first.data1.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      276 2014-06-03 18:13:34.000000 json-spec-0.9.9/tests/fixtures/first.data2.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      720 2014-06-03 18:07:17.000000 json-spec-0.9.9/tests/fixtures/first.schema.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1354 2014-06-11 09:17:02.000000 json-spec-0.9.9/tests/fixtures/five.schema.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      402 2014-06-03 18:18:54.000000 json-spec-0.9.9/tests/fixtures/four.base.schema.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      660 2014-06-03 18:17:56.000000 json-spec-0.9.9/tests/fixtures/four.data.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3583 2014-06-11 16:43:11.000000 json-spec-0.9.9/tests/fixtures/four.entry.schema.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      272 2014-06-03 18:15:19.000000 json-spec-0.9.9/tests/fixtures/second.data1.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      788 2014-06-03 18:14:36.000000 json-spec-0.9.9/tests/fixtures/second.schema.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      145 2014-06-03 18:16:50.000000 json-spec-0.9.9/tests/fixtures/three.data1.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      173 2014-06-03 18:17:15.000000 json-spec-0.9.9/tests/fixtures/three.data2.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1270 2014-06-03 18:16:09.000000 json-spec-0.9.9/tests/fixtures/three.schema.json
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/suite/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       39 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/.git
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)        5 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/.gitignore
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       98 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/.travis.yml
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/suite/bin/
+-rwxr-xr-x   0 xavierbarbosa   (501) staff       (20)     9059 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/bin/jsonschema_suite
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1057 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/LICENSE
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3612 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/README.md
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/suite/remotes/
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/suite/remotes/folder/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       25 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/remotes/folder/folderInteger.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)       25 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/remotes/integer.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      110 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/remotes/subSchemas.json
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:53.000000 json-spec-0.9.9/tests/suite/tests/
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/suite/tests/draft3/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2257 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/additionalItems.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2194 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/additionalProperties.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2989 2014-07-17 16:15:08.000000 json-spec-0.9.9/tests/suite/tests/draft3/dependencies.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1936 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/disallow.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1544 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/divisibleBy.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1964 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/enum.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2591 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/extends.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1136 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/items.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1063 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/maximum.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      706 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/maxItems.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      895 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/maxLength.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1063 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/minimum.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      693 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/minItems.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      886 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/minLength.json
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/suite/tests/draft3/optional/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1663 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/optional/bignum.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     6577 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/optional/format.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      463 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/optional/jsregex.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      384 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/optional/zeroTerminatedFloats.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      582 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/pattern.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/patternProperties.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2881 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/properties.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3922 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/ref.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1961 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/refRemote.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1282 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/required.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)    13225 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/type.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2613 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft3/uniqueItems.json
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/suite/tests/draft4/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2282 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/additionalItems.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2194 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/additionalProperties.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3025 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/allOf.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1608 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/anyOf.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      854 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/definitions.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3139 2014-07-16 10:16:27.000000 json-spec-0.9.9/tests/suite/tests/draft4/dependencies.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1975 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/enum.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1136 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/items.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1063 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/maximum.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      706 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/maxItems.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      896 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/maxLength.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      759 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/maxProperties.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1063 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/minimum.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      693 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/minItems.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      886 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/minLength.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      725 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/minProperties.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1525 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/multipleOf.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2266 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/not.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1607 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/oneOf.json
+drwxr-xr-x   0 xavierbarbosa   (501) staff       (20)        0 2014-08-13 14:01:55.000000 json-spec-0.9.9/tests/suite/tests/draft4/optional/
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1663 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/optional/bignum.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4434 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/optional/format.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      384 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/optional/zeroTerminatedFloats.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      582 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/pattern.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3365 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/patternProperties.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2881 2014-07-16 09:33:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/properties.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     3903 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/ref.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1961 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/refRemote.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      923 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/required.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     9306 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/type.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2613 2014-07-16 07:17:37.000000 json-spec-0.9.9/tests/suite/tests/draft4/uniqueItems.json
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     4545 2014-08-13 13:55:23.000000 json-spec-0.9.9/tests/test_commands.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2075 2014-07-23 08:45:50.000000 json-spec-0.9.9/tests/test_draft03.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1969 2014-07-18 07:28:07.000000 json-spec-0.9.9/tests/test_draft04.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      949 2014-06-11 16:43:11.000000 json-spec-0.9.9/tests/test_errors.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     2688 2014-07-24 12:47:00.000000 json-spec-0.9.9/tests/test_errors2.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5047 2014-07-23 08:34:25.000000 json-spec-0.9.9/tests/test_operations.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     5220 2014-07-16 07:02:29.000000 json-spec-0.9.9/tests/test_pointer.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      977 2014-07-16 10:52:54.000000 json-spec-0.9.9/tests/test_provider.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1726 2014-06-11 16:43:12.000000 json-spec-0.9.9/tests/test_reference.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)     1814 2014-06-12 06:54:29.000000 json-spec-0.9.9/tests/test_util.py
+-rw-r--r--   0 xavierbarbosa   (501) staff       (20)      640 2014-07-28 21:29:31.000000 json-spec-0.9.9/tox.ini
```

### Comparing `json-spec-0.9.8/ChangeLog` & `json-spec-0.9.9/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+0.9.9
+-----
+
+* added cli operations
+* remove version on doc
+* fix the doc
+* fix uninstall
+* fix doc
+
 0.9.8
 -----
 
 * better cli error formating
 * 0.9.7
 
 0.9.7
```

### Comparing `json-spec-0.9.8/CONTRIBUTING.rst` & `json-spec-0.9.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/docs/conf.py` & `json-spec-0.9.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #sys.path.insert(0, os.path.abspath('.'))
 
 # Get the project root dir, which is the parent dir of this
-cwd = os.getcwd()
-project_root = os.path.dirname(cwd)
+project_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 # Insert the project root dir as the first element in the PYTHONPATH.
 # This lets us ensure that the source package is imported, and that its
 # version is used.
 sys.path.insert(0, os.path.join(project_root, 'src', 'jsonspec'))
+sys.path.insert(0, os.path.join(project_root, 'src'))
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -58,16 +58,16 @@
 copyright = u'2014, Xavier Barbosa'
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
-version = '0.9.7'
-release = '0.9.7'
+version = ''
+release = ''
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
```

### Comparing `json-spec-0.9.8/docs/index.rst` & `json-spec-0.9.9/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 This library implements tools inspired by several cleaver specifications around JSON.
 
 **Features:**
 
 :jsonspec.cli:
 
-    Expose `JSON Pointer`_ and `JSON Schema`_ to your console:
+    Expose `JSON Pointer`_ , `JSON Schema`_ and `JSON Patch`_ to your console:
 
     .. code-block:: bash
 
-        json-extract '#/foo/1' --document-json='{"foo": ["bar", "baz"]}'
-        json-validate --schema-file=schema.json < doc.json
+        json extract '#/foo/1' --document-json='{"foo": ["bar", "baz"]}'
+        json validate --schema-file=schema.json < doc.json
+        cat doc.json | json add '#/foo/1' --fragment='{"foo": ["bar", "baz"]}'
 
 :jsonspec.pointer:
 
     Implements `JSON Pointer`_ and `Relative JSON Pointer`_, it offers a way to target a subelement.
 
 :jsonspec.reference:
```

### Comparing `json-spec-0.9.8/docs/make.bat` & `json-spec-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/docs/Makefile` & `json-spec-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/docs/operations.rst` & `json-spec-0.9.9/docs/operations.rst`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/docs/pointer.rst` & `json-spec-0.9.9/docs/pointer.rst`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/docs/reference.rst` & `json-spec-0.9.9/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/docs/validators.rst` & `json-spec-0.9.9/docs/validators.rst`

 * *Files 2% similar despite different names*

```diff
@@ -121,30 +121,30 @@
       - pip install json-spec[ip]
     * - regex
       - validate regex
       - 
     * - uri
       - validate uri
       - 
-    * - css:color
+    * - css.color
       - validate css color
       - 
-    * - rfc3339:datetime
+    * - rfc3339.datetime
       - see rfc3339_
       - 
-    * - utc:datetime
+    * - utc.datetime
       - YYYY-MM-ddThh:mm:SSZ
       - 
-    * - utc:date
+    * - utc.date
       - YYYY-MM-dd
       - 
-    * - utc:time
+    * - utc.time
       - hh:mm:SS
       - 
-    * - utc:millisec
+    * - utc.millisec
       - any integer, float
       - 
 
 
 Some formats rely on external modules, and they are not enabled by default.
 
 Each draft validator aliases they formats to these formats. See :meth:`draft04 <validators.Draft04Validator.validate_format>` and :meth:`draft03 <validators.Draft03Validator.validate_format>` methods for more details.
@@ -184,16 +184,14 @@
 .. autoclass:: validators.Factory
     :members:
 
 
 Exceptions
 ----------
 
-.. autofunction:: validators.error
-
 .. autoclass:: validators.CompilationError
     :members:
 
 .. autoclass:: validators.ReferenceError
     :members:
 
 .. autoclass:: validators.ValidationError
```

### Comparing `json-spec-0.9.8/examples/simple.json` & `json-spec-0.9.9/examples/simple.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/examples/test.py` & `json-spec-0.9.9/examples/test.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/LICENSE` & `json-spec-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/PKG-INFO` & `json-spec-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: json-spec
-Version: 0.9.8
+Version: 0.9.9
 Summary: Implements JSON Schema, JSON Pointer and JSON Reference.
 Home-page: http://github.com/johnnoone/json-spec
 Author: Xavier Barbosa
 Author-email: clint.northwood@gmail.com
 License: BSD
 Description: Json Spec
         =========
@@ -42,30 +42,30 @@
         
         ...
         
         
         CLI Usage
         ---------
         
-        This module expose 2 cli commands.
+        This module expose cli commands like:
         
         
         **json-extract** will extract parts of your json document::
         
-            $ json-extract '#/foo/1' --document-json='{"foo": ["bar", "baz"]}'
-            $ echo '{"foo": ["bar", "baz"]}' | json-extract '#/foo/1'
-            $ json-extract '#/foo/1' --document-file=doc.json
-            $ json-extract '#/foo/1' < doc.json
+            $ json extract '#/foo/1' --document-json='{"foo": ["bar", "baz"]}'
+            $ echo '{"foo": ["bar", "baz"]}' | json extract '#/foo/1'
+            $ json extract '#/foo/1' --document-file=doc.json
+            $ json extract '#/foo/1' < doc.json
         
         **json-validate** will validate your document against a schema::
         
-            $ json-validate --schema-file=schema.json --document-json='{"foo": ["bar", "baz"]}'
-            $ echo '{"foo": ["bar", "baz"]}' | json-validate --schema-file=schema.json
-            $ json-validate --schema-file=schema.json --document-file=doc.json
-            $ json-validate --schema-file=schema.json < doc.json
+            $ json validate --schema-file=schema.json --document-json='{"foo": ["bar", "baz"]}'
+            $ echo '{"foo": ["bar", "baz"]}' | json validate --schema-file=schema.json
+            $ json validate --schema-file=schema.json --document-file=doc.json
+            $ json validate --schema-file=schema.json < doc.json
         
         
         Library usage
         -------------
         
         Let say you want to fetch / validate JSON like objects in you python scripts.
```

### Comparing `json-spec-0.9.8/README.rst` & `json-spec-0.9.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,30 @@
 
 ...
 
 
 CLI Usage
 ---------
 
-This module expose 2 cli commands.
+This module expose cli commands like:
 
 
 **json-extract** will extract parts of your json document::
 
-    $ json-extract '#/foo/1' --document-json='{"foo": ["bar", "baz"]}'
-    $ echo '{"foo": ["bar", "baz"]}' | json-extract '#/foo/1'
-    $ json-extract '#/foo/1' --document-file=doc.json
-    $ json-extract '#/foo/1' < doc.json
+    $ json extract '#/foo/1' --document-json='{"foo": ["bar", "baz"]}'
+    $ echo '{"foo": ["bar", "baz"]}' | json extract '#/foo/1'
+    $ json extract '#/foo/1' --document-file=doc.json
+    $ json extract '#/foo/1' < doc.json
 
 **json-validate** will validate your document against a schema::
 
-    $ json-validate --schema-file=schema.json --document-json='{"foo": ["bar", "baz"]}'
-    $ echo '{"foo": ["bar", "baz"]}' | json-validate --schema-file=schema.json
-    $ json-validate --schema-file=schema.json --document-file=doc.json
-    $ json-validate --schema-file=schema.json < doc.json
+    $ json validate --schema-file=schema.json --document-json='{"foo": ["bar", "baz"]}'
+    $ echo '{"foo": ["bar", "baz"]}' | json validate --schema-file=schema.json
+    $ json validate --schema-file=schema.json --document-file=doc.json
+    $ json validate --schema-file=schema.json < doc.json
 
 
 Library usage
 -------------
 
 Let say you want to fetch / validate JSON like objects in you python scripts.
```

### Comparing `json-spec-0.9.8/setup.cfg` & `json-spec-0.9.9/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -27,31 +27,39 @@
 
 [global]
 setup-hooks = 
 	pbr.hooks.setup_hook
 
 [entry_points]
 console_scripts = 
-	json-validate = jsonspec.cli:validate_cmd
-	json-extract = jsonspec.cli:extract_cmd
+	json = jsonspec.cli:main
+jsonspec.cli.commands = 
+	validate = jsonspec.cli:ValidateCommand
+	extract = jsonspec.cli:ExtractCommand
+	add = jsonspec.cli:AddCommand
+	remove = jsonspec.cli:RemoveCommand
+	replace = jsonspec.cli:ReplaceCommand
+	move = jsonspec.cli:MoveCommand
+	copy = jsonspec.cli:CopyCommand
+	check = jsonspec.cli:CheckCommand
 jsonspec.reference.contributions = 
 	spec = jsonspec.reference.providers:SpecProvider
 jsonspec.validators.formats = 
 	email = jsonspec.validators.util:validate_email
 	hostname = jsonspec.validators.util:validate_hostname
 	ipv4 = jsonspec.validators.util:validate_ipv4 [ip]
 	ipv6 = jsonspec.validators.util:validate_ipv6 [ip]
 	regex = jsonspec.validators.util:validate_regex
 	uri = jsonspec.validators.util:validate_uri
-	css:color = jsonspec.validators.util:validate_css_color
-	rfc3339:datetime = jsonspec.validators.util:validate_rfc3339_datetime
-	utc:datetime = jsonspec.validators.util:validate_utc_datetime
-	utc:date = jsonspec.validators.util:validate_utc_date
-	utc:time = jsonspec.validators.util:validate_utc_time
-	utc:millisec = jsonspec.validators.util:validate_utc_millisec
+	css.color = jsonspec.validators.util:validate_css_color
+	rfc3339.datetime = jsonspec.validators.util:validate_rfc3339_datetime
+	utc.datetime = jsonspec.validators.util:validate_utc_datetime
+	utc.date = jsonspec.validators.util:validate_utc_date
+	utc.time = jsonspec.validators.util:validate_utc_time
+	utc.millisec = jsonspec.validators.util:validate_utc_millisec
 
 [files]
 packages_root = src
 packages = 
 	jsonspec
 	jsonspec.operations
 	jsonspec.pointer
@@ -67,10 +75,10 @@
 [bdist_wheel]
 universal = 1
 
 [pytest]
 
 [egg_info]
 tag_svn_revision = 0
-tag_build = 
 tag_date = 0
+tag_build =
```

### Comparing `json-spec-0.9.8/src/json_spec.egg-info/entry_points.txt` & `json-spec-0.9.9/src/json_spec.egg-info/entry_points.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 [console_scripts]
-json-extract = jsonspec.cli:extract_cmd
-json-validate = jsonspec.cli:validate_cmd
+json = jsonspec.cli:main
+
+[jsonspec.cli.commands]
+add = jsonspec.cli:AddCommand
+check = jsonspec.cli:CheckCommand
+copy = jsonspec.cli:CopyCommand
+extract = jsonspec.cli:ExtractCommand
+move = jsonspec.cli:MoveCommand
+remove = jsonspec.cli:RemoveCommand
+replace = jsonspec.cli:ReplaceCommand
+validate = jsonspec.cli:ValidateCommand
 
 [jsonspec.reference.contributions]
 spec = jsonspec.reference.providers:SpecProvider
 
 [jsonspec.validators.formats]
-css:color = jsonspec.validators.util:validate_css_color
+css.color = jsonspec.validators.util:validate_css_color
 email = jsonspec.validators.util:validate_email
 hostname = jsonspec.validators.util:validate_hostname
 ipv4 = jsonspec.validators.util:validate_ipv4 [ip]
 ipv6 = jsonspec.validators.util:validate_ipv6 [ip]
 regex = jsonspec.validators.util:validate_regex
-rfc3339:datetime = jsonspec.validators.util:validate_rfc3339_datetime
+rfc3339.datetime = jsonspec.validators.util:validate_rfc3339_datetime
 uri = jsonspec.validators.util:validate_uri
-utc:date = jsonspec.validators.util:validate_utc_date
-utc:datetime = jsonspec.validators.util:validate_utc_datetime
-utc:millisec = jsonspec.validators.util:validate_utc_millisec
-utc:time = jsonspec.validators.util:validate_utc_time
+utc.date = jsonspec.validators.util:validate_utc_date
+utc.datetime = jsonspec.validators.util:validate_utc_datetime
+utc.millisec = jsonspec.validators.util:validate_utc_millisec
+utc.time = jsonspec.validators.util:validate_utc_time
```

### Comparing `json-spec-0.9.8/src/json_spec.egg-info/PKG-INFO` & `json-spec-0.9.9/src/json_spec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: json-spec
-Version: 0.9.8
+Version: 0.9.9
 Summary: Implements JSON Schema, JSON Pointer and JSON Reference.
 Home-page: http://github.com/johnnoone/json-spec
 Author: Xavier Barbosa
 Author-email: clint.northwood@gmail.com
 License: BSD
 Description: Json Spec
         =========
@@ -42,30 +42,30 @@
         
         ...
         
         
         CLI Usage
         ---------
         
-        This module expose 2 cli commands.
+        This module expose cli commands like:
         
         
         **json-extract** will extract parts of your json document::
         
-            $ json-extract '#/foo/1' --document-json='{"foo": ["bar", "baz"]}'
-            $ echo '{"foo": ["bar", "baz"]}' | json-extract '#/foo/1'
-            $ json-extract '#/foo/1' --document-file=doc.json
-            $ json-extract '#/foo/1' < doc.json
+            $ json extract '#/foo/1' --document-json='{"foo": ["bar", "baz"]}'
+            $ echo '{"foo": ["bar", "baz"]}' | json extract '#/foo/1'
+            $ json extract '#/foo/1' --document-file=doc.json
+            $ json extract '#/foo/1' < doc.json
         
         **json-validate** will validate your document against a schema::
         
-            $ json-validate --schema-file=schema.json --document-json='{"foo": ["bar", "baz"]}'
-            $ echo '{"foo": ["bar", "baz"]}' | json-validate --schema-file=schema.json
-            $ json-validate --schema-file=schema.json --document-file=doc.json
-            $ json-validate --schema-file=schema.json < doc.json
+            $ json validate --schema-file=schema.json --document-json='{"foo": ["bar", "baz"]}'
+            $ echo '{"foo": ["bar", "baz"]}' | json validate --schema-file=schema.json
+            $ json validate --schema-file=schema.json --document-file=doc.json
+            $ json validate --schema-file=schema.json < doc.json
         
         
         Library usage
         -------------
         
         Let say you want to fetch / validate JSON like objects in you python scripts.
```

### Comparing `json-spec-0.9.8/src/json_spec.egg-info/PKG-INFO 2` & `json-spec-0.9.9/src/json_spec.egg-info/PKG-INFO 2`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/driver.py` & `json-spec-0.9.9/src/jsonspec/driver.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/misc/schemas/address.json` & `json-spec-0.9.9/src/jsonspec/misc/schemas/address.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/misc/schemas/calendar.json` & `json-spec-0.9.9/src/jsonspec/misc/schemas/calendar.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/card.json` & `json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/card.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/hyper-schema.json` & `json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/misc/schemas/draft-03/schema.json` & `json-spec-0.9.9/src/jsonspec/misc/schemas/draft-03/schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/misc/schemas/draft-04/hyper-schema.json` & `json-spec-0.9.9/src/jsonspec/misc/schemas/draft-04/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/misc/schemas/draft-04/schema.json` & `json-spec-0.9.9/src/jsonspec/misc/schemas/draft-04/schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/operations/__init__.py` & `json-spec-0.9.9/src/jsonspec/operations/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
     jsonspec.operations
     ~~~~~~~~~~~~~~~~~~~
 """
 
+from __future__ import absolute_import
+
 __all__ = ['check', 'remove', 'add', 'replace', 'move', 'copy',
            'Error', 'NonexistentTarget', 'Target']
 
 from .exceptions import Error, NonexistentTarget
 from .bases import Target
```

### Comparing `json-spec-0.9.8/src/jsonspec/operations/bases.py` & `json-spec-0.9.9/src/jsonspec/operations/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
     jsonspec.operations.bases
     ~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 
+from __future__ import absolute_import
+
 __all__ = ['Target']
 
 from copy import deepcopy
 import logging
 from jsonspec.pointer import Pointer
 from jsonspec.pointer import ExtractError, OutOfBounds, OutOfRange, LastElement
 from .exceptions import Error, NonexistentTarget
```

### Comparing `json-spec-0.9.8/src/jsonspec/pointer/__init__.py` & `json-spec-0.9.9/src/jsonspec/pointer/__init__.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/pointer/bases.py` & `json-spec-0.9.9/src/jsonspec/pointer/bases.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/pointer/exceptions.py` & `json-spec-0.9.9/src/jsonspec/pointer/exceptions.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/pointer/stages.py` & `json-spec-0.9.9/src/jsonspec/pointer/stages.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/reference/__init__.py` & `json-spec-0.9.9/src/jsonspec/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/reference/bases.py` & `json-spec-0.9.9/src/jsonspec/reference/bases.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/reference/providers.py` & `json-spec-0.9.9/src/jsonspec/reference/providers.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/reference/util.py` & `json-spec-0.9.9/src/jsonspec/reference/util.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/validators/__init__.py` & `json-spec-0.9.9/src/jsonspec/validators/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
     ~~~~~~~~~~~~~~~~~~~
 
 """
 
 __all__ = ['load', 'register', 'Factory', 'Context',
            'Validator', 'ReferenceValidator',
            'Draft03Validator', 'Draft04Validator',
-           'error', 'CompilationError', 'ReferenceError', 'ValidationError']
+           'CompilationError', 'ReferenceError', 'ValidationError']
 
 from .bases import Validator, ReferenceValidator
-from .exceptions import error, CompilationError, ReferenceError, ValidationError  # noqa
+from .exceptions import CompilationError, ReferenceError, ValidationError
 from .factorize import register, Factory, Context
 from . import draft04  # noqa
 from . import draft03  # noqa
 from .draft03 import Draft03Validator  # noqa
 from .draft04 import Draft04Validator  # noqa
```

### Comparing `json-spec-0.9.8/src/jsonspec/validators/bases.py` & `json-spec-0.9.9/src/jsonspec/validators/bases.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
     jsonspec.validators.bases
     ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 """
 
-__all__ = ['error', 'ValidationError', 'Validator', 'ReferenceValidator']
+from __future__ import absolute_import
+
+__all__ = ['ValidationError', 'Validator', 'ReferenceValidator']
 
 import logging
 from abc import abstractmethod, ABCMeta
 from six import add_metaclass
 from jsonspec.pointer import DocumentPointer
-from .exceptions import error, ValidationError
+from .exceptions import ValidationError
 
 
 logger = logging.getLogger(__name__)
 
 
 @add_metaclass(ABCMeta)
 class Validator(object):
```

### Comparing `json-spec-0.9.8/src/jsonspec/validators/draft03.py` & `json-spec-0.9.9/src/jsonspec/validators/draft03.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
     jsonspec.validators.draft03
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Implements JSON Schema draft03.
 """
 
+from __future__ import absolute_import
+
 __all__ = ['compile', 'Draft03Validator']
 
 import logging
 import os.path
 import re
 from copy import deepcopy
 from decimal import Decimal
@@ -421,40 +423,40 @@
         return obj
 
     def validate_format(self, obj, pointer=None):
         """
         ================= ============
         Expected draft03  Alias of
         ----------------- ------------
-        color             css:color
-        date-time         utc:datetime
-        date              utc:date
-        time              utc:time
-        utc-millisec      utc:millisec
+        color             css.color
+        date-time         utc.datetime
+        date              utc.date
+        time              utc.time
+        utc-millisec      utc.millisec
         regex             regex
-        style             css:style
+        style             css.style
         phone             phone
         uri               uri
         email             email
         ip-address        ipv4
         ipv6              ipv6
         host-name         hostname
         ================= ============
 
         """
 
         if 'format' in self.attrs:
             substituted = {
-                'color': 'css:color',
-                'date-time': 'utc:datetime',
-                'date': 'utc:date',
-                'time': 'utc:time',
-                'utc-millisec': 'utc:millisec',
+                'color': 'css.color',
+                'date-time': 'utc.datetime',
+                'date': 'utc.date',
+                'time': 'utc.time',
+                'utc-millisec': 'utc.millisec',
                 'regex': 'regex',
-                'style': 'css:style',
+                'style': 'css.style',
                 'phone': 'phone',
                 'uri': 'uri',
                 'email': 'email',
                 'ip-address': 'ipv4',
                 'ipv6': 'ipv6',
                 'host-name': 'hostname',
             }.get(self.attrs['format'], self.attrs['format'])
```

### Comparing `json-spec-0.9.8/src/jsonspec/validators/draft04.py` & `json-spec-0.9.9/src/jsonspec/validators/draft04.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
     jsonspec.validators.draft04
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Implements JSON Schema draft04.
 """
 
+from __future__ import absolute_import
+
 __all__ = ['compile', 'Draft04Validator']
 
 import logging
 import os.path
 import re
 from copy import deepcopy
 from decimal import Decimal
@@ -392,26 +394,26 @@
         return obj
 
     def validate_format(self, obj, pointer=None):
         """
         ================= ============
         Expected draft04  Alias of
         ----------------- ------------
-        date-time         rfc3339:datetime
+        date-time         rfc3339.datetime
         email             email
         hostname          hostname
         ipv4              ipv4
         ipv6              ipv6
         uri               uri
         ================= ============
 
         """
         if 'format' in self.attrs:
             substituted = {
-                'date-time': 'rfc3339:datetime',
+                'date-time': 'rfc3339.datetime',
                 'email': 'email',
                 'hostname': 'hostname',
                 'ipv4': 'ipv4',
                 'ipv6': 'ipv6',
                 'uri': 'uri',
             }.get(self.attrs['format'], self.attrs['format'])
             logger.debug('use %s', substituted)
```

### Comparing `json-spec-0.9.8/src/jsonspec/validators/exceptions.py` & `json-spec-0.9.9/src/jsonspec/validators/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,18 @@
+"""
+    jsonspec.validators.exceptions
+    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-__all__ = ['error', 'CompilationError', 'ReferenceError', 'ValidationError']
+"""
 
-from collections import defaultdict
-from six import wraps
+from __future__ import absolute_import
 
+__all__ = ['CompilationError', 'ReferenceError', 'ValidationError']
 
-def error(meth):
-    @wraps(meth)
-    def wrapper(self, obj, *args, **kwargs):
-        try:
-            return meth(self, obj, *args, **kwargs)
-        except ValidationError as error:
-            if not error.obj:
-                error.obj = obj
-            if not error.pointer:
-                error.pointer = self.uri
-            raise
-    return wrapper
+from collections import defaultdict
 
 
 class CompilationError(Exception):
     """Raised while schema parsing"""
     def __init__(self, message, schema):
         super(CompilationError, self).__init__(message, schema)
         self.schema = schema
```

### Comparing `json-spec-0.9.8/src/jsonspec/validators/factorize.py` & `json-spec-0.9.9/src/jsonspec/validators/factorize.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/src/jsonspec/validators/formats.py` & `json-spec-0.9.9/src/jsonspec/validators/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
     jsonspec.validators.formats
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 """
 
+from __future__ import absolute_import
+
 __all__ = ['register', 'FormatRegistry']
 
 import logging
 from functools import partial
 from pkg_resources import iter_entry_points, DistributionNotFound
 from .exceptions import CompilationError
```

### Comparing `json-spec-0.9.8/src/jsonspec/validators/util.py` & `json-spec-0.9.9/src/jsonspec/validators/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
     jsonspec.validators.util
     ~~~~~~~~~~~~~~~~~~~~~~~~
 
 """
 
+from __future__ import absolute_import
+
 __all__ = []
 
 import logging
 import re
 import time
 from copy import deepcopy
 from decimal import Decimal
```

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13747.767380` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13747.767380`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13750.659383` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13750.659383`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13751.870161` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13751.870161`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13754.725564` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13754.725564`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13757.87138` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13757.87138`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13759.913660` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13759.913660`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13760.814424` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13760.814424`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13763.284703` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13763.284703`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13765.696865` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13765.696865`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13766.217187` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13766.217187`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13767.563441` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13767.563441`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13772.315171` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13772.315171`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13774.53270` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13774.53270`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13776.480507` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13776.480507`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13848.148603` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13848.148603`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13851.883200` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13851.883200`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13852.658197` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13852.658197`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13855.981187` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13855.981187`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13858.162103` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13858.162103`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13860.756322` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13860.756322`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13861.558717` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13861.558717`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13864.839483` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13864.839483`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13866.711117` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13866.711117`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13867.481307` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13867.481307`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13868.292406` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13868.292406`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13873.16479` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13873.16479`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13875.755524` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13875.755524`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.13877.538157` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.13877.538157`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2890.971498` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2890.971498`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2893.380811` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2893.380811`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2894.793495` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2894.793495`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2928.597283` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2928.597283`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2931.192801` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2931.192801`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2932.217942` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2932.217942`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2936.233109` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2936.233109`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2940.212753` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2940.212753`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2955.883132` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2955.883132`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2958.989772` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2958.989772`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2959.860425` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2959.860425`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2963.816177` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2963.816177`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2965.224896` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2965.224896`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2982.986653` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2982.986653`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2985.374311` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2985.374311`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2986.865546` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2986.865546`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2990.591765` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2990.591765`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2992.165742` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2992.165742`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2995.662249` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2995.662249`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.2998.744678` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.2998.744678`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3037.34254` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3037.34254`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3040.245703` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3040.245703`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3041.402808` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3041.402808`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3044.851117` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3044.851117`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3045.205944` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3045.205944`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3049.367076` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3049.367076`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3051.497611` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3051.497611`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3054.349643` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3054.349643`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3057.398766` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3057.398766`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3085.965903` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3085.965903`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3088.825419` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3088.825419`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3089.232615` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3089.232615`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3092.436248` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3092.436248`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3095.904202` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3095.904202`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3097.390316` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3097.390316`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3100.97279` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3100.97279`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3103.875510` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3103.875510`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3105.771180` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3105.771180`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3106.253758` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3106.253758`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3107.994561` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3107.994561`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3120.464422` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3120.464422`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3125.43493` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3125.43493`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3126.120944` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3126.120944`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3129.405140` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3129.405140`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3132.21149` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3132.21149`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3134.760557` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3134.760557`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3135.702900` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3135.702900`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3138.345249` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3138.345249`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3140.618324` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3140.618324`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3141.304302` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3141.304302`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3142.803594` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3142.803594`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3147.599067` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3147.599067`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3158.411930` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3158.411930`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3161.934483` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3161.934483`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3162.638446` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3162.638446`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3165.30416` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3165.30416`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3170.833718` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3170.833718`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3172.319935` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3172.319935`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3173.761134` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3173.761134`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3176.720397` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3176.720397`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3178.85727` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3178.85727`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3179.868910` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3179.868910`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3180.240143` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3180.240143`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3185.704742` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3185.704742`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3196.399093` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3196.399093`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3199.588691` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3199.588691`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3200.680544` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3200.680544`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3203.440856` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3203.440856`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3206.290324` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3206.290324`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3208.564692` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3208.564692`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3209.81838` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3209.81838`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3212.832848` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3212.832848`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3214.644239` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3214.644239`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3215.524698` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3215.524698`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3216.42847` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3216.42847`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3221.533410` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3221.533410`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3234.388312` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3234.388312`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3239.775417` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3239.775417`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3240.557245` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3240.557245`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3243.788730` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3243.788730`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3246.569653` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3246.569653`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3248.843454` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3248.843454`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3249.165956` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3249.165956`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3252.306359` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3252.306359`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3254.372835` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3254.372835`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3255.163085` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3255.163085`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3256.990053` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3256.990053`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3261.351666` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3261.351666`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3270.227618` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3270.227618`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3273.65115` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3273.65115`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3274.237674` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3274.237674`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3277.19176` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3277.19176`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3280.898598` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3280.898598`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3282.817350` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3282.817350`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3283.45632` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3283.45632`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3286.420993` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3286.420993`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3288.53949` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3288.53949`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3289.352556` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3289.352556`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3290.992008` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3290.992008`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3295.184522` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3295.184522`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3371.384759` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3371.384759`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3374.818857` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3374.818857`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3375.499649` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3375.499649`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3378.68842` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3378.68842`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3381.949045` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3381.949045`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3383.803880` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3383.803880`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3384.450316` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3384.450316`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3387.830297` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3387.830297`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3389.699913` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3389.699913`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3390.518846` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3390.518846`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3391.881649` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3391.881649`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3396.541112` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3396.541112`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3441.966418` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3441.966418`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3444.746082` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3444.746082`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3445.389212` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3445.389212`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3448.669825` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3448.669825`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3451.277331` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3451.277331`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3453.289143` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3453.289143`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3454.270660` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3454.270660`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3457.246427` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3457.246427`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3459.861391` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3459.861391`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3460.34642` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3460.34642`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3461.488045` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3461.488045`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3466.73300` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3466.73300`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3486.358902` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3486.358902`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3489.33416` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3489.33416`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3490.359594` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3490.359594`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3493.956052` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3493.956052`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3496.412731` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3496.412731`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3498.678016` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3498.678016`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3499.653310` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3499.653310`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3502.596799` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3502.596799`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3504.746277` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3504.746277`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3506.628550` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3506.628550`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3507.403336` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3507.403336`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3512.572538` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3512.572538`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3529.610576` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3529.610576`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3532.775761` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3532.775761`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3533.315530` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3533.315530`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3536.588954` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3536.588954`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3539.967848` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3539.967848`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3541.22712` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3541.22712`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3542.763221` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3542.763221`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3545.825074` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3545.825074`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3547.736530` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3547.736530`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3548.135588` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3548.135588`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3549.508720` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3549.508720`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3554.240623` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3554.240623`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3972.942596` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3972.942596`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3975.159309` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3975.159309`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3976.791534` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3976.791534`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3979.772513` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3979.772513`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3982.279342` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3982.279342`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3984.468176` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3984.468176`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3985.566692` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3985.566692`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3988.692617` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3988.692617`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3990.65022` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3990.65022`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3991.162196` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3991.162196`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3992.692482` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3992.692482`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3997.506601` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3997.506601`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.3999.467478` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.3999.467478`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4001.122983` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4001.122983`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4386.103901` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4386.103901`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4389.898871` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4389.898871`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4390.632899` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4390.632899`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4393.470355` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4393.470355`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4396.156602` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4396.156602`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4398.335494` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4398.335494`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4399.783461` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4399.783461`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4402.386347` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4402.386347`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4404.323159` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4404.323159`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4405.955599` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4405.955599`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4406.891161` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4406.891161`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4411.478689` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4411.478689`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4413.968975` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4413.968975`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4415.419854` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4415.419854`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4426.141710` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4426.141710`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4429.937892` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4429.937892`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4430.821441` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4430.821441`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4433.89739` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4433.89739`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4436.770096` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4436.770096`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4438.411035` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4438.411035`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4439.293733` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4439.293733`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4442.287569` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4442.287569`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4444.159726` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4444.159726`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4445.710963` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4445.710963`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4446.450598` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4446.450598`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4451.294775` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4451.294775`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4453.638786` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4453.638786`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4455.38743` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4455.38743`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4467.379476` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4467.379476`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4470.341302` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4470.341302`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4471.812343` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4471.812343`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4474.991156` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4474.991156`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4477.375084` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4477.375084`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4479.626998` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4479.626998`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4480.740785` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4480.740785`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4483.230982` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4483.230982`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4485.229894` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4485.229894`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4486.698391` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4486.698391`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4487.369377` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4487.369377`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4492.927826` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4492.927826`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4494.717195` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4494.717195`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4496.17482` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4496.17482`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4504.364378` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4504.364378`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4507.352679` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4507.352679`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4508.176855` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4508.176855`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4511.298714` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4511.298714`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4514.641365` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4514.641365`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4516.977717` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4516.977717`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4517.350469` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4517.350469`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4520.675089` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4520.675089`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4522.387199` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4522.387199`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4523.690505` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4523.690505`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4524.889767` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4524.889767`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4529.248185` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4529.248185`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4531.237339` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4531.237339`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4533.707872` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4533.707872`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4743.717641` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4743.717641`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4746.324090` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4746.324090`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4747.508813` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4747.508813`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4750.992548` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4750.992548`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4753.754804` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4753.754804`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4755.405723` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4755.405723`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4756.396775` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4756.396775`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4759.88261` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4759.88261`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4761.575275` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4761.575275`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4762.161881` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4762.161881`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4763.893870` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4763.893870`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4768.149540` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4768.149540`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4770.671103` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4770.671103`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.4772.827193` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.4772.827193`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5664.515422` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5664.515422`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5667.105989` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5667.105989`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5668.35343` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5668.35343`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5671.860490` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5671.860490`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5674.189043` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5674.189043`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5676.535254` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5676.535254`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5677.102839` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5677.102839`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5680.286131` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5680.286131`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5682.664259` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5682.664259`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5683.977639` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5683.977639`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5684.172089` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5684.172089`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5689.710149` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5689.710149`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5691.525107` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5691.525107`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.le-piaf-2.cafe.intra.5693.536998` & `json-spec-0.9.9/tests/.coverage.le-piaf-2.cafe.intra.5693.536998`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10951.421015` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10951.421015`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10954.428544` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10954.428544`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10955.515651` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10955.515651`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10958.374497` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10958.374497`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10961.951865` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10961.951865`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10963.11090` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10963.11090`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10964.235322` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10964.235322`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10967.915676` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10967.915676`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10969.453178` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10969.453178`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10970.375256` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10970.375256`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10971.286286` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10971.286286`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10976.971196` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10976.971196`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10978.682256` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10978.682256`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10980.206840` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10980.206840`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10991.289358` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10991.289358`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10994.686238` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10994.686238`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10995.496508` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10995.496508`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.10998.373400` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.10998.373400`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11001.427568` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11001.427568`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11003.479443` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11003.479443`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11004.275617` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11004.275617`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11007.407176` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11007.407176`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11009.692787` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11009.692787`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11010.861199` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11010.861199`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11011.548903` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11011.548903`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11016.713601` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11016.713601`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11018.425276` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11018.425276`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11020.717207` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11020.717207`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11027.481779` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11027.481779`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11030.193078` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11030.193078`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11031.558282` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11031.558282`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11034.934266` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11034.934266`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11037.482667` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11037.482667`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11039.92172` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11039.92172`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11040.580421` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11040.580421`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11043.250772` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11043.250772`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11045.419672` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11045.419672`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11046.638359` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11046.638359`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11047.919858` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11047.919858`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11052.713388` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11052.713388`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11054.765457` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11054.765457`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11056.624922` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11056.624922`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11079.32142` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11079.32142`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11082.563451` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11082.563451`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11083.791770` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11083.791770`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11086.862515` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11086.862515`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11089.653131` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11089.653131`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11091.118511` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11091.118511`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11092.423477` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11092.423477`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11095.250029` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11095.250029`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11097.571002` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11097.571002`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11098.347740` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11098.347740`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11099.987225` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11099.987225`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11104.426307` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11104.426307`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11106.955388` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11106.955388`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11108.581593` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11108.581593`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11214.938510` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11214.938510`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11217.646151` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11217.646151`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11218.439338` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11218.439338`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11221.32430` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11221.32430`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11224.576114` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11224.576114`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11226.149202` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11226.149202`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11227.460050` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11227.460050`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11230.552639` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11230.552639`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11232.351813` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11232.351813`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11233.166456` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11233.166456`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11234.465792` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11234.465792`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11239.469005` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11239.469005`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11241.207429` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11241.207429`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11243.420688` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11243.420688`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11254.37161` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11254.37161`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11257.983127` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11257.983127`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11258.865944` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11258.865944`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11261.611179` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11261.611179`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11264.878658` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11264.878658`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11266.494999` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11266.494999`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11267.165792` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11267.165792`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11270.547077` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11270.547077`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11272.5829` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11272.5829`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11273.209790` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11273.209790`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11274.892427` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11274.892427`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11279.813165` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11279.813165`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11281.103429` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11281.103429`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11283.214539` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11283.214539`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11335.350941` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11335.350941`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11338.635226` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11338.635226`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11339.166257` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11339.166257`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11342.330369` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11342.330369`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11345.410963` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11345.410963`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11347.612141` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11347.612141`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11348.579233` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11348.579233`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11351.410803` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11351.410803`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11353.363743` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11353.363743`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11354.83605` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11354.83605`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11355.869925` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11355.869925`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11360.730957` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11360.730957`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11362.913135` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11362.913135`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11364.590973` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11364.590973`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11441.798921` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11441.798921`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11444.13221` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11444.13221`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11445.542803` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11445.542803`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11448.769610` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11448.769610`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11451.89753` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11451.89753`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11453.504155` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11453.504155`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11454.962200` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11454.962200`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11457.969910` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11457.969910`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11459.197891` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11459.197891`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11460.131903` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11460.131903`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11461.163111` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11461.163111`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11466.694589` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11466.694589`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11468.116318` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11468.116318`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/.coverage.Le-Piaf-2.local.11470.200781` & `json-spec-0.9.9/tests/.coverage.Le-Piaf-2.local.11470.200781`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/__init__.py` & `json-spec-0.9.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/fixtures/first.schema.json` & `json-spec-0.9.9/tests/fixtures/first.schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/fixtures/five.schema.json` & `json-spec-0.9.9/tests/fixtures/five.schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/fixtures/four.data.json` & `json-spec-0.9.9/tests/fixtures/four.data.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/fixtures/four.entry.schema.json` & `json-spec-0.9.9/tests/fixtures/four.entry.schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/fixtures/second.schema.json` & `json-spec-0.9.9/tests/fixtures/second.schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/fixtures/three.schema.json` & `json-spec-0.9.9/tests/fixtures/three.schema.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/bin/jsonschema_suite` & `json-spec-0.9.9/tests/suite/bin/jsonschema_suite`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/LICENSE` & `json-spec-0.9.9/tests/suite/LICENSE`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/README.md` & `json-spec-0.9.9/tests/suite/README.md`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/additionalItems.json` & `json-spec-0.9.9/tests/suite/tests/draft3/additionalItems.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/additionalProperties.json` & `json-spec-0.9.9/tests/suite/tests/draft3/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/dependencies.json` & `json-spec-0.9.9/tests/suite/tests/draft3/dependencies.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/disallow.json` & `json-spec-0.9.9/tests/suite/tests/draft3/disallow.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/divisibleBy.json` & `json-spec-0.9.9/tests/suite/tests/draft3/divisibleBy.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/enum.json` & `json-spec-0.9.9/tests/suite/tests/draft3/enum.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/extends.json` & `json-spec-0.9.9/tests/suite/tests/draft3/extends.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/items.json` & `json-spec-0.9.9/tests/suite/tests/draft3/items.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/maximum.json` & `json-spec-0.9.9/tests/suite/tests/draft3/maximum.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/maxItems.json` & `json-spec-0.9.9/tests/suite/tests/draft3/maxItems.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/maxLength.json` & `json-spec-0.9.9/tests/suite/tests/draft3/maxLength.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/minimum.json` & `json-spec-0.9.9/tests/suite/tests/draft3/minimum.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/minItems.json` & `json-spec-0.9.9/tests/suite/tests/draft3/minItems.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/minLength.json` & `json-spec-0.9.9/tests/suite/tests/draft3/minLength.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/optional/bignum.json` & `json-spec-0.9.9/tests/suite/tests/draft3/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/optional/format.json` & `json-spec-0.9.9/tests/suite/tests/draft3/optional/format.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/pattern.json` & `json-spec-0.9.9/tests/suite/tests/draft3/pattern.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/patternProperties.json` & `json-spec-0.9.9/tests/suite/tests/draft3/patternProperties.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/properties.json` & `json-spec-0.9.9/tests/suite/tests/draft3/properties.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/ref.json` & `json-spec-0.9.9/tests/suite/tests/draft3/ref.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/refRemote.json` & `json-spec-0.9.9/tests/suite/tests/draft3/refRemote.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/required.json` & `json-spec-0.9.9/tests/suite/tests/draft3/required.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/type.json` & `json-spec-0.9.9/tests/suite/tests/draft3/type.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft3/uniqueItems.json` & `json-spec-0.9.9/tests/suite/tests/draft3/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/additionalItems.json` & `json-spec-0.9.9/tests/suite/tests/draft4/additionalItems.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/additionalProperties.json` & `json-spec-0.9.9/tests/suite/tests/draft4/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/allOf.json` & `json-spec-0.9.9/tests/suite/tests/draft4/allOf.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/anyOf.json` & `json-spec-0.9.9/tests/suite/tests/draft4/anyOf.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/definitions.json` & `json-spec-0.9.9/tests/suite/tests/draft4/definitions.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/dependencies.json` & `json-spec-0.9.9/tests/suite/tests/draft4/dependencies.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/enum.json` & `json-spec-0.9.9/tests/suite/tests/draft4/enum.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/items.json` & `json-spec-0.9.9/tests/suite/tests/draft4/items.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/maximum.json` & `json-spec-0.9.9/tests/suite/tests/draft4/maximum.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/maxItems.json` & `json-spec-0.9.9/tests/suite/tests/draft4/maxItems.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/maxLength.json` & `json-spec-0.9.9/tests/suite/tests/draft4/maxLength.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/maxProperties.json` & `json-spec-0.9.9/tests/suite/tests/draft4/maxProperties.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/minimum.json` & `json-spec-0.9.9/tests/suite/tests/draft4/minimum.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/minItems.json` & `json-spec-0.9.9/tests/suite/tests/draft4/minItems.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/minLength.json` & `json-spec-0.9.9/tests/suite/tests/draft4/minLength.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/minProperties.json` & `json-spec-0.9.9/tests/suite/tests/draft4/minProperties.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/multipleOf.json` & `json-spec-0.9.9/tests/suite/tests/draft4/multipleOf.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/not.json` & `json-spec-0.9.9/tests/suite/tests/draft4/not.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/oneOf.json` & `json-spec-0.9.9/tests/suite/tests/draft4/oneOf.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/optional/bignum.json` & `json-spec-0.9.9/tests/suite/tests/draft4/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/optional/format.json` & `json-spec-0.9.9/tests/suite/tests/draft4/optional/format.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/pattern.json` & `json-spec-0.9.9/tests/suite/tests/draft4/pattern.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/patternProperties.json` & `json-spec-0.9.9/tests/suite/tests/draft4/patternProperties.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/properties.json` & `json-spec-0.9.9/tests/suite/tests/draft4/properties.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/ref.json` & `json-spec-0.9.9/tests/suite/tests/draft4/ref.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/refRemote.json` & `json-spec-0.9.9/tests/suite/tests/draft4/refRemote.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/required.json` & `json-spec-0.9.9/tests/suite/tests/draft4/required.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/type.json` & `json-spec-0.9.9/tests/suite/tests/draft4/type.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/suite/tests/draft4/uniqueItems.json` & `json-spec-0.9.9/tests/suite/tests/draft4/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_draft03.py` & `json-spec-0.9.9/tests/test_draft03.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_draft04.py` & `json-spec-0.9.9/tests/test_draft04.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_errors.py` & `json-spec-0.9.9/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_errors2.py` & `json-spec-0.9.9/tests/test_errors2.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_operations.py` & `json-spec-0.9.9/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_pointer.py` & `json-spec-0.9.9/tests/test_pointer.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_provider.py` & `json-spec-0.9.9/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_reference.py` & `json-spec-0.9.9/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `json-spec-0.9.8/tests/test_util.py` & `json-spec-0.9.9/tests/test_util.py`

 * *Files identical despite different names*

