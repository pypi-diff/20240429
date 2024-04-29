# Comparing `tmp/aiida_flexpart-0.1.0.tar.gz` & `tmp/aiida_flexpart-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_flexpart-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_flexpart-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_flexpart-0.1.0.tar` & `aiida_flexpart-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0       28 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/.coveragerc
--rw-r--r--   0        0        0     1186 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/.github/check_version.py
--rwxr-xr-x   0        0        0      195 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/.github/install_aiida_github.sh
--rw-r--r--   0        0        0     1567 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      998 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/.github/workflows/publish-on-pypi.yml
--rw-r--r--   0        0        0      115 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/.gitignore
--rw-r--r--   0        0        0      906 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      119 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     1072 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/LICENSE
--rw-r--r--   0        0        0       35 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0     6516 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/README.md
--rw-r--r--   0        0        0      155 2024-04-10 09:39:41.493658 aiida_flexpart-0.1.0/aiida_flexpart/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/calculations/__init__.py
--rw-r--r--   0        0        0     7815 2024-04-10 09:34:44.662785 aiida_flexpart-0.1.0/aiida_flexpart/calculations/flexpart_cosmo.py
--rw-r--r--   0        0        0     7706 2024-02-21 10:19:53.749891 aiida_flexpart-0.1.0/aiida_flexpart/calculations/flexpart_ifs.py
--rw-r--r--   0        0        0     2307 2024-04-10 09:34:44.662785 aiida_flexpart-0.1.0/aiida_flexpart/calculations/flexpart_post.py
--rw-r--r--   0        0        0     2790 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/helpers.py
--rw-r--r--   0        0        0        0 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/parsers/__init__.py
--rw-r--r--   0        0        0     2088 2024-04-10 09:34:44.662785 aiida_flexpart-0.1.0/aiida_flexpart/parsers/flexpart_cosmo.py
--rw-r--r--   0        0        0     2189 2024-04-10 09:34:44.662785 aiida_flexpart-0.1.0/aiida_flexpart/parsers/flexpart_ifs.py
--rw-r--r--   0        0        0     1853 2024-04-10 09:34:44.672785 aiida_flexpart-0.1.0/aiida_flexpart/parsers/flexpart_post.py
--rw-r--r--   0        0        0      696 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/templates/AGECLASSES.j2
--rw-r--r--   0        0        0     8969 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/templates/COMMAND.j2
--rw-r--r--   0        0        0     8385 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/aiida_flexpart/templates/COMMAND_ifs.j2
--rw-r--r--   0        0        0     1837 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/templates/OUTGRID.j2
--rw-r--r--   0        0        0     1626 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/templates/OUTGRID_NEST.j2
--rw-r--r--   0        0        0     1419 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/aiida_flexpart/templates/OUTGRID_NEST_ifs.j2
--rw-r--r--   0        0        0     1630 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/aiida_flexpart/templates/OUTGRID_ifs.j2
--rw-r--r--   0        0        0     2506 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/templates/RELEASES.j2
--rw-r--r--   0        0        0        0 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/templates/__init__.py
--rw-r--r--   0        0        0    10080 2024-01-08 11:55:22.967945 aiida_flexpart-0.1.0/aiida_flexpart/utils.py
--rw-r--r--   0        0        0        0 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/aiida_flexpart/workflows/__init__.py
--rw-r--r--   0        0        0    13827 2024-04-10 09:34:44.672785 aiida_flexpart-0.1.0/aiida_flexpart/workflows/multi_dates_workflow.py
--rw-r--r--   0        0        0      737 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/config/code_bash_cosmo.yaml
--rw-r--r--   0        0        0      733 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/config/code_bash_ifs.yaml
--rw-r--r--   0        0        0      570 2024-01-12 08:49:27.452751 aiida_flexpart-0.1.0/config/code_flexpart_cosmo.yaml
--rw-r--r--   0        0        0      475 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/config/code_flexpart_ifs.yaml
--rw-r--r--   0        0        0      766 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/config/code_post_processing.yaml
--rw-r--r--   0        0        0      347 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/config/computer-daint-direct.yaml
--rw-r--r--   0        0        0      544 2024-01-12 08:49:27.452751 aiida_flexpart-0.1.0/config/computer-daint.yaml
--rw-r--r--   0        0        0      503 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/config/daint-configure.yaml
--rw-r--r--   0        0        0      558 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/conftest.py
--rw-r--r--   0        0        0        7 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/.gitignore
--rwxr-xr-x   0        0        0     1541 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/Makefile
--rwxr-xr-x   0        0        0    11696 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0     2828 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/source/developer_guide/index.rst
--rw-r--r--   0        0        0    76300 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/source/images/AiiDA_transparent_logo.png
--rwxr-xr-x   0        0        0     1296 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0     1280 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/source/user_guide/get_started.rst
--rw-r--r--   0        0        0       94 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0      243 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/docs/source/user_guide/tutorial.rst
--rw-r--r--   0        0        0     3842 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/examples/example_cosmo.py
--rw-r--r--   0        0        0     3716 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/examples/example_ifs.py
--rw-r--r--   0        0        0     4795 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/examples/example_workflow.py
--rw-r--r--   0        0        0     8049 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/examples/example_workflow_combi.py
--rw-r--r--   0        0        0     2310 2024-01-12 08:49:27.452751 aiida_flexpart-0.1.0/examples/inputs/command.yaml
--rw-r--r--   0        0        0      138 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/examples/inputs/input_phy.yaml
--rw-r--r--   0        0        0      638 2024-02-21 10:19:53.749891 aiida_flexpart-0.1.0/examples/inputs/location_groups.yaml
--rw-r--r--   0        0        0    10216 2024-02-21 10:19:53.749891 aiida_flexpart-0.1.0/examples/inputs/locations.yaml
--rw-r--r--   0        0        0      726 2024-01-08 11:25:26.863008 aiida_flexpart-0.1.0/examples/inputs/meteo_inputs.yaml
--rw-r--r--   0        0        0     3078 2024-02-21 10:19:53.749891 aiida_flexpart-0.1.0/examples/inputs/outgrid.yaml
--rw-r--r--   0        0        0      661 2024-01-08 11:25:20.013008 aiida_flexpart-0.1.0/examples/inputs/outgrid_nest.yaml
--rw-r--r--   0        0        0      108 2023-10-26 09:18:51.171533 aiida_flexpart-0.1.0/examples/inputs/release.yaml
--rw-r--r--   0        0        0     2325 2024-04-10 09:40:13.678752 aiida_flexpart-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7718 1970-01-01 00:00:00.000000 aiida_flexpart-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/.coveragerc
+-rw-r--r--   0        0        0     1186 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/.github/check_version.py
+-rwxr-xr-x   0        0        0      195 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/.github/install_aiida_github.sh
+-rw-r--r--   0        0        0     1567 2024-02-15 19:40:55.039407 aiida_flexpart-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      998 2024-02-15 19:40:55.039407 aiida_flexpart-0.1.1/.github/workflows/publish-on-pypi.yml
+-rw-r--r--   0        0        0      115 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/.gitignore
+-rw-r--r--   0        0        0      906 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      119 2024-02-15 19:40:55.039407 aiida_flexpart-0.1.1/.readthedocs.yml
+-rw-r--r--   0        0        0     1072 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/LICENSE
+-rw-r--r--   0        0        0       35 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     6516 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/README.md
+-rw-r--r--   0        0        0      155 2024-04-22 07:11:24.253085 aiida_flexpart-0.1.1/aiida_flexpart/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/aiida_flexpart/calculations/__init__.py
+-rw-r--r--   0        0        0     3333 2024-04-22 15:04:30.107137 aiida_flexpart-0.1.1/aiida_flexpart/calculations/collect_sens.py
+-rw-r--r--   0        0        0     7815 2024-02-29 19:05:13.960450 aiida_flexpart-0.1.1/aiida_flexpart/calculations/flexpart_cosmo.py
+-rw-r--r--   0        0        0     7706 2024-02-15 19:40:55.039407 aiida_flexpart-0.1.1/aiida_flexpart/calculations/flexpart_ifs.py
+-rw-r--r--   0        0        0     2320 2024-04-29 16:37:24.338024 aiida_flexpart-0.1.1/aiida_flexpart/calculations/flexpart_post.py
+-rw-r--r--   0        0        0     2790 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/aiida_flexpart/helpers.py
+-rw-r--r--   0        0        0        0 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/aiida_flexpart/parsers/__init__.py
+-rw-r--r--   0        0        0     2137 2024-04-22 07:11:24.253085 aiida_flexpart-0.1.1/aiida_flexpart/parsers/flexpart_cosmo.py
+-rw-r--r--   0        0        0     2038 2024-04-22 07:11:24.254085 aiida_flexpart-0.1.1/aiida_flexpart/parsers/flexpart_ifs.py
+-rw-r--r--   0        0        0     1853 2024-04-18 07:29:17.487089 aiida_flexpart-0.1.1/aiida_flexpart/parsers/flexpart_post.py
+-rw-r--r--   0        0        0      696 2023-12-06 19:22:02.013263 aiida_flexpart-0.1.1/aiida_flexpart/templates/AGECLASSES.j2
+-rw-r--r--   0        0        0     8969 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/aiida_flexpart/templates/COMMAND.j2
+-rw-r--r--   0        0        0     8385 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/aiida_flexpart/templates/COMMAND_ifs.j2
+-rw-r--r--   0        0        0     1837 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/aiida_flexpart/templates/OUTGRID.j2
+-rw-r--r--   0        0        0     1626 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/aiida_flexpart/templates/OUTGRID_NEST.j2
+-rw-r--r--   0        0        0     1419 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/aiida_flexpart/templates/OUTGRID_NEST_ifs.j2
+-rw-r--r--   0        0        0     1630 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/aiida_flexpart/templates/OUTGRID_ifs.j2
+-rw-r--r--   0        0        0     2506 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/aiida_flexpart/templates/RELEASES.j2
+-rw-r--r--   0        0        0        0 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/aiida_flexpart/templates/__init__.py
+-rw-r--r--   0        0        0    10080 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/aiida_flexpart/utils.py
+-rw-r--r--   0        0        0        0 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/aiida_flexpart/workflows/__init__.py
+-rw-r--r--   0        0        0    15099 2024-04-29 07:24:12.524047 aiida_flexpart-0.1.1/aiida_flexpart/workflows/multi_dates_workflow.py
+-rw-r--r--   0        0        0      737 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/config/code_bash_cosmo.yaml
+-rw-r--r--   0        0        0      733 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/config/code_bash_ifs.yaml
+-rw-r--r--   0        0        0      570 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/config/code_flexpart_cosmo.yaml
+-rw-r--r--   0        0        0      475 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/config/code_flexpart_ifs.yaml
+-rw-r--r--   0        0        0      766 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/config/code_post_processing.yaml
+-rw-r--r--   0        0        0      347 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/config/computer-daint-direct.yaml
+-rw-r--r--   0        0        0      544 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/config/computer-daint.yaml
+-rw-r--r--   0        0        0      503 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/config/daint-configure.yaml
+-rw-r--r--   0        0        0      570 2024-04-22 07:11:24.254085 aiida_flexpart-0.1.1/config/params.yaml
+-rw-r--r--   0        0        0      558 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/conftest.py
+-rw-r--r--   0        0        0        7 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/docs/.gitignore
+-rwxr-xr-x   0        0        0     1541 2023-12-06 19:22:02.014263 aiida_flexpart-0.1.1/docs/Makefile
+-rwxr-xr-x   0        0        0    11696 2023-12-06 19:22:02.015263 aiida_flexpart-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0     2828 2023-12-06 19:22:02.015263 aiida_flexpart-0.1.1/docs/source/developer_guide/index.rst
+-rw-r--r--   0        0        0    76300 2023-12-06 19:22:02.015263 aiida_flexpart-0.1.1/docs/source/images/AiiDA_transparent_logo.png
+-rwxr-xr-x   0        0        0     1296 2023-12-06 19:22:02.015263 aiida_flexpart-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1280 2023-12-06 19:22:02.016263 aiida_flexpart-0.1.1/docs/source/user_guide/get_started.rst
+-rw-r--r--   0        0        0       94 2023-12-06 19:22:02.016263 aiida_flexpart-0.1.1/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0      243 2023-12-06 19:22:02.016263 aiida_flexpart-0.1.1/docs/source/user_guide/tutorial.rst
+-rw-r--r--   0        0        0     3842 2023-12-07 14:02:10.748042 aiida_flexpart-0.1.1/examples/example_cosmo.py
+-rw-r--r--   0        0        0     3716 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/examples/example_ifs.py
+-rw-r--r--   0        0        0     4795 2023-12-06 19:22:02.016263 aiida_flexpart-0.1.1/examples/example_workflow.py
+-rw-r--r--   0        0        0     8049 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/examples/example_workflow_combi.py
+-rw-r--r--   0        0        0     2310 2024-02-15 19:40:49.656331 aiida_flexpart-0.1.1/examples/inputs/command.yaml
+-rw-r--r--   0        0        0      138 2023-12-06 19:22:02.016263 aiida_flexpart-0.1.1/examples/inputs/input_phy.yaml
+-rw-r--r--   0        0        0      638 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/examples/inputs/location_groups.yaml
+-rw-r--r--   0        0        0    10216 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/examples/inputs/locations.yaml
+-rw-r--r--   0        0        0      726 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/examples/inputs/meteo_inputs.yaml
+-rw-r--r--   0        0        0     3078 2024-02-15 19:40:55.040407 aiida_flexpart-0.1.1/examples/inputs/outgrid.yaml
+-rw-r--r--   0        0        0      661 2024-02-15 19:40:49.656331 aiida_flexpart-0.1.1/examples/inputs/outgrid_nest.yaml
+-rw-r--r--   0        0        0      108 2023-12-06 19:22:02.016263 aiida_flexpart-0.1.1/examples/inputs/release.yaml
+-rw-r--r--   0        0        0     2426 2024-04-29 07:21:54.815869 aiida_flexpart-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7718 1970-01-01 00:00:00.000000 aiida_flexpart-0.1.1/PKG-INFO
```

### Comparing `aiida_flexpart-0.1.0/.github/check_version.py` & `aiida_flexpart-0.1.1/.github/check_version.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/.github/workflows/ci.yml` & `aiida_flexpart-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/.github/workflows/publish-on-pypi.yml` & `aiida_flexpart-0.1.1/.github/workflows/publish-on-pypi.yml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/.pre-commit-config.yaml` & `aiida_flexpart-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/LICENSE` & `aiida_flexpart-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/README.md` & `aiida_flexpart-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/calculations/flexpart_cosmo.py` & `aiida_flexpart-0.1.1/aiida_flexpart/calculations/flexpart_cosmo.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/calculations/flexpart_ifs.py` & `aiida_flexpart-0.1.1/aiida_flexpart/calculations/flexpart_ifs.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/calculations/flexpart_post.py` & `aiida_flexpart-0.1.1/aiida_flexpart/calculations/flexpart_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,24 +32,24 @@
         #exit codes
         spec.outputs.dynamic = True
         spec.exit_code(300, 'ERROR_MISSING_OUTPUT_FILES', message='Calculation did not produce all expected output files.')
 
     def prepare_for_submission(self, folder):
 
         params  = ['-m',self.inputs.input_dir.get_remote_path(),
-                   '-r','./'
+                   '-r','./','-p'
                   ]
         if 'input_offline_dir' in self.inputs:
             params += ['-n',self.inputs.input_offline_dir.get_remote_path()]
 
         codeinfo = common.CodeInfo()
         codeinfo.cmdline_params = params
         codeinfo.code_uuid = self.inputs.code.uuid
         codeinfo.stdout_name = self.metadata.options.output_filename
         codeinfo.withmpi = self.inputs.metadata.options.withmpi
 
         # Prepare a `CalcInfo` to be returned to the engine
         calcinfo = common.CalcInfo()
         calcinfo.codes_info = [codeinfo]
