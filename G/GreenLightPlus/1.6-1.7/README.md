# Comparing `tmp/greenlightplus-1.6.tar.gz` & `tmp/greenlightplus-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenlightplus-1.6.tar", last modified: Mon Apr 29 14:27:49 2024, max compression
+gzip compressed data, was "greenlightplus-1.7.tar", last modified: Mon Apr 29 17:36:57 2024, max compression
```

## Comparing `greenlightplus-1.6.tar` & `greenlightplus-1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 14:27:49.229707 greenlightplus-1.6/
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 14:27:49.218527 greenlightplus-1.6/GreenLightPlus/
--rw-r--r--   0 daidai     (501) staff       (20)    19173 2024-04-29 14:21:22.000000 greenlightplus-1.6/GreenLightPlus/README.md
--rw-r--r--   0 daidai     (501) staff       (20)      689 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/__init__.py
--rw-r--r--   0 daidai     (501) staff       (20)        0 2024-04-29 09:33:33.000000 greenlightplus-1.6/GreenLightPlus/config.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 14:27:49.221043 greenlightplus-1.6/GreenLightPlus/core/
--rw-r--r--   0 daidai     (501) staff       (20)    10378 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/core/green_light_model.py
--rw-r--r--   0 daidai     (501) staff       (20)    14630 2024-04-09 21:32:30.000000 greenlightplus-1.6/GreenLightPlus/core/greenhouse_env.py
--rw-r--r--   0 daidai     (501) staff       (20)    61665 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/core/greenhouse_geometry.py
--rw-r--r--   0 daidai     (501) staff       (20)    10046 2024-04-29 12:21:20.000000 greenlightplus-1.6/GreenLightPlus/core/greenlight_energyplus_simulation.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 14:27:49.226196 greenlightplus-1.6/GreenLightPlus/create_green_light_model/
--rw-r--r--   0 daidai     (501) staff       (20)     5614 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/change_res.py
--rw-r--r--   0 daidai     (501) staff       (20)     2713 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/create_green_light_model.py
--rw-r--r--   0 daidai     (501) staff       (20)     5257 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/ode.py
--rw-r--r--   0 daidai     (501) staff       (20)     3637 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_default_lamp_params.py
--rw-r--r--   0 daidai     (501) staff       (20)     3151 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_dep_params.py
--rw-r--r--   0 daidai     (501) staff       (20)    74154 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_aux.py
--rw-r--r--   0 daidai     (501) staff       (20)     2543 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_control.py
--rw-r--r--   0 daidai     (501) staff       (20)     3639 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_control_init.py
--rw-r--r--   0 daidai     (501) staff       (20)     4083 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_init.py
--rw-r--r--   0 daidai     (501) staff       (20)     5291 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_input.py
--rw-r--r--   0 daidai     (501) staff       (20)    11637 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_odes.py
--rw-r--r--   0 daidai     (501) staff       (20)    19680 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_params.py
--rw-r--r--   0 daidai     (501) staff       (20)     1895 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_states.py
--rw-r--r--   0 daidai     (501) staff       (20)     1307 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_time.py
--rw-r--r--   0 daidai     (501) staff       (20)     3001 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 14:27:49.226641 greenlightplus-1.6/GreenLightPlus/result_analysis/
--rw-r--r--   0 daidai     (501) staff       (20)     3167 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/result_analysis/energy_analysis.py
--rw-r--r--   0 daidai     (501) staff       (20)     3312 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/result_analysis/energy_yield_analysis.py
--rw-r--r--   0 daidai     (501) staff       (20)     7263 2024-04-16 09:09:37.000000 greenlightplus-1.6/GreenLightPlus/result_analysis/plot_green_light.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 14:27:49.228801 greenlightplus-1.6/GreenLightPlus/service_functions/
--rw-r--r--   0 daidai     (501) staff       (20)      798 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/co2_dens2ppm.py
--rw-r--r--   0 daidai     (501) staff       (20)      794 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/co2_ppm2dens.py
--rw-r--r--   0 daidai     (501) staff       (20)    15456 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/convert_epw2csv.py
--rw-r--r--   0 daidai     (501) staff       (20)    11525 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/cut_energy_plus_data.py
--rw-r--r--   0 daidai     (501) staff       (20)     9761 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/funcs.py
--rw-r--r--   0 daidai     (501) staff       (20)     3543 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/make_artificial_input.py
--rw-r--r--   0 daidai     (501) staff       (20)     1677 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/rh2vapor_dens.py
--rw-r--r--   0 daidai     (501) staff       (20)     1401 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/vapor_dens2pres.py
--rw-r--r--   0 daidai     (501) staff       (20)     1379 2024-04-09 19:17:21.000000 greenlightplus-1.6/GreenLightPlus/service_functions/vp2dens.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 14:27:49.229147 greenlightplus-1.6/GreenLightPlus.egg-info/
--rw-r--r--   0 daidai     (501) staff       (20)    20383 2024-04-29 14:27:49.000000 greenlightplus-1.6/GreenLightPlus.egg-info/PKG-INFO
--rw-r--r--   0 daidai     (501) staff       (20)     2006 2024-04-29 14:27:49.000000 greenlightplus-1.6/GreenLightPlus.egg-info/SOURCES.txt
--rw-r--r--   0 daidai     (501) staff       (20)        1 2024-04-29 14:27:49.000000 greenlightplus-1.6/GreenLightPlus.egg-info/dependency_links.txt
--rw-r--r--   0 daidai     (501) staff       (20)       59 2024-04-29 14:27:49.000000 greenlightplus-1.6/GreenLightPlus.egg-info/entry_points.txt
--rw-r--r--   0 daidai     (501) staff       (20)      102 2024-04-29 14:27:49.000000 greenlightplus-1.6/GreenLightPlus.egg-info/requires.txt
--rw-r--r--   0 daidai     (501) staff       (20)       15 2024-04-29 14:27:49.000000 greenlightplus-1.6/GreenLightPlus.egg-info/top_level.txt
--rw-r--r--   0 daidai     (501) staff       (20)    20383 2024-04-29 14:27:49.229588 greenlightplus-1.6/PKG-INFO
--rw-r--r--   0 daidai     (501) staff       (20)     1362 2024-04-29 14:27:43.000000 greenlightplus-1.6/pyproject.toml
--rw-r--r--   0 daidai     (501) staff       (20)       38 2024-04-29 14:27:49.229923 greenlightplus-1.6/setup.cfg
--rw-r--r--   0 daidai     (501) staff       (20)       85 2024-04-29 08:39:56.000000 greenlightplus-1.6/setup.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 17:36:57.718127 greenlightplus-1.7/
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 17:36:57.706978 greenlightplus-1.7/GreenLightPlus/
+-rw-r--r--   0 daidai     (501) staff       (20)    22246 2024-04-29 17:35:24.000000 greenlightplus-1.7/GreenLightPlus/README.md
+-rw-r--r--   0 daidai     (501) staff       (20)      689 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/__init__.py
+-rw-r--r--   0 daidai     (501) staff       (20)        0 2024-04-29 09:33:33.000000 greenlightplus-1.7/GreenLightPlus/config.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 17:36:57.709093 greenlightplus-1.7/GreenLightPlus/core/
+-rw-r--r--   0 daidai     (501) staff       (20)    10378 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/core/green_light_model.py
+-rw-r--r--   0 daidai     (501) staff       (20)    14630 2024-04-09 21:32:30.000000 greenlightplus-1.7/GreenLightPlus/core/greenhouse_env.py
+-rw-r--r--   0 daidai     (501) staff       (20)    61665 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/core/greenhouse_geometry.py
+-rw-r--r--   0 daidai     (501) staff       (20)    10046 2024-04-29 12:21:20.000000 greenlightplus-1.7/GreenLightPlus/core/greenlight_energyplus_simulation.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 17:36:57.713288 greenlightplus-1.7/GreenLightPlus/create_green_light_model/
+-rw-r--r--   0 daidai     (501) staff       (20)     5614 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/change_res.py
+-rw-r--r--   0 daidai     (501) staff       (20)     2713 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/create_green_light_model.py
+-rw-r--r--   0 daidai     (501) staff       (20)     5257 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/ode.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3637 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_default_lamp_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3151 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_dep_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)    74154 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_aux.py
+-rw-r--r--   0 daidai     (501) staff       (20)     2543 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_control.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3639 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_control_init.py
+-rw-r--r--   0 daidai     (501) staff       (20)     4083 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_init.py
+-rw-r--r--   0 daidai     (501) staff       (20)     5291 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_input.py
+-rw-r--r--   0 daidai     (501) staff       (20)    11637 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_odes.py
+-rw-r--r--   0 daidai     (501) staff       (20)    19680 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1895 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_states.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1307 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_time.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3001 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 17:36:57.713877 greenlightplus-1.7/GreenLightPlus/result_analysis/
+-rw-r--r--   0 daidai     (501) staff       (20)     3167 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/result_analysis/energy_analysis.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3312 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/result_analysis/energy_yield_analysis.py
+-rw-r--r--   0 daidai     (501) staff       (20)     7263 2024-04-16 09:09:37.000000 greenlightplus-1.7/GreenLightPlus/result_analysis/plot_green_light.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 17:36:57.717097 greenlightplus-1.7/GreenLightPlus/service_functions/
+-rw-r--r--   0 daidai     (501) staff       (20)      798 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/co2_dens2ppm.py
+-rw-r--r--   0 daidai     (501) staff       (20)      794 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/co2_ppm2dens.py
+-rw-r--r--   0 daidai     (501) staff       (20)    15456 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/convert_epw2csv.py
+-rw-r--r--   0 daidai     (501) staff       (20)    11525 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/cut_energy_plus_data.py
+-rw-r--r--   0 daidai     (501) staff       (20)     9761 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/funcs.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3543 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/make_artificial_input.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1677 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/rh2vapor_dens.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1401 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/vapor_dens2pres.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1379 2024-04-09 19:17:21.000000 greenlightplus-1.7/GreenLightPlus/service_functions/vp2dens.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 17:36:57.717405 greenlightplus-1.7/GreenLightPlus.egg-info/
+-rw-r--r--   0 daidai     (501) staff       (20)    23455 2024-04-29 17:36:57.000000 greenlightplus-1.7/GreenLightPlus.egg-info/PKG-INFO
+-rw-r--r--   0 daidai     (501) staff       (20)     2006 2024-04-29 17:36:57.000000 greenlightplus-1.7/GreenLightPlus.egg-info/SOURCES.txt
+-rw-r--r--   0 daidai     (501) staff       (20)        1 2024-04-29 17:36:57.000000 greenlightplus-1.7/GreenLightPlus.egg-info/dependency_links.txt
+-rw-r--r--   0 daidai     (501) staff       (20)       59 2024-04-29 17:36:57.000000 greenlightplus-1.7/GreenLightPlus.egg-info/entry_points.txt
+-rw-r--r--   0 daidai     (501) staff       (20)      102 2024-04-29 17:36:57.000000 greenlightplus-1.7/GreenLightPlus.egg-info/requires.txt
+-rw-r--r--   0 daidai     (501) staff       (20)       15 2024-04-29 17:36:57.000000 greenlightplus-1.7/GreenLightPlus.egg-info/top_level.txt
+-rw-r--r--   0 daidai     (501) staff       (20)    23455 2024-04-29 17:36:57.717996 greenlightplus-1.7/PKG-INFO
+-rw-r--r--   0 daidai     (501) staff       (20)     1362 2024-04-29 17:36:43.000000 greenlightplus-1.7/pyproject.toml
+-rw-r--r--   0 daidai     (501) staff       (20)       38 2024-04-29 17:36:57.718373 greenlightplus-1.7/setup.cfg
+-rw-r--r--   0 daidai     (501) staff       (20)       85 2024-04-29 08:39:56.000000 greenlightplus-1.7/setup.py
```

### Comparing `greenlightplus-1.6/GreenLightPlus/README.md` & `greenlightplus-1.7/GreenLightPlus/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 ## Languages
 - [English](README.md)
 - [中文](README_zh.md)
 
 # GreenLightPlus
 
