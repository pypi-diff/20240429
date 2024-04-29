# Comparing `tmp/socon_embedded-0.1a4.tar.gz` & `tmp/socon_embedded-0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socon_embedded-0.1a4.tar", last modified: Thu Apr 18 13:03:21 2024, max compression
+gzip compressed data, was "socon_embedded-0.1a5.tar", last modified: Mon Apr 29 08:32:21 2024, max compression
```

## Comparing `socon_embedded-0.1a4.tar` & `socon_embedded-0.1a5.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.261208 socon_embedded-0.1a4/
--rw-rw-rw-   0        0        0      986 2023-07-27 15:39:35.000000 socon_embedded-0.1a4/.gitignore
--rw-rw-rw-   0        0        0      127 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/AUTHORS
--rw-rw-rw-   0        0        0     5352 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1556 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/LICENSE
--rw-rw-rw-   0        0        0     1767 2024-04-18 13:03:21.251022 socon_embedded-0.1a4/PKG-INFO
--rw-rw-rw-   0        0        0      670 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/README.rst
--rw-rw-rw-   0        0        0        0 2023-07-13 15:45:21.000000 socon_embedded-0.1a4/__init__.py
--rw-rw-rw-   0        0        0      128 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/plugins.py
--rw-rw-rw-   0        0        0     1286 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/pyproject.toml
--rw-rw-rw-   0        0        0       98 2024-01-25 15:49:53.000000 socon_embedded-0.1a4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 13:03:21.261208 socon_embedded-0.1a4/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.736597 socon_embedded-0.1a4/socon_embedded/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a4/socon_embedded/__init__.py
--rw-rw-rw-   0        0        0      424 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded/_version.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.817664 socon_embedded-0.1a4/socon_embedded/action/
--rw-rw-rw-   0        0        0      771 2024-04-11 12:13:38.000000 socon_embedded-0.1a4/socon_embedded/action/__init__.py
--rw-rw-rw-   0        0        0      664 2024-04-11 09:42:54.000000 socon_embedded-0.1a4/socon_embedded/action/call.py
--rw-rw-rw-   0        0        0     2917 2024-04-11 09:41:05.000000 socon_embedded-0.1a4/socon_embedded/action/copy.py
--rw-rw-rw-   0        0        0      256 2024-04-11 09:44:01.000000 socon_embedded-0.1a4/socon_embedded/action/move.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.847310 socon_embedded-0.1a4/socon_embedded/builder/
--rw-rw-rw-   0        0        0    10354 2024-04-11 13:05:46.000000 socon_embedded-0.1a4/socon_embedded/builder/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-08-09 17:55:43.000000 socon_embedded-0.1a4/socon_embedded/builder/parser.py
--rw-rw-rw-   0        0        0     1203 2023-08-10 13:33:57.000000 socon_embedded-0.1a4/socon_embedded/builder/result.py
--rw-rw-rw-   0        0        0      564 2023-08-08 10:14:56.000000 socon_embedded-0.1a4/socon_embedded/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.878832 socon_embedded-0.1a4/socon_embedded/executor/
--rw-rw-rw-   0        0        0        0 2024-04-11 11:55:38.000000 socon_embedded-0.1a4/socon_embedded/executor/__init__.py
--rw-rw-rw-   0        0        0    10090 2024-04-11 13:37:06.000000 socon_embedded-0.1a4/socon_embedded/executor/app_executor.py
--rw-rw-rw-   0        0        0     4352 2024-04-12 12:59:49.000000 socon_embedded-0.1a4/socon_embedded/executor/task_executor.py
--rw-rw-rw-   0        0        0      818 2024-04-11 12:15:08.000000 socon_embedded-0.1a4/socon_embedded/executor/task_result.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.888949 socon_embedded-0.1a4/socon_embedded/management/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a4/socon_embedded/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.903704 socon_embedded-0.1a4/socon_embedded/management/commands/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:12.000000 socon_embedded-0.1a4/socon_embedded/management/commands/__init__.py
--rw-rw-rw-   0        0        0     7842 2024-04-11 13:07:03.000000 socon_embedded-0.1a4/socon_embedded/management/commands/build.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.909263 socon_embedded-0.1a4/socon_embedded/management/commands/subcommands/
--rw-rw-rw-   0        0        0        0 2023-08-08 10:14:56.000000 socon_embedded-0.1a4/socon_embedded/management/commands/subcommands/__init__.py
--rw-rw-rw-   0        0        0     1956 2024-04-11 12:47:56.000000 socon_embedded-0.1a4/socon_embedded/management/commands/subcommands/from_file.py
--rw-rw-rw-   0        0        0     2950 2024-04-12 07:54:43.000000 socon_embedded-0.1a4/socon_embedded/managers.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.940645 socon_embedded-0.1a4/socon_embedded/schema/
--rw-rw-rw-   0        0        0        0 2023-08-07 08:27:21.000000 socon_embedded-0.1a4/socon_embedded/schema/__init__.py
--rw-rw-rw-   0        0        0     8498 2024-04-11 12:13:57.000000 socon_embedded-0.1a4/socon_embedded/schema/apps.py
--rw-rw-rw-   0        0        0      736 2023-08-08 10:14:56.000000 socon_embedded-0.1a4/socon_embedded/schema/base.py
--rw-rw-rw-   0        0        0     4133 2024-04-18 13:01:30.000000 socon_embedded-0.1a4/socon_embedded/schema/task.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.981744 socon_embedded-0.1a4/socon_embedded/utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a4/socon_embedded/utils/__init__.py
--rw-rw-rw-   0        0        0     2523 2024-04-04 12:31:10.000000 socon_embedded-0.1a4/socon_embedded/utils/converter.py
--rw-rw-rw-   0        0        0      493 2023-07-27 15:38:12.000000 socon_embedded-0.1a4/socon_embedded/utils/jinja.py
--rw-rw-rw-   0        0        0     1773 2023-08-08 10:14:56.000000 socon_embedded-0.1a4/socon_embedded/utils/loader.py
--rw-rw-rw-   0        0        0     2192 2023-07-27 15:38:12.000000 socon_embedded-0.1a4/socon_embedded/utils/parser.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.251022 socon_embedded-0.1a4/socon_embedded.egg-info/
--rw-rw-rw-   0        0        0     1767 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2529 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.004200 socon_embedded-0.1a4/tests/
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.054293 socon_embedded-0.1a4/tests/action/
--rw-rw-rw-   0        0        0      267 2024-04-11 12:46:08.000000 socon_embedded-0.1a4/tests/action/__init__.py
--rw-rw-rw-   0        0        0      720 2024-04-11 12:45:24.000000 socon_embedded-0.1a4/tests/action/test_call_command.py
--rw-rw-rw-   0        0        0     1755 2024-04-11 12:44:43.000000 socon_embedded-0.1a4/tests/action/test_copy.py
--rw-rw-rw-   0        0        0      626 2024-04-12 08:59:07.000000 socon_embedded-0.1a4/tests/action/test_discover.py
--rw-rw-rw-   0        0        0        0 2024-04-11 12:45:29.000000 socon_embedded-0.1a4/tests/action/test_move.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.075089 socon_embedded-0.1a4/tests/commands/
--rw-rw-rw-   0        0        0        0 2024-04-11 12:32:35.000000 socon_embedded-0.1a4/tests/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.085297 socon_embedded-0.1a4/tests/commands/datafixtures/
--rw-rw-rw-   0        0        0      397 2024-04-11 13:02:05.000000 socon_embedded-0.1a4/tests/commands/datafixtures/simple_app_config.yml
--rw-rw-rw-   0        0        0      493 2024-04-11 13:02:22.000000 socon_embedded-0.1a4/tests/commands/datafixtures/simple_app_with_task.yml
--rw-rw-rw-   0        0        0      370 2024-04-11 12:36:04.000000 socon_embedded-0.1a4/tests/commands/test_build_command.py
--rw-rw-rw-   0        0        0      439 2024-04-12 08:53:56.000000 socon_embedded-0.1a4/tests/commands/test_from_file.py
--rw-rw-rw-   0        0        0      330 2024-04-12 08:52:00.000000 socon_embedded-0.1a4/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.105917 socon_embedded-0.1a4/tests/executor/
--rw-rw-rw-   0        0        0        0 2024-04-11 12:18:37.000000 socon_embedded-0.1a4/tests/executor/__init__.py
--rw-rw-rw-   0        0        0       72 2024-04-11 12:28:37.000000 socon_embedded-0.1a4/tests/executor/test_task_executor.py
--rw-rw-rw-   0        0        0      580 2024-04-11 12:23:44.000000 socon_embedded-0.1a4/tests/executor/test_task_result.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.117991 socon_embedded-0.1a4/tests/management/
--rw-rw-rw-   0        0        0        0 2024-04-11 12:58:57.000000 socon_embedded-0.1a4/tests/management/__init__.py
--rw-rw-rw-   0        0        0       33 2024-04-11 12:59:16.000000 socon_embedded-0.1a4/tests/management/config.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.117991 socon_embedded-0.1a4/tests/projects/
--rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon_embedded-0.1a4/tests/projects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.157568 socon_embedded-0.1a4/tests/projects/test_project/
--rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon_embedded-0.1a4/tests/projects/test_project/__init__.py
--rw-rw-rw-   0        0        0      361 2024-04-12 08:56:26.000000 socon_embedded-0.1a4/tests/projects/test_project/action.py
--rw-rw-rw-   0        0        0      287 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/tests/projects/test_project/builder.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.166789 socon_embedded-0.1a4/tests/projects/test_project/management/
--rw-rw-rw-   0        0        0       33 2024-04-12 08:51:00.000000 socon_embedded-0.1a4/tests/projects/test_project/management/config.py
--rw-rw-rw-   0        0        0      171 2024-04-12 08:51:38.000000 socon_embedded-0.1a4/tests/projects/test_project/projects.py
--rw-rw-rw-   0        0        0       77 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/tests/pytest.ini
--rw-rw-rw-   0        0        0       62 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/tests/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.178391 socon_embedded-0.1a4/tests/schema/
--rw-rw-rw-   0        0        0        0 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/tests/schema/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.239667 socon_embedded-0.1a4/tests/schema/datafixtures/
--rw-rw-rw-   0        0        0       80 2024-04-04 13:07:32.000000 socon_embedded-0.1a4/tests/schema/datafixtures/action_extra_args.yml
--rw-rw-rw-   0        0        0       47 2024-04-02 13:14:24.000000 socon_embedded-0.1a4/tests/schema/datafixtures/bad_action.yml
--rw-rw-rw-   0        0        0       59 2024-04-02 13:13:17.000000 socon_embedded-0.1a4/tests/schema/datafixtures/copy_schema.yml
--rw-rw-rw-   0        0        0       91 2024-04-02 15:27:00.000000 socon_embedded-0.1a4/tests/schema/datafixtures/multiple_valid_action.yml
--rw-rw-rw-   0        0        0       19 2024-04-02 15:22:54.000000 socon_embedded-0.1a4/tests/schema/datafixtures/no_action.yml
--rw-rw-rw-   0        0        0       77 2024-04-02 13:15:18.000000 socon_embedded-0.1a4/tests/schema/datafixtures/set_action.yml
--rw-rw-rw-   0        0        0     2050 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/tests/schema/test_app_registry.py
--rw-rw-rw-   0        0        0     2652 2024-04-11 12:14:54.000000 socon_embedded-0.1a4/tests/schema/test_tasks.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.251022 socon_embedded-0.1a4/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:39:35.000000 socon_embedded-0.1a4/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     2275 2023-07-27 15:39:35.000000 socon_embedded-0.1a4/tests/utils/test_splitter.py
--rw-rw-rw-   0        0        0     1361 2023-07-27 15:39:35.000000 socon_embedded-0.1a4/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.920753 socon_embedded-0.1a5/
+-rw-rw-rw-   0        0        0      986 2023-07-27 15:39:35.000000 socon_embedded-0.1a5/.gitignore
+-rw-rw-rw-   0        0        0      127 2023-07-14 08:31:36.000000 socon_embedded-0.1a5/AUTHORS
+-rw-rw-rw-   0        0        0     5352 2023-07-14 08:31:36.000000 socon_embedded-0.1a5/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     1556 2023-07-14 08:31:36.000000 socon_embedded-0.1a5/LICENSE
+-rw-rw-rw-   0        0        0     1767 2024-04-29 08:32:21.904149 socon_embedded-0.1a5/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-11-20 08:57:35.000000 socon_embedded-0.1a5/README.rst
+-rw-rw-rw-   0        0        0        0 2023-07-13 15:45:21.000000 socon_embedded-0.1a5/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-07-14 08:31:36.000000 socon_embedded-0.1a5/plugins.py
+-rw-rw-rw-   0        0        0     1286 2023-11-20 08:57:35.000000 socon_embedded-0.1a5/pyproject.toml
+-rw-rw-rw-   0        0        0       98 2024-04-29 08:28:26.000000 socon_embedded-0.1a5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:32:21.920753 socon_embedded-0.1a5/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-07-14 08:31:36.000000 socon_embedded-0.1a5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.420245 socon_embedded-0.1a5/socon_embedded/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a5/socon_embedded/__init__.py
+-rw-rw-rw-   0        0        0      424 2024-04-29 08:32:20.000000 socon_embedded-0.1a5/socon_embedded/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.495436 socon_embedded-0.1a5/socon_embedded/action/
+-rw-rw-rw-   0        0        0      771 2024-04-11 12:13:38.000000 socon_embedded-0.1a5/socon_embedded/action/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-04-11 09:42:54.000000 socon_embedded-0.1a5/socon_embedded/action/call.py
+-rw-rw-rw-   0        0        0     2917 2024-04-11 09:41:05.000000 socon_embedded-0.1a5/socon_embedded/action/copy.py
+-rw-rw-rw-   0        0        0      256 2024-04-11 09:44:01.000000 socon_embedded-0.1a5/socon_embedded/action/move.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.539415 socon_embedded-0.1a5/socon_embedded/builder/
+-rw-rw-rw-   0        0        0    10354 2024-04-11 13:05:46.000000 socon_embedded-0.1a5/socon_embedded/builder/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-08-09 17:55:43.000000 socon_embedded-0.1a5/socon_embedded/builder/parser.py
+-rw-rw-rw-   0        0        0     1203 2023-08-10 13:33:57.000000 socon_embedded-0.1a5/socon_embedded/builder/result.py
+-rw-rw-rw-   0        0        0      564 2023-08-08 10:14:56.000000 socon_embedded-0.1a5/socon_embedded/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.567802 socon_embedded-0.1a5/socon_embedded/executor/
+-rw-rw-rw-   0        0        0        0 2024-04-11 11:55:38.000000 socon_embedded-0.1a5/socon_embedded/executor/__init__.py
+-rw-rw-rw-   0        0        0    10090 2024-04-11 13:37:06.000000 socon_embedded-0.1a5/socon_embedded/executor/app_executor.py
+-rw-rw-rw-   0        0        0     4352 2024-04-12 12:59:49.000000 socon_embedded-0.1a5/socon_embedded/executor/task_executor.py
+-rw-rw-rw-   0        0        0      818 2024-04-11 12:15:08.000000 socon_embedded-0.1a5/socon_embedded/executor/task_result.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.568851 socon_embedded-0.1a5/socon_embedded/management/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a5/socon_embedded/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.580096 socon_embedded-0.1a5/socon_embedded/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:12.000000 socon_embedded-0.1a5/socon_embedded/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     7842 2024-04-11 13:07:03.000000 socon_embedded-0.1a5/socon_embedded/management/commands/build.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.580096 socon_embedded-0.1a5/socon_embedded/management/commands/subcommands/
+-rw-rw-rw-   0        0        0        0 2023-08-08 10:14:56.000000 socon_embedded-0.1a5/socon_embedded/management/commands/subcommands/__init__.py
+-rw-rw-rw-   0        0        0     1956 2024-04-11 12:47:56.000000 socon_embedded-0.1a5/socon_embedded/management/commands/subcommands/from_file.py
+-rw-rw-rw-   0        0        0     2950 2024-04-12 07:54:43.000000 socon_embedded-0.1a5/socon_embedded/managers.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.611400 socon_embedded-0.1a5/socon_embedded/schema/
+-rw-rw-rw-   0        0        0        0 2023-08-07 08:27:21.000000 socon_embedded-0.1a5/socon_embedded/schema/__init__.py
+-rw-rw-rw-   0        0        0     8498 2024-04-29 08:30:54.000000 socon_embedded-0.1a5/socon_embedded/schema/apps.py
+-rw-rw-rw-   0        0        0      736 2023-08-08 10:14:56.000000 socon_embedded-0.1a5/socon_embedded/schema/base.py
+-rw-rw-rw-   0        0        0     4133 2024-04-18 13:01:30.000000 socon_embedded-0.1a5/socon_embedded/schema/task.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.645002 socon_embedded-0.1a5/socon_embedded/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a5/socon_embedded/utils/__init__.py
+-rw-rw-rw-   0        0        0     2523 2024-04-04 12:31:10.000000 socon_embedded-0.1a5/socon_embedded/utils/converter.py
+-rw-rw-rw-   0        0        0      493 2023-07-27 15:38:12.000000 socon_embedded-0.1a5/socon_embedded/utils/jinja.py
+-rw-rw-rw-   0        0        0     1773 2023-08-08 10:14:56.000000 socon_embedded-0.1a5/socon_embedded/utils/loader.py
+-rw-rw-rw-   0        0        0     2192 2023-07-27 15:38:12.000000 socon_embedded-0.1a5/socon_embedded/utils/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.904149 socon_embedded-0.1a5/socon_embedded.egg-info/
+-rw-rw-rw-   0        0        0     1767 2024-04-29 08:32:21.000000 socon_embedded-0.1a5/socon_embedded.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2529 2024-04-29 08:32:21.000000 socon_embedded-0.1a5/socon_embedded.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:32:21.000000 socon_embedded-0.1a5/socon_embedded.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-04-29 08:32:21.000000 socon_embedded-0.1a5/socon_embedded.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-29 08:32:21.000000 socon_embedded-0.1a5/socon_embedded.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.680350 socon_embedded-0.1a5/tests/
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.727239 socon_embedded-0.1a5/tests/action/
+-rw-rw-rw-   0        0        0      267 2024-04-11 12:46:08.000000 socon_embedded-0.1a5/tests/action/__init__.py
+-rw-rw-rw-   0        0        0      720 2024-04-11 12:45:24.000000 socon_embedded-0.1a5/tests/action/test_call_command.py
+-rw-rw-rw-   0        0        0     1755 2024-04-11 12:44:43.000000 socon_embedded-0.1a5/tests/action/test_copy.py
+-rw-rw-rw-   0        0        0      626 2024-04-12 08:59:07.000000 socon_embedded-0.1a5/tests/action/test_discover.py
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:45:29.000000 socon_embedded-0.1a5/tests/action/test_move.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.742903 socon_embedded-0.1a5/tests/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:32:35.000000 socon_embedded-0.1a5/tests/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.758503 socon_embedded-0.1a5/tests/commands/datafixtures/
+-rw-rw-rw-   0        0        0      397 2024-04-11 13:02:05.000000 socon_embedded-0.1a5/tests/commands/datafixtures/simple_app_config.yml
+-rw-rw-rw-   0        0        0      493 2024-04-11 13:02:22.000000 socon_embedded-0.1a5/tests/commands/datafixtures/simple_app_with_task.yml
+-rw-rw-rw-   0        0        0      370 2024-04-11 12:36:04.000000 socon_embedded-0.1a5/tests/commands/test_build_command.py
+-rw-rw-rw-   0        0        0      439 2024-04-12 08:53:56.000000 socon_embedded-0.1a5/tests/commands/test_from_file.py
+-rw-rw-rw-   0        0        0      330 2024-04-12 08:52:00.000000 socon_embedded-0.1a5/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.780313 socon_embedded-0.1a5/tests/executor/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:18:37.000000 socon_embedded-0.1a5/tests/executor/__init__.py
+-rw-rw-rw-   0        0        0       72 2024-04-11 12:28:37.000000 socon_embedded-0.1a5/tests/executor/test_task_executor.py
+-rw-rw-rw-   0        0        0      580 2024-04-11 12:23:44.000000 socon_embedded-0.1a5/tests/executor/test_task_result.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.780313 socon_embedded-0.1a5/tests/management/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:58:57.000000 socon_embedded-0.1a5/tests/management/__init__.py
+-rw-rw-rw-   0        0        0       33 2024-04-11 12:59:16.000000 socon_embedded-0.1a5/tests/management/config.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.780313 socon_embedded-0.1a5/tests/projects/
+-rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon_embedded-0.1a5/tests/projects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.811617 socon_embedded-0.1a5/tests/projects/test_project/
+-rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon_embedded-0.1a5/tests/projects/test_project/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-04-12 08:56:26.000000 socon_embedded-0.1a5/tests/projects/test_project/action.py
+-rw-rw-rw-   0        0        0      287 2023-11-20 08:57:35.000000 socon_embedded-0.1a5/tests/projects/test_project/builder.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.827236 socon_embedded-0.1a5/tests/projects/test_project/management/
+-rw-rw-rw-   0        0        0       33 2024-04-12 08:51:00.000000 socon_embedded-0.1a5/tests/projects/test_project/management/config.py
+-rw-rw-rw-   0        0        0      171 2024-04-12 08:51:38.000000 socon_embedded-0.1a5/tests/projects/test_project/projects.py
+-rw-rw-rw-   0        0        0       77 2023-11-20 08:57:35.000000 socon_embedded-0.1a5/tests/pytest.ini
+-rw-rw-rw-   0        0        0       62 2023-07-14 08:31:36.000000 socon_embedded-0.1a5/tests/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.842867 socon_embedded-0.1a5/tests/schema/
+-rw-rw-rw-   0        0        0        0 2023-11-20 08:57:35.000000 socon_embedded-0.1a5/tests/schema/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.888476 socon_embedded-0.1a5/tests/schema/datafixtures/
+-rw-rw-rw-   0        0        0       80 2024-04-04 13:07:32.000000 socon_embedded-0.1a5/tests/schema/datafixtures/action_extra_args.yml
+-rw-rw-rw-   0        0        0       47 2024-04-02 13:14:24.000000 socon_embedded-0.1a5/tests/schema/datafixtures/bad_action.yml
+-rw-rw-rw-   0        0        0       59 2024-04-02 13:13:17.000000 socon_embedded-0.1a5/tests/schema/datafixtures/copy_schema.yml
+-rw-rw-rw-   0        0        0       91 2024-04-02 15:27:00.000000 socon_embedded-0.1a5/tests/schema/datafixtures/multiple_valid_action.yml
+-rw-rw-rw-   0        0        0       19 2024-04-02 15:22:54.000000 socon_embedded-0.1a5/tests/schema/datafixtures/no_action.yml
+-rw-rw-rw-   0        0        0       77 2024-04-02 13:15:18.000000 socon_embedded-0.1a5/tests/schema/datafixtures/set_action.yml
+-rw-rw-rw-   0        0        0     2050 2023-11-20 08:57:35.000000 socon_embedded-0.1a5/tests/schema/test_app_registry.py
+-rw-rw-rw-   0        0        0     2652 2024-04-11 12:14:54.000000 socon_embedded-0.1a5/tests/schema/test_tasks.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:32:21.904149 socon_embedded-0.1a5/tests/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:39:35.000000 socon_embedded-0.1a5/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     2275 2023-07-27 15:39:35.000000 socon_embedded-0.1a5/tests/utils/test_splitter.py
+-rw-rw-rw-   0        0        0     1361 2023-07-27 15:39:35.000000 socon_embedded-0.1a5/tox.ini
```

### Comparing `socon_embedded-0.1a4/.gitignore` & `socon_embedded-0.1a5/.gitignore`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/CODE_OF_CONDUCT.md` & `socon_embedded-0.1a5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/LICENSE` & `socon_embedded-0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/PKG-INFO` & `socon_embedded-0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socon-embedded
-Version: 0.1a4
+Version: 0.1a5
 Summary: Build/Flash tool plugin for socon
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/socon-dev/socon-embedded
 Keywords: build,flasH,embedded,socon
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: PyYAML==6.0
 Requires-Dist: Jinja2==3.1.2
-Requires-Dist: datalookup==1.0.0
+Requires-Dist: datalookup==1.0.1
 Requires-Dist: pydantic==2.5.3
 Requires-Dist: socon==0.2.1
 Requires-Dist: junitparser==3.1.0
 
 ==============
 Socon-embedded
 ==============
```

