# Comparing `tmp/ansys_optislang_core-0.6.3.tar.gz` & `tmp/ansys_optislang_core-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_optislang_core-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_optislang_core-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_optislang_core-0.6.3.tar` & `ansys_optislang_core-0.7.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1089 2024-03-20 11:09:00.900567 ansys_optislang_core-0.6.3/LICENSE
--rw-r--r--   0        0        0     7415 2024-03-20 11:09:00.900567 ansys_optislang_core-0.6.3/README.rst
--rw-r--r--   0        0        0     2286 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     2527 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/__init__.py
--rw-r--r--   0        0        0     7107 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/application.py
--rw-r--r--   0        0        0     3328 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/encoding.py
--rw-r--r--   0        0        0     2100 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/errors.py
--rw-r--r--   0        0        0     2250 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp
--rw-r--r--   0        0        0   235264 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb
--rw-r--r--   0        0        0     3813 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py
--rw-r--r--   0        0        0    28174 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf
--rw-r--r--   0        0        0    73304 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf
--rw-r--r--   0        0        0    25280 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf
--rw-r--r--   0        0        0    47797 2024-03-20 11:09:00.908567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf
--rw-r--r--   0        0        0   146518 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/omdb_files.opf
--rw-r--r--   0        0        0   212239 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf
--rw-r--r--   0        0        0      299 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.bat
--rw-r--r--   0        0        0     2966 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py
--rw-r--r--   0        0        0     4438 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s
--rw-r--r--   0        0        0      194 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.sh
--rw-r--r--   0        0        0     1401 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt
--rw-r--r--   0        0        0     1989 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt
--rw-r--r--   0        0        0     4596 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py
--rw-r--r--   0        0        0     4081 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py
--rw-r--r--   0        0        0     5483 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py
--rw-r--r--   0        0        0     5002 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py
--rw-r--r--   0        0        0     4428 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py
--rw-r--r--   0        0        0     4992 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py
--rw-r--r--   0        0        0    10784 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py
--rw-r--r--   0        0        0     7325 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py
--rw-r--r--   0        0        0     1629 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py
--rw-r--r--   0        0        0     3755 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py
--rw-r--r--   0        0        0     2405 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py
--rw-r--r--   0        0        0     1906 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py
--rw-r--r--   0        0        0     2521 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py
--rw-r--r--   0        0        0     1780 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py
--rw-r--r--   0        0        0     5243 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py
--rw-r--r--   0        0        0     2872 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac
--rw-r--r--   0        0        0      686 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out
--rw-r--r--   0        0        0    10909 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s
--rw-r--r--   0        0        0      686 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out
--rw-r--r--   0        0        0    10785 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s
--rw-r--r--   0        0        0    34914 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz
--rw-r--r--   0        0        0     3222 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py
--rw-r--r--   0        0        0     6443 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py
--rw-r--r--   0        0        0     2164 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py
--rw-r--r--   0        0        0     5697 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py
--rw-r--r--   0        0        0     1240 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/__init__.py
--rw-r--r--   0        0        0     3090 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/downloads.py
--rw-r--r--   0        0        0     7119 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/examples.py
--rw-r--r--   0        0        0     7816 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/io.py
--rw-r--r--   0        0        0    10077 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/logging.py
--rw-r--r--   0        0        0    12455 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/managers.py
--rw-r--r--   0        0        0    30303 2024-03-20 11:09:00.912567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/node_types.py
--rw-r--r--   0        0        0    52873 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/nodes.py
--rw-r--r--   0        0        0    36757 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/optislang.py
--rw-r--r--   0        0        0    42940 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/osl_process.py
--rw-r--r--   0        0        0     5738 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/osl_server.py
--rw-r--r--   0        0        0    13914 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/project.py
--rw-r--r--   0        0        0   132757 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/project_parametric.py
--rw-r--r--   0        0        0     8562 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/application.py
--rw-r--r--   0        0        0    20317 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/managers.py
--rw-r--r--   0        0        0   115198 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/nodes.py
--rw-r--r--   0        0        0   172888 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/osl_server.py
--rw-r--r--   0        0        0    20093 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/project.py
--rw-r--r--   0        0        0    58732 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/server_commands.py
--rw-r--r--   0        0        0    20854 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/server_queries.py
--rw-r--r--   0        0        0    16155 2024-03-20 11:09:00.916567 ansys_optislang_core-0.6.3/src/ansys/optislang/core/utils.py
--rw-r--r--   0        0        0     9143 1970-01-01 00:00:00.000000 ansys_optislang_core-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-29 09:33:35.871300 ansys_optislang_core-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7471 2024-04-29 09:33:35.871300 ansys_optislang_core-0.7.0/README.rst
+-rw-r--r--   0        0        0     2253 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2198 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/__init__.py
+-rw-r--r--   0        0        0     7292 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/application.py
+-rw-r--r--   0        0        0     3328 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/encoding.py
+-rw-r--r--   0        0        0     2100 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/errors.py
+-rw-r--r--   0        0        0     2250 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp
+-rw-r--r--   0        0        0   235264 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb
+-rw-r--r--   0        0        0     3813 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py
+-rw-r--r--   0        0        0    28174 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf
+-rw-r--r--   0        0        0    73304 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf
+-rw-r--r--   0        0        0    25280 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf
+-rw-r--r--   0        0        0    47797 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf
+-rw-r--r--   0        0        0   146518 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/omdb_files.opf
+-rw-r--r--   0        0        0   212239 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf
+-rw-r--r--   0        0        0      299 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.bat
+-rw-r--r--   0        0        0     2966 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py
+-rw-r--r--   0        0        0     4438 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s
+-rw-r--r--   0        0        0      194 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.sh
+-rw-r--r--   0        0        0     1401 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt
+-rw-r--r--   0        0        0     1989 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt
+-rw-r--r--   0        0        0     4596 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py
+-rw-r--r--   0        0        0     4081 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py
+-rw-r--r--   0        0        0     5483 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py
+-rw-r--r--   0        0        0     5002 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py
+-rw-r--r--   0        0        0     4428 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py
+-rw-r--r--   0        0        0     4992 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py
+-rw-r--r--   0        0        0    10784 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py
+-rw-r--r--   0        0        0     7325 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py
+-rw-r--r--   0        0        0     1629 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py
+-rw-r--r--   0        0        0     3755 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py
+-rw-r--r--   0        0        0     2405 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py
+-rw-r--r--   0        0        0     1906 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py
+-rw-r--r--   0        0        0     2521 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py
+-rw-r--r--   0        0        0     1780 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py
+-rw-r--r--   0        0        0     5243 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py
+-rw-r--r--   0        0        0     2872 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac
+-rw-r--r--   0        0        0      686 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out
+-rw-r--r--   0        0        0    10909 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s
+-rw-r--r--   0        0        0      686 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out
+-rw-r--r--   0        0        0    10785 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s
+-rw-r--r--   0        0        0    34914 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz
+-rw-r--r--   0        0        0     3222 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py
+-rw-r--r--   0        0        0     6443 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py
+-rw-r--r--   0        0        0     2164 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py
+-rw-r--r--   0        0        0     5697 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py
+-rw-r--r--   0        0        0     1240 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/__init__.py
+-rw-r--r--   0        0        0     3090 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/downloads.py
+-rw-r--r--   0        0        0     7119 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/examples.py
+-rw-r--r--   0        0        0     7808 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/io.py
+-rw-r--r--   0        0        0    10077 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/logging.py
+-rw-r--r--   0        0        0    12455 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/managers.py
+-rw-r--r--   0        0        0    30303 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/node_types.py
+-rw-r--r--   0        0        0    52843 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/nodes.py
+-rw-r--r--   0        0        0    36959 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/optislang.py
+-rw-r--r--   0        0        0    42928 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/osl_process.py
+-rw-r--r--   0        0        0     5738 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/osl_server.py
+-rw-r--r--   0        0        0    13918 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/project.py
+-rw-r--r--   0        0        0   132646 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/project_parametric.py
+-rw-r--r--   0        0        0     8922 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/application.py
+-rw-r--r--   0        0        0    20317 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/managers.py
+-rw-r--r--   0        0        0   116145 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/nodes.py
+-rw-r--r--   0        0        0   178734 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/osl_server.py
+-rw-r--r--   0        0        0    20093 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/project.py
+-rw-r--r--   0        0        0    59114 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/server_commands.py
+-rw-r--r--   0        0        0    25617 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/server_queries.py
+-rw-r--r--   0        0        0    16155 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/utils.py
+-rw-r--r--   0        0        0     9157 1970-01-01 00:00:00.000000 ansys_optislang_core-0.7.0/PKG-INFO
```

### Comparing `ansys_optislang_core-0.6.3/LICENSE` & `ansys_optislang_core-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/README.rst` & `ansys_optislang_core-0.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 ===========
 |pyansys| |python| |pypi| |PyPIact| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.7-blue
-   :target: https://pypi.org/project/pyoptislang/
+.. |python| image:: https://img.shields.io/pypi/pyversions/ansys-optislang-core?logo=pypi
+   :target: https://pypi.org/project/ansys-optislang-core/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-optislang-core.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-optislang-core/
 
 .. |PyPIact| image:: https://img.shields.io/pypi/dm/ansys-optislang-core.svg?label=PyPI%20downloads
    :target: https://pypi.org/project/ansys-optislang-core/
@@ -43,27 +43,28 @@
 - Remote connections to Ansys optiSLang instances via TCP/IP
 - Create new Ansys optiSLang project
 - Open existing Ansys optiSLang project
 - Control Ansys optiSLang project execution
 - Save Ansys optiSLang project
 - Execute classic Ansys optiSLang Python API script on backend side
 - Evaluate designs on root project level
+- Create and connect nodes
 
 
 Documentation and issues
 ------------------------
 For comprehensive information on PyOptiSLang, see the latest release
 `documentation <https://optislang.docs.pyansys.com>`_. On the
 `PyOptiSLang Issues <https://github.com/ansys/pyoptislang/issues>`_ page,
 you can create issues to submit questions, report bugs, and request new features.
 This is the best place to post questions and code.
 
 Installation
 ------------
-The ``ansys-optislang-core`` package supports Python 3.7 through 3.11 on
+The ``ansys-optislang-core`` package supports Python 3.8 through 3.12 on
 Windows and Linux. Three modes of installation are available:
 
 - User installation
 - Developer installation
 - Offline installation
 
 For either a developer or offline installation, consider using a `virtual environment
@@ -109,20 +110,20 @@
 external networks. From the `Releases <https://github.com/ansys/pyoptislang/releases>`_
 page in the PyOptiSLang repository, you can find the wheelhouses for a particular release in its
 assets and download the wheelhouse corresponding to your setup.
 
 You can then install PyOptiSLang and all of its dependencies from one single entry point
 that can be shared internally, which eases the security review of the PyOptiSLang package content.
 
-For example, on Linux with Python 3.7, unzip the wheelhouse and install PyOptiSLang with code
+For example, on Linux with Python 3.8, unzip the wheelhouse and install PyOptiSLang with code
 like this:
 
 .. code:: bash
 
-    unzip PyOptiSLang-v0.1.0-wheelhouse-Linux-3.7.zip wheelhouse
+    unzip PyOptiSLang-v0.1.0-wheelhouse-Linux-3.8.zip wheelhouse
     pip install ansys-optislang-core -f wheelhouse --no-index --upgrade --ignore-installed
 
 If you're on Windows with Python 3.9, unzip the wheelhouse to a wheelhouse directory and
 then install using the same ``pip`` command as in the preceding Linux code example.
 
 Dependencies
 --------------
```

### Comparing `ansys_optislang_core-0.6.3/pyproject.toml` & `ansys_optislang_core-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-optislang-core"
-version = "0.6.3"
+version = "0.7.0"
 description = "A Python wrapper for Ansys optiSLang application."
 readme = "README.rst"
-requires-python = ">=3.7,<4"
+requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"},
 ]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "importlib-metadata>=4.0,<8",
     "psutil>=5.9",
     "Deprecated>=1.2.14",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.4.4",