-GreenLightPlus is a ToolKit for greenhouse environment simulation and energy consumption-yield analysis. It combines the original GreenLight model and the EnergyPlus simulation tool to investigate the energy consumption and output of different greenhouse structures.
+GreenLightPlus is a Python toolkit for greenhouse environment simulation and energy consumption and yield optimization, developed based on David Katzin's MATLAB version of the [GreenLight](https://github.com/davkat1/GreenLight) model. Compared to the original model, GreenLightPlus provides the following improvements and extensions:
 
-## Features
+- Ported the original model from MATLAB to Python, improving accessibility and extensibility.
+- Supports the generation of various greenhouse geometric structures for comparative analysis.
+- Integrates EnergyPlus simulation functionality for more accurate energy consumption calculations.
+- Includes a built-in reinforcement learning environment that can be used with AI algorithms to optimize greenhouse control strategies.
 
-- **Simulation and Analysis**: Provides comprehensive greenhouse environment simulation and energy consumption analysis.
-- **Diverse Greenhouse Structures**: Supports generating six different greenhouse geometries.
-- **Reinforcement Learning Environment**: Includes a customized reinforcement learning environment for greenhouse control tasks.
-- **Integrated Simulation**: Combines the GreenLight model with EnergyPlus simulations, offering in-depth energy consumption and yield research for different greenhouse configurations.
+GreenLightPlus aims to help users design and manage greenhouses more efficiently, achieving energy optimization and crop yield enhancement. By using this toolkit, users can explore different greenhouse design options, evaluate their energy performance, and employ advanced optimization algorithms to find the best control strategies, improving the economic and environmental benefits of the greenhouse.
+
+## Key Features
+
+- **Comprehensive Greenhouse Environment Simulation**: GreenLightPlus provides a complete greenhouse environment simulation, including the dynamic changes of key parameters such as temperature, humidity, light, and CO2 concentration, as well as the simulation of crop growth processes.
+
+- **Flexible Greenhouse Geometric Modeling**: The toolkit supports the generation of six common types of greenhouse geometric structures, including triangular, semi-circular, flat arch, Gothic arch, sawtooth, and sawtooth arch. Users can choose the appropriate structure for analysis based on their requirements.
+
+- **Reinforcement Learning Optimization Strategies**: GreenLightPlus includes a built-in reinforcement learning environment specifically designed for greenhouse control tasks. Users can utilize this environment to train AI models that automatically learn optimal greenhouse control strategies, improving energy utilization efficiency and crop yield.
+
+- **Energy Consumption Analysis and Yield Prediction**: Through integration with EnergyPlus, GreenLightPlus can perform detailed energy consumption analyses for different greenhouse configurations and predict crop yields based on environmental conditions and control strategies, providing important information for greenhouse design and operation.
 
 ## Core Modules
 
 - `green_light_model.py` - Implements the Python-based GreenLight model for greenhouse environment simulation.
 - `greenhouse_env.py` - Defines the greenhouse environment class for reinforcement learning.
 - `greenhouse_geometry.py` - Used to generate geometric models for different greenhouse structures.
 - `greenlight_energyplus_simulation.py` - Combines the GreenLight model and EnergyPlus for simulation and analysis.
