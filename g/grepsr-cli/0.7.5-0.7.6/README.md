# Comparing `tmp/grepsr-cli-0.7.5.tar.gz` & `tmp/grepsr_cli-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grepsr-cli-0.7.5.tar", last modified: Wed May 17 10:48:52 2023, max compression
+gzip compressed data, was "grepsr_cli-0.7.6.tar", last modified: Mon Apr 29 04:39:33 2024, max compression
```

## Comparing `grepsr-cli-0.7.5.tar` & `grepsr_cli-0.7.6.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2023-05-17 10:48:13.000000 grepsr-cli-0.7.5/.version
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1219 2023-04-21 07:31:11.000000 grepsr-cli-0.7.5/CHANGELOG.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/LICENSE.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/MANIFEST.in
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3178 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2899 2023-05-17 10:47:33.000000 grepsr-cli-0.7.5/README.md
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.852318 grepsr-cli-0.7.5/grepsr_cli.egg-info/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3178 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1245 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/entry_points.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/requires.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2023-05-17 10:48:52.000000 grepsr-cli-0.7.5/grepsr_cli.egg-info/top_level.txt
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.852318 grepsr-cli-0.7.5/grepsrcli/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.852318 grepsr-cli-0.7.5/grepsrcli/controllers/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/controllers/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/controllers/base.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    16858 2023-05-17 10:47:33.000000 grepsr-cli-0.7.5/grepsrcli/controllers/crawler.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/controllers/generate.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/controllers/report.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/grepsrcli/core/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/core/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr-cli-0.7.5/grepsrcli/core/aws_s3.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-03-02 07:11:29.000000 grepsr-cli-0.7.5/grepsrcli/core/config.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/core/exc.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/core/input_prompts.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr-cli-0.7.5/grepsrcli/core/message_log.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/core/report_api.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-03-02 07:11:29.000000 grepsr-cli-0.7.5/grepsrcli/core/sdk_setup.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     5716 2023-05-17 10:47:33.000000 grepsr-cli-0.7.5/grepsrcli/core/test_local.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    11117 2023-04-21 07:32:16.000000 grepsr-cli-0.7.5/grepsrcli/core/utils.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/grepsrcli/ext/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/ext/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2157 2023-05-17 10:47:33.000000 grepsr-cli-0.7.5/grepsrcli/main.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/grepsrcli/plugins/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/plugins/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/grepsrcli/templates/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/autocomplete.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/autocomplete_zsh.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/composer.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/node_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1846 2023-03-07 07:03:13.000000 grepsr-cli-0.7.5/grepsrcli/templates/php_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3087 2023-03-07 07:03:13.000000 grepsr-cli-0.7.5/grepsrcli/templates/php_brp_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1904 2023-04-21 07:31:11.000000 grepsr-cli-0.7.5/grepsrcli/templates/php_vc_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/grepsrcli/templates/py_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/requirements-dev.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2023-04-21 07:31:11.000000 grepsr-cli-0.7.5/requirements.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/setup.cfg
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr-cli-0.7.5/setup.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2023-05-17 10:48:52.856318 grepsr-cli-0.7.5/tests/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      949 2023-01-07 17:34:33.000000 grepsr-cli-0.7.5/tests/test_grepsrcli.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2024-04-29 04:33:45.000000 grepsr_cli-0.7.6/.version
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1240 2024-04-25 17:55:02.000000 grepsr_cli-0.7.6/CHANGELOG.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/LICENSE.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/MANIFEST.in
+-rw-r--r--   0 zznix     (1000) zznix     (1000)     3369 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2837 2024-04-25 17:55:17.000000 grepsr_cli-0.7.6/README.md
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/grepsr_cli.egg-info/
+-rw-r--r--   0 zznix     (1000) zznix     (1000)     3369 2024-04-29 04:39:33.000000 grepsr_cli-0.7.6/grepsr_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1264 2024-04-29 04:39:33.000000 grepsr_cli-0.7.6/grepsr_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2024-04-29 04:39:33.000000 grepsr_cli-0.7.6/grepsr_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2024-04-29 04:39:33.000000 grepsr_cli-0.7.6/grepsr_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2024-04-29 04:39:33.000000 grepsr_cli-0.7.6/grepsr_cli.egg-info/requires.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2024-04-29 04:39:33.000000 grepsr_cli-0.7.6/grepsr_cli.egg-info/top_level.txt
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/grepsrcli/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/grepsrcli/controllers/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/controllers/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2023-06-06 11:43:01.000000 grepsr_cli-0.7.6/grepsrcli/controllers/base.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    17060 2024-04-29 04:33:42.000000 grepsr_cli-0.7.6/grepsrcli/controllers/crawler.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/controllers/generate.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/controllers/report.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/grepsrcli/core/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/core/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr_cli-0.7.6/grepsrcli/core/aws_s3.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-06-05 10:31:03.000000 grepsr_cli-0.7.6/grepsrcli/core/config.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/core/exc.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/core/input_prompts.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr_cli-0.7.6/grepsrcli/core/message_log.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/core/report_api.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-09-06 03:15:01.000000 grepsr_cli-0.7.6/grepsrcli/core/sdk_setup.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     5713 2024-04-26 05:25:47.000000 grepsr_cli-0.7.6/grepsrcli/core/test_local.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    13635 2024-04-25 17:32:12.000000 grepsr_cli-0.7.6/grepsrcli/core/utils.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/grepsrcli/ext/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/ext/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2169 2024-04-25 17:32:12.000000 grepsr_cli-0.7.6/grepsrcli/main.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/grepsrcli/plugins/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/plugins/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/grepsrcli/templates/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/templates/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/templates/autocomplete.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/templates/autocomplete_zsh.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/templates/composer.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/templates/node_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2006 2024-04-25 17:41:04.000000 grepsr_cli-0.7.6/grepsrcli/templates/php_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3087 2023-03-07 07:03:13.000000 grepsr_cli-0.7.6/grepsrcli/templates/php_brp_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1729 2024-04-25 17:44:50.000000 grepsr_cli-0.7.6/grepsrcli/templates/php_vc_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/grepsrcli/templates/py_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/requirements-dev.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2024-04-25 18:23:41.000000 grepsr_cli-0.7.6/requirements.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2024-04-29 04:39:33.939321 grepsr_cli-0.7.6/setup.cfg
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr_cli-0.7.6/setup.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-04-29 04:39:33.935320 grepsr_cli-0.7.6/tests/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      980 2024-04-25 17:32:12.000000 grepsr_cli-0.7.6/tests/test_grepsrcli.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      932 2024-04-25 17:32:12.000000 grepsr_cli-0.7.6/tests/test_unit.py
```

### Comparing `grepsr-cli-0.7.5/CHANGELOG.md` & `grepsr_cli-0.7.6/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Grepsr Cli Change History
 