-    "pytest-cov==4.1.0",
+    "pytest==8.1.2",
+    "pytest-cov==5.0.0",
     "matplotlib>=3.5.3",
 ]
 doc = [
-    "ansys-sphinx-theme==0.13.1",
-    "matplotlib==3.8.2",
-    "numpydoc==1.6.0",
-    "pypandoc==1.12",
+    "ansys-sphinx-theme==0.15.2",
+    "matplotlib==3.8.4",
+    "numpydoc==1.7.0",
+    "pypandoc==1.13",
     "Sphinx==7.2.6",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.15.0",
     "sphinxcontrib-images==0.9.4",
 ]
 build = [
     "build>=0.8.0",
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/__init__.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,49 +22,36 @@
 
 """
 optiSLang.
 
 core
 """
 
+import importlib.metadata
+import importlib.util
 import os
 import sys
 
-try:
-    import importlib.metadata as importlib_metadata
-except ModuleNotFoundError:
-    import importlib_metadata
-
 from ansys.optislang.core.logging import OslLogger
 
 LOG = OslLogger(loglevel="ERROR", log_to_file=False, log_to_stdout=True)
 LOG.logger.debug("Loaded logging module as LOG")
 
-__version__ = importlib_metadata.version(__name__.replace(".", "-"))
+__version__ = importlib.metadata.version(__name__.replace(".", "-"))
 
 IRON_PYTHON = sys.platform == "cli"
-WINDOWS = os.name == "nt"
-LINUX = os.name == "posix"
 PY3 = sys.version_info[0] >= 3
 # First supported version of optiSLang: 2023R1
 FIRST_SUPPORTED_VERSION = 231
 
 from ansys.optislang.core.optislang import Optislang
 from ansys.optislang.core.osl_process import OslServerProcess, ServerNotification
 
-# Setup data directory
-USER_DATA_PATH = None
-LOCAL_DOWNLOADED_EXAMPLES_PATH = None
-try:
-    import pkgutil
-
-    spec = pkgutil.get_loader("ansys.optislang.core")
-    USER_DATA_PATH = os.path.dirname(spec.get_filename())
-    if not os.path.exists(USER_DATA_PATH):  # pragma: no cover
-        os.makedirs(USER_DATA_PATH)
-
-    LOCAL_DOWNLOADED_EXAMPLES_PATH = os.path.join(USER_DATA_PATH, "examples")
-    if not os.path.exists(LOCAL_DOWNLOADED_EXAMPLES_PATH):  # pragma: no cover
-        os.makedirs(LOCAL_DOWNLOADED_EXAMPLES_PATH)
-    os.environ["OSL_EXAMPLES"] = LOCAL_DOWNLOADED_EXAMPLES_PATH
-except:  # pragma: no cover
-    pass
+# Provide examples directory path
+examples = "ansys.optislang.core.examples"
+if spec := importlib.util.find_spec(examples):
+    if spec.origin:
+        os.environ["OSL_EXAMPLES"] = os.path.dirname(spec.origin)
+    else:
+        LOG.logger.warning(f"Could not set path to examples. Missing spec for module {examples}.")
+else:
+    LOG.logger.warning(f"Could not set path to examples. Missing origin for module {examples}.")
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/application.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 """Contains abstract ``Application`` class."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 if TYPE_CHECKING:
     from ansys.optislang.core.osl_server import OslVersion
     from ansys.optislang.core.project import Project
 
 
 class Application(ABC):
@@ -38,20 +38,20 @@
     @abstractmethod
     def __init__(self):  # pragma: no cover
         """``Application`` class is an abstract base class and cannot be instantiated."""
         pass
 
     @property
     @abstractmethod
-    def project(self) -> Union[Project, None]:
+    def project(self) -> Optional[Project]:
         """Instance of the ``Project`` class.
 
         Returns
         -------
-        Union[Project, None]
+        Optional[Project]
             Loaded project. If no project is loaded, ``None`` is returned.
         """
         pass
 
     @property
     @abstractmethod
     def version(self) -> OslVersion:  # pragma: no cover
@@ -95,14 +95,15 @@
     @abstractmethod
     def open(
         self,
         file_path: Union[str, Path],
         force: bool = True,
         restore: bool = False,
         reset: bool = False,
+        project_properties_file: Optional[str] = None,
     ) -> None:  # pragma: no cover
         """Open a project.
 
         Parameters
         ----------
         file_path : Union[str, pathlib.Path]
             Path to the optiSLang project file to open.
@@ -113,14 +114,16 @@
             - Timestamp of the (auto) save point is newer than the project timestamp.
             - Project (file) is incomplete.
 
         restore : bool, optional
             Whether to restore the project from the last (auto) save point (if present).
         reset : bool, optional
             Whether to reset the project after loading it.
+        project_properties_file : Optional[str], optional
+            Project properties file to import, by default ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
         OslCommandError
             Raised when a command or query fails.
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/encoding.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/encoding.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/errors.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/omdb_files.opf` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/omdb_files.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/__init__.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/downloads.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/examples/examples.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/examples.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/io.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 """Module for input/output functionality."""
 from __future__ import annotations
 
 from enum import Enum
 from pathlib import Path
 import time
-from typing import Union
+from typing import Optional, Union
 
 from ansys.optislang.core.utils import enum_from_str
 
 
 class File:
     """Provides for operating on files."""
 
@@ -90,34 +90,34 @@
         -------
         str
             File name
         """
         return self.path.name
 
     @property
-    def last_modified_seconds(self) -> Union[float, None]:
+    def last_modified_seconds(self) -> Optional[float]:
         """Last modified time as a timestamp.
 
         Returns
         -------
-        Union[float, None]
+        Optional[float]
             Last modified time in seconds since the Epoch, `None` if file doesn't exist.
         """
         if self.exists:
             return self.path.stat().st_mtime
         else:
             return None
 
     @property
-    def last_modified_str(self) -> Union[str, None]:
+    def last_modified_str(self) -> Optional[str]:
         """Last modified time as a datetime.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             Last modified time as string, `None` if file doesn't exist.
         """
         if self.exists:
             return time.ctime(self.last_modified_seconds)
         else:
             return None
 
@@ -129,20 +129,20 @@
         -------
         Path
             Path the the file
         """
         return self.__path
 
     @property
-    def size(self) -> Union[int, None]:
+    def size(self) -> Optional[int]:
         """File size in bytes.
 
         Returns
         -------
-        Union[int, None]
+        Optional[int]
             File size in bytes, `None` in file doesn't exist.
         """
         if self.exists:
             return self.path.stat().st_size
         else:
             return None
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/logging.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/managers.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/managers.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/node_types.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/node_types.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/nodes.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1053,26 +1053,26 @@
         """``System`` class is an abstract base class and cannot be instantiated."""
         pass
 
     @abstractmethod
     def create_node(
         self,
         type_: NodeType,
-        name: Union[str, None] = None,
-        design_flow: Union[DesignFlow, None] = None,
+        name: Optional[str] = None,
+        design_flow: Optional[DesignFlow] = None,
     ) -> Node:  # pragma: no cover
         """Create a new node in current system in active project.
 
         Parameters
         ----------
         type_ : NodeType
             Type of created node.
-        name : Union[str, None], optional
+        name : Optional[str], optional
             Name of created node, by default None.
-        design_flow : Union[DesignFlow, None], optional
+        design_flow : Optional[DesignFlow], optional
             Design flow, by default None.
 
         Returns
         -------
         Node
             Instance of the created node.
 
@@ -1099,15 +1099,15 @@
             Raised when the timeout float value expires.
         """
         pass
 
     @abstractmethod
     def find_node_by_uid(
         self, uid: str, search_depth: int = 1
-    ) -> Union[Node, None]:  # pragma: no cover
+    ) -> Optional[Node]:  # pragma: no cover
         """Find a node in the system with a specified unique ID.
 
         This method searches only in the descendant nodes for the current system.
 
         Parameters
         ----------
         uid : str
@@ -1115,15 +1115,15 @@
         search_depth: int, optional
             Depth of the node subtree to search. The default is ``1``, which corresponds
             to direct children nodes of the current system. Set to ``-1`` to search throughout
             the full depth.
 
         Returns
         -------
-        Union[Node, None]
+        Optional[Node]
             ``Node`` with the specified unique ID. If this ID isn't located in any
             descendant node, ``None`` is returned.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
@@ -1528,20 +1528,20 @@
         SlotType
             Type of current slot.
         """
         pass
 
     @property
     @abstractmethod
-    def type_hint(self) -> Union[str, None]:  # pragma: no cover
+    def type_hint(self) -> Optional[str]:  # pragma: no cover
         """Get type hint.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             Data type of the current slot, ``None`` if not specified.
         """
         pass
 
     @abstractmethod
     def get_connections(self) -> Tuple[Edge]:  # pragma: no cover
         """Get connections for the current slot.
@@ -1576,29 +1576,29 @@
     @staticmethod
     @abstractmethod
     def create_slot(
         osl_server: OslServer,
         node: Node,
         name: str,
         type_: SlotType,
-        type_hint: Union[str, None] = None,
+        type_hint: Optional[str] = None,
     ) -> Slot:  # pragma: no cover
         """Create instance of new slot.
 
         Parameters
         ----------
         osl_server: OslServer
             Object providing access to the optiSLang server.
         node : Node
             Node to which slot belongs to.
         name : str
             Slot name.
         type_ : SlotType
             Slot type.
-        type_hint : Union[str, None], optional
+        type_hint : Optional[str], optional
             Slot's expected data type, by default None.
 
         Returns
         -------
         Slot
             Instance of InputSlot, OutputSlot, InnerInputSlot or InnerOutputSlot class.
         """
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/optislang.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/optislang.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Contains Optislang class, which provides the Python API for the optiSLang app."""
 from __future__ import annotations
 
+from importlib.metadata import version
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Mapping, Optional, Sequence, Tuple, Union
 
 from deprecated.sphinx import deprecated
-from importlib_metadata import version
 
 from ansys.optislang.core import LOG
 from ansys.optislang.core.tcp.application import TcpApplicationProxy
 from ansys.optislang.core.tcp.osl_server import TcpOslServer
 
 if TYPE_CHECKING:
     from ansys.optislang.core.application import Application
@@ -451,47 +451,47 @@
         -------
         Optional[Project]
             Loaded project. If no project is loaded, ``None`` is returned.
         """
         return self.application.project
 
     @property
-    def timeout(self) -> Union[float, None]:
+    def timeout(self) -> Optional[float]:
         """Get the timeout value for executing commands.
 
         Returns
         -------
-        timeout: Union[float, None]
+        timeout: Optional[float]
             Timeout in seconds to perform commands. This value must be greater
             than zero or ``None``. The default is ``None``. Another function
             raises a timeout exception if the timeout value has elapsed before
             an operation has completed. If the timeout is ``None``, functions
             wait until they're finished, and no timeout exception is raised.
         """
         return self.__osl_server.timeout
 
     @timeout.setter
-    def timeout(self, timeout: Union[float, None] = None) -> None:
+    def timeout(self, timeout: Optional[float] = None) -> None:
         """Set the timeout value for the executing commands.
 
         Parameters
         ----------
-        timeout: Union[float, None]
+        timeout: Optional[float], optional
             Timeout in seconds to perform commands. This value must be greater
             than zero or ``None``. The default is ``None``. Another function
             raises a timeout exception if the timeout value has elapsed before
             an operation has completed. If the timeout is ``None``, functions
             wait until they're finished, and no timeout exception is raised.
 
         Raises
         ------
         ValueError
             Raised when the timeout value is less than or equal to 0.
         TypeError
-            Raised when the timeout is not a Union[float, None].
+            Raised when the timeout is not a type of ``float`` or  ``None``.
         """
         self.__osl_server.timeout = timeout
 
     def dispose(self) -> None:
         """Close all local threads and unregister listeners.
 
         Raises
@@ -559,20 +559,20 @@
             Raised when parsing version numbers from string fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         return self.__osl_server.osl_version
 
     @deprecated(version="0.5.0", reason="Use :py:attr:`Optislang.timeout` instead.")
-    def get_timeout(self) -> Union[float, None]:
+    def get_timeout(self) -> Optional[float]:
         """Get the timeout value for executing commands.
 
         Returns
         -------
-        timeout: Union[float, None]
+        timeout: Optional[float]
             Timeout in seconds to perform commands. This value must be greater
             than zero or ``None``. The default is ``None``. Another function
             raises a timeout exception if the timeout value has elapsed before
             an operation has completed. If the timeout is ``None``, functions
             wait until they're finished, and no timeout exception is raised.
         """
         return self.osl_server.timeout
@@ -634,14 +634,15 @@
     )
     def open(
         self,
         file_path: Union[str, Path],
         force: bool = True,
         restore: bool = False,
         reset: bool = False,
+        project_properties_file: Optional[str] = None,
     ) -> None:
         """Open a project.
 
         Parameters
         ----------
         file_path : Union[str, pathlib.Path]
             Path to the optiSLang project file to open.
@@ -652,25 +653,33 @@
             - Timestamp of the (auto) save point is newer than the project timestamp.
             - Project (file) is incomplete.
 
         restore : bool, optional
             Whether to restore the project from the last (auto) save point (if present).
         reset : bool, optional
             Whether to reset the project after loading it.
+        project_properties_file : Optional[str], optional
+            Project properties file to import, by default ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
         OslCommandError
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        self.application.open(file_path=file_path, force=force, restore=restore, reset=reset)
+        self.application.open(
+            file_path=file_path,
+            force=force,
+            restore=restore,
+            reset=reset,
+            project_properties_file=project_properties_file,
+        )
 
     @deprecated(
         version="0.6.0",
         reason=(
             "This functionality was moved to "
             ":py:class:`Project <ansys.optislang.core.project.Project>`."
         ),
@@ -855,48 +864,47 @@
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         self.application.save_copy(file_path)
 
     @deprecated(version="0.5.0", reason="Use :py:attr:`Optislang.timeout` instead.")
-    def set_timeout(self, timeout: Union[float, None] = None) -> None:
+    def set_timeout(self, timeout: Optional[float] = None) -> None:
         """Set the timeout value for the executing commands.
 
         Parameters
         ----------
-        timeout: Union[float, None]
+        timeout: Optional[float]
             Timeout in seconds to perform commands. This value must be greater
             than zero or ``None``. The default is ``None``. Another function
             raises a timeout exception if the timeout value has elapsed before
             an operation has completed. If the timeout is ``None``, functions
             wait until they're finished, and no timeout exception is raised.
 
         Raises
         ------
         ValueError
             Raised when the timeout value is less than or equal to 0.
         TypeError
-            Raised when the timeout is not a Union[float, None].
+            Raised when the timeout is not type of ``float`` or ``None``.
         """
         self.osl_server.timeout = timeout
 
     def shutdown(self, force: bool = False) -> None:
         """Shut down the optiSLang server.
 
         This method stops the server from listening for incoming connections, discards
         pending requests, and shuts down the server. In batch mode, the project runs
         until execution finishes and then optiSLang is shut down.
 
         Parameters
         ----------
         force : bool, optional
             Whether to forcibly shut down a local optiSLang server. The default is
-            ``False``. This parameter has no effect when the connection established
-            is to a remote optiSLang server. In all cases, an attempt is made to
+            ``False``. In all cases, an attempt is made to
             shut down the optiSLang server in the proper way. However, if the
             ``force`` parameter is ``True``, after a while, the process is forcibly
             shut down without an exception being raised.
 
         Raises
         ------
         OslCommunicationError
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/osl_process.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/osl_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         if self.__batch:
             if project_path is None:
                 self.__tempdir = tempfile.TemporaryDirectory()
                 project_path = Path(self.__tempdir.name) / self.__class__.DEFAULT_PROJECT_FILE
 
         self.__project_path = self.__class__.__validated_path(project_path, "project_path")
 
-        if self.__project_path.suffix != ".opf":
+        if self.__project_path is not None and self.__project_path.suffix != ".opf":
             raise ValueError("Invalid optiSLang project file.")
 
         self.__server_info = self.__class__.__validated_path(server_info, "server_info")
         self.__import_project_properties_file = self.__class__.__validated_path(
             import_project_properties_file, "import_project_properties_file"
         )
         self.__export_project_properties_file = self.__class__.__validated_path(
@@ -434,20 +434,20 @@
         -------
         bool
             ``True`` if optiSLang TCP server is enabled; ``False`` otherwise.
         """
         return self.__enable_tcp_server
 
     @property
-    def server_info(self) -> Union[Path, None]:
+    def server_info(self) -> Optional[Path]:
         """Path to the server information file.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path]
             Path to the server information file, if defined; ``None`` otherwise.
         """
         return self.__server_info
 
     @property
     def log_commands(self) -> bool:
         """Get whether to display server events in the Message log pane.
@@ -562,20 +562,20 @@
         -------
         Tuple[str, ...]
             Additional command line arguments, if defined; ``None`` otherwise.
         """
         return self.__additional_args
 
     @property
-    def pid(self) -> Union[int, None]:
+    def pid(self) -> Optional[int]:
         """Process ID.
 
         Returns
         -------
-        Union[int, None]
+        Optional[int]
             Process ID, if exists; ``None`` otherwise.
         """
         return None if self.__process is None else self.__process.pid
 
     @property
     def shutdown_on_finished(self) -> str:
         """Whether to shut down when execution is finished.
@@ -584,87 +584,87 @@
         -------
         str
             Whether to shut down when execution is finished.
         """
         return self.__shutdown_on_finished
 
     @property
-    def import_project_properties_file(self) -> Union[Path, None]:
+    def import_project_properties_file(self) -> Optional[Path]:
         """Path to the project properties import file.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path]
             Path to the project properties import file, if defined; ``None`` otherwise.
         """
         return self.__import_project_properties_file
 
     @property
-    def export_project_properties_file(self) -> Union[Path, None]:
+    def export_project_properties_file(self) -> Optional[Path]:
         """Path to the project properties export file.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path]
             Path to the project properties export file, if defined; ``None`` otherwise.
         """
         return self.__export_project_properties_file
 
     @property
-    def import_placeholders_file(self) -> Union[Path, None]:
+    def import_placeholders_file(self) -> Optional[Path]:
         """Path to the placeholders import file.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path]
             Path to the placeholders import file, if defined; ``None`` otherwise.
         """
         return self.__import_placeholders_file
 
     @property
-    def export_placeholders_file(self) -> Union[Path, None]:
+    def export_placeholders_file(self) -> Optional[Path]:
         """Path to the placeholders export file.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path, None]
             Path to the placeholders export file, if defined; ``None`` otherwise.
         """
         return self.__export_placeholders_file
 
     @property
-    def output_file(self) -> Union[Path, None]:
+    def output_file(self) -> Optional[Path]:
         """Path to the output file for writing project run results to.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path]
             Path to the output file for writing project run results to, if defined;
             ``None`` otherwise.
         """
         return self.__output_file
 
     @property
-    def dump_project_state(self) -> Union[Path, None]:
+    def dump_project_state(self) -> Optional[Path]:
         """Path to a project state dump file to export.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path]
             Path to a project state dump file to export, if defined; ``None`` otherwise.
         """
         return self.__dump_project_state
 
     @property
-    def opx_project_definition_file(self) -> Union[Path, None]:
+    def opx_project_definition_file(self) -> Optional[Path]:
         """Path to the OPX project definition file.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path]
             Path to the OPX project definition file, if defined;
             ``None`` otherwise.
         """
         return self.__opx_project_definition_file
 
     def __enter__(self):
         """Enter the context."""
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/osl_server.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/osl_server.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/project.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 """Contains abstract ``Project`` class."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import TYPE_CHECKING, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Sequence, Tuple, Union
 
 if TYPE_CHECKING:
     from ansys.optislang.core.io import RegisteredFile
     from ansys.optislang.core.nodes import RootSystem
     from ansys.optislang.core.project_parametric import Design
 
 
@@ -99,20 +99,20 @@
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         pass
 
     @abstractmethod
-    def get_description(self) -> Union[str, None]:  # pragma: no cover
+    def get_description(self) -> Optional[str]:  # pragma: no cover
         """Get the description of the optiSLang project.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             Description of the optiSLang project. If no project is loaded in optiSLang,
             ``None`` is returned.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/project_parametric.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/project_parametric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1188,15 +1188,15 @@
             Expression value type. Defaults to ``None``.
         criterion: Union[CriterionType, str], optional
             Comparison symbol type, e. g. 'min'. By default ``ComparisonType.LESSLIMITSTATE``.
         limit_expression: str, optional
             Limit expression. By default ``"0"``.
         limit_expression_value: Optional[Union[tuple, bool, float, complex, list, dict]], optional
             Limit expression value. Defaults to ``None``.
-        limit_expression_value_type: Optional[Union[CriterionValueType, None]], optional
+        limit_expression_value_type: Optional[CriterionValueType], optional
             Limit expression value type. Defaults to ``None``.
         value: Optional[Union[tuple, bool, float, complex, list, dict]], optional
             Criterion value. By default ``None``.
         value_type: Optional[CriterionValueType], optional
             Type of the criterion value. By default ``None``.
         """
         super().__init__(
@@ -2360,45 +2360,45 @@
         """
         if parameters is not None:
             self.__distribution_parameters = tuple(parameters)
         else:
             self.__distribution_parameters = None
 
     @property
-    def statistical_moments(self) -> Union[Tuple[float], None]:
+    def statistical_moments(self) -> Optional[Tuple[float]]:
         """Statistical moments of the distribution."""
         return self.__statistical_moments
 
     @statistical_moments.setter
-    def statistical_moments(self, moments: Union[Sequence[float], None]):
+    def statistical_moments(self, moments: Optional[Sequence[float]]):
         """Set the statistical moments of the distribution.
 
         Parameters
         ----------
-        moments : Sequence[float]
+        moments : Optional[Sequence[float]]
             Statistical moments of the distribution.
         """
         if moments is not None:
             self.__statistical_moments = tuple(moments)
         else:
             self.__statistical_moments = None
 
     @property
-    def cov(self) -> Union[float, None]:
+    def cov(self) -> Optional[float]:
         """COV of the distribution."""
         return self.__cov
 
     @cov.setter
-    def cov(self, cov: Union[float, None]):
-        """Set the statistical moments of the distribution.
+    def cov(self, cov: Optional[float]):
+        """Set the COV of the distribution.
 
         Parameters
         ----------
-        moments : Sequence[float]
-            Statistical moments of the distribution.
+        cov : Optional[float]
+            COV of the distribution.
         """
         self.__cov = cov
 
     def to_dict(self) -> dict:
         """Convert an instance of the ``MixedParameter`` class to a dictionary.
 
         Returns
@@ -2870,26 +2870,26 @@
         """
         if moments is not None:
             self.__statistical_moments = tuple(moments)
         else:
             self.__statistical_moments = None
 
     @property
-    def cov(self) -> Union[float, None]:
+    def cov(self) -> Optional[float]:
         """COV of the distribution."""
         return self.__cov
 
     @cov.setter
-    def cov(self, cov: Union[float, None]):
-        """Set the statistical moments of the distribution.
+    def cov(self, cov: Optional[float]):
+        """Set the COV of the distribution.
 
         Parameters
         ----------
-        moments : Sequence[float]
-            Statistical moments of the distribution.
+        cov : Optional[float]
+            COV of the distribution.
         """
         self.__cov = cov
 
     def to_dict(self) -> dict:
         """Convert an instance of the ``StochasticParameter`` to dictionary.
 
         Returns
@@ -3257,16 +3257,16 @@
         ] = [],
         feasibility: Optional[bool] = None,
         design_id: Optional[int] = None,
         status: DesignStatus = DesignStatus.IDLE,
     ) -> None:
         """Initialize a new instance of the ``Design`` class."""
         self.__constraints: List[DesignVariable] = []
-        self.__feasibility: Union[bool, None] = feasibility
-        self.__id: Union[int, None] = design_id
+        self.__feasibility: Optional[bool] = feasibility
+        self.__id: Optional[int] = design_id
         self.__limit_states: List[DesignVariable] = []
         self.__objectives: List[DesignVariable] = []
         self.__parameters: List[DesignVariable] = []
         self.__responses: List[DesignVariable] = []
         self.__status: DesignStatus = status
         self.__variables: List[DesignVariable] = []
 
@@ -3293,20 +3293,20 @@
 
     @property
     def constraints_names(self) -> Tuple[str, ...]:
         """Tuple of all constraint names."""
         return tuple([constraint.name for constraint in self.__constraints])
 
     @property
-    def feasibility(self) -> Union[bool, None]:
+    def feasibility(self) -> Optional[bool]:
         """Feasibility of the design. If the design is not evaluated, ``None`` is returned."""
         return self.__feasibility
 
     @property
-    def id(self) -> Union[int, None]:
+    def id(self) -> Optional[int]:
         """ID of the design. If no ID is assigned, ``None`` is returned."""
         return self.__id
 
     @property
     def limit_states(self) -> Tuple[DesignVariable, ...]:
         """Tuple of all limit states."""
         return tuple(self.__limit_states)
@@ -3489,27 +3489,27 @@
             raise TypeError(f"Invalid type of name: `{type(name)}`.")
 
         if index is not None:
             self.__parameters[index].value = value
         else:
             self.__parameters.append(DesignVariable(name=name, value=value))
 
-    def __find_name_index(self, name: str, type_: str) -> Union[int, None]:
+    def __find_name_index(self, name: str, type_: str) -> Optional[int]:
         """Find the index of a criterion, parameter, response, or variable by name.
 
         Parameters
         ----------
         name: str
             Name of the criterion, parameter, response, or variable.
         type_: str
             Union['constraint', 'limit_state', 'objective', 'parameter', 'response', 'variable']
 
         Returns
         -------
-        Union[int, None]
+        Optional[int]
             Position of the name in the list. If the name is not found, ``None`` is returned.
 
         Raises
         ------
         TypeError
             Raised when an unknown type is given.
         RuntimeError
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/application.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 """Contains tcp ``Application`` class."""
 from __future__ import annotations
 
 import logging
 from pathlib import Path
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 from ansys.optislang.core.application import Application
 from ansys.optislang.core.tcp.project import TcpProjectProxy
 
 if TYPE_CHECKING:
     from ansys.optislang.core.osl_server import OslVersion
     from ansys.optislang.core.tcp.osl_server import TcpOslServer
@@ -47,20 +47,20 @@
         self.__project = (
             TcpProjectProxy(osl_server=self.__osl_server, uid=project_uid, logger=self._logger)
             if project_uid
             else None
         )
 
     @property
-    def project(self) -> Union[TcpProjectProxy, None]:
+    def project(self) -> Optional[TcpProjectProxy]:
         """Instance of the ``TcpProjectProxy`` class.
 
         Returns
         -------
-        Union[TcpProjectProxy, None]
+        Optional[TcpProjectProxy]
             Loaded project. If no project is loaded, ``None`` is returned.
         """
         return self.__project
 
     @property
     def version(self) -> OslVersion:
         """Version of used optiSLang.
@@ -105,14 +105,15 @@
 
     def open(
         self,
         file_path: Union[str, Path],
         force: bool = True,
         restore: bool = False,
         reset: bool = False,
+        project_properties_file: Optional[str] = None,
     ) -> None:
         """Open a project.
 
         Parameters
         ----------
         file_path : Union[str, pathlib.Path]
             Path to the optiSLang project file to open.
@@ -123,25 +124,33 @@
             - Timestamp of the (auto) save point is newer than the project timestamp.
             - Project (file) is incomplete.
 
         restore : bool, optional
             Whether to restore the project from the last (auto) save point (if present).
         reset : bool, optional
             Whether to reset the project after loading it.
+        project_properties_file : Optional[str], optional
+            Project properties file to import, by default ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
         OslCommandError
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        self.__osl_server.open(file_path=file_path, force=force, restore=restore, reset=reset)
+        self.__osl_server.open(
+            file_path=file_path,
+            force=force,
+            restore=restore,
+            reset=reset,
+            project_properties_file=project_properties_file,
+        )
         self.__project = TcpProjectProxy(
             osl_server=self.__osl_server,
             uid=self.__get_project_uid(),
         )
 
     def save(self) -> None:
         """Save changes to the project data and settings.
@@ -208,33 +217,36 @@
         OslCommandError
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         self.__osl_server.save_copy(file_path=file_path)
 
-    def __get_project_uid(self) -> Union[str, None]:
+    def __get_project_uid(self) -> Optional[str]:
         """Get project uid.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             Project uid. If no project is loaded in the optiSLang, returns `None`.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        project_tree = self.__osl_server.get_full_project_tree_with_properties()
-        return project_tree.get("projects", [{}])[0].get("system", {}).get("uid", None)
+        try:
+            project_tree = self.__osl_server.get_full_project_tree_with_properties()
+            return project_tree.get("projects", [{}])[0].get("system", {}).get("uid", None)
+        except:
+            return None
 
     # FUTURES:
 
     # close method doesn't work properly in optiSLang 2023R1, therefore it was commented out
     # TODO: Add this after it's fixed on optiSLang server side.
     # def close(self) -> None:
     #     """Close the current project.
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/managers.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/managers.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/nodes.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,19 @@
             Raised when an error occurs while communicating with the server.
         OslCommandError
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         try:
-            self._osl_server.get_actor_info(self.uid)
+            self._osl_server.get_actor_info(
+                self.uid,
+                include_log_messages=False,
+                include_integrations_registered_locations=False,
+            )
             return True
         except Exception as e:
             if isinstance(e, OslCommandError) and "No such actor" in str(e):
                 return False
             else:
                 raise
 
@@ -368,15 +372,19 @@
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
         OslCommandError
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        actor_info = self._osl_server.get_actor_info(uid=self.__uid)
+        actor_info = self._osl_server.get_actor_info(
+            uid=self.__uid,
+            include_log_messages=False,
+            include_integrations_registered_locations=False,
+        )
         return actor_info["name"]
 
     def get_output_slots(self, name: Optional[str] = None) -> Tuple[TcpOutputSlotProxy, ...]:
         """Get current node's output slots.
 
         Parameters
         ----------
@@ -577,15 +585,19 @@
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
         OslCommandError
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        actor_info = self._osl_server.get_actor_info(uid=self.__uid)
+        actor_info = self._osl_server.get_actor_info(
+            uid=self.__uid,
+            include_log_messages=False,
+            include_integrations_registered_locations=False,
+        )
         return actor_info["status"]
 
     @deprecated(version="0.6.0", reason="Use :py:attr:`TcpNodeProxy.type` instead.")
     def get_type(self) -> NodeType:
         """Get the type of the node.
 
         Returns
@@ -598,15 +610,19 @@
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
         OslCommandError
             Raised when a command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
-        actor_info = self._osl_server.get_actor_info(uid=self.__uid)
+        actor_info = self._osl_server.get_actor_info(
+            uid=self.__uid,
+            include_log_messages=False,
+            include_integrations_registered_locations=False,
+        )
         return get_node_type_from_str(node_id=actor_info["type"])
 
     def set_property(self, name: str, value: Any) -> None:
         """Set node's property.
 
         Parameters
         ----------
@@ -687,15 +703,19 @@
             ) and isinstance(slot_type, SlotType):
                 # `[receiving_slot, sending_slot]_is_inner` key included in connection dict
                 if slot_type_key in connection.keys():
                     if not connection[slot_type_key] == slot_type_is_inner:
                         continue
                 # `[receiving_slot, sending_slot]_is_inner` key not included in connection dict
                 else:
-                    info = self._osl_server.get_actor_info(connection[uid_keys[0]])
+                    info = self._osl_server.get_actor_info(
+                        connection[uid_keys[0]],
+                        include_log_messages=False,
+                        include_integrations_registered_locations=False,
+                    )
                     if True in [
                         item["name"] == connection[slot_name_keys[0]]
                         for item in info[slot_type.name.lower() + "_slots"]
                     ]:
                         connection[slot_name_keys[0] + "_is_inner"] = slot_type_is_inner
                     else:
                         continue
@@ -744,23 +764,23 @@
         return self.__class__._find_parent_node_info(
             tree=parent_tree,
             parent_uid=root_system_uid,
             node_uid=self.uid,
         )
 
     def _get_slots(
-        self, type_: Union[SlotType, None] = None, name: Union[str, None] = None
+        self, type_: Optional[SlotType] = None, name: Optional[str] = None
     ) -> Tuple[TcpSlotProxy, ...]:
         """Get current node's slots of given type and name.
 
         Parameters
         ----------
-        type_: Union[SlotType, None], optional
+        type_: Optional[SlotType], optional
             Type of slots to be returned, by default ``None``.
-        name : Union[str, None], optional
+        name : Optional[str], optional
             Slot name, by default ``None``.
 
         Returns
         -------
         Tuple[TcpSlotProxy, ...]
             Tuple of current node's slots of given type.
 
@@ -1556,24 +1576,24 @@
             type_=type_,
             logger=logger,
         )
 
     def create_node(
         self,
         type_: Union[NodeType, str],
-        name: Union[str, None] = None,
+        name: Optional[str] = None,
         design_flow: Optional[Union[DesignFlow, str]] = None,
     ) -> TcpNodeProxy:
         """Create a new node in current system in active project.
 
         Parameters
         ----------
         type_ : Union[NodeType, str]
             Type of created node.
-        name : Union[str, None], optional
+        name : Optional[str], optional
             Name of created node, by default None.
         design_flow : Optional[Union[DesignFlow, str]], optional
             Design flow, by default ``None``.
 
         Returns
         -------
         TcpNodeProxy
@@ -1613,15 +1633,17 @@
             algorithm_type=algorithm_type,
             integration_type=integration_type,
             mop_node_type=mop_node_type,
             node_type=node_type,
             parent_uid=self.uid,
             design_flow=design_flow_name,
         )
-        info = self._osl_server.get_actor_info(uid=uid)
+        info = self._osl_server.get_actor_info(
+            uid=uid, include_log_messages=False, include_integrations_registered_locations=False
+        )
         info["is_parametric_system"] = "estimated_designs" in info.keys()
         return create_nodes_from_properties_dicts(
             osl_server=self._osl_server, properties_dicts_list=[info], logger=self._logger
         )[0]
 
     def delete_children_nodes(self) -> None:
         """Delete all children nodes from the active project.
@@ -1635,15 +1657,15 @@
         TimeoutError
             Raised when the timeout float value expires.
         """
         nodes = self.get_nodes()
         for node in nodes:
             node.delete()
 
-    def find_node_by_uid(self, uid: str, search_depth: int = 1) -> Union[TcpNodeProxy, None]:
+    def find_node_by_uid(self, uid: str, search_depth: int = 1) -> Optional[TcpNodeProxy]:
         """Find a node in the system with a specified unique ID.
 
         This method searches only in the descendant nodes for the current system.
 
         Parameters
         ----------
         uid : str
@@ -1651,15 +1673,15 @@
         search_depth: int, optional
             Depth of the node subtree to search. The default is ``1``, which corresponds
             to direct children nodes of the current system. Set to ``-1`` to search throughout
             the full depth.
 
         Returns
         -------
-        Union[TcpNodeProxy, None]
+        Optional[TcpNodeProxy]
             ``TcpNodeProxy`` with the specified unique ID. If this ID isn't located in any
             descendant node, ``None`` is returned.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with the server.
@@ -1859,25 +1881,25 @@
             if node["kind"] == "system":
                 __class__._find_subtree(tree=node, uid=uid, nodes_tree=nodes_tree)
         return nodes_tree
 
     @staticmethod
     def _get_subtypes(
         addin_type: AddinType,
-    ) -> Tuple[Union[str, None], Union[str, None], Union[str, None], Union[str, None]]:
+    ) -> Tuple[Optional[str], Optional[str], Optional[str], Optional[str]]:
         """Get subtypes in tcp server input format.
 
         Parameters
         ----------
         addin_type: AddinType
             Node's subtype.
 
         Returns
         -------
-        Tuple[Union[str, None], Union[str, None], Union[str, None], Union[str, None]]
+        Tuple[Optional[str], Optional[str], Optional[str], Optional[str]]
             algorithm_type, integration_type, mop_node_type, node_type
         """
         if not isinstance(addin_type, AddinType):
             raise TypeError(f"Unsupported value of addin_type: ``{type(addin_type)}``.")
 
         algorithm_type, integration_type, mop_node_type, node_type = None, None, None, None
         if addin_type == AddinType.BUILT_IN:
@@ -2669,29 +2691,29 @@
 
     def __init__(
         self,
         osl_server: TcpOslServer,
         node: TcpNodeProxy,
         name: str,
         type_: SlotType,
-        type_hint: Union[str, None] = None,
+        type_hint: Optional[str] = None,
     ) -> None:
         """Create an ``TcpSlotProxy`` instance.
 
         Parameters
         ----------
         osl_server: TcpOslServer
             Object providing access to the optiSLang server.
         node : TcpNodeProxy
             Node to which the slot belongs.
         name : str
            Slot name.
         type_ : SlotType
             Slot type.
-        type_hint : Union[str, None], optional
+        type_hint : Optional[str], optional
             Description, by default None.
         """
         self._osl_server = osl_server
         self.__node = node
         self.__name = name
         self.__type = type_
         self.__type_hint = type_hint
@@ -2730,20 +2752,20 @@
         -------
         SlotType
             Type of current slot.
         """
         return self.__type
 
     @property
-    def type_hint(self) -> Union[str, None]:
+    def type_hint(self) -> Optional[str]:
         """Get type hint.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             Data type of the current slot, ``None`` if not specified.
         """
         return self.__type_hint
 
     def get_connections(self) -> Tuple[Edge]:
         """Get connections for the current slot.
 
@@ -2907,29 +2929,29 @@
 
     def __init__(
         self,
         osl_server: TcpOslServer,
         node: TcpNodeProxy,
         name: str,
         type_: SlotType,
-        type_hint: Union[str, None] = None,
+        type_hint: Optional[str] = None,
     ) -> None:
         """Create an ``TcpInputSlotProxy`` instance.
 
         Parameters
         ----------
         osl_server: TcpOslServer
             Object providing access to the optiSLang server.
         node : TcpNodeProxy
             Node to which the slot belongs.
         name : str
            Slot name.
         type_ : SlotType
             Slot type.
-        type_hint : Union[str, None], optional
+        type_hint : Optional[str], optional
             Description, by default None.
         """
         super().__init__(
             osl_server=osl_server,
             node=node,
             name=name,
             type_=type_,
@@ -2994,29 +3016,29 @@
 
     def __init__(
         self,
         osl_server: TcpOslServer,
         node: TcpNodeProxy,
         name: str,
         type_: SlotType,
-        type_hint: Union[str, None] = None,
+        type_hint: Optional[str] = None,
     ) -> None:
         """Create an ``OutputSlotProxy`` instance.
 
         Parameters
         ----------
         osl_server: TcpOslServer
             Object providing access to the optiSLang server.
         node : TcpNodeProxy
             Node to which the slot belongs.
         name : str
            Slot name.
         type_ : SlotType
             Slot type.
-        type_hint : Union[str, None], optional
+        type_hint : Optional[str], optional
             Description, by default None.
         """
         super().__init__(
             osl_server=osl_server,
             node=node,
             name=name,
             type_=type_,
@@ -3081,29 +3103,29 @@
 
     def __init__(
         self,
         osl_server: TcpOslServer,
         node: TcpNodeProxy,
         name: str,
         type_: SlotType,
-        type_hint: Union[str, None] = None,
+        type_hint: Optional[str] = None,
     ) -> None:
         """Create a ``InnerInputSlotProxy`` instance.
 
         Parameters
         ----------
         osl_server: TcpOslServer
             Object providing access to the optiSLang server.
         node : TcpNodeProxy
             Node to which the slot belongs.
         name : str
            Slot name.
         type_ : SlotType
             Slot type.
-        type_hint : Union[str, None], optional
+        type_hint : Optional[str], optional
             Description, by default None.
         """
         super().__init__(
             osl_server=osl_server,
             node=node,
             name=name,
             type_=type_,
@@ -3152,29 +3174,29 @@
 
     def __init__(
         self,
         osl_server: TcpOslServer,
         node: TcpNodeProxy,
         name: str,
         type_: SlotType,
-        type_hint: Union[str, None] = None,
+        type_hint: Optional[str] = None,
     ) -> None:
         """Create a ``InnerOutputSlotProxy`` instance.
 
         Parameters
         ----------
         osl_server: TcpOslServer
             Object providing access to the optiSLang server.
         node : TcpNodeProxy
             Node to which the slot belongs.
         name : str
            Slot name.
         type_ : SlotType
             Slot type.
-        type_hint : Union[str, None], optional
+        type_hint : Optional[str], optional
             Description, by default None.
         """
         super().__init__(
             osl_server=osl_server,
             node=node,
             name=name,
             type_=type_,
@@ -3264,15 +3286,19 @@
         SlotType.INNER_INPUT
         if connection.get("receiving_slot_is_inner", None)
         else SlotType.INPUT
         if connection.get("receiving_slot_is_inner") is False
         else None
     )
     if rec_slot_type is None:
-        info = osl_server.get_actor_info(connection["receiving_uuid"])
+        info = osl_server.get_actor_info(
+            connection["receiving_uuid"],
+            include_log_messages=False,
+            include_integrations_registered_locations=False,
+        )
         if True in [item["name"] == rec_slot_name for item in info["input_slots"]]:
             rec_slot_type = SlotType.INPUT
         elif True in [item["name"] == rec_slot_name for item in info.get("inner_input_slots", [])]:
             rec_slot_type = SlotType.INNER_INPUT
         else:
             raise ValueError(f"Slot ``{rec_slot_name}`` doesn't exist for given node.")
     rec_slot = create_slot_from_project_tree(
@@ -3291,15 +3317,19 @@
         SlotType.INNER_OUTPUT
         if connection.get("sending_slot_is_inner", None)
         else SlotType.OUTPUT
         if connection.get("sending_slot_is_inner") is False
         else None
     )
     if sen_slot_type is None:
-        info = osl_server.get_actor_info(connection["sending_uuid"])
+        info = osl_server.get_actor_info(
+            connection["sending_uuid"],
+            include_log_messages=False,
+            include_integrations_registered_locations=False,
+        )
         if True in [item["name"] == sen_slot_name for item in info["output_slots"]]:
             sen_slot_type = SlotType.OUTPUT
         elif True in [item["name"] == sen_slot_name for item in info.get("inner_output_slots", [])]:
             sen_slot_type = SlotType.INNER_OUTPUT
         else:
             raise ValueError(f"Slot ``{rec_slot_name}`` doesn't exist for given node.")
     sen_slot = create_slot_from_project_tree(
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/osl_server.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/osl_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,22 +54,22 @@
 )
 from ansys.optislang.core.osl_process import OslServerProcess, ServerNotification
 from ansys.optislang.core.osl_server import OslServer, OslVersion
 from ansys.optislang.core.tcp import server_commands as commands
 from ansys.optislang.core.tcp import server_queries as queries
 
 
-def _get_current_timeout(initial_timeout: Union[float, None], start_time: float) -> Optional[float]:
+def _get_current_timeout(initial_timeout: Optional[float], start_time: float) -> Optional[float]:
     """Get actual timeout value.
 
     The function will raise a timeout exception if the timeout has expired.
 
     Parameters
     ----------
-    initial_timeout : float, None
+    initial_timeout : Optional[float]
         Initial timeout value. For non-zero value, the new timeout value is computed.
         If the timeout period value has elapsed, the timeout exception is raised.
         For zero value, the non-blocking mode is assumed and zero value is returned.
         For ``None``, the blocking mode is assumed and ``None`` is returned.
     start_time : float
         The time when the initial time out starts to count down. It is defined in seconds
         since the epoch as a floating point number.
@@ -297,24 +297,24 @@
         Returns
         -------
         bool
             True if the connection has been established; False otherwise.
         """
         return self.__socket is not None
 
-    def connect(self, host: str, port: int, timeout: Union[float, None] = 2) -> None:
+    def connect(self, host: str, port: int, timeout: Optional[float] = 2) -> None:
         """Connect to the plain TCP/IP server.
 
         Parameters
         ----------
         host : str
             A string representation of an IPv4/v6 address or domain name.
         port : int
             A numeric port number.
-        timeout : Union[float, None], optional
+        timeout : Optional[float], optional
             Timeout in seconds to establish a connection. If a non-zero value is given,
             the function will raise a timeout exception if the timeout period value has elapsed
             before the operation has completed. If zero is given, the non-blocking mode is used.
             If ``None`` is given, the blocking mode is used. Defaults to 2 s.
 
         Raises
         ------
@@ -353,22 +353,22 @@
 
     def disconnect(self) -> None:
         """Disconnect from the server."""
         if self.is_connected:
             self.__socket.close()
             self.__socket = None
 
-    def send_msg(self, msg: str, timeout: Union[float, None] = 5) -> None:
+    def send_msg(self, msg: str, timeout: Optional[float] = 5) -> None:
         """Send message to the server.
 
         Parameters
         ----------
         msg : str
             Message to send.
-        timeout : Union[float, None], optional
+        timeout : Optional[float], optional
             Timeout in seconds to send a message. If a non-zero value is given,
             the function will raise a timeout exception if the timeout period value has elapsed
             before the operation has completed. If zero is given, the non-blocking mode is used.
             If ``None`` is given, the blocking mode is used. Defaults to 5 s.
 
         Raises
         ------
@@ -389,22 +389,22 @@
         data_len = len(data)
 
         header = struct.pack("!QQ", data_len, data_len)
 
         self.__socket.settimeout(timeout)
         self.__socket.sendall(header + data)
 
-    def send_file(self, file_path: Union[str, Path], timeout: Union[float, None] = 5) -> None:
+    def send_file(self, file_path: Union[str, Path], timeout: Optional[float] = 5) -> None:
         """Send content of the file to the server.
 
         Parameters
         ----------
         file_path : Union[str, pathlib.Path]
             Path to the file whose content is to be sent to the server.
-        timeout : Union[float, None], optional
+        timeout : Optional[float], optional
             Timeout in seconds to send the buffer of the read part of the file. If a non-zero value
             is given, the function will raise a timeout exception if the timeout period value
             has elapsed before the operation has completed. If zero is given, the non-blocking mode
             is used. If ``None`` is given, the blocking mode is used. Defaults to 5 s.
         Raises
         ------
         ConnectionNotEstablishedError
@@ -434,20 +434,20 @@
             self.__socket.settimeout(timeout)
             self.__socket.sendall(header)
             load = file.read(self.__class__._BUFFER_SIZE)
             while load:
                 self.__socket.send(load)
                 load = file.read(self.__class__._BUFFER_SIZE)
 
-    def receive_msg(self, timeout: Union[float, None] = 5) -> str:
+    def receive_msg(self, timeout: Optional[float] = 5) -> str:
         """Receive message from the server.
 
         Parameters
         ----------
-        timeout : Union[float, None], optional
+        timeout : Optional[float], optional
             Timeout in seconds to receive a message. The function will raise a timeout exception
             if the timeout period value has elapsed before the operation has completed. If ``None``
             is given, the blocking mode is used. Defaults to 5 s.
 
         Returns
         -------
         str
@@ -483,22 +483,22 @@
         remain_timeout = _get_current_timeout(timeout, start_time)
         data = self._receive_bytes(msg_len, remain_timeout)
         if len(data) != msg_len:
             raise ResponseFormatError("Received data does not match declared data size.")
 
         return force_text(data)
 
-    def receive_file(self, file_path: Union[str, Path], timeout: Union[float, None] = 5) -> None:
+    def receive_file(self, file_path: Union[str, Path], timeout: Optional[float] = 5) -> None:
         """Receive file from the server.
 
         Parameters
         ----------
         file_path : Union[str, pathlib.Path]
             Path where the received file is to be saved.
-        timeout : Union[float, None], optional
+        timeout : Optional[float], optional
             Timeout in seconds to receive a buffer of the file part. The function will raise
             a timeout exception if the timeout period value has elapsed before the operation
             has completed. If ``None`` is given, the blocking mode is used. Defaults to 5 s.
 
         Raises
         ------
         ConnectionNotEstablishedError
@@ -526,20 +526,20 @@
             raise EmptyResponseError("The empty file has been received.")
 
         remain_timeout = _get_current_timeout(timeout, start_time)
         self._fetch_file(file_len, file_path, remain_timeout)
         if os.path.getsize(file_path) != file_len:
             raise ResponseFormatError("Received data does not match declared data size.")
 
-    def _recv_response_length(self, timeout: Union[float, None]) -> int:
+    def _recv_response_length(self, timeout: Optional[float]) -> int:
         """Receive length of the response.
 
         Parameters
         ----------
-        timeout : Union[float, None], optional
+        timeout : Optional[float]
             Timeout in seconds to receive the response length. The function will raise a timeout
             exception if the timeout period value has elapsed before the operation has completed.
             If ``None`` is given, the blocking mode is used.
 
         Returns
         -------
         int
@@ -572,22 +572,22 @@
                 "Server response format unrecognized. Response sizes do not match."
             )
 
         response_len = response_len_1
 
         return response_len
 
-    def _receive_bytes(self, count: int, timeout: Union[float, None]) -> bytes:
+    def _receive_bytes(self, count: int, timeout: Optional[float]) -> bytes:
         """Receive specified number of bytes from the server.
 
         Parameters
         ----------
         count : int
             Number of bytes to be received from the server.
-        timeout : Union[float, None], optional
+        timeout : Optional[float]
             Timeout in seconds to receive specified number of bytes. The function will raise
             a timeout exception if the timeout period value has elapsed before the operation
             has completed. If ``None`` is given, the blocking mode is used.
 
         Returns
         -------
         bytes
@@ -623,25 +623,25 @@
             if not chunk:
                 break
             received += chunk
             received_len += len(chunk)
         return received
 
     def _fetch_file(
-        self, file_len: int, file_path: Union[str, Path], timeout: Union[float, None]
+        self, file_len: int, file_path: Union[str, Path], timeout: Optional[float]
     ) -> None:
         """Write received bytes from the server to the file.
 
         Parameters
         ----------
         file_len : int
             Number of bytes to be written.
         file_path : Union[str, pathlib.Path]
             Path to the file to which the received data is to be written.
-        timeout : Union[float, None], optional
+        timeout : Optional[float]
             Timeout in seconds to receive bytes from the server and write them to the file.
             The function will raise a timeout exception if the timeout period value has
             elapsed before the operation has completed. If ``None`` is given, the blocking mode
             is used.
 
         Raises
         ------
@@ -775,15 +775,15 @@
 
     @property
     def name(self) -> str:
         """Instance name used for naming self.__thread."""
         return self.__name
 
     @property
-    def timeout(self) -> Union[float, None]:
+    def timeout(self) -> Optional[float]:
         """Timeout in seconds to receive a message."""
         return self.__timeout
 
     @timeout.setter
     def timeout(self, timeout) -> None:
         self.__timeout = timeout
 
@@ -1243,23 +1243,23 @@
             if self.__osl_version[0] < 23:
                 self._logger.warning(
                     f"The version of the used Ansys optiSLang ({self.__osl_version_string})"
                     " is not fully supported. Please use at least version 23.1."
                 )
 
     @property
-    def host(self) -> Union[str, None]:
+    def host(self) -> Optional[str]:
         """Get optiSLang server address or domain name.
 
         Get a string representation of an IPv4/v6 address or domain name
         of the running optiSLang server.
 
         Returns
         -------
-        timeout: Union[int, None]
+        timeout: Optional[int]
             The IPv4/v6 address or domain name of the running optiSLang server, if applicable.
             Defaults to ``None``.
         """
         return self.__host
 
     @property
     def max_request_attempts_register(self) -> FunctionsAttributeRegister:
@@ -1289,20 +1289,20 @@
         -------
         str
             optiSLang version.
         """
         return self.__osl_version_string
 
     @property
-    def port(self) -> Union[int, None]:
+    def port(self) -> Optional[int]:
         """Get the port the osl server is listening on.
 
         Returns
         -------
-        timeout: Union[int, None]
+        timeout: Optional[int]
             The port the osl server is listening on, if applicable.
             Defaults to ``None``.
         """
         return self.__port
 
     @property
     def timeout(self) -> Optional[float]:
@@ -1312,20 +1312,20 @@
         -------
         timeout: Optional[float]
             Timeout in seconds to perform commands.
         """
         return self.timeouts_register.default_value
 
     @timeout.setter
-    def timeout(self, timeout: Union[float, None] = 30) -> None:
+    def timeout(self, timeout: Optional[float] = 30) -> None:
         """Set default timeout value for execution of commands.
 
         Parameters
         ----------
-        timeout: Union[float, None]
+        timeout: Optional[float]
             Timeout in seconds to perform commands, it must be greater than zero or ``None``.
             Another functions will raise a timeout exception if the timeout period value has
             elapsed before the operation has completed.
             If ``None`` is given, functions will wait until they're finished (no timeout
             exception is raised). Defaults to ``30``.
         """
         self.timeouts_register.default_value = timeout
@@ -1412,41 +1412,41 @@
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
     def create_node(
         self,
         type_: str,
-        name: Union[str, None] = None,
+        name: Optional[str] = None,
         algorithm_type: str = None,
         integration_type: str = None,
         mop_node_type: str = None,
         node_type: str = None,
-        parent_uid: Union[str, None] = None,
-        design_flow: Union[str, None] = None,
+        parent_uid: Optional[str] = None,
+        design_flow: Optional[str] = None,
     ) -> str:
         """Create a new node of given type.
 
         Parameters
         ----------
         type_ : str
             Type of the node.
-        name : Union[str, None], optional
+        name : Optional[str], optional
             Node name, by default ``None``.
         algorithm_type : str, optional
             Algorithm type, e. g. 'algorithm_plugin', by default None.
         integration_type : str, optional
             Integration type, e. g. 'integration_plugin', by default None.
         mop_node_type : str, optional
             MOP node type, e. g. 'python_based_mop_node_plugin', by default None.
         node_type: str, optional
             Node type, e. g. 'python_based_node_plugin`, by default None.
-        parent_uid : Union[str, None], optional
+        parent_uid : Optional[str], optional
             Parent uid, by default ``None``.
-        design_flow : Union[str, None], optional
+        design_flow : Optional[str], optional
             Design flow option, by default ``None``.
 
         Returns
         -------
         str
             Uid of the created node.
 
@@ -1631,21 +1631,30 @@
         current_func_name = self.evaluate_design.__name__
         return self.send_command(
             command=commands.evaluate_design(evaluate_dict, self.__password),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
-    def get_actor_info(self, uid: str) -> Dict:
+    def get_actor_info(
+        self,
+        uid: str,
+        include_log_messages: bool = True,
+        include_integrations_registered_locations: bool = True,
+    ) -> Dict:
         """Get info about actor defined by uid.
 
         Parameters
         ----------
         uid : str
             Actor uid.
+        include_log_messages: bool, optional
+            Whether actor log messages are to be included.
+        include_integrations_registered_locations: bool, optional
+            Whether registered integration locations are to be included.
 
         Returns
         -------
         Dict
             Info about actor defined by uid.
 
         Raises
@@ -1655,15 +1664,20 @@
         OslCommandError
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         current_func_name = self.get_actor_info.__name__
         return self.send_command(
-            command=queries.actor_info(uid=uid, password=self.__password),
+            command=queries.actor_info(
+                uid=uid,
+                include_log_messages=include_log_messages,
+                include_integrations_registered_locations=include_integrations_registered_locations,
+                password=self.__password,
+            ),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
     def get_actor_internal_variables(
         self, uid: str, include_reference_values: bool = True
     ) -> List[dict]:
@@ -1909,27 +1923,30 @@
         )
 
     def get_actor_status_info(
         self,
         uid: str,
         hid: str,
         include_designs: bool = True,
+        include_design_values: bool = True,
         include_non_scalar_design_values: bool = False,
         include_algorithm_info: bool = False,
     ) -> Dict:
         """Get status info about actor defined by actor uid and state Hid.
 
         Parameters
         ----------
         uid : str
             Actor uid.
         hid: str
             State/Design hierarchical id.
         include_designs: bool
             Include (result) designs in status info response.
+        include_design_values: bool
+            Include values in (result) designs.
         include_non_scalar_design_values: bool
             Include non scalar values in (result) designs.
         include_algorithm_info: bool
             Include algorithm result info in status info response.
         Returns
         -------
         Dict
@@ -1945,14 +1962,15 @@
         """
         current_func_name = self.get_actor_status_info.__name__
         return self.send_command(
             command=queries.actor_status_info(
                 uid=uid,
                 hid=hid,
                 include_designs=include_designs,
+                include_design_values=include_design_values,
                 include_non_scalar_design_values=include_non_scalar_design_values,
                 include_algorithm_info=include_algorithm_info,
                 password=self.__password,
             ),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
@@ -2194,25 +2212,37 @@
             ),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )["number_of_samples"]
 
     def get_full_project_status_info(
         self,
+        include_designs: bool = True,
+        include_design_values: bool = True,
         include_non_scalar_design_values: bool = False,
         include_algorithm_info: bool = False,
+        include_log_messages: bool = True,
+        include_integrations_registered_locations: bool = True,
     ) -> Dict:
         """Get full project status info.
 
         Parameters
         ----------
+        include_designs: bool
+            Include (result) designs in status info response.
+        include_design_values: bool
+            Include values in (result) designs.
         include_non_scalar_design_values: bool
             Include non scalar values in (result) designs.
         include_algorithm_info: bool
             Include algorithm result info in status info response.
+        include_log_messages: bool, optional
+            Whether actor log messages are to be included.
+        include_integrations_registered_locations: bool, optional
+            Whether registered integration locations are to be included.
         Returns
         -------
         Dict
             Full project status info.
 
         Raises
         ------
@@ -2222,16 +2252,20 @@
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         current_func_name = self.get_full_project_status_info.__name__
         return self.send_command(
             command=queries.full_project_status_info(
+                include_designs=include_designs,
+                include_design_values=include_design_values,
                 include_non_scalar_design_values=include_non_scalar_design_values,
                 include_algorithm_info=include_algorithm_info,
+                include_log_messages=include_log_messages,
+                include_integrations_registered_locations=include_integrations_registered_locations,
                 password=self.__password,
             ),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
     def get_full_project_tree(self) -> Dict:
@@ -2278,24 +2312,83 @@
         current_func_name = self.get_full_project_tree_with_properties.__name__
         return self.send_command(
             command=queries.full_project_tree_with_properties(password=self.__password),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
+    def get_full_subtree_status_info(
+        self,
+        uid: str,
+        include_designs: bool = True,
+        include_design_values: bool = True,
+        include_non_scalar_design_values: bool = False,
+        include_algorithm_info: bool = False,
+        include_log_messages: bool = True,
+        include_integrations_registered_locations: bool = True,
+    ) -> Dict:
+        """Get full status info for a sub tree.
+
+        Parameters
+        ----------
+        uid : str
+            Actor uid.
+        include_designs: bool
+            Include (result) designs in status info response.
+        include_design_values: bool
+            Include values in (result) designs.
+        include_non_scalar_design_values: bool
+            Include non scalar values in (result) designs.
+        include_algorithm_info: bool
+            Include algorithm result info in status info response.
+        include_log_messages: bool, optional
+            Whether actor log messages are to be included.
+        include_integrations_registered_locations: bool, optional
+            Whether registered integration locations are to be included.
+
+        Returns
+        -------
+        Dict
+            Status info for the specified sub tree.
+
+        Raises
+        ------
+        OslCommunicationError
+            Raised when an error occurs while communicating with server.
+        OslCommandError
+            Raised when the command or query fails.
+        TimeoutError
+            Raised when the timeout float value expires.
+        """
+        current_func_name = self.get_full_subtree_status_info.__name__
+        return self.send_command(
+            command=queries.full_subtree_status_info(
+                uid=uid,
+                include_designs=include_designs,
+                include_design_values=include_design_values,
+                include_non_scalar_design_values=include_non_scalar_design_values,
+                include_algorithm_info=include_algorithm_info,
+                include_log_messages=include_log_messages,
+                include_integrations_registered_locations=include_integrations_registered_locations,
+                password=self.__password,
+            ),
+            timeout=self.timeouts_register.get_value(current_func_name),
+            max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
+        )
+
     @deprecated(version="0.6.0", reason="Use :py:attr:`TcpOslServer.host` instead.")
-    def get_host(self) -> Union[str, None]:
+    def get_host(self) -> Optional[str]:
         """Get optiSLang server address or domain name.
 
         Get a string representation of an IPv4/v6 address or domain name
         of the running optiSLang server.
 
         Returns
         -------
-        timeout: Union[int, None]
+        timeout: Optional[str]
             The IPv4/v6 address or domain name of the running optiSLang server, if applicable.
             Defaults to ``None``.
         """
         return self.__host
 
     def get_hpc_licensing_forwarded_environment(self, uid: str) -> Dict:
         """Get hpc licensing forwarded environment for certain actor.
@@ -2436,38 +2529,38 @@
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         return self._get_osl_version_string()
 
     @deprecated(version="0.6.0", reason="Use :py:attr:`TcpOslServer.port` instead.")
-    def get_port(self) -> Union[int, None]:
+    def get_port(self) -> Optional[int]:
         """Get the port the osl server is listening on.
 
         Returns
         -------
-        timeout: Union[int, None]
+        timeout: Optional[int]
             The port the osl server is listening on, if applicable.
             Defaults to ``None``.
         """
         return self.__port
 
     @deprecated(
         version="0.6.0",
         reason=(
             "This functionality was moved to "
             ":py:class:`Project <ansys.optislang.core.project.Project>`."
         ),
     )
-    def get_project_description(self) -> Union[str, None]:
+    def get_project_description(self) -> Optional[str]:
         """Get description of optiSLang project.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             optiSLang project description. If no project is loaded in the optiSLang,
             returns ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
@@ -2486,20 +2579,20 @@
     @deprecated(
         version="0.6.0",
         reason=(
             "This functionality was moved to "
             ":py:class:`Project <ansys.optislang.core.project.Project>`."
         ),
     )
-    def get_project_location(self) -> Union[Path, None]:
+    def get_project_location(self) -> Optional[Path]:
         """Get path to the optiSLang project file.
 
         Returns
         -------
-        Union[pathlib.Path, None]
+        Optional[pathlib.Path]
             Path to the optiSLang project file. If no project is loaded in the optiSLang,
             returns ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
@@ -2515,20 +2608,20 @@
     @deprecated(
         version="0.6.0",
         reason=(
             "This functionality was moved to "
             ":py:class:`Project <ansys.optislang.core.project.Project>`."
         ),
     )
-    def get_project_name(self) -> Union[str, None]:
+    def get_project_name(self) -> Optional[str]:
         """Get name of the optiSLang project.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             Name of the optiSLang project. If no project is loaded in the optiSLang,
             returns ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
@@ -2545,20 +2638,20 @@
     @deprecated(
         version="0.6.0",
         reason=(
             "This functionality was moved to "
             ":py:class:`Project <ansys.optislang.core.project.Project>`."
         ),
     )
-    def get_project_status(self) -> Union[str, None]:
+    def get_project_status(self) -> Optional[str]:
         """Get status of the optiSLang project.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             optiSLang project status. If no project is loaded in the optiSLang,
             returns ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
@@ -2641,14 +2734,51 @@
         current_func_name = self.get_project_tree_systems_with_properties.__name__
         return self.send_command(
             command=queries.project_tree_systems_with_properties(password=self.__password),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
+    def get_result_design(
+        self,
+        uid: str,
+        design_id: str,
+    ) -> Dict:
+        """Get specific result design values defined by actor uid and design ID.
+
+        Parameters
+        ----------
+        uid : str
+            Actor uid.
+        design_id: str
+            Design ID.
+        Returns
+        -------
+        Dict
+            Result design values.
+        Raises
+        ------
+        OslCommunicationError
+            Raised when an error occurs while communicating with server.
+        OslCommandError
+            Raised when the command or query fails.
+        TimeoutError
+            Raised when the timeout float value expires.
+        """
+        current_func_name = self.get_result_design.__name__
+        return self.send_command(
+            command=queries.result_design(
+                uid=uid,
+                design_id=design_id,
+                password=self.__password,
+            ),
+            timeout=self.timeouts_register.get_value(current_func_name),
+            max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
+        )
+
     def get_server_info(self) -> Dict:
         """Get information about the application, the server configuration and the open projects.
 
         Returns
         -------
         Dict
             Information data as dictionary.
@@ -2697,27 +2827,36 @@
             ).get("status")
             == "success"
         )
 
     def get_systems_status_info(
         self,
         include_designs: bool = True,
+        include_design_values: bool = True,
         include_non_scalar_design_values: bool = False,
         include_algorithm_info: bool = False,
+        include_log_messages: bool = True,
+        include_integrations_registered_locations: bool = True,
     ) -> Dict:
         """Get project status info, including systems only.
 
         Parameters
         ----------
         include_designs: bool
             Include (result) designs in status info response.
+        include_design_values: bool
+            Include values in (result) designs.
         include_non_scalar_design_values: bool
             Include non scalar values in (result) designs.
         include_algorithm_info: bool
             Include algorithm result info in status info response.
+        include_log_messages: bool, optional
+            Whether actor log messages are to be included.
+        include_integrations_registered_locations: bool, optional
+            Whether registered integration locations are to be included.
         Returns
         -------
         Dict
             Project status info including systems only.
 
         Raises
         ------
@@ -2728,32 +2867,35 @@
         TimeoutError
             Raised when the timeout float value expires.
         """
         current_func_name = self.get_systems_status_info.__name__
         return self.send_command(
             command=queries.systems_status_info(
                 include_designs=include_designs,
+                include_design_values=include_design_values,
                 include_non_scalar_design_values=include_non_scalar_design_values,
                 include_algorithm_info=include_algorithm_info,
+                include_log_messages=include_log_messages,
+                include_integrations_registered_locations=include_integrations_registered_locations,
                 password=self.__password,
             ),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
     @deprecated(
         version="0.5.0",
         reason="Use :py:attr:`TcpOslServer.timeouts_register.default_value` instead.",
     )
-    def get_timeout(self) -> Union[float, None]:
+    def get_timeout(self) -> Optional[float]:
         """Get current timeout value for execution of commands.
 
         Returns
         -------
-        timeout: Union[float, None]
+        timeout: Optional[float]
             Timeout in seconds to perform commands.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
@@ -2842,14 +2984,15 @@
 
     def open(
         self,
         file_path: Union[str, Path],
         force: bool = True,
         restore: bool = False,
         reset: bool = False,
+        project_properties_file: Optional[str] = None,
     ) -> None:
         """Open a new project.
 
         Parameters
         ----------
         file_path : Union[str, pathlib.Path]
             Path to the optiSLang project file to open.
@@ -2858,14 +3001,16 @@
             Non-critical errors include:
             - Timestamp of (auto) save point newer than project timestamp
             - Project (file) incomplete
         restore : bool, optional
             Whether to restore project from last (auto) save point (if present).
         reset : bool, optional
             Whether to reset project after load.
+        project_properties_file : Optional[str], optional
+            Project properties file to import, by default ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
             Raised when the command or query fails.
@@ -2889,14 +3034,15 @@
         self.send_command(
             command=commands.open(
                 path=str(file_path.as_posix()),
                 do_force=force,
                 do_restore=restore,
                 do_reset=reset,
                 password=self.__password,
+                project_properties_file=project_properties_file,
             ),
             timeout=self.timeouts_register.get_value(current_func_name),
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
     def re_register_locations_as_parameter(self, uid: str) -> None:
         """Adjust all input locations with the already registered parameters.
@@ -3545,15 +3691,15 @@
     def send_command(self, command: str, **kwargs) -> Dict:
         """Send command or query to the optiSLang server.
 
         Parameters
         ----------
         command: str
             Command or query to be executed on optiSLang server.
-        timeout: Union[float, None], optional
+        timeout: Optional[float], optional
             Timeout to execute command. If not provided,
             `TcpOslServer.timeouts_register.default_value` is used.
         max_request_attempts: int, optional
             Maximum number of attempts to execute command. If not provided,
             `TcpOslServer.max_request_attempts_register.default_value` is used.
 
         Returns
@@ -3698,32 +3844,32 @@
             max_request_attempts=self.max_request_attempts_register.get_value(current_func_name),
         )
 
     @deprecated(
         version="0.5.0",
         reason="Use :py:attr:`TcpOslServer.timeouts_register.default_value` instead.",
     )
-    def set_timeout(self, timeout: Union[float, None] = None) -> None:
+    def set_timeout(self, timeout: Optional[float] = None) -> None:
         """Set timeout value for execution of commands.
 
         Parameters
         ----------
-        timeout: Union[float, None]
+        timeout: Optional[float]
             Timeout in seconds to perform commands, it must be greater than zero or ``None``.
             Another functions will raise a timeout exception if the timeout period value has
             elapsed before the operation has completed.
             If ``None`` is given, functions will wait until they're finished (no timeout
             exception is raised). Defaults to ``30``.
 
         Raises
         ------
         ValueError
             Raised when timeout <= 0.
         TypeError
-            Raised when timeout not Union[float, None].
+            Raised when timeout not type of ``float`` or ``None``.
         """
         self.timeouts_register.default_value = timeout
 
     def shutdown(self, force: bool = False) -> None:
         """Shutdown the optiSLang server.
 
         Stop listening for incoming connections, discard pending requests, and shut down
@@ -3749,27 +3895,26 @@
         TimeoutError
             Raised when the parameter force is ``False`` and the timeout float value expires.
         """
         self.__stop_listeners_registration_thread()
         self.__unregister_all_listeners()
         self.__dispose_all_listeners()
 
-        if self.__shutdown_on_finished in (False, None):
-            try:
-                current_func_name = self.shutdown.__name__
-                self.send_command(
-                    command=commands.shutdown(self.__password),
-                    timeout=self.timeouts_register.get_value(current_func_name),
-                    max_request_attempts=self.max_request_attempts_register.get_value(
-                        current_func_name
-                    ),
-                )
-            except Exception:
-                if not force or self.__osl_process is None:
-                    raise
+        try:
+            current_func_name = self.shutdown.__name__
+            self.send_command(
+                command=commands.shutdown(force=force, password=self.__password),
+                timeout=self.timeouts_register.get_value(current_func_name),
+                max_request_attempts=self.max_request_attempts_register.get_value(
+                    current_func_name
+                ),
+            )
+        except Exception:
+            if not force or self.__osl_process is None:
+                raise
 
         # If desired actively force osl process to terminate
         if force and self.__osl_process is not None:
             self._force_shutdown_local_process()
 
     def start(self, wait_for_started: bool = True, wait_for_finished: bool = True) -> None:
         """Start project execution.
@@ -4206,23 +4351,23 @@
         )
 
         if not listener.is_initialized():
             raise RuntimeError("Cannot start listener of optiSLang server port.")
 
         return listener
 
-    def __create_exec_started_listener(self, timeout: Union[float, None] = None) -> TcpOslListener:
+    def __create_exec_started_listener(self, timeout: Optional[float] = None) -> TcpOslListener:
         """Create exec_started listener and add to self.__listeners.
 
         Returns
         -------
         exec_started_listener: TcpOslListener
             Listener registered to the optiSLang server and subscribed
             for push notifications.
-        timeout: Union[float, None]
+        timeout: Optional[float], optional
             Listener's timeout.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
@@ -4244,23 +4389,23 @@
                 ServerNotification.CHECK_FAILED,
             ],
         )
         exec_started_listener.refresh_listener_registration = True
         self.__listeners["exec_started_listener"] = exec_started_listener
         return exec_started_listener
 
-    def __create_exec_finished_listener(self, timeout: Union[float, None] = None) -> TcpOslListener:
+    def __create_exec_finished_listener(self, timeout: Optional[float] = None) -> TcpOslListener:
         """Create exec_finished listener and add to self.__listeners.
 
         Returns
         -------
         exec_finished_listener: TcpOslListener
             Listener registered to the optiSLang server and subscribed
             for push notifications.
-        timeout: Union[float, None]
+        timeout: Optional[float], optional
             Listener's timeout.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
         OslCommandError
@@ -4304,20 +4449,20 @@
 
     def __dispose_all_listeners(self) -> None:
         """Dispose all listeners."""
         for listener in self.__listeners.values():
             listener.dispose()
         self.__listeners = {}
 
-    def __get_project_status(self) -> Union[str, None]:
+    def __get_project_status(self) -> Optional[str]:
         """Get status of the optiSLang project.
 
         Returns
         -------
-        Union[str, None]
+        Optional[str]
             optiSLang project status. If no project is loaded in the optiSLang,
             returns ``None``.
 
         Raises
         ------
         OslCommunicationError
             Raised when an error occurs while communicating with server.
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/project.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/project.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/server_commands.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/server_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,15 +578,20 @@
     str
         JSON string of ``new`` command.
     """
     return _to_json(_gen_server_command(command=_NEW, password=password))
 
 
 def open(
-    path: str, do_force: bool, do_restore: bool, do_reset: bool, password: Optional[str] = None
+    path: str,
+    do_force: bool,
+    do_restore: bool,
+    do_reset: bool,
+    password: Optional[str] = None,
+    project_properties_file: Optional[str] = None,
 ) -> str:
     """Generate JSON string of ``open`` command.
 
     Parameters
     ----------
     path: str
         path.
@@ -594,25 +599,29 @@
         True/False.
     do_restore: bool
         True/False.
     do_reset: bool
         True/False.
     password : Optional[str], optional
         Password, by default ``None``.
+    project_properties_file : Optional[str], optional
+        Project properties file to import, by default ``None``.
 
     Returns
     -------
     str
         JSON string of ``open`` command.
     """
     args: CommandArgs = {}
     args["path"] = path
     args["do_force"] = do_force
     args["do_restore"] = do_restore
     args["do_reset"] = do_reset
+    if project_properties_file is not None:
+        args["project_properties_file"] = project_properties_file
 
     return _to_json(_gen_server_command(command=_OPEN, args=args, password=password))
 
 
 def pause(password: Optional[str] = None) -> str:
     """Generate JSON string of pause command.
 
@@ -1716,28 +1725,31 @@
     return _to_json(
         _gen_server_command(
             command=_SHOW_NODE_DIALOG, actor_uid=actor_uid, args=args, password=password
         )
     )
 
 
-def shutdown(password: Optional[str] = None) -> str:
+def shutdown(force: bool = False, password: Optional[str] = None) -> str:
     """Generate JSON string of ``shutdown`` command.
 
     Parameters
     ----------
     password : Optional[str], optional
         Password, by default ``None``.
 
     Returns
     -------
     str
         JSON string of ``shutdown`` command.
     """
-    return _to_json(_gen_server_command(command=_SHUTDOWN, password=password))
+    args: CommandArgs = {}
+    args["force"] = force
+
+    return _to_json(_gen_server_command(command=_SHUTDOWN, args=args, password=password))
 
 
 def shutdown_when_finished(password: Optional[str] = None) -> str:
     """Generate JSON string of ``shutdown_when_finished`` command.
 
     Parameters
     ----------
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/tcp/server_queries.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/server_queries.py`

 * *Files 19% similar despite different names*

```diff
@@ -47,35 +47,49 @@
 _GET_CRITERIA = "GET_CRITERIA"
 _GET_CRITERION = "GET_CRITERION"
 _HPC_LICENSING_FORWARDED_ENVIRONMENT = "HPC_LICENSING_FORWARDED_ENVIRONMENT"
 _INPUT_SLOT_VALUE = "INPUT_SLOT_VALUE"
 _OUTPUT_SLOT_VALUE = "OUTPUT_SLOT_VALUE"
 _PROJECT_TREE_SYSTEMS = "PROJECT_TREE_SYSTEMS"
 _PROJECT_TREE_SYSTEMS_WITH_PROPERTIES = "PROJECT_TREE_SYSTEMS_WITH_PROPERTIES"
+_RESULT_DESIGN = "RESULT_DESIGN"
 _SERVER_INFO = "SERVER_INFO"
 _SERVER_IS_ALIVE = "SERVER_IS_ALIVE"
 _SYSTEMS_STATUS_INFO = "SYSTEMS_STATUS_INFO"
+_FULL_SUBTREE_STATUS_INFO = "FULL_SUBTREE_STATUS_INFO"
 
 
-def actor_info(uid: str, password: Optional[str] = None) -> str:
+def actor_info(
+    uid: str,
+    include_log_messages: bool = True,
+    include_integrations_registered_locations: bool = True,
+    password: Optional[str] = None,
+) -> str:
     """Generate JSON string of actor_info query.
 
     Parameters
     ----------
     uid: str
         Uid entry.
+    include_log_messages: bool, optional
+        Whether actor log messages are to be included.
+    include_integrations_registered_locations: bool, optional
+        Whether registered integration locations are to be included.
     password : Optional[str], optional
         Password, by default ``None``.
 
     Returns
     -------
     str
         JSON string of actor_info query.
     """
-    return _to_json(_gen_query(what=_ACTOR_INFO, uid=uid, password=password))
+    args: QueryArgs = {}
+    args["include_log_messages"] = include_log_messages
+    args["include_integrations_registered_locations"] = include_integrations_registered_locations
+    return _to_json(_gen_query(what=_ACTOR_INFO, uid=uid, args=args, password=password))
 
 
 def actor_internal_variables(
     uid: str, include_reference_values: bool = True, password: Optional[str] = None
 ) -> str:
     """Generate JSON string of actor_internal_variables query.
 
@@ -263,42 +277,46 @@
     return _to_json(_gen_query(what=_ACTOR_STATES, uid=uid, args=args, password=password))
 
 
 def actor_status_info(
     uid: str,
     hid: str,
     include_designs: bool = True,
+    include_design_values: bool = True,
     include_non_scalar_design_values: bool = False,
     include_algorithm_info: bool = False,
     password: Optional[str] = None,
 ) -> str:
     """Generate JSON string of actor_status_info query.
 
     Parameters
     ----------
     uid: str
         Uid entry.
     hid: str
         Hid entry.
     include_designs: bool
         Include (result) designs in status info response.
+    include_design_values: bool
+        Include values in (result) designs.
     include_non_scalar_design_values: bool
         Include non scalar values in (result) designs.
     include_algorithm_info: bool
         Include algorithm result info in status info response.
     password : Optional[str], optional
         Password. Defaults to ``None``.
 
     Returns
     -------
     str
         JSON string of actor_status_info query.
     """
     args: QueryArgs = {}
     args["include_designs"] = include_designs
+    args["include_design_values"] = include_design_values
     args["include_non_scalar_design_values"] = include_non_scalar_design_values
     args["include_algorithm_info"] = include_algorithm_info
     return _to_json(
         _gen_query(what=_ACTOR_STATUS_INFO, uid=uid, args=args, hid=hid, password=password)
     )
 
 
@@ -435,37 +453,53 @@
             args=args,
             password=password,
         )
     )
 
 
 def full_project_status_info(
+    include_designs: bool = True,
+    include_design_values: bool = True,
     include_non_scalar_design_values: bool = False,
     include_algorithm_info: bool = False,
+    include_log_messages: bool = True,
+    include_integrations_registered_locations: bool = True,
     password: Optional[str] = None,
 ) -> str:
     """Generate JSON string of full_project_status_info query.
 
     Parameters
     ----------
+    include_designs: bool
+        Include (result) designs in status info response.
+    include_design_values: bool
+        Include values in (result) designs.
     include_non_scalar_design_values: bool
         Include non scalar values in (result) designs.
     include_algorithm_info: bool
         Include algorithm result info in status info response.
+    include_log_messages: bool, optional
+        Whether actor log messages are to be included.
+    include_integrations_registered_locations: bool, optional
+        Whether registered integration locations are to be included.
     password : Optional[str], optional
         Password. Defaults to ``None``.
 
     Returns
     -------
     str
         JSON string of full_project_status_info query.
     """
     args: QueryArgs = {}