@@ -28,15 +38,15 @@
 
 To ensure users can smoothly use the GreenLightPlus package in combination with EnergyPlus for simulations, we need to provide detailed guidance on downloading and installing EnergyPlus. Here are the steps for downloading and installing EnergyPlus, as well as obtaining the necessary weather files, which can be included in the README:
 
 ---
 
 ## Prerequisites: Installing EnergyPlus
 
-To run the EnergyPlus-combined simulations in the GreenLightPlus package, you need to have EnergyPlus installed on your system. The following steps will guide you through downloading and installing EnergyPlus on a Linux system.
+To run the EnergyPlus-combined simulations in the GreenLightPlus package, you need to have EnergyPlus installed on your system. 
 
 ### Download and Install
 
 1. **Download EnergyPlus**: Use the `wget` command to download the Linux version of EnergyPlus from the official GitHub repository.
 
    ```bash
    wget https://github.com/NREL/EnergyPlus/releases/download/v23.2.0/EnergyPlus-23.2.0-7636e6b3e9-Linux-Ubuntu22.04-x86_64.tar.gz
@@ -224,15 +234,27 @@
 
 #### Functionality Description
 
 This example code demonstrates how to use the GreenLightModel class to run greenhouse environment simulations. By looping through the growing season, the simulation steps through the environmental changes, and the `calculate_energy_consumption` function is used to evaluate energy consumption and yield. Finally, the `plot_green_light` function visualizes the results of the entire simulation process, showing the changes in various environmental parameters inside the greenhouse, such as temperature, humidity, CO2 concentration, and lighting and heating energy consumption over time.
 
 #### Result Display
 
-The `plot_green_light` function will generate a chart displaying the changes in environmental parameters inside and outside the greenhouse, such as temperature, humidity, CO2 concentration, as well as lighting and heating energy consumption. This will help users evaluate the effectiveness of the simulation and optimize the greenhouse design.
+The `plot_green_light` function generates a comprehensive figure displaying the changes in environmental parameters and crop growth dynamics within the simulated greenhouse. The figure includes the following subplots:
+
+1. Indoor and outdoor temperature in degrees Celsius (°C).
+2. Indoor and outdoor vapor pressure in Pascals (Pa).
+3. Indoor and outdoor relative humidity as a percentage (%).
+4. Indoor and outdoor CO2 concentration in both milligrams per cubic meter (mg m^{-3}) and parts per million (ppm).
+5. Outdoor global solar radiation, PAR (Photosynthetically Active Radiation) above the canopy from both sun and lamps, lamp electric input, and PAR above the canopy from sun and lamps separately, all in Watts per square meter (W m^{-2}).
+6. PPFD (Photosynthetic Photon Flux Density) from the sun and lamps in micromoles of PAR per square meter per second (μmol (PAR) m^{-2} s^{-1}).
+7. Net assimilation of CO2, net photosynthesis, growth respiration, and maintenance respiration in milligrams per square meter per second (mg m^{-2} s^{-1}).
+8. Fruit, stem, and leaf dry weight in milligrams of CH2O per square meter (mg (CH2O) m^{-2}), buffer content also in mg (CH2O) m^{-2}, and LAI (Leaf Area Index) in square meters per square meter (m^2 m^{-2}).
+9. Fruit dry weight in milligrams of CH2O per square meter (mg (CH2O) m^{-2}) and fruit harvest in milligrams of CH2O per square meter per second (mg (CH2O) m^{-2} s^{-1}).
+10. Various temperature states of the greenhouse components in degrees Celsius (°C).
+
 
 ![alt text](image-1.png)
 
 ### 3. Using GreenLightPlus to Run Combined GreenLight and EnergyPlus Simulations
 
 GreenLightPlus integrates the GreenLight model and EnergyPlus, providing higher accuracy greenhouse environment simulations and more detailed energy consumption analyses.
 
@@ -391,14 +413,18 @@
 
 This example code demonstrates how to use Ray RLlib and the PPO algorithm to train a reinforcement learning model for greenhouse environment optimization. By adjusting the environment parameters and training settings, you can explore different strategies to improve the greenhouse's energy efficiency and crop yield.
 
 #### Result Display
 
 Checkpoints will be saved periodically during the training process, and the current training results will be printed. These results help users evaluate the algorithm's performance and iteratively optimize the greenhouse management strategies.
 
+
 ## Contributing
 
 Contributions through Pull Requests or Issues for feature enhancements or bug reports are welcome.
 
 ## License
 
-This project is licensed under the GNU GPLv3 License. See the `LICENSE` file for details.
+This project is licensed under the GNU GPLv3 License. See the `LICENSE` file for details.
+
+## References
+David Katzin, Simon van Mourik, Frank Kempkes, and Eldert J. Van Henten. 2020. "GreenLight - An Open Source Model for Greenhouses with Supplemental Lighting: Evaluation of Heat Requirements under LED and HPS Lamps." Biosystems Engineering 194: 61–81. https://doi.org/10.1016/j.biosystemseng.2020.03.010
```