+## current version
+
+
 ## 0.7.2
 {Changes to gcli codebase from last version (0.7.0 [23 Mar 2022])}
 
 README.md
 > updated readme highlighting new features, edge cases and development notes
 
 grepsrcli/controllers/crawler.py
```

### Comparing `grepsr-cli-0.7.5/PKG-INFO` & `grepsr_cli-0.7.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: grepsr-cli
-Version: 0.7.5
-Summary: A Cli tool for Grepsr Developers
-Home-page: https://bitbucket.org/grepsr/grepsr-cli/
-Author: grepsr
-Author-email: dev@grepsr.com
-License: unlicensed
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # A Cli tool for Grepsr Developers
 
 ## Installation
 ```
 $ pip install grepsr-cli
 ```
 
@@ -80,11 +69,10 @@
 ```bash
 git clone git@bitbucket.org:zznixt07/gcli.git grepsrcli
 cd grepsrcli
 pip install -e .
 ```
 
 ## Features Added
-- stash untracked files to avoid failure when applying stash.
 - drop stash after pushed successully. Before this, all stashes were always kept.
 - run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
-- auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
+- auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
```

### Comparing `grepsr-cli-0.7.5/README.md` & `grepsr_cli-0.7.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: grepsr-cli
+Version: 0.7.6
+Summary: A Cli tool for Grepsr Developers
+Home-page: https://bitbucket.org/grepsr/grepsr-cli/
+Author: grepsr
+Author-email: dev@grepsr.com
+License: unlicensed
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: cement>=3.0.4
+Requires-Dist: Jinja2>=2.11.3
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: colorlog>=4.8.0
+Requires-Dist: semver>=2.13.0
+Requires-Dist: terminaltables>=3.1.0
+Requires-Dist: requests>=2.25.1
+Requires-Dist: boto3<2.0.0,>=1.9.0
+
 # A Cli tool for Grepsr Developers
 
 ## Installation
 ```
 $ pip install grepsr-cli
 ```
 