+    args["include_designs"] = include_designs
+    args["include_design_values"] = include_design_values
     args["include_non_scalar_design_values"] = include_non_scalar_design_values
     args["include_algorithm_info"] = include_algorithm_info
+    args["include_log_messages"] = include_log_messages
+    args["include_integrations_registered_locations"] = include_integrations_registered_locations
     return _to_json(_gen_query(what=_FULL_PROJECT_STATUS_INFO, args=args, password=password))
 
 
 def full_project_tree(password: Optional[str] = None) -> str:
     """Generate JSON string of full_project_tree query.
 
     Parameters
@@ -493,14 +527,62 @@
     -------
     str
         JSON string of full_project_tree_with_properties query.
     """
     return _to_json(_gen_query(what=_FULL_PROJECT_TREE_WITH_PROPERTIES, password=password))
 
 
+def full_subtree_status_info(
+    uid: str,
+    include_designs: bool = True,
+    include_design_values: bool = True,
+    include_non_scalar_design_values: bool = False,
+    include_algorithm_info: bool = False,
+    include_log_messages: bool = True,
+    include_integrations_registered_locations: bool = True,
+    password: Optional[str] = None,
+) -> str:
+    """Generate JSON string of full_subtree_status_info query.
+
+    Parameters
+    ----------
+    uid: str
+        Uid entry.
+    include_designs: bool
+        Include (result) designs in status info response.
+    include_design_values: bool
+        Include values in (result) designs.
+    include_non_scalar_design_values: bool
+        Include non scalar values in (result) designs.
+    include_algorithm_info: bool
+        Include algorithm result info in status info response.
+    include_log_messages: bool, optional
+        Whether actor log messages are to be included.
+    include_integrations_registered_locations: bool, optional
+        Whether registered integration locations are to be included.
+    password : Optional[str], optional
+        Password. Defaults to ``None``.
+
+    Returns
+    -------
+    str
+        JSON string of systems_status_info query.
+    """
+    args: QueryArgs = {}
+    args["include_designs"] = include_designs
+    args["include_design_values"] = include_design_values
+    args["include_non_scalar_design_values"] = include_non_scalar_design_values
+    args["include_algorithm_info"] = include_algorithm_info
+    args["include_log_messages"] = include_log_messages
+    args["include_integrations_registered_locations"] = include_integrations_registered_locations
+    return _to_json(
+        _gen_query(what=_FULL_SUBTREE_STATUS_INFO, uid=uid, args=args, password=password)
+    )
+
+
 def get_criteria(uid: str, password: Optional[str] = None) -> str:
     """Generate JSON string of get_criteria query.
 
     Parameters
     ----------
     uid: str
         Uid entry.
@@ -635,14 +717,40 @@
     -------
     str
         JSON string of project_tree_with_properties query.
     """
     return _to_json(_gen_query(what=_PROJECT_TREE_SYSTEMS_WITH_PROPERTIES, password=password))
 
 