### Comparing `greenlightplus-1.6/GreenLightPlus/__init__.py` & `greenlightplus-1.7/GreenLightPlus/__init__.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/core/green_light_model.py` & `greenlightplus-1.7/GreenLightPlus/core/green_light_model.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/core/greenhouse_env.py` & `greenlightplus-1.7/GreenLightPlus/core/greenhouse_env.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/core/greenhouse_geometry.py` & `greenlightplus-1.7/GreenLightPlus/core/greenhouse_geometry.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/core/greenlight_energyplus_simulation.py` & `greenlightplus-1.7/GreenLightPlus/core/greenlight_energyplus_simulation.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/change_res.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/change_res.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/create_green_light_model.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/create_green_light_model.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/ode.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/ode.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_default_lamp_params.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_default_lamp_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_dep_params.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_dep_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_aux.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_aux.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_control.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_control.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_control_init.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_control_init.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_init.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_init.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_input.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_input.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_odes.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_odes.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_params.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_states.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_states.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_gl_time.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_gl_time.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py` & `greenlightplus-1.7/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/result_analysis/energy_analysis.py` & `greenlightplus-1.7/GreenLightPlus/result_analysis/energy_analysis.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/result_analysis/energy_yield_analysis.py` & `greenlightplus-1.7/GreenLightPlus/result_analysis/energy_yield_analysis.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/result_analysis/plot_green_light.py` & `greenlightplus-1.7/GreenLightPlus/result_analysis/plot_green_light.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/co2_dens2ppm.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/co2_dens2ppm.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/co2_ppm2dens.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/co2_ppm2dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/convert_epw2csv.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/convert_epw2csv.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/cut_energy_plus_data.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/cut_energy_plus_data.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/funcs.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/funcs.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/make_artificial_input.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/make_artificial_input.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/rh2vapor_dens.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/rh2vapor_dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/vapor_dens2pres.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/vapor_dens2pres.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus/service_functions/vp2dens.py` & `greenlightplus-1.7/GreenLightPlus/service_functions/vp2dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/GreenLightPlus.egg-info/PKG-INFO` & `greenlightplus-1.7/GreenLightPlus.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GreenLightPlus
-Version: 1.6
+Version: 1.7
 Summary: Greenhouse Simulation and Optimization Toolkit
 Author-email: Daidai Qiu <qiu.daidai@outlook.com>
 Project-URL: Homepage, https://github.com/greenpeer/GreenLightPlus
 Project-URL: Bug Reports, https://github.com/greenpeer/GreenLightPlus/issues
 Project-URL: Source, https://github.com/greenpeer/GreenLightPlus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -31,22 +31,32 @@
 
 ## Languages
 - [English](README.md)
 - [中文](README_zh.md)
 
 # GreenLightPlus
 