-        calcinfo.retrieve_list = ['grid_time_*.nc', 'boundary_sensitivity_*.nc', 'aiida.out']
+        calcinfo.retrieve_list = ['grid_time_*.nc', 'boundary_sensitivity_*.nc','*.png', 'aiida.out']
 
         return calcinfo
```

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/helpers.py` & `aiida_flexpart-0.1.1/aiida_flexpart/helpers.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/parsers/flexpart_cosmo.py` & `aiida_flexpart-0.1.1/aiida_flexpart/parsers/flexpart_cosmo.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
             self.logger.error("Found files '{}', expected to find '{}'".format(
                 files_retrieved, files_expected))
             return self.exit_codes.ERROR_MISSING_OUTPUT_FILES
 
         # add output file
         self.logger.info(f"Parsing '{output_filename}'")
         with self.retrieved.open(output_filename, 'r') as handle:
-            output_node = SinglefileData(file=handle)
-            self.out('output_file', output_node)
             content = handle.read()
+            output_node = SinglefileData(file=handle)
             if 'CONGRATULATIONS' not in content:
+                self.out('output_file', output_node)
                 return ExitCode(1)
 
+        self.out('output_file', output_node)
         return ExitCode(0)
```

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/parsers/flexpart_ifs.py` & `aiida_flexpart-0.1.1/aiida_flexpart/parsers/flexpart_ifs.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,20 +41,17 @@
         if not set(files_expected) <= set(files_retrieved):
             self.logger.error(
                 f"Found files '{files_retrieved}', expected to find '{files_expected}'"
             )
             return self.exit_codes.ERROR_MISSING_OUTPUT_FILES
 
         # check aiida.out content