+def result_design(
+    uid: str,
+    design_id: str,
+    password: Optional[str] = None,
+) -> str:
+    """Generate JSON string of result_design query.
+
+    Parameters
+    ----------
+    uid: str
+        Uid entry.
+    design_id: str
+        Design ID entry.
+    password : Optional[str], optional
+        Password. Defaults to ``None``.
+
+    Returns
+    -------
+    str
+        JSON string of result_design query.
+    """
+    return _to_json(
+        _gen_query(what=_RESULT_DESIGN, uid=uid, design_id=design_id, password=password)
+    )
+
+
 def server_info(password: Optional[str] = None) -> str:
     """Generate JSON string of server_info query.
 
     Parameters
     ----------
     password : Optional[str], optional
         Password, by default ``None``.
@@ -669,50 +777,63 @@
         JSON string of server_is_alive query.
     """
     return _to_json(_gen_query(what=_SERVER_IS_ALIVE, password=password))
 
 
 def systems_status_info(
     include_designs: bool = True,
+    include_design_values: bool = True,
     include_non_scalar_design_values: bool = False,
     include_algorithm_info: bool = False,
+    include_log_messages: bool = True,
+    include_integrations_registered_locations: bool = True,
     password: Optional[str] = None,
 ) -> str:
     """Generate JSON string of systems_status_info query.
 
     Parameters
     ----------
     include_designs: bool
         Include (result) designs in status info response.
+    include_design_values: bool
+        Include values in (result) designs.
     include_non_scalar_design_values: bool
         Include non scalar values in (result) designs.
     include_algorithm_info: bool
         Include algorithm result info in status info response.
+    include_log_messages: bool, optional
+        Whether actor log messages are to be included.
+    include_integrations_registered_locations: bool, optional
+        Whether registered integration locations are to be included.
     password : Optional[str], optional
         Password. Defaults to ``None``.
 
     Returns
     -------
     str
         JSON string of systems_status_info query.
     """
     args: QueryArgs = {}
     args["include_designs"] = include_designs