-GreenLightPlus is a ToolKit for greenhouse environment simulation and energy consumption-yield analysis. It combines the original GreenLight model and the EnergyPlus simulation tool to investigate the energy consumption and output of different greenhouse structures.
+GreenLightPlus is a Python toolkit for greenhouse environment simulation and energy consumption and yield optimization, developed based on David Katzin's MATLAB version of the [GreenLight](https://github.com/davkat1/GreenLight) model. Compared to the original model, GreenLightPlus provides the following improvements and extensions:
 
-## Features
+- Ported the original model from MATLAB to Python, improving accessibility and extensibility.
+- Supports the generation of various greenhouse geometric structures for comparative analysis.
+- Integrates EnergyPlus simulation functionality for more accurate energy consumption calculations.
+- Includes a built-in reinforcement learning environment that can be used with AI algorithms to optimize greenhouse control strategies.
 
-- **Simulation and Analysis**: Provides comprehensive greenhouse environment simulation and energy consumption analysis.
-- **Diverse Greenhouse Structures**: Supports generating six different greenhouse geometries.
-- **Reinforcement Learning Environment**: Includes a customized reinforcement learning environment for greenhouse control tasks.
-- **Integrated Simulation**: Combines the GreenLight model with EnergyPlus simulations, offering in-depth energy consumption and yield research for different greenhouse configurations.
+GreenLightPlus aims to help users design and manage greenhouses more efficiently, achieving energy optimization and crop yield enhancement. By using this toolkit, users can explore different greenhouse design options, evaluate their energy performance, and employ advanced optimization algorithms to find the best control strategies, improving the economic and environmental benefits of the greenhouse.
+
+## Key Features
+
+- **Comprehensive Greenhouse Environment Simulation**: GreenLightPlus provides a complete greenhouse environment simulation, including the dynamic changes of key parameters such as temperature, humidity, light, and CO2 concentration, as well as the simulation of crop growth processes.
+
+- **Flexible Greenhouse Geometric Modeling**: The toolkit supports the generation of six common types of greenhouse geometric structures, including triangular, semi-circular, flat arch, Gothic arch, sawtooth, and sawtooth arch. Users can choose the appropriate structure for analysis based on their requirements.
+
+- **Reinforcement Learning Optimization Strategies**: GreenLightPlus includes a built-in reinforcement learning environment specifically designed for greenhouse control tasks. Users can utilize this environment to train AI models that automatically learn optimal greenhouse control strategies, improving energy utilization efficiency and crop yield.
+
+- **Energy Consumption Analysis and Yield Prediction**: Through integration with EnergyPlus, GreenLightPlus can perform detailed energy consumption analyses for different greenhouse configurations and predict crop yields based on environmental conditions and control strategies, providing important information for greenhouse design and operation.
 
 ## Core Modules
 
 - `green_light_model.py` - Implements the Python-based GreenLight model for greenhouse environment simulation.
 - `greenhouse_env.py` - Defines the greenhouse environment class for reinforcement learning.
 - `greenhouse_geometry.py` - Used to generate geometric models for different greenhouse structures.
 - `greenlight_energyplus_simulation.py` - Combines the GreenLight model and EnergyPlus for simulation and analysis.