### Comparing `socon_embedded-0.1a4/README.rst` & `socon_embedded-0.1a5/README.rst`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/pyproject.toml` & `socon_embedded-0.1a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/action/__init__.py` & `socon_embedded-0.1a5/socon_embedded/action/__init__.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/action/call.py` & `socon_embedded-0.1a5/socon_embedded/action/call.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/action/copy.py` & `socon_embedded-0.1a5/socon_embedded/action/copy.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/builder/__init__.py` & `socon_embedded-0.1a5/socon_embedded/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/builder/parser.py` & `socon_embedded-0.1a5/socon_embedded/builder/parser.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/builder/result.py` & `socon_embedded-0.1a5/socon_embedded/builder/result.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/exceptions.py` & `socon_embedded-0.1a5/socon_embedded/exceptions.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/executor/app_executor.py` & `socon_embedded-0.1a5/socon_embedded/executor/app_executor.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/executor/task_executor.py` & `socon_embedded-0.1a5/socon_embedded/executor/task_executor.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/executor/task_result.py` & `socon_embedded-0.1a5/socon_embedded/executor/task_result.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/management/commands/build.py` & `socon_embedded-0.1a5/socon_embedded/management/commands/build.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/management/commands/subcommands/from_file.py` & `socon_embedded-0.1a5/socon_embedded/management/commands/subcommands/from_file.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/managers.py` & `socon_embedded-0.1a5/socon_embedded/managers.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/schema/apps.py` & `socon_embedded-0.1a5/socon_embedded/schema/apps.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/schema/base.py` & `socon_embedded-0.1a5/socon_embedded/schema/base.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/schema/task.py` & `socon_embedded-0.1a5/socon_embedded/schema/task.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/utils/converter.py` & `socon_embedded-0.1a5/socon_embedded/utils/converter.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/utils/loader.py` & `socon_embedded-0.1a5/socon_embedded/utils/loader.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded/utils/parser.py` & `socon_embedded-0.1a5/socon_embedded/utils/parser.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/socon_embedded.egg-info/PKG-INFO` & `socon_embedded-0.1a5/socon_embedded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socon-embedded
-Version: 0.1a4
+Version: 0.1a5
 Summary: Build/Flash tool plugin for socon
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/socon-dev/socon-embedded
 Keywords: build,flasH,embedded,socon
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: PyYAML==6.0
 Requires-Dist: Jinja2==3.1.2