+    args["include_design_values"] = include_design_values
     args["include_non_scalar_design_values"] = include_non_scalar_design_values
     args["include_algorithm_info"] = include_algorithm_info
+    args["include_log_messages"] = include_log_messages
+    args["include_integrations_registered_locations"] = include_integrations_registered_locations
     return _to_json(_gen_query(what=_SYSTEMS_STATUS_INFO, args=args, password=password))
 
 
 def _gen_query(
     what: str,
     password: Optional[str],
     uid: Optional[str] = None,
     hid: Optional[str] = None,
     args: Optional[QueryArgs] = None,
     slot_name: Optional[str] = None,
+    design_id: Optional[str] = None,
 ) -> Dict:
     """Generate query in desired format.
 
     Parameters
     ----------
     what : str
         Command type.
@@ -722,14 +843,16 @@
         Uid entry. Defaults to ``None``.
     hid: Optional[str], optional
         Hid entry. Defaults to ``None``.
     args: Optional[QueryArgs], optional
         Dictionary of features, e.g. "feature": "FEATURE_NAME".
     slot_name: Optional[str], optional
         Slot name. Defaults to ``None``.
+    design_id: Optional[str], optional
+        Design ID. Defaults to ``None``.
 
     Returns
     -------
     Dict
         Dictionary with specified query inputs.
     """
     query: Dict[str, Any] = {}