@@ -59,15 +69,15 @@
 
 To ensure users can smoothly use the GreenLightPlus package in combination with EnergyPlus for simulations, we need to provide detailed guidance on downloading and installing EnergyPlus. Here are the steps for downloading and installing EnergyPlus, as well as obtaining the necessary weather files, which can be included in the README:
 
 ---
 
 ## Prerequisites: Installing EnergyPlus
 
-To run the EnergyPlus-combined simulations in the GreenLightPlus package, you need to have EnergyPlus installed on your system. The following steps will guide you through downloading and installing EnergyPlus on a Linux system.
+To run the EnergyPlus-combined simulations in the GreenLightPlus package, you need to have EnergyPlus installed on your system. 
 
 ### Download and Install
 
 1. **Download EnergyPlus**: Use the `wget` command to download the Linux version of EnergyPlus from the official GitHub repository.
 
    ```bash
    wget https://github.com/NREL/EnergyPlus/releases/download/v23.2.0/EnergyPlus-23.2.0-7636e6b3e9-Linux-Ubuntu22.04-x86_64.tar.gz
@@ -255,15 +265,27 @@
 
 #### Functionality Description
 
 This example code demonstrates how to use the GreenLightModel class to run greenhouse environment simulations. By looping through the growing season, the simulation steps through the environmental changes, and the `calculate_energy_consumption` function is used to evaluate energy consumption and yield. Finally, the `plot_green_light` function visualizes the results of the entire simulation process, showing the changes in various environmental parameters inside the greenhouse, such as temperature, humidity, CO2 concentration, and lighting and heating energy consumption over time.
 
 #### Result Display
 
-The `plot_green_light` function will generate a chart displaying the changes in environmental parameters inside and outside the greenhouse, such as temperature, humidity, CO2 concentration, as well as lighting and heating energy consumption. This will help users evaluate the effectiveness of the simulation and optimize the greenhouse design.
+The `plot_green_light` function generates a comprehensive figure displaying the changes in environmental parameters and crop growth dynamics within the simulated greenhouse. The figure includes the following subplots:
+
+1. Indoor and outdoor temperature in degrees Celsius (°C).
+2. Indoor and outdoor vapor pressure in Pascals (Pa).
+3. Indoor and outdoor relative humidity as a percentage (%).
+4. Indoor and outdoor CO2 concentration in both milligrams per cubic meter (mg m^{-3}) and parts per million (ppm).
+5. Outdoor global solar radiation, PAR (Photosynthetically Active Radiation) above the canopy from both sun and lamps, lamp electric input, and PAR above the canopy from sun and lamps separately, all in Watts per square meter (W m^{-2}).
+6. PPFD (Photosynthetic Photon Flux Density) from the sun and lamps in micromoles of PAR per square meter per second (μmol (PAR) m^{-2} s^{-1}).
+7. Net assimilation of CO2, net photosynthesis, growth respiration, and maintenance respiration in milligrams per square meter per second (mg m^{-2} s^{-1}).
+8. Fruit, stem, and leaf dry weight in milligrams of CH2O per square meter (mg (CH2O) m^{-2}), buffer content also in mg (CH2O) m^{-2}, and LAI (Leaf Area Index) in square meters per square meter (m^2 m^{-2}).
+9. Fruit dry weight in milligrams of CH2O per square meter (mg (CH2O) m^{-2}) and fruit harvest in milligrams of CH2O per square meter per second (mg (CH2O) m^{-2} s^{-1}).
+10. Various temperature states of the greenhouse components in degrees Celsius (°C).
+
 
 ![alt text](image-1.png)
 
 ### 3. Using GreenLightPlus to Run Combined GreenLight and EnergyPlus Simulations
 
 GreenLightPlus integrates the GreenLight model and EnergyPlus, providing higher accuracy greenhouse environment simulations and more detailed energy consumption analyses.
 
@@ -422,14 +444,18 @@
 
 This example code demonstrates how to use Ray RLlib and the PPO algorithm to train a reinforcement learning model for greenhouse environment optimization. By adjusting the environment parameters and training settings, you can explore different strategies to improve the greenhouse's energy efficiency and crop yield.
 
 #### Result Display
 
 Checkpoints will be saved periodically during the training process, and the current training results will be printed. These results help users evaluate the algorithm's performance and iteratively optimize the greenhouse management strategies.
 
+
 ## Contributing
 
 Contributions through Pull Requests or Issues for feature enhancements or bug reports are welcome.
 
 ## License
 
 This project is licensed under the GNU GPLv3 License. See the `LICENSE` file for details.
+
+## References
+David Katzin, Simon van Mourik, Frank Kempkes, and Eldert J. Van Henten. 2020. "GreenLight - An Open Source Model for Greenhouses with Supplemental Lighting: Evaluation of Heat Requirements under LED and HPS Lamps." Biosystems Engineering 194: 61–81. https://doi.org/10.1016/j.biosystemseng.2020.03.010
```