@@ -69,11 +88,10 @@
 ```bash
 git clone git@bitbucket.org:zznixt07/gcli.git grepsrcli
 cd grepsrcli
 pip install -e .
 ```
 
 ## Features Added
-- stash untracked files to avoid failure when applying stash.
 - drop stash after pushed successully. Before this, all stashes were always kept.
 - run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
-- auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
+- auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
```

### Comparing `grepsr-cli-0.7.5/grepsr_cli.egg-info/PKG-INFO` & `grepsr_cli-0.7.6/grepsr_cli.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: cement>=3.0.4
+Requires-Dist: Jinja2>=2.11.3
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: colorlog>=4.8.0
+Requires-Dist: semver>=2.13.0
+Requires-Dist: terminaltables>=3.1.0
+Requires-Dist: requests>=2.25.1
+Requires-Dist: boto3<2.0.0,>=1.9.0
 
 # A Cli tool for Grepsr Developers
 
 ## Installation
 ```
 $ pip install grepsr-cli
 ```
@@ -80,11 +88,10 @@
 ```bash
 git clone git@bitbucket.org:zznixt07/gcli.git grepsrcli
 cd grepsrcli
 pip install -e .
 ```
 
 ## Features Added
-- stash untracked files to avoid failure when applying stash.
 - drop stash after pushed successully. Before this, all stashes were always kept.
 - run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
 - auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
```

### Comparing `grepsr-cli-0.7.5/grepsr_cli.egg-info/SOURCES.txt` & `grepsr_cli-0.7.6/grepsr_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 grepsrcli/templates/autocomplete_zsh.jinja2
 grepsrcli/templates/composer.jinja2
 grepsrcli/templates/node_boilerplate.jinja2
 grepsrcli/templates/php_boilerplate.jinja2
 grepsrcli/templates/php_brp_boilerplate.jinja2
 grepsrcli/templates/php_vc_boilerplate.jinja2
 grepsrcli/templates/py_boilerplate.jinja2
-tests/test_grepsrcli.py
+tests/test_grepsrcli.py
+tests/test_unit.py
```

### Comparing `grepsr-cli-0.7.5/grepsrcli/controllers/base.py` & `grepsr_cli-0.7.6/grepsrcli/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/controllers/crawler.py` & `grepsr_cli-0.7.6/grepsrcli/controllers/crawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from os import system, path
+import os
 import sys
-import time
 import subprocess
+import multiprocessing
+import signal
 import json
 import pathlib
-from semver import VersionInfo
 from cement import Controller, ex
 from ..core.config import load_config
 from ..core.utils import (
     create_boilerplate,
+    list_dependencies,
+    list_dependents,
     render_boilerplate,
     get_plugin_info,
     get_plugin_path,
     show_schema,
     user_input,
-    insert_all_chained_dependencies
+    insert_all_chained_dependencies,
+    does_plugin_have_modifications,
+    read_text,
+    return_cmd_with_progress,
+    update_version_file,
+    verbosify,
+    write_text
 )
 from ..core.test_local import TestLocal
 from ..core.message_log import Log
 from ..core.aws_s3 import S3
 
-
 class CrawlerBase(Controller):
     class Meta:
         label = 'crawler_base'
 
 
 class Crawler(Controller):
     config = load_config('config.yml')
@@ -255,121 +263,105 @@
             if not plugin_dir_path:
                 self.app.log.error(f'Could not find plugin: {plugin_name}')
                 continue
 
             plugin_info = get_plugin_info(plugin_dir_path)
             if plugin_info:
                 base_class = plugin_info['base_class']
-                if base_class != 'Vtx_Service_Plugin':
+                if not base_class.startswith('Vtx_Service_Plugin'):
                     if base_class not in plugin_info['dependencies']:
                         msg = f'Plugin extends {base_class} but does not declare it as a dependency.'
                         self.app.log.warning(msg)
