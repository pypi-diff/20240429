# Comparing `tmp/apio-0.9.3.tar.gz` & `tmp/apio-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apio-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "apio-0.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apio-0.9.3.tar` & `apio-0.9.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      938 2024-04-02 17:40:48.537737 apio-0.9.3/.github/workflows/Publish.yml
--rw-r--r--   0        0        0      583 2024-04-02 17:40:48.537737 apio-0.9.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      330 2024-04-02 17:40:48.537737 apio-0.9.3/.gitignore
--rw-r--r--   0        0        0     6379 2024-04-02 17:40:48.537737 apio-0.9.3/.vscode/launch.json
--rw-r--r--   0        0        0    18047 2024-04-02 17:40:48.537737 apio-0.9.3/LICENSE
--rw-r--r--   0        0        0     1092 2024-04-02 17:40:48.537737 apio-0.9.3/Makefile
--rw-r--r--   0        0        0     4683 2024-04-02 17:40:48.537737 apio-0.9.3/README.md
--rw-r--r--   0        0        0      747 2024-04-02 17:40:48.537737 apio-0.9.3/apio/__init__.py
--rw-r--r--   0        0        0     5752 2024-04-02 17:40:48.537737 apio-0.9.3/apio/__main__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/boards.py
--rw-r--r--   0        0        0     3160 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/build.py
--rw-r--r--   0        0        0     1400 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/clean.py
--rw-r--r--   0        0        0     1603 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/config.py
--rw-r--r--   0        0        0     1850 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/drivers.py
--rw-r--r--   0        0        0     2277 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/examples.py
--rw-r--r--   0        0        0     1571 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/graph.py
--rw-r--r--   0        0        0     2341 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/init.py
--rw-r--r--   0        0        0     2642 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/install.py
--rw-r--r--   0        0        0     2035 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/lint.py
--rw-r--r--   0        0        0      530 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/raw.py
--rw-r--r--   0        0        0     1003 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/sim.py
--rw-r--r--   0        0        0     1913 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/system.py
--rw-r--r--   0        0        0     1233 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/test.py
--rw-r--r--   0        0        0     2631 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/time.py
--rw-r--r--   0        0        0     2382 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/uninstall.py
--rw-r--r--   0        0        0     1889 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/upgrade.py
--rw-r--r--   0        0        0     3944 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/upload.py
--rw-r--r--   0        0        0     1473 2024-04-02 17:40:48.537737 apio-0.9.3/apio/commands/verify.py
--rw-r--r--   0        0        0        0 2024-04-02 17:40:48.537737 apio-0.9.3/apio/managers/__init__.py
--rw-r--r--   0        0        0    12869 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/arguments.py
--rw-r--r--   0        0        0     3000 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/downloader.py
--rw-r--r--   0        0        0    17082 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/drivers.py
--rw-r--r--   0        0        0    10465 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/examples.py
--rw-r--r--   0        0        0    17535 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/installer.py
--rw-r--r--   0        0        0     7344 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/project.py
--rw-r--r--   0        0        0    35402 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/scons.py
--rw-r--r--   0        0        0     9638 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/system.py
--rw-r--r--   0        0        0     3798 2024-04-02 17:40:48.541737 apio-0.9.3/apio/managers/unpacker.py
--rw-r--r--   0        0        0     6051 2024-04-02 17:40:48.541737 apio-0.9.3/apio/profile.py
--rw-r--r--   0        0        0    14985 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources.py
--rw-r--r--   0        0        0     1225 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/80-fpga-ftdi.rules
--rw-r--r--   0        0        0      356 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/80-fpga-serial.rules
--rw-r--r--   0        0        0    15689 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/boards.json
--rw-r--r--   0        0        0      345 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/distribution.json
--rw-r--r--   0        0        0    13399 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/ecp5/SConstruct
--rw-r--r--   0        0        0     7638 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/fpgas.json
--rw-r--r--   0        0        0    13272 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/ice40/SConstruct
--rw-r--r--   0        0        0     1987 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/packages.json
--rw-r--r--   0        0        0     1639 2024-04-02 17:40:48.541737 apio-0.9.3/apio/resources/programmers.json
--rw-r--r--   0        0        0    25124 2024-04-02 17:40:48.541737 apio-0.9.3/apio/util.py
--rwxr-xr-x   0        0        0      517 2024-04-02 17:40:48.541737 apio-0.9.3/apio_run.py
--rw-r--r--   0        0        0     1182 2024-04-02 17:40:48.541737 apio-0.9.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/__init__.py
--rw-r--r--   0        0        0     9653 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_build.py
--rw-r--r--   0        0        0     1564 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_clean.py
--rw-r--r--   0        0        0      565 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_graph.py
--rw-r--r--   0        0        0      527 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_lint.py
--rw-r--r--   0        0        0      515 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_sim.py
--rw-r--r--   0        0        0      517 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_test.py
--rw-r--r--   0        0        0     1126 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_time.py
--rw-r--r--   0        0        0     3182 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_upload.py
--rw-r--r--   0        0        0      631 2024-04-02 17:40:48.581738 apio-0.9.3/test/code_commands/test_verify.py
--rw-r--r--   0        0        0     2665 2024-04-02 17:40:48.581738 apio-0.9.3/test/conftest.py
--rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/__init__.py
--rw-r--r--   0        0        0      754 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_boards.py
--rw-r--r--   0        0        0      769 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_config.py
--rw-r--r--   0        0        0      490 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_drivers.py
--rw-r--r--   0        0        0     1116 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_examples.py
--rw-r--r--   0        0        0     3964 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_init.py
--rw-r--r--   0        0        0      843 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_install.py
--rw-r--r--   0        0        0     1266 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_system.py
--rw-r--r--   0        0        0      949 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_uninstall.py
--rw-r--r--   0        0        0      657 2024-04-02 17:40:48.581738 apio-0.9.3/test/env_commands/test_upgrade.py
--rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test/packages/__init__.py
--rw-r--r--   0        0        0     8867 2024-04-02 17:40:48.581738 apio-0.9.3/test/packages/test_complete.py
--rw-r--r--   0        0        0     1741 2024-04-02 17:40:48.581738 apio-0.9.3/test/test_apio.py
--rw-r--r--   0        0        0        0 2024-04-02 17:40:48.581738 apio-0.9.3/test2/__init__.py
--rw-r--r--   0        0        0     2666 2024-04-02 17:40:48.581738 apio-0.9.3/test2/test_ledon.py
--rw-r--r--   0        0        0      268 2024-04-02 17:40:48.581738 apio-0.9.3/tox.ini
--rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 apio-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      938 2024-04-29 17:15:12.727241 apio-0.9.4/.github/workflows/Publish.yml
+-rw-r--r--   0        0        0      583 2024-04-29 17:15:12.727241 apio-0.9.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      330 2024-04-29 17:15:12.727241 apio-0.9.4/.gitignore
+-rw-r--r--   0        0        0     6379 2024-04-29 17:15:12.727241 apio-0.9.4/.vscode/launch.json
+-rw-r--r--   0        0        0    18047 2024-04-29 17:15:12.727241 apio-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1092 2024-04-29 17:15:12.727241 apio-0.9.4/Makefile
+-rw-r--r--   0        0        0     4683 2024-04-29 17:15:12.727241 apio-0.9.4/README.md
+-rw-r--r--   0        0        0      747 2024-04-29 17:15:12.727241 apio-0.9.4/apio/__init__.py
+-rw-r--r--   0        0        0     5752 2024-04-29 17:15:12.727241 apio-0.9.4/apio/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/boards.py
+-rw-r--r--   0        0        0     3160 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/build.py
+-rw-r--r--   0        0        0     1400 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/clean.py
+-rw-r--r--   0        0        0     1603 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/config.py
+-rw-r--r--   0        0        0     1850 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/drivers.py
+-rw-r--r--   0        0        0     2277 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/examples.py
+-rw-r--r--   0        0        0     1571 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/graph.py
+-rw-r--r--   0        0        0     2341 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/init.py
+-rw-r--r--   0        0        0     2642 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/install.py
+-rw-r--r--   0        0        0     2035 2024-04-29 17:15:12.727241 apio-0.9.4/apio/commands/lint.py
+-rw-r--r--   0        0        0      530 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/raw.py
+-rw-r--r--   0        0        0     1003 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/sim.py
+-rw-r--r--   0        0        0     1913 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/system.py
+-rw-r--r--   0        0        0     1233 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/test.py
+-rw-r--r--   0        0        0     2631 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/time.py
+-rw-r--r--   0        0        0     2382 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/uninstall.py
+-rw-r--r--   0        0        0     1889 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/upgrade.py
+-rw-r--r--   0        0        0     3944 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/upload.py
+-rw-r--r--   0        0        0     1473 2024-04-29 17:15:12.731241 apio-0.9.4/apio/commands/verify.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/__init__.py
+-rw-r--r--   0        0        0    12869 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/arguments.py
+-rw-r--r--   0        0        0     3000 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/downloader.py
+-rw-r--r--   0        0        0    17082 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/drivers.py
+-rw-r--r--   0        0        0    10465 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/examples.py
+-rw-r--r--   0        0        0    17535 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/installer.py
+-rw-r--r--   0        0        0     7344 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/project.py
+-rw-r--r--   0        0        0    35403 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/scons.py
+-rw-r--r--   0        0        0     9638 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/system.py
+-rw-r--r--   0        0        0     3798 2024-04-29 17:15:12.731241 apio-0.9.4/apio/managers/unpacker.py
+-rw-r--r--   0        0        0     6051 2024-04-29 17:15:12.731241 apio-0.9.4/apio/profile.py
+-rw-r--r--   0        0        0    14985 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources.py
+-rw-r--r--   0        0        0     1225 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/80-fpga-ftdi.rules
+-rw-r--r--   0        0        0      356 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/80-fpga-serial.rules
+-rw-r--r--   0        0        0    15689 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/boards.json
+-rw-r--r--   0        0        0      345 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/distribution.json
+-rw-r--r--   0        0        0    13399 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/ecp5/SConstruct
+-rw-r--r--   0        0        0     7638 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/fpgas.json
+-rw-r--r--   0        0        0    13272 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/ice40/SConstruct
+-rw-r--r--   0        0        0     1987 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/packages.json
+-rw-r--r--   0        0        0     1639 2024-04-29 17:15:12.731241 apio-0.9.4/apio/resources/programmers.json
+-rw-r--r--   0        0        0    25933 2024-04-29 17:15:12.731241 apio-0.9.4/apio/util.py
+-rwxr-xr-x   0        0        0      517 2024-04-29 17:15:12.731241 apio-0.9.4/apio_run.py
+-rw-r--r--   0        0        0     1182 2024-04-29 17:15:12.731241 apio-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 17:15:12.771241 apio-0.9.4/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/__init__.py
+-rw-r--r--   0        0        0     9653 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_build.py
+-rw-r--r--   0        0        0     1564 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_clean.py
+-rw-r--r--   0        0        0      565 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_graph.py
+-rw-r--r--   0        0        0      527 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_lint.py
+-rw-r--r--   0        0        0      515 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_sim.py
+-rw-r--r--   0        0        0      517 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_test.py
+-rw-r--r--   0        0        0     1126 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_time.py
+-rw-r--r--   0        0        0     3182 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_upload.py
+-rw-r--r--   0        0        0      631 2024-04-29 17:15:12.771241 apio-0.9.4/test/code_commands/test_verify.py
+-rw-r--r--   0        0        0     2665 2024-04-29 17:15:12.771241 apio-0.9.4/test/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/__init__.py
+-rw-r--r--   0        0        0      754 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_boards.py
+-rw-r--r--   0        0        0      769 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_config.py
+-rw-r--r--   0        0        0      490 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_drivers.py
+-rw-r--r--   0        0        0     1116 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_examples.py
+-rw-r--r--   0        0        0     3964 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_init.py
+-rw-r--r--   0        0        0      843 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_install.py
+-rw-r--r--   0        0        0     1266 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_system.py
+-rw-r--r--   0        0        0      949 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_uninstall.py
+-rw-r--r--   0        0        0      657 2024-04-29 17:15:12.771241 apio-0.9.4/test/env_commands/test_upgrade.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:15:12.771241 apio-0.9.4/test/packages/__init__.py
+-rw-r--r--   0        0        0     8867 2024-04-29 17:15:12.771241 apio-0.9.4/test/packages/test_complete.py
+-rw-r--r--   0        0        0     1741 2024-04-29 17:15:12.771241 apio-0.9.4/test/test_apio.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:15:12.771241 apio-0.9.4/test2/__init__.py
+-rw-r--r--   0        0        0     2666 2024-04-29 17:15:12.771241 apio-0.9.4/test2/test_ledon.py
+-rw-r--r--   0        0        0      268 2024-04-29 17:15:12.771241 apio-0.9.4/tox.ini
+-rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 apio-0.9.4/PKG-INFO
```

### Comparing `apio-0.9.3/.github/workflows/Publish.yml` & `apio-0.9.4/.github/workflows/Publish.yml`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/.github/workflows/build.yml` & `apio-0.9.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/.vscode/launch.json` & `apio-0.9.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/LICENSE` & `apio-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/Makefile` & `apio-0.9.4/Makefile`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/README.md` & `apio-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/__init__.py` & `apio-0.9.4/apio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # -- Licence GPLv2
 
 # --------------------------------------------
 # - Information for the Distribution package
 # --------------------------------------------
 
 # -- Developer: Change this number when releasing a new version