### Comparing `greenlightplus-1.6/GreenLightPlus.egg-info/SOURCES.txt` & `greenlightplus-1.7/GreenLightPlus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.6/PKG-INFO` & `greenlightplus-1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GreenLightPlus
-Version: 1.6
+Version: 1.7
 Summary: Greenhouse Simulation and Optimization Toolkit
 Author-email: Daidai Qiu <qiu.daidai@outlook.com>
 Project-URL: Homepage, https://github.com/greenpeer/GreenLightPlus
 Project-URL: Bug Reports, https://github.com/greenpeer/GreenLightPlus/issues
 Project-URL: Source, https://github.com/greenpeer/GreenLightPlus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -31,22 +31,32 @@
 
 ## Languages
 - [English](README.md)
 - [中文](README_zh.md)
 
 # GreenLightPlus
 
-GreenLightPlus is a ToolKit for greenhouse environment simulation and energy consumption-yield analysis. It combines the original GreenLight model and the EnergyPlus simulation tool to investigate the energy consumption and output of different greenhouse structures.
+GreenLightPlus is a Python toolkit for greenhouse environment simulation and energy consumption and yield optimization, developed based on David Katzin's MATLAB version of the [GreenLight](https://github.com/davkat1/GreenLight) model. Compared to the original model, GreenLightPlus provides the following improvements and extensions:
 
-## Features
+- Ported the original model from MATLAB to Python, improving accessibility and extensibility.
+- Supports the generation of various greenhouse geometric structures for comparative analysis.
+- Integrates EnergyPlus simulation functionality for more accurate energy consumption calculations.
+- Includes a built-in reinforcement learning environment that can be used with AI algorithms to optimize greenhouse control strategies.
 
-- **Simulation and Analysis**: Provides comprehensive greenhouse environment simulation and energy consumption analysis.
-- **Diverse Greenhouse Structures**: Supports generating six different greenhouse geometries.
-- **Reinforcement Learning Environment**: Includes a customized reinforcement learning environment for greenhouse control tasks.
-- **Integrated Simulation**: Combines the GreenLight model with EnergyPlus simulations, offering in-depth energy consumption and yield research for different greenhouse configurations.
+GreenLightPlus aims to help users design and manage greenhouses more efficiently, achieving energy optimization and crop yield enhancement. By using this toolkit, users can explore different greenhouse design options, evaluate their energy performance, and employ advanced optimization algorithms to find the best control strategies, improving the economic and environmental benefits of the greenhouse.
+
+## Key Features
+
+- **Comprehensive Greenhouse Environment Simulation**: GreenLightPlus provides a complete greenhouse environment simulation, including the dynamic changes of key parameters such as temperature, humidity, light, and CO2 concentration, as well as the simulation of crop growth processes.
+
+- **Flexible Greenhouse Geometric Modeling**: The toolkit supports the generation of six common types of greenhouse geometric structures, including triangular, semi-circular, flat arch, Gothic arch, sawtooth, and sawtooth arch. Users can choose the appropriate structure for analysis based on their requirements.
+
+- **Reinforcement Learning Optimization Strategies**: GreenLightPlus includes a built-in reinforcement learning environment specifically designed for greenhouse control tasks. Users can utilize this environment to train AI models that automatically learn optimal greenhouse control strategies, improving energy utilization efficiency and crop yield.
+
+- **Energy Consumption Analysis and Yield Prediction**: Through integration with EnergyPlus, GreenLightPlus can perform detailed energy consumption analyses for different greenhouse configurations and predict crop yields based on environmental conditions and control strategies, providing important information for greenhouse design and operation.
 
 ## Core Modules
 
 - `green_light_model.py` - Implements the Python-based GreenLight model for greenhouse environment simulation.
 - `greenhouse_env.py` - Defines the greenhouse environment class for reinforcement learning.
 - `greenhouse_geometry.py` - Used to generate geometric models for different greenhouse structures.
 - `greenlight_energyplus_simulation.py` - Combines the GreenLight model and EnergyPlus for simulation and analysis.
@@ -59,15 +69,15 @@
 
 To ensure users can smoothly use the GreenLightPlus package in combination with EnergyPlus for simulations, we need to provide detailed guidance on downloading and installing EnergyPlus. Here are the steps for downloading and installing EnergyPlus, as well as obtaining the necessary weather files, which can be included in the README:
 
 ---
 
 ## Prerequisites: Installing EnergyPlus
 