-Requires-Dist: datalookup==1.0.0
+Requires-Dist: datalookup==1.0.1
 Requires-Dist: pydantic==2.5.3
 Requires-Dist: socon==0.2.1
 Requires-Dist: junitparser==3.1.0
 
 ==============
 Socon-embedded
 ==============
```

### Comparing `socon_embedded-0.1a4/socon_embedded.egg-info/SOURCES.txt` & `socon_embedded-0.1a5/socon_embedded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/tests/action/test_call_command.py` & `socon_embedded-0.1a5/tests/action/test_call_command.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/tests/action/test_copy.py` & `socon_embedded-0.1a5/tests/action/test_copy.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/tests/action/test_discover.py` & `socon_embedded-0.1a5/tests/action/test_discover.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/tests/executor/test_task_result.py` & `socon_embedded-0.1a5/tests/executor/test_task_result.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/tests/schema/test_app_registry.py` & `socon_embedded-0.1a5/tests/schema/test_app_registry.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/tests/schema/test_tasks.py` & `socon_embedded-0.1a5/tests/schema/test_tasks.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/tests/utils/test_splitter.py` & `socon_embedded-0.1a5/tests/utils/test_splitter.py`

 * *Files identical despite different names*

### Comparing `socon_embedded-0.1a4/tox.ini` & `socon_embedded-0.1a5/tox.ini`

 * *Files identical despite different names*