-                        # if user_input(f'[Experimental] Do you want to automatically add dependencies?') == 'Y':
-                        #     insert_all_chained_dependencies(plugin_name)
-                        # go_fwd = user_input(f'Do you want to continue?')
-                        # if go_fwd == 'N':
-                        #     continue
-            # add .version or update .version
-            version_path = '{}/.version'.format(plugin_dir_path)
-            if path.exists(version_path):
-                with open(version_path, 'r') as f:
-                    version_info = VersionInfo.parse(f.read())
-                    if(major_flag):
-                        version_info = version_info.next_version(
-                            part='major')
-                    elif(minor_flag):
-                        version_info = version_info.next_version(
-                            part='minor')
-                    else:
-                        version_info = version_info.bump_patch()
-
-                    version_info = str(version_info)
-                    with open(version_path, 'w') as w:
-                        w.write(version_info)
-
-                self.app.log.info(
-                    "[{}] [{}] {}".format(deploy_type, version_info, deploy_message))
-            else:
-                if plugin_info:
-                    # if its already deployed then the service probabily works fine.
-                    # if its the first deploy, we annoy the user.
-                    if not plugin_info.get('pid_forced'):
-                        # TODO: maybe read all files and check if any service already has pid in which case force ought to be required.
-                        self.app.log.warning("PID was not forced. This may cause issues.")
-
-                with open(version_path, 'w') as f:
-                    if major_flag:
-                        version_info = "1.0.0"
-                    elif minor_flag:
-                        version_info = "0.1.0"
-                    else:
-                        version_info = "0.0.1"
-
-                    f.write(version_info)
-
-                self.app.log.info(
-                    "[{}] [{}] {}".format(deploy_type, version_info, deploy_message))
+                        if user_input(f'[Experimental] Do you want to automatically add dependencies?') == 'Y':
+                            insert_all_chained_dependencies(plugin_name)
+                        go_fwd = user_input(f'Do you want to continue?')
+                        if go_fwd == 'N':
+                            continue
+            
 
             if verbose_mode is False:
                 sys.stdout.write(
                     "Deploying: [%s]" % (" " * toolbar_width))
                 sys.stdout.write("\b" * (toolbar_width + 1))
                 sys.stdout.flush()
             try:
                 quiet_mode = "" if verbose_mode else "--quiet"
-                cd_to_repo_cmd = f"cd {plugin_dir_path} && cd .."
+                root_repo_dir = path.dirname(plugin_dir_path)
                 # dont pop stash. cuz if there is a merge conflict, good luck with that.
                 # instead apply stash and if and only if everything has passed, then drop the stash.