-To run the EnergyPlus-combined simulations in the GreenLightPlus package, you need to have EnergyPlus installed on your system. The following steps will guide you through downloading and installing EnergyPlus on a Linux system.
+To run the EnergyPlus-combined simulations in the GreenLightPlus package, you need to have EnergyPlus installed on your system. 
 
 ### Download and Install
 
 1. **Download EnergyPlus**: Use the `wget` command to download the Linux version of EnergyPlus from the official GitHub repository.
 
    ```bash
    wget https://github.com/NREL/EnergyPlus/releases/download/v23.2.0/EnergyPlus-23.2.0-7636e6b3e9-Linux-Ubuntu22.04-x86_64.tar.gz
@@ -255,15 +265,27 @@
 
 #### Functionality Description
 
 This example code demonstrates how to use the GreenLightModel class to run greenhouse environment simulations. By looping through the growing season, the simulation steps through the environmental changes, and the `calculate_energy_consumption` function is used to evaluate energy consumption and yield. Finally, the `plot_green_light` function visualizes the results of the entire simulation process, showing the changes in various environmental parameters inside the greenhouse, such as temperature, humidity, CO2 concentration, and lighting and heating energy consumption over time.
 
 #### Result Display
 
-The `plot_green_light` function will generate a chart displaying the changes in environmental parameters inside and outside the greenhouse, such as temperature, humidity, CO2 concentration, as well as lighting and heating energy consumption. This will help users evaluate the effectiveness of the simulation and optimize the greenhouse design.
+The `plot_green_light` function generates a comprehensive figure displaying the changes in environmental parameters and crop growth dynamics within the simulated greenhouse. The figure includes the following subplots:
+
+1. Indoor and outdoor temperature in degrees Celsius (°C).
+2. Indoor and outdoor vapor pressure in Pascals (Pa).
+3. Indoor and outdoor relative humidity as a percentage (%).
+4. Indoor and outdoor CO2 concentration in both milligrams per cubic meter (mg m^{-3}) and parts per million (ppm).
+5. Outdoor global solar radiation, PAR (Photosynthetically Active Radiation) above the canopy from both sun and lamps, lamp electric input, and PAR above the canopy from sun and lamps separately, all in Watts per square meter (W m^{-2}).
+6. PPFD (Photosynthetic Photon Flux Density) from the sun and lamps in micromoles of PAR per square meter per second (μmol (PAR) m^{-2} s^{-1}).
+7. Net assimilation of CO2, net photosynthesis, growth respiration, and maintenance respiration in milligrams per square meter per second (mg m^{-2} s^{-1}).
+8. Fruit, stem, and leaf dry weight in milligrams of CH2O per square meter (mg (CH2O) m^{-2}), buffer content also in mg (CH2O) m^{-2}, and LAI (Leaf Area Index) in square meters per square meter (m^2 m^{-2}).
+9. Fruit dry weight in milligrams of CH2O per square meter (mg (CH2O) m^{-2}) and fruit harvest in milligrams of CH2O per square meter per second (mg (CH2O) m^{-2} s^{-1}).
+10. Various temperature states of the greenhouse components in degrees Celsius (°C).
+
 
 ![alt text](image-1.png)
 
 ### 3. Using GreenLightPlus to Run Combined GreenLight and EnergyPlus Simulations
 
 GreenLightPlus integrates the GreenLight model and EnergyPlus, providing higher accuracy greenhouse environment simulations and more detailed energy consumption analyses.
 
@@ -422,14 +444,18 @@
 
 This example code demonstrates how to use Ray RLlib and the PPO algorithm to train a reinforcement learning model for greenhouse environment optimization. By adjusting the environment parameters and training settings, you can explore different strategies to improve the greenhouse's energy efficiency and crop yield.
 
 #### Result Display
 
 Checkpoints will be saved periodically during the training process, and the current training results will be printed. These results help users evaluate the algorithm's performance and iteratively optimize the greenhouse management strategies.
 
+
 ## Contributing
 
 Contributions through Pull Requests or Issues for feature enhancements or bug reports are welcome.
 
 ## License
 
 This project is licensed under the GNU GPLv3 License. See the `LICENSE` file for details.
+
+## References
+David Katzin, Simon van Mourik, Frank Kempkes, and Eldert J. Van Henten. 2020. "GreenLight - An Open Source Model for Greenhouses with Supplemental Lighting: Evaluation of Heat Requirements under LED and HPS Lamps." Biosystems Engineering 194: 61–81. https://doi.org/10.1016/j.biosystemseng.2020.03.010
```

### Comparing `greenlightplus-1.6/pyproject.toml` & `greenlightplus-1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GreenLightPlus"
-version = "1.6"
+version = "1.7"
 authors = [
     {name = "Daidai Qiu", email = "qiu.daidai@outlook.com"}
 ]
 description = "Greenhouse Simulation and Optimization Toolkit"
 readme = "GreenLightPlus/README.md"
 requires-python = ">=3.8"
 classifiers = [
```