+        self.logger.info(f"Parsing '{output_filename}'")
         with self.retrieved.open(output_filename, 'r') as handle:
             content = handle.read()
             output_node = orm.SinglefileData(file=handle)
             if 'CONGRATULATIONS' not in content:
                 self.out('output_file', output_node)
                 return engine.ExitCode(1)
-        # add output file
-        self.logger.info(f"Parsing '{output_filename}'")
-        with self.retrieved.open(output_filename, 'rb') as handle:
-            output_node = orm.SinglefileData(file=handle)
-        self.out('output_file', output_node)
 
+        self.out('output_file', output_node)
         return engine.ExitCode(0)
```

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/parsers/flexpart_post.py` & `aiida_flexpart-0.1.1/aiida_flexpart/parsers/flexpart_post.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/templates/AGECLASSES.j2` & `aiida_flexpart-0.1.1/aiida_flexpart/templates/AGECLASSES.j2`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/templates/COMMAND.j2` & `aiida_flexpart-0.1.1/aiida_flexpart/templates/COMMAND.j2`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/templates/COMMAND_ifs.j2` & `aiida_flexpart-0.1.1/aiida_flexpart/templates/COMMAND_ifs.j2`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/templates/OUTGRID.j2` & `aiida_flexpart-0.1.1/aiida_flexpart/templates/OUTGRID.j2`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/templates/OUTGRID_NEST.j2` & `aiida_flexpart-0.1.1/aiida_flexpart/templates/OUTGRID_NEST.j2`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/templates/OUTGRID_NEST_ifs.j2` & `aiida_flexpart-0.1.1/aiida_flexpart/templates/OUTGRID_NEST_ifs.j2`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/templates/OUTGRID_ifs.j2` & `aiida_flexpart-0.1.1/aiida_flexpart/templates/OUTGRID_ifs.j2`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/templates/RELEASES.j2` & `aiida_flexpart-0.1.1/aiida_flexpart/templates/RELEASES.j2`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/utils.py` & `aiida_flexpart-0.1.1/aiida_flexpart/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/aiida_flexpart/workflows/multi_dates_workflow.py` & `aiida_flexpart-0.1.1/aiida_flexpart/workflows/multi_dates_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         #codes
         spec.input('fcosmo_code', valid_type=orm.AbstractCode)
         spec.input('check_meteo_cosmo_code', valid_type=orm.AbstractCode)
         spec.input('fifs_code', valid_type=orm.AbstractCode)
         spec.input('check_meteo_ifs_code', valid_type=orm.AbstractCode)
         spec.input('post_processing_code', valid_type=orm.AbstractCode)
 
+        #extras
+        spec.input('name', valid_type=str, non_db=True, required=False)
+
         # Basic Inputs
         spec.input('simulation_dates',
                    valid_type=orm.List,
                    help='A list of the starting dates of the simulations')
         spec.input('model', valid_type=orm.List, required=True)
         spec.input('model_offline', valid_type=orm.List, required=True)
         spec.input('offline_integration_time', valid_type=orm.Int)
@@ -104,18 +107,20 @@
         # Outputs
         #spec.output('output_file', valid_type=orm.SinglefileData)
         spec.outputs.dynamic = True
         # What the workflow will do, step-by-step
         spec.outline(
             cls.setup,
             engine.while_(cls.condition)(
-                engine.if_(cls.run_cosmo)(engine.if_(
-                    cls.prepare_meteo_folder_cosmo)(cls.run_cosmo_simulation)),
-                engine.if_(cls.run_ifs)(engine.if_(
-                    cls.prepare_meteo_folder_ifs)(cls.run_ifs_simulation)),
+                engine.if_(cls.run_cosmo)(
+                    engine.if_(cls.prepare_meteo_folder_cosmo)(
+                        cls.run_cosmo_simulation)),
+                engine.if_(cls.run_ifs)(
+                    engine.if_(cls.prepare_meteo_folder_ifs)(
+                        cls.run_ifs_simulation)),
                 cls.post_processing,
             ),
             cls.results,
         )
 
     def condition(self):
         """multi dates loop"""
@@ -153,14 +158,32 @@
         self.ctx.input_phy = self.inputs.input_phy
         self.ctx.locations = self.inputs.locations
 
         #others
         self.ctx.outgrid = self.inputs.outgrid
         self.ctx.species = self.inputs.species
         self.ctx.land_use = self.inputs.land_use
+        if 'name' in self.inputs:
+            out_n = 'None'
+            if 'outgrid_nest' in self.inputs:
+                out_n = self.inputs.outgrid_nest.get_dict()
+            self.node.base.extras.set(
+                self.inputs.name, {
+                    'command': self.ctx.command.get_dict(),
+                    'input_phy': self.ctx.input_phy.get_dict(),
+                    'release': self.ctx.release_settings.get_dict(),
+                    'locations': self.ctx.locations.get_dict(),
+                    'integration_time': self.ctx.integration_time.value,
+                    'offline_integration_time':
+                    self.ctx.offline_integration_time.value,
+                    'model': self.inputs.model,
+                    'model_offline': self.inputs.model_offline,
+                    'outgrid': self.inputs.outgrid.get_dict(),
+                    'outgrid_nest': out_n
+                })
 
     def prepare_meteo_folder_ifs(self):
         """prepare meteo folder"""
         age_class_ = self.inputs.integration_time.value * 3600
         if self.ctx.offline_integration_time > 0:
             age_class_ = self.inputs.offline_integration_time.value * 3600
         e_date, s_date = get_simulation_period(
@@ -271,17 +294,19 @@
         builder.model_settings = {
             'release_settings': self.ctx.release_settings,
             'locations': self.ctx.locations,
             'command': orm.Dict(dict=new_dict),
             'input_phy': self.ctx.input_phy,
         }
 
-        builder.outgrid = self.ctx.outgrid
+        builder.outgrid = orm.Dict(
+            list(self.ctx.outgrid.get_dict().values())[0])
         if 'outgrid_nest' in self.inputs:
-            builder.outgrid_nest = self.inputs.outgrid_nest
+            builder.outgrid_nest = orm.Dict(
+                list(self.inputs.outgrid_nest.get_dict().values())[0])
         builder.species = self.ctx.species
         builder.land_use = self.ctx.land_use
         builder.meteo_path = self.inputs.meteo_path
 
         # Walltime, memory, and resources.
         builder.metadata.description = 'Test workflow to submit a flexpart calculation'
         builder.metadata.options = self.inputs.flexpartcosmo.metadata.options
@@ -325,17 +350,19 @@
         #model settings
         builder.model_settings = {
             'release_settings': self.ctx.release_settings,
             'locations': self.ctx.locations,
             'command': orm.Dict(dict=new_dict),
         }
 
-        builder.outgrid = self.ctx.outgrid
+        builder.outgrid = orm.Dict(
+            list(self.ctx.outgrid.get_dict().values())[0])
         if 'outgrid_nest' in self.inputs:
-            builder.outgrid_nest = self.inputs.outgrid_nest
+            builder.outgrid_nest = orm.Dict(
+                list(self.inputs.outgrid_nest.get_dict().values())[0])
         builder.species = self.ctx.species
         builder.land_use = self.inputs.land_use_ifs
 
         # Walltime, memory, and resources.
         builder.metadata.description = 'Test workflow to submit a flexpart calculation'
         builder.metadata.options = self.inputs.flexpartifs.metadata.options
```