-                # TODO: only apply stash if git stash stashed > 0 files.
-                cmds = [
-                    cd_to_repo_cmd,
-                    f'git stash --include-untracked {quiet_mode}',
+                # TODO: only apply stash if `git stash` stashed >0 files.
+                git_sync_cmds = [
+                    f'git stash {quiet_mode}',
                     f'git pull origin master {quiet_mode}',
                     f'git stash apply {quiet_mode}',
+                ]
+                if verbose_mode:
+                    cmd = verbosify(git_sync_cmds)
+                else:
+                    cmd = return_cmd_with_progress(git_sync_cmds, toolbar_width)
+                try:
+                    proc = subprocess.run(cmd, shell=True, check=True, timeout=100, cwd=root_repo_dir)
+                except subprocess.TimeoutExpired:
+                    self.app.log.error(f'timed out on syncing rep for {plugin_name}')
+                    continue
+                
+                if not does_plugin_have_modifications(plugin_name, root_repo_dir):
+                    plugin_abs_path = path.join(plugin_dir_path, plugin_name + '.php')
+                    self.app.log.warning(f'No changes detected for {plugin_name}. Adding newline')
+                    write_text(plugin_abs_path, read_text(plugin_abs_path) + "\n")
+                    
+                version_info = update_version_file(plugin_dir_path, major_flag, minor_flag)
+                if plugin_info and version_info == '0.0.1':
+                    # if its already deployed then the service probabily works fine.
+                    # if its the first deploy, we annoy the user.
+                    if not plugin_info.get('pid_forced'):
+                        self.app.log.warning("PID was not forced. This may cause issues.")
+
+                commit_msg = f'[{deploy_type}] [{version_info}] {deploy_message}'
+                # self.app.log.info(commit_msg)
+                main_git_cmds = [
                     f'git add {plugin_name}/',
-                    f'git commit -m "[{deploy_type}] [{version_info}] {deploy_message}" {quiet_mode}',
+                    f'git commit -m "{commit_msg}" {quiet_mode}',
                     f'git push origin master {quiet_mode}',
                 ]
                 post_deploy_cmds = [
-                    cd_to_repo_cmd,
                     f'git stash drop {quiet_mode}'
                 ]
-                try:
-                    multiplier = toolbar_width // len(cmds)
-                except ZeroDivisionError:
-                    multiplier = 0
+                
                 if verbose_mode:
-                    multiplier = 0
-                # just echo some dashes after each command for progress. lol.
-                echoer = 'echo -n ' + '-' * multiplier
-                # .join() only does n-1 additions. Hence add a echoer at last. And then echo remaining to fill the bar (caused by floor division)
-                cmd = f' && {echoer} &&'.join(cmds) + f' && {echoer}' + f' && echo -n {"-" * (toolbar_width - (len(cmds) * multiplier))}'
+                    cmd = verbosify(main_git_cmds)
+                else:
+                    cmd = return_cmd_with_progress(main_git_cmds, toolbar_width)
                 try:
-                    proc = subprocess.run(cmd, shell=True, check=True, timeout=300)
+                    proc = subprocess.run(cmd, shell=True, check=True, timeout=300, cwd=root_repo_dir)
                     if proc.returncode == 0:
-                        proc = subprocess.run(' && '.join(post_deploy_cmds), shell=True)
+                        proc = subprocess.run(' && '.join(post_deploy_cmds), shell=True, cwd=root_repo_dir)
                         if proc.returncode != 0:
                             self.app.log.warning('Failed to drop the latest stash.')
 
                 except subprocess.TimeoutExpired:
                     self.app.log.error(f'Timeout occured when deploying {plugin_name}')
 
             except subprocess.CalledProcessError as e:
-                self.app.log.error(f'There was a problem deploying {plugin_name}')
+                if verbose_mode:
+                    self.app.log.error(e)
 
+                self.app.log.error(f'There was a problem deploying {plugin_name}')
                 return
 
             if verbose_mode is False:
                 sys.stdout.flush()
                 sys.stdout.write("\n")
 
             show_schema(plugin_dir_path)
 
             try:
                 app_url = f'https://platform.grepsr.com/projects/{plugin_info["pid"]}'
+                if plugin_info.get('rid'):
+                    app_url += f'/reports/{plugin_info["rid"]}'
                 self.app.log.info(f"App Url: {app_url}")
             except KeyError:
                 self.app.log.warning(f"Cannot find pid in plugin, please find the project's url manually")
 
             self.app.log.info(
                 f"Plugin: {plugin_name} deployed successfully")
 
@@ -439,7 +431,32 @@
 
             render_boilerplate(boilerplate='composer.jinja2', data=data,
                                destination_path=target_plugin_path + '/composer.json')
             system(
                 f""" cd {target_plugin_path} &&  composer install""")
         else:
             Log.error(f"Target plugin: {target_plugin_name} not found")
+
+
+    @ex(
+        help="list all the dependents of this given plugin",
+        arguments=[
+            (['-s'], {
+                "action": "store",
+                "dest": 'plugin_name'
+            })
+        ]
+    )
+    def list_dependents(self):
+        plugin_name = self.app.pargs.plugin_name
+    
+        if plugin_name is None:
+            self.app.log.error("no service code provided")
+            return False
+        plugin_dir_path = get_plugin_path(plugin_name, all_types=True)
+
+        if not plugin_dir_path:
+            self.app.log.error(f'Could not find plugin: {plugin_name}')
+            return
+        
+        for dependents in list_dependents(plugin_name):
+            print(dependents)
```

### Comparing `grepsr-cli-0.7.5/grepsrcli/controllers/generate.py` & `grepsr_cli-0.7.6/grepsrcli/controllers/generate.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/controllers/report.py` & `grepsr_cli-0.7.6/grepsrcli/controllers/report.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/core/aws_s3.py` & `grepsr_cli-0.7.6/grepsrcli/core/aws_s3.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/core/config.py` & `grepsr_cli-0.7.6/grepsrcli/core/config.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/core/message_log.py` & `grepsr_cli-0.7.6/grepsrcli/core/message_log.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/core/report_api.py` & `grepsr_cli-0.7.6/grepsrcli/core/report_api.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/core/sdk_setup.py` & `grepsr_cli-0.7.6/grepsrcli/core/sdk_setup.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/core/test_local.py` & `grepsr_cli-0.7.6/grepsrcli/core/test_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             original_entrypoints = get_docker_entrypoints(image_name=docker_image_name)
             sh_contents.append(f'source {original_entrypoints[0]} {sdk_args} {pipe_params}')
             write_text(custom_shell_file_local, '\n'.join(sh_contents))
 
             bash_cmd = f'source /tmp/{custom_shell_file}'
 
         commands = [
-                'docker run -t -i --network="host" --rm',
+                'docker run -t --network="host" --rm',
                 f'-v {self.base_path}:/home/grepsr/vortex-plugins/{path.basename(self.base_path)}',
                 f'-v {self.tmp_path}:/tmp',
                 f'-e APP_ENV={self.config["app_env"]}',
                 " ".join(env_vars),
                 f'--entrypoint=""' if not only_service else '',
                 docker_image_name,
                 f'bash -ci "{bash_cmd}"' if not only_service else sdk_args,
```

### Comparing `grepsr-cli-0.7.5/grepsrcli/core/utils.py` & `grepsr_cli-0.7.6/grepsrcli/core/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import subprocess
 from pathlib import Path
+from typing import List
 from os import listdir, path, mkdir
 import re
 from jinja2 import Template
 from .config import load_config
 from terminaltables import SingleTable
 from .message_log import Log
 
@@ -149,15 +150,15 @@
             break
         plugin_path = path.join(plugin_dir_path, plugin_name + '.php')
         contents = read_text(plugin_path)
         match = CLASS_DECLARATION_PATTERN.search(contents)
         if not match:
             break
         base_class = match.group(1)
-        if base_class == 'Vtx_Service_Plugin':
+        if base_class.startswith('Vtx_Service_Plugin'):
             break
         plugin_name = base_class
         dependencies.add(plugin_name)
     return list(dependencies)
 
 def insert_all_chained_dependencies(plugin_name):
     """add dependencies if the dependencies follow service_code/service_code.php pattern, however deep"""
@@ -178,32 +179,46 @@
     mappings['Dependencies'] = ','.join(list(set(dependencies + original_deps)))
     contents = set_comment_block(contents, mappings)
     write_text(plugin_path, contents)
     return True
 
 def set_comment_block(script, mappings):
     comment_block = ' * ' + '\n * '.join([f'{k}: {v}' for k, v in mappings.items()])
-    subbed = COMMENT_BLOCK_PATTERN.sub('\\1' + comment_block + '\\3', script)
+    subbed = COMMENT_BLOCK_PATTERN.sub('\\1' + comment_block + '\\3', script, 1)
     return subbed
 
 def get_comment_block(script):
     match = COMMENT_BLOCK_PATTERN.search(script)
     if not match:
         return {}
     doc = match.group(2)
     lines = doc.splitlines()
     mappings = {}
     for line in lines:
         splitted = line.lstrip(' *').split(':', 1)
         if len(splitted) != 2:
+            # TOOD: dont skip this,
             continue
         k, v = splitted
         mappings[k.strip()] = v.strip()
     return mappings
 
+def list_dependents(plugin_name):
+    plugin_dir_path = get_plugin_path(plugin_name)
+    repo_path = path.dirname(plugin_dir_path)
+    dependents = []
+    for directory in listdir(repo_path):
+        plugin_path = path.join(repo_path, directory)
+        if path.isfile(plugin_path):
+            continue
+        if get_plugin_info(plugin_path).get('base_class') == plugin_name:
+            dependents.append(directory)
+    return dependents
+            
+
 def get_plugin_info(plugin_path):
     """ get plugin's info like service_name,pid,description from the plugin's base folder.
     It does so by reading the file and looking at the info from plugin which is commented
     at the beginning.
 
     Args:
         plugin_path (str): the path of the directory where we find the plugin.
@@ -301,8 +316,62 @@
 def read_text(file_path):
     "helper function to read text from file with compatible encoding and no newline magic"
 
     # turn off universal-newline mode for less surprises.
     with open(file_path, 'r', encoding='UTF-8', newline='') as fd:
         contents = fd.read()
 
-    return contents
+    return contents
+
+
+def update_version_file(plugin_dir_path, major_flag, minor_flag):
+    from semver import VersionInfo
+
+    # create .version file or update .version file
+    version_path = '{}/.version'.format(plugin_dir_path)
+    if path.exists(version_path):
+        version_info = VersionInfo.parse(read_text(version_path))
+        if major_flag:
+            version_info = version_info.next_version(
+                part='major')
+        elif minor_flag:
+            version_info = version_info.next_version(
+                part='minor')
+        else:
+            version_info = version_info.bump_patch()
+        version_info = str(version_info)
+    else:
+        if major_flag:
+            version_info = "1.0.0"
+        elif minor_flag:
+            version_info = "0.1.0"
+        else:
+            version_info = "0.0.1"
+
+    write_text(version_path, version_info)
+
+    return version_info
+
+def return_cmd_with_progress(cmds, toolbar_width):
+    try:
+        multiplier = toolbar_width // len(cmds)
+    except ZeroDivisionError:
+        multiplier = 0
+    # just echo some dashes after each command for progress. lol.
+    echoer = 'echo -n ' + '-' * multiplier
+    # .join() only does n-1 additions. Hence add a echoer at last. And then echo remaining to fill the bar (caused by floor division)
+    cmd = f' && {echoer} &&'.join(cmds) + f' && {echoer}' + f' && echo -n {"-" * (toolbar_width - (len(cmds) * multiplier))}'
+    return cmd
+
+def does_plugin_have_modifications(plugin_name, root_repo_dir):
+    """check if plugin has any modification in the code
+    """
+    # TODO: handle untracked file. untracked file have newline added incorrectly.
+    proc = subprocess.run(f'git diff -s --exit-code {plugin_name}/{plugin_name}.php', shell=True, timeout=100, cwd=root_repo_dir)
+    if proc.returncode == 0:
+        return False
+    elif proc.returncode == 1:
+        return True
+    return None
+
+def verbosify(cmds: List[str]) -> str:
+    return ' && '.join([f'echo {cmd} && {cmd}' for cmd in cmds])
```

### Comparing `grepsr-cli-0.7.5/grepsrcli/main.py` & `grepsr_cli-0.7.6/grepsrcli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,13 +79,13 @@
 
             if app.debug is True:
                 import traceback
                 traceback.print_exc()
 
         except CaughtSignal as e:
             # Default Cement signals are SIGINT and SIGTERM, exit 0 (non-error)
-            print('\n%s' % e)
+            print('\n%s' % e, flush=True)
             app.exit_code = 0
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `grepsr-cli-0.7.5/grepsrcli/templates/autocomplete_zsh.jinja2` & `grepsr_cli-0.7.6/grepsrcli/templates/autocomplete_zsh.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/templates/node_boilerplate.jinja2` & `grepsr_cli-0.7.6/grepsrcli/templates/node_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/templates/php_boilerplate.jinja2` & `grepsr_cli-0.7.6/grepsrcli/templates/php_boilerplate.jinja2`

 * *Files 24% similar despite different names*

```diff
@@ -2,49 +2,48 @@
 /**
  * Name: {{plugin_name}}
  * Description: {{plugin_name}}
  * PID: {{pid}}
  */
 //ini_set('memory_limit', '256M');
 
-class {{plugin_name}} extends Vtx_Service_Plugin
-{
-    private $colHeaders;
-    protected $baseUrl;
-    protected $domainUrl;
+class {{plugin_name}} extends Vtx_Service_Plugin {
+    private $colHeaders = [
+    ];
+    protected $baseUrl = '';
+    protected $domainUrl = '';
     private $cache;
 
-    public function __construct()
-    {
+    public function __construct() {
         parent::__construct();
-     
-        $this->colHeaders = array(
-        );
-        $this->baseUrl = "";
-        $this->domainUrl = "";
-        
         //$this->cache = new Vtx_Service_Data_Cache(__CLASS__);
-        
     }
 
-    private function newSession()
-    {
+    public function newSession() {
         $this->resetCurl(true);
-        $this->resetHolaSuperProxy();
-
         $this->useProxy = true;
 
+        /*
+        $holaZone = 'grepsr';
+        $holaCountry = 'US';
+        if (method_exists($this, 'enableProxy')) {
+            $this->enableProxy('HOLA', $holaCountry, $holaZone);
+        } else {
+            $this->resetHolaSuperProxy();
+            $this->enableHola($holaCountry);
+            $this->setHolaZone($holaZone);
+        }
+        */
 
         $this->setHeaders('Accept-Encoding', 'gzip, deflate, br');
         $this->setHeaders('Accept', 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8');
         $this->setHeaders('Accept-Language', 'en-US,en;q=0.5');
         $this->setHeaders('Connection', 'keep-alive');
         $this->setHeaders('Upgrade-Insecure-Requests', '1');
-        $this->setHeaders('User-Agent', 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/76.0.3809.100 Safari/537.36');
-        //$this->setHeaders('Host',"%Host%");
+        $this->setHeaders('User-Agent', 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.67 Safari/537.36');
 
         //$this->setCurlOption(CURLOPT_HTTP_VERSION, CURL_HTTP_VERSION_1_0);
         //$this->setCurlOption(CURLOPT_CONNECTTIMEOUT, 180);
         //$this->setCurlOption(CURLOPT_TIMEOUT, 180);
     }
 
     public function main($params)
```

### Comparing `grepsr-cli-0.7.5/grepsrcli/templates/php_brp_boilerplate.jinja2` & `grepsr_cli-0.7.6/grepsrcli/templates/php_brp_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/grepsrcli/templates/php_vc_boilerplate.jinja2` & `grepsr_cli-0.7.6/grepsrcli/templates/php_vc_boilerplate.jinja2`

 * *Files 9% similar despite different names*

```diff
@@ -39,27 +39,24 @@
 
         $this->setHeaders('Accept-Encoding', 'gzip, deflate, br');
         $this->setHeaders('Accept', 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8');
         $this->setHeaders('Accept-Language', 'en-US,en;q=0.5');
         $this->setHeaders('Connection', 'keep-alive');
         $this->setHeaders('Upgrade-Insecure-Requests', '1');
         $this->setHeaders('User-Agent', 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/76.0.3809.100 Safari/537.36');
-        //$this->setHeaders('Host', "%Host%");
 
-        //$this->setCurlOption(CURLOPT_HTTP_VERSION, CURL_HTTP_VERSION_1_0);
         //$this->setCurlOption(CURLOPT_CONNECTTIMEOUT, 180);
         //$this->setCurlOption(CURLOPT_TIMEOUT, 180);
     }
 
     public function main($params)
     {
 	    echo("Crawling : " . $this->domainUrl . PHP_EOL);
         $this->dataSet->setPageName(get_class($this) . '_%s', [date('Ymd')]);
         $this->newSession();
         $this->switchProxy();
 
         //$this->loadDocument($this->baseUrl);
-        echo("Happy Crawling ! \n-cli-helper \n");
 
         return $this;
     }
 }
```

### Comparing `grepsr-cli-0.7.5/grepsrcli/templates/py_boilerplate.jinja2` & `grepsr_cli-0.7.6/grepsrcli/templates/py_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/setup.py` & `grepsr_cli-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `grepsr-cli-0.7.5/tests/test_grepsrcli.py` & `grepsr_cli-0.7.6/tests/test_grepsrcli.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,25 @@
     # test that debug mode is functional
     argv = ['--debug']
     with GrepsrCliTest(argv=argv) as app:
         app.run()
         assert app.debug is True
 
 
-def test_command1():
-    # test command1 without arguments
-    argv = ['command1']
-    with GrepsrCliTest(argv=argv) as app:
-        app.run()
-        data,output = app.last_rendered
-        assert data['foo'] == 'bar'
-        assert output.find('Foo => bar')
+# def test_command1():
+#     # test command1 without arguments
+#     argv = ['command1']
+#     with GrepsrCliTest(argv=argv) as app:
+#         app.run()
+#         data,output = app.last_rendered
+#         assert data['foo'] == 'bar'
+#         assert output.find('Foo => bar')
 
 
-    # test command1 with arguments
-    argv = ['command1', '--foo', 'not-bar']
-    with GrepsrCliTest(argv=argv) as app:
-        app.run()
-        data,output = app.last_rendered
-        assert data['foo'] == 'not-bar'
-        assert output.find('Foo => not-bar')
+#     # test command1 with arguments
+#     argv = ['command1', '--foo', 'not-bar']
+#     with GrepsrCliTest(argv=argv) as app:
+#         app.run()
+#         data,output = app.last_rendered
+#         assert data['foo'] == 'not-bar'
+#         assert output.find('Foo => not-bar')
+
```

