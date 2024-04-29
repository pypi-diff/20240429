# Comparing `tmp/greenlightplus-1.0.tar.gz` & `tmp/greenlightplus-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenlightplus-1.0.tar", last modified: Mon Apr 29 09:13:32 2024, max compression
+gzip compressed data, was "greenlightplus-1.1.tar", last modified: Mon Apr 29 09:26:21 2024, max compression
```

## Comparing `greenlightplus-1.0.tar` & `greenlightplus-1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:13:32.728000 greenlightplus-1.0/
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:13:32.715700 greenlightplus-1.0/GreenLightPlus/
--rw-r--r--   0 daidai     (501) staff       (20)     9221 2024-04-09 19:53:32.000000 greenlightplus-1.0/GreenLightPlus/README.md
--rw-r--r--   0 daidai     (501) staff       (20)      689 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/__init__.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:13:32.718898 greenlightplus-1.0/GreenLightPlus/core/
--rw-r--r--   0 daidai     (501) staff       (20)    10378 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/core/green_light_model.py
--rw-r--r--   0 daidai     (501) staff       (20)    14630 2024-04-09 21:32:30.000000 greenlightplus-1.0/GreenLightPlus/core/greenhouse_env.py
--rw-r--r--   0 daidai     (501) staff       (20)    61665 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/core/greenhouse_geometry.py
--rw-r--r--   0 daidai     (501) staff       (20)    10185 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/core/greenlight_energyplus_simulation.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:13:32.724002 greenlightplus-1.0/GreenLightPlus/create_green_light_model/
--rw-r--r--   0 daidai     (501) staff       (20)     5614 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/change_res.py
--rw-r--r--   0 daidai     (501) staff       (20)     2713 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/create_green_light_model.py
--rw-r--r--   0 daidai     (501) staff       (20)     5257 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/ode.py
--rw-r--r--   0 daidai     (501) staff       (20)     3637 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_default_lamp_params.py
--rw-r--r--   0 daidai     (501) staff       (20)     3151 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_dep_params.py
--rw-r--r--   0 daidai     (501) staff       (20)    74154 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_aux.py
--rw-r--r--   0 daidai     (501) staff       (20)     2543 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_control.py
--rw-r--r--   0 daidai     (501) staff       (20)     3639 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_control_init.py
--rw-r--r--   0 daidai     (501) staff       (20)     4083 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_init.py
--rw-r--r--   0 daidai     (501) staff       (20)     5291 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_input.py
--rw-r--r--   0 daidai     (501) staff       (20)    11637 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_odes.py
--rw-r--r--   0 daidai     (501) staff       (20)    19680 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_params.py
--rw-r--r--   0 daidai     (501) staff       (20)     1895 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_states.py
--rw-r--r--   0 daidai     (501) staff       (20)     1307 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_time.py
--rw-r--r--   0 daidai     (501) staff       (20)     3001 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:13:32.724592 greenlightplus-1.0/GreenLightPlus/result_analysis/
--rw-r--r--   0 daidai     (501) staff       (20)     3167 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/result_analysis/energy_analysis.py
--rw-r--r--   0 daidai     (501) staff       (20)     3312 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/result_analysis/energy_yield_analysis.py
--rw-r--r--   0 daidai     (501) staff       (20)     7263 2024-04-16 09:09:37.000000 greenlightplus-1.0/GreenLightPlus/result_analysis/plot_green_light.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:13:32.726750 greenlightplus-1.0/GreenLightPlus/service_functions/
--rw-r--r--   0 daidai     (501) staff       (20)      798 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/co2_dens2ppm.py
--rw-r--r--   0 daidai     (501) staff       (20)      794 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/co2_ppm2dens.py
--rw-r--r--   0 daidai     (501) staff       (20)    15456 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/convert_epw2csv.py
--rw-r--r--   0 daidai     (501) staff       (20)    11525 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/cut_energy_plus_data.py
--rw-r--r--   0 daidai     (501) staff       (20)     9761 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/funcs.py
--rw-r--r--   0 daidai     (501) staff       (20)     3543 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/make_artificial_input.py
--rw-r--r--   0 daidai     (501) staff       (20)     1677 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/rh2vapor_dens.py
--rw-r--r--   0 daidai     (501) staff       (20)     1401 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/vapor_dens2pres.py
--rw-r--r--   0 daidai     (501) staff       (20)     1379 2024-04-09 19:17:21.000000 greenlightplus-1.0/GreenLightPlus/service_functions/vp2dens.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:13:32.727195 greenlightplus-1.0/GreenLightPlus.egg-info/
--rw-r--r--   0 daidai     (501) staff       (20)    10404 2024-04-29 09:13:32.000000 greenlightplus-1.0/GreenLightPlus.egg-info/PKG-INFO
--rw-r--r--   0 daidai     (501) staff       (20)     1981 2024-04-29 09:13:32.000000 greenlightplus-1.0/GreenLightPlus.egg-info/SOURCES.txt
--rw-r--r--   0 daidai     (501) staff       (20)        1 2024-04-29 09:13:32.000000 greenlightplus-1.0/GreenLightPlus.egg-info/dependency_links.txt
--rw-r--r--   0 daidai     (501) staff       (20)       59 2024-04-29 09:13:32.000000 greenlightplus-1.0/GreenLightPlus.egg-info/entry_points.txt
--rw-r--r--   0 daidai     (501) staff       (20)      102 2024-04-29 09:13:32.000000 greenlightplus-1.0/GreenLightPlus.egg-info/requires.txt
--rw-r--r--   0 daidai     (501) staff       (20)       15 2024-04-29 09:13:32.000000 greenlightplus-1.0/GreenLightPlus.egg-info/top_level.txt
--rw-r--r--   0 daidai     (501) staff       (20)    10404 2024-04-29 09:13:32.727809 greenlightplus-1.0/PKG-INFO
--rw-r--r--   0 daidai     (501) staff       (20)     1336 2024-04-29 09:13:17.000000 greenlightplus-1.0/pyproject.toml
--rw-r--r--   0 daidai     (501) staff       (20)       38 2024-04-29 09:13:32.728259 greenlightplus-1.0/setup.cfg
--rw-r--r--   0 daidai     (501) staff       (20)       85 2024-04-29 08:39:56.000000 greenlightplus-1.0/setup.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:26:21.247351 greenlightplus-1.1/
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:26:21.235789 greenlightplus-1.1/GreenLightPlus/
+-rw-r--r--   0 daidai     (501) staff       (20)     9221 2024-04-09 19:53:32.000000 greenlightplus-1.1/GreenLightPlus/README.md
+-rw-r--r--   0 daidai     (501) staff       (20)      689 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/__init__.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:26:21.238834 greenlightplus-1.1/GreenLightPlus/core/
+-rw-r--r--   0 daidai     (501) staff       (20)    10378 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/core/green_light_model.py
+-rw-r--r--   0 daidai     (501) staff       (20)    14630 2024-04-09 21:32:30.000000 greenlightplus-1.1/GreenLightPlus/core/greenhouse_env.py
+-rw-r--r--   0 daidai     (501) staff       (20)    61665 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/core/greenhouse_geometry.py
+-rw-r--r--   0 daidai     (501) staff       (20)    10165 2024-04-29 09:25:39.000000 greenlightplus-1.1/GreenLightPlus/core/greenlight_energyplus_simulation.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:26:21.243828 greenlightplus-1.1/GreenLightPlus/create_green_light_model/
+-rw-r--r--   0 daidai     (501) staff       (20)     5614 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/change_res.py
+-rw-r--r--   0 daidai     (501) staff       (20)     2713 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/create_green_light_model.py
+-rw-r--r--   0 daidai     (501) staff       (20)     5257 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/ode.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3637 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_default_lamp_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3151 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_dep_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)    74154 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_aux.py
+-rw-r--r--   0 daidai     (501) staff       (20)     2543 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_control.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3639 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_control_init.py
+-rw-r--r--   0 daidai     (501) staff       (20)     4083 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_init.py
+-rw-r--r--   0 daidai     (501) staff       (20)     5291 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_input.py
+-rw-r--r--   0 daidai     (501) staff       (20)    11637 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_odes.py
+-rw-r--r--   0 daidai     (501) staff       (20)    19680 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1895 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_states.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1307 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_time.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3001 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:26:21.244305 greenlightplus-1.1/GreenLightPlus/result_analysis/
+-rw-r--r--   0 daidai     (501) staff       (20)     3167 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/result_analysis/energy_analysis.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3312 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/result_analysis/energy_yield_analysis.py
+-rw-r--r--   0 daidai     (501) staff       (20)     7263 2024-04-16 09:09:37.000000 greenlightplus-1.1/GreenLightPlus/result_analysis/plot_green_light.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:26:21.246410 greenlightplus-1.1/GreenLightPlus/service_functions/
+-rw-r--r--   0 daidai     (501) staff       (20)      798 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/co2_dens2ppm.py
+-rw-r--r--   0 daidai     (501) staff       (20)      794 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/co2_ppm2dens.py
+-rw-r--r--   0 daidai     (501) staff       (20)    15456 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/convert_epw2csv.py
+-rw-r--r--   0 daidai     (501) staff       (20)    11525 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/cut_energy_plus_data.py
+-rw-r--r--   0 daidai     (501) staff       (20)     9761 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/funcs.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3543 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/make_artificial_input.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1677 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/rh2vapor_dens.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1401 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/vapor_dens2pres.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1379 2024-04-09 19:17:21.000000 greenlightplus-1.1/GreenLightPlus/service_functions/vp2dens.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:26:21.246732 greenlightplus-1.1/GreenLightPlus.egg-info/
+-rw-r--r--   0 daidai     (501) staff       (20)    10404 2024-04-29 09:26:21.000000 greenlightplus-1.1/GreenLightPlus.egg-info/PKG-INFO
+-rw-r--r--   0 daidai     (501) staff       (20)     1981 2024-04-29 09:26:21.000000 greenlightplus-1.1/GreenLightPlus.egg-info/SOURCES.txt
+-rw-r--r--   0 daidai     (501) staff       (20)        1 2024-04-29 09:26:21.000000 greenlightplus-1.1/GreenLightPlus.egg-info/dependency_links.txt
+-rw-r--r--   0 daidai     (501) staff       (20)       59 2024-04-29 09:26:21.000000 greenlightplus-1.1/GreenLightPlus.egg-info/entry_points.txt
+-rw-r--r--   0 daidai     (501) staff       (20)      102 2024-04-29 09:26:21.000000 greenlightplus-1.1/GreenLightPlus.egg-info/requires.txt
+-rw-r--r--   0 daidai     (501) staff       (20)       15 2024-04-29 09:26:21.000000 greenlightplus-1.1/GreenLightPlus.egg-info/top_level.txt
+-rw-r--r--   0 daidai     (501) staff       (20)    10404 2024-04-29 09:26:21.247212 greenlightplus-1.1/PKG-INFO
+-rw-r--r--   0 daidai     (501) staff       (20)     1336 2024-04-29 09:23:48.000000 greenlightplus-1.1/pyproject.toml
+-rw-r--r--   0 daidai     (501) staff       (20)       38 2024-04-29 09:26:21.247591 greenlightplus-1.1/setup.cfg
+-rw-r--r--   0 daidai     (501) staff       (20)       85 2024-04-29 08:39:56.000000 greenlightplus-1.1/setup.py
```

### Comparing `greenlightplus-1.0/GreenLightPlus/README.md` & `greenlightplus-1.1/GreenLightPlus/README.md`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/__init__.py` & `greenlightplus-1.1/GreenLightPlus/__init__.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/core/green_light_model.py` & `greenlightplus-1.1/GreenLightPlus/core/green_light_model.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/core/greenhouse_env.py` & `greenlightplus-1.1/GreenLightPlus/core/greenhouse_env.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/core/greenhouse_geometry.py` & `greenlightplus-1.1/GreenLightPlus/core/greenhouse_geometry.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/core/greenlight_energyplus_simulation.py` & `greenlightplus-1.1/GreenLightPlus/core/greenlight_energyplus_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 # 将EnergyPlus安装目录添加到Python模块搜索路径
-sys.path.insert(0, "/Applications/EnergyPlus-23-2-0")
+sys.path.insert(0, "/EnergyPlus")
 from pyenergyplus.plugin import EnergyPlusPlugin
 from pyenergyplus.api import EnergyPlusAPI
 from ..service_functions.funcs import calculate_energy_consumption, extract_last_value_from_nested_dict
 from .green_light_model import GreenLightModel
 
 
 class GreenhouseSimulation(EnergyPlusPlugin):
```

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/change_res.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/change_res.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/create_green_light_model.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/create_green_light_model.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/ode.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/ode.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_default_lamp_params.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_default_lamp_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_dep_params.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_dep_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_aux.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_aux.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_control.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_control.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_control_init.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_control_init.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_init.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_init.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_input.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_input.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_odes.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_odes.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_params.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_states.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_states.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_gl_time.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_gl_time.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py` & `greenlightplus-1.1/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/result_analysis/energy_analysis.py` & `greenlightplus-1.1/GreenLightPlus/result_analysis/energy_analysis.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/result_analysis/energy_yield_analysis.py` & `greenlightplus-1.1/GreenLightPlus/result_analysis/energy_yield_analysis.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/result_analysis/plot_green_light.py` & `greenlightplus-1.1/GreenLightPlus/result_analysis/plot_green_light.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/co2_dens2ppm.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/co2_dens2ppm.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/co2_ppm2dens.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/co2_ppm2dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/convert_epw2csv.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/convert_epw2csv.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/cut_energy_plus_data.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/cut_energy_plus_data.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/funcs.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/funcs.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/make_artificial_input.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/make_artificial_input.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/rh2vapor_dens.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/rh2vapor_dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/vapor_dens2pres.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/vapor_dens2pres.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus/service_functions/vp2dens.py` & `greenlightplus-1.1/GreenLightPlus/service_functions/vp2dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/GreenLightPlus.egg-info/PKG-INFO` & `greenlightplus-1.1/GreenLightPlus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GreenLightPlus
-Version: 1.0
+Version: 1.1
 Summary: Greenhouse Simulation and Optimization Toolkit
 Author-email: Daidai Qiu <qiu.daidai@outlook.com>
 Project-URL: Homepage, https://github.com/greenpeer/GreenLightPlus
 Project-URL: Bug Reports, https://github.com/greenpeer/GreenLightPlus/issues
 Project-URL: Source, https://github.com/greenpeer/GreenLightPlus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `greenlightplus-1.0/GreenLightPlus.egg-info/SOURCES.txt` & `greenlightplus-1.1/GreenLightPlus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.0/PKG-INFO` & `greenlightplus-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GreenLightPlus
-Version: 1.0
+Version: 1.1
 Summary: Greenhouse Simulation and Optimization Toolkit
 Author-email: Daidai Qiu <qiu.daidai@outlook.com>
 Project-URL: Homepage, https://github.com/greenpeer/GreenLightPlus
 Project-URL: Bug Reports, https://github.com/greenpeer/GreenLightPlus/issues
 Project-URL: Source, https://github.com/greenpeer/GreenLightPlus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `greenlightplus-1.0/pyproject.toml` & `greenlightplus-1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GreenLightPlus"
-version = "1.0"
+version = "1.1"
 authors = [
     {name = "Daidai Qiu", email = "qiu.daidai@outlook.com"}
 ]
 description = "Greenhouse Simulation and Optimization Toolkit"
 readme = "GreenLightPlus/README.md"
 requires-python = ">=3.8"
 classifiers = [
```