### Comparing `aiida_flexpart-0.1.0/config/code_bash_cosmo.yaml` & `aiida_flexpart-0.1.1/config/code_bash_cosmo.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/config/code_bash_ifs.yaml` & `aiida_flexpart-0.1.1/config/code_bash_ifs.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/config/code_flexpart_cosmo.yaml` & `aiida_flexpart-0.1.1/config/code_flexpart_cosmo.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/config/code_post_processing.yaml` & `aiida_flexpart-0.1.1/config/code_post_processing.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/config/computer-daint.yaml` & `aiida_flexpart-0.1.1/config/computer-daint.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/conftest.py` & `aiida_flexpart-0.1.1/conftest.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/docs/Makefile` & `aiida_flexpart-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/docs/source/conf.py` & `aiida_flexpart-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/docs/source/developer_guide/index.rst` & `aiida_flexpart-0.1.1/docs/source/developer_guide/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/docs/source/images/AiiDA_transparent_logo.png` & `aiida_flexpart-0.1.1/docs/source/images/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/docs/source/index.rst` & `aiida_flexpart-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/docs/source/user_guide/get_started.rst` & `aiida_flexpart-0.1.1/docs/source/user_guide/get_started.rst`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/example_cosmo.py` & `aiida_flexpart-0.1.1/examples/example_cosmo.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/example_ifs.py` & `aiida_flexpart-0.1.1/examples/example_ifs.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/example_workflow.py` & `aiida_flexpart-0.1.1/examples/example_workflow.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/example_workflow_combi.py` & `aiida_flexpart-0.1.1/examples/example_workflow_combi.py`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/inputs/command.yaml` & `aiida_flexpart-0.1.1/examples/inputs/command.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/inputs/location_groups.yaml` & `aiida_flexpart-0.1.1/examples/inputs/location_groups.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/inputs/locations.yaml` & `aiida_flexpart-0.1.1/examples/inputs/locations.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/inputs/meteo_inputs.yaml` & `aiida_flexpart-0.1.1/examples/inputs/meteo_inputs.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/inputs/outgrid.yaml` & `aiida_flexpart-0.1.1/examples/inputs/outgrid.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/examples/inputs/outgrid_nest.yaml` & `aiida_flexpart-0.1.1/examples/inputs/outgrid_nest.yaml`

 * *Files identical despite different names*