@@ -738,14 +861,16 @@
         query["uid"] = uid
     if hid is not None:
         query["hid"] = hid
     if args is not None:
         query["args"] = args
     if slot_name is not None:
         query["slot_name"] = slot_name
+    if design_id is not None:
+        query["design_id"] = design_id
     if password is not None:
         query["Password"] = password
     return query
 
 
 def _to_json(dict: Dict) -> str:
     """Convert dictionary to JSON.
```

### Comparing `ansys_optislang_core-0.6.3/src/ansys/optislang/core/utils.py` & `ansys_optislang_core-0.7.0/src/ansys/optislang/core/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.6.3/PKG-INFO` & `ansys_optislang_core-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: ansys-optislang-core
-Version: 0.6.3
+Version: 0.7.0
 Summary: A Python wrapper for Ansys optiSLang application.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: importlib-metadata>=4.0,<8
 Requires-Dist: psutil>=5.9
 Requires-Dist: Deprecated>=1.2.14
 Requires-Dist: build>=0.8.0 ; extra == "build"
 Requires-Dist: twine>=4.0.1 ; extra == "build"
-Requires-Dist: ansys-sphinx-theme==0.13.1 ; extra == "doc"
-Requires-Dist: matplotlib==3.8.2 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
-Requires-Dist: pypandoc==1.12 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
+Requires-Dist: matplotlib==3.8.4 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
+Requires-Dist: pypandoc==1.13 ; extra == "doc"
 Requires-Dist: Sphinx==7.2.6 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.15.0 ; extra == "doc"
 Requires-Dist: sphinxcontrib-images==0.9.4 ; extra == "doc"
-Requires-Dist: pytest==7.4.4 ; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
+Requires-Dist: pytest==8.1.2 ; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Requires-Dist: matplotlib>=3.5.3 ; extra == "tests"
 Project-URL: Documentation, https://optislang.docs.pyansys.com
 Project-URL: Homepage, https://optislang.docs.pyansys.com
 Project-URL: Source, https://github.com/ansys/pyoptislang
 Project-URL: Tracker, https://github.com/ansys/pyoptislang/issues
 Provides-Extra: build
 Provides-Extra: doc
@@ -45,16 +44,16 @@
 ===========
 |pyansys| |python| |pypi| |PyPIact| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |python| image:: https://img.shields.io/badge/Python-%3E%3D3.7-blue
-   :target: https://pypi.org/project/pyoptislang/
+.. |python| image:: https://img.shields.io/pypi/pyversions/ansys-optislang-core?logo=pypi
+   :target: https://pypi.org/project/ansys-optislang-core/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-optislang-core.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-optislang-core/
 
 .. |PyPIact| image:: https://img.shields.io/pypi/dm/ansys-optislang-core.svg?label=PyPI%20downloads
    :target: https://pypi.org/project/ansys-optislang-core/
@@ -86,27 +85,28 @@
 - Remote connections to Ansys optiSLang instances via TCP/IP
 - Create new Ansys optiSLang project
 - Open existing Ansys optiSLang project
 - Control Ansys optiSLang project execution
 - Save Ansys optiSLang project
 - Execute classic Ansys optiSLang Python API script on backend side
 - Evaluate designs on root project level
+- Create and connect nodes
 
 
 Documentation and issues
 ------------------------
 For comprehensive information on PyOptiSLang, see the latest release
 `documentation <https://optislang.docs.pyansys.com>`_. On the
 `PyOptiSLang Issues <https://github.com/ansys/pyoptislang/issues>`_ page,
 you can create issues to submit questions, report bugs, and request new features.
 This is the best place to post questions and code.
 
 Installation
 ------------
-The ``ansys-optislang-core`` package supports Python 3.7 through 3.11 on
+The ``ansys-optislang-core`` package supports Python 3.8 through 3.12 on
 Windows and Linux. Three modes of installation are available:
 
 - User installation
 - Developer installation
 - Offline installation
 
 For either a developer or offline installation, consider using a `virtual environment
@@ -152,20 +152,20 @@
 external networks. From the `Releases <https://github.com/ansys/pyoptislang/releases>`_
 page in the PyOptiSLang repository, you can find the wheelhouses for a particular release in its
 assets and download the wheelhouse corresponding to your setup.
 
 You can then install PyOptiSLang and all of its dependencies from one single entry point
 that can be shared internally, which eases the security review of the PyOptiSLang package content.
 
-For example, on Linux with Python 3.7, unzip the wheelhouse and install PyOptiSLang with code
+For example, on Linux with Python 3.8, unzip the wheelhouse and install PyOptiSLang with code
 like this:
 
 .. code:: bash
 
-    unzip PyOptiSLang-v0.1.0-wheelhouse-Linux-3.7.zip wheelhouse
+    unzip PyOptiSLang-v0.1.0-wheelhouse-Linux-3.8.zip wheelhouse
     pip install ansys-optislang-core -f wheelhouse --no-index --upgrade --ignore-installed
 
 If you're on Windows with Python 3.9, unzip the wheelhouse to a wheelhouse directory and
 then install using the same ``pip`` command as in the preceding Linux code example.
 
 Dependencies
 --------------
```