-VERSION = (0, 9, 3)
+VERSION = (0, 9, 4)
 
 # -- Get the version as a string. Ex: "0.10.1"
 __version__ = ".".join([str(s) for s in VERSION])
 
 __title__ = "apio"
 __description__ = "Open source ecosystem for open FPGA boards"
 __url__ = "https://github.com/FPGAwars/apio"
```

### Comparing `apio-0.9.3/apio/__main__.py` & `apio-0.9.4/apio/__main__.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/boards.py` & `apio-0.9.4/apio/commands/boards.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/build.py` & `apio-0.9.4/apio/commands/build.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/clean.py` & `apio-0.9.4/apio/commands/clean.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/config.py` & `apio-0.9.4/apio/commands/config.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/drivers.py` & `apio-0.9.4/apio/commands/drivers.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/examples.py` & `apio-0.9.4/apio/commands/examples.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/graph.py` & `apio-0.9.4/apio/commands/graph.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/init.py` & `apio-0.9.4/apio/commands/init.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/install.py` & `apio-0.9.4/apio/commands/install.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/lint.py` & `apio-0.9.4/apio/commands/lint.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/raw.py` & `apio-0.9.4/apio/commands/raw.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/sim.py` & `apio-0.9.4/apio/commands/sim.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/system.py` & `apio-0.9.4/apio/commands/system.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/test.py` & `apio-0.9.4/apio/commands/test.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/time.py` & `apio-0.9.4/apio/commands/time.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/uninstall.py` & `apio-0.9.4/apio/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/upgrade.py` & `apio-0.9.4/apio/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/upload.py` & `apio-0.9.4/apio/commands/upload.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/commands/verify.py` & `apio-0.9.4/apio/commands/verify.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/managers/arguments.py` & `apio-0.9.4/apio/managers/arguments.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/managers/downloader.py` & `apio-0.9.4/apio/managers/downloader.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/managers/drivers.py` & `apio-0.9.4/apio/managers/drivers.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/managers/examples.py` & `apio-0.9.4/apio/managers/examples.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/managers/installer.py` & `apio-0.9.4/apio/managers/installer.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/managers/project.py` & `apio-0.9.4/apio/managers/project.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/managers/scons.py` & `apio-0.9.4/apio/managers/scons.py`

 * *Files 0% similar despite different names*

```diff
@@ -942,15 +942,15 @@
             # -- Board name string in color
             board_color = click.style(processing_board, fg="cyan", bold=True)
 
             # -- Print information on the console
             click.echo(f"[{date_time_str}] Processing {board_color}")
 
             # -- Print a horizontal line