### Comparing `aiida_flexpart-0.1.0/pyproject.toml` & `aiida_flexpart-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [tool.flit.module]
 name = "aiida_flexpart"
 
 [project]
 name = "aiida-flexpart"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = {file = 'LICENSE'}
 description = "AiiDA plugin for the FLEXPART code (simulation of atmospheric transport processes)."
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
@@ -51,14 +51,15 @@
     "sphinx-rtd-theme",
 ]
 
 [project.entry-points."aiida.calculations"]
 "flexpart.cosmo" = "aiida_flexpart.calculations.flexpart_cosmo:FlexpartCosmoCalculation"
 "flexpart.ifs" = "aiida_flexpart.calculations.flexpart_ifs:FlexpartIfsCalculation"
 "flexpart.post" = "aiida_flexpart.calculations.flexpart_post:PostProcessingCalculation"
+"collect.sensitivities" = "aiida_flexpart.calculations.collect_sens:CollectSensitivitiesCalculation"
 
 [project.entry-points."aiida.parsers"]
 "flexpart.cosmo" = "aiida_flexpart.parsers.flexpart_cosmo:FlexpartCosmoParser"
 "flexpart.ifs" = "aiida_flexpart.parsers.flexpart_ifs:FlexpartIfsParser"
 "flexpart.post" = "aiida_flexpart.parsers.flexpart_post:FlexpartPostParser"
 
 [project.entry-points."aiida.workflows"]
```

### Comparing `aiida_flexpart-0.1.0/PKG-INFO` & `aiida_flexpart-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-flexpart
-Version: 0.1.0
+Version: 0.1.1
 Summary: AiiDA plugin for the FLEXPART code (simulation of atmospheric transport processes).
 Author: 
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