-            click.secho("─" * terminal_width, bold=True)
+            click.secho("-" * terminal_width, bold=True)
 
         # -- Command to execute: scons -Q apio_cmd flags
         scons_command = ["scons"] + ["-Q", command] + variables
 
         # -- Execute the scons builder!
         result = util.exec_command(
             scons_command,
@@ -967,25 +967,25 @@
         # -- Calculate the time it took to execute the command
         duration = time.time() - start_time
 
         # -- Summary
         summary_text = f" Took {duration:.2f} seconds "
 
         # -- Half line
-        half_line = "═" * int(((terminal_width - len(summary_text) - 10) / 2))
+        half_line = "=" * int(((terminal_width - len(summary_text) - 10) / 2))
 
         # -- Status message
         status = (
             click.style(" ERROR ", fg="red", bold=True)
             if is_error
             else click.style("SUCCESS", fg="green", bold=True)
         )
 
         # -- Print all the information!
-        click.echo(
+        util.safe_click(
             f"{half_line} [{status}]{summary_text}{half_line}",
             err=is_error,
         )
 
         # -- Return the exit code
         return exit_code
```

### Comparing `apio-0.9.3/apio/managers/system.py` & `apio-0.9.4/apio/managers/system.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/managers/unpacker.py` & `apio-0.9.4/apio/managers/unpacker.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/profile.py` & `apio-0.9.4/apio/profile.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/resources.py` & `apio-0.9.4/apio/resources.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/resources/80-fpga-ftdi.rules` & `apio-0.9.4/apio/resources/80-fpga-ftdi.rules`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/resources/boards.json` & `apio-0.9.4/apio/resources/boards.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/resources/ecp5/SConstruct` & `apio-0.9.4/apio/resources/ecp5/SConstruct`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/resources/fpgas.json` & `apio-0.9.4/apio/resources/fpgas.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/resources/ice40/SConstruct` & `apio-0.9.4/apio/resources/ice40/SConstruct`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/resources/packages.json` & `apio-0.9.4/apio/resources/packages.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/resources/programmers.json` & `apio-0.9.4/apio/resources/programmers.json`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/apio/util.py` & `apio-0.9.4/apio/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -881,7 +881,25 @@
 def context_settings():
     """Return a common Click command settings that adds
     the alias -h to --help
     """
     # Per https://click.palletsprojects.com/en/8.1.x/documentation/
     #     #help-parameter-customization
     return {"help_option_names": ["-h", "--help"]}
+
+
+def safe_click(text, *args, **kwargs):
+    """Prints text to the console handling potential Unicode errors,
+    forwarding any additional arguments to click.echo. This permits
+    avoid the need of setting encode environment variables for utf-8"""
+
+    error_flag = kwargs.pop("err", False)
+
+    try:
+        click.echo(text, err=error_flag, *args, **kwargs)
+    except UnicodeEncodeError:
+        cleaned_text = text.encode("ascii", errors="replace").decode("ascii")
+        # if encoding fails, after retry without errors , bad characters are
+        # replaced by '?' character, and is better replace for = because is the
+        # most common character error
+        cleaned_text = "".join([ch if ord(ch) < 128 else "=" for ch in text])
+        click.echo(cleaned_text, err=error_flag, *args, **kwargs)
```

### Comparing `apio-0.9.3/apio_run.py` & `apio-0.9.4/apio_run.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/pyproject.toml` & `apio-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_build.py` & `apio-0.9.4/test/code_commands/test_build.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_clean.py` & `apio-0.9.4/test/code_commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_graph.py` & `apio-0.9.4/test/code_commands/test_graph.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_lint.py` & `apio-0.9.4/test/code_commands/test_lint.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_sim.py` & `apio-0.9.4/test/code_commands/test_sim.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_test.py` & `apio-0.9.4/test/code_commands/test_test.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_time.py` & `apio-0.9.4/test/code_commands/test_time.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_upload.py` & `apio-0.9.4/test/code_commands/test_upload.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/code_commands/test_verify.py` & `apio-0.9.4/test/code_commands/test_verify.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/conftest.py` & `apio-0.9.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/env_commands/test_boards.py` & `apio-0.9.4/test/env_commands/test_boards.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/env_commands/test_config.py` & `apio-0.9.4/test/env_commands/test_config.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/env_commands/test_examples.py` & `apio-0.9.4/test/env_commands/test_examples.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/env_commands/test_init.py` & `apio-0.9.4/test/env_commands/test_init.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/env_commands/test_install.py` & `apio-0.9.4/test/env_commands/test_install.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/env_commands/test_system.py` & `apio-0.9.4/test/env_commands/test_system.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/env_commands/test_uninstall.py` & `apio-0.9.4/test/env_commands/test_uninstall.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/env_commands/test_upgrade.py` & `apio-0.9.4/test/env_commands/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/packages/test_complete.py` & `apio-0.9.4/test/packages/test_complete.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test/test_apio.py` & `apio-0.9.4/test/test_apio.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/test2/test_ledon.py` & `apio-0.9.4/test2/test_ledon.py`

 * *Files identical despite different names*

### Comparing `apio-0.9.3/PKG-INFO` & `apio-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apio
-Version: 0.9.3
+Version: 0.9.4
 Summary: Open source ecosystem for open FPGA boards
 Home-page: https://github.com/FPGAwars/apio
 Author: Jesus Arroyo
 Author-email: jesus.jkhlg@gmail.com 
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

