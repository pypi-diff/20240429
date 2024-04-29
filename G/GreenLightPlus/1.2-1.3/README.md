# Comparing `tmp/greenlightplus-1.2.tar.gz` & `tmp/greenlightplus-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenlightplus-1.2.tar", last modified: Mon Apr 29 09:45:02 2024, max compression
+gzip compressed data, was "greenlightplus-1.3.tar", last modified: Mon Apr 29 11:54:26 2024, max compression
```

## Comparing `greenlightplus-1.2.tar` & `greenlightplus-1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:45:02.176974 greenlightplus-1.2/
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:45:02.161671 greenlightplus-1.2/GreenLightPlus/
--rw-r--r--   0 daidai     (501) staff       (20)     9221 2024-04-09 19:53:32.000000 greenlightplus-1.2/GreenLightPlus/README.md
--rw-r--r--   0 daidai     (501) staff       (20)      689 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/__init__.py
--rw-r--r--   0 daidai     (501) staff       (20)        0 2024-04-29 09:33:33.000000 greenlightplus-1.2/GreenLightPlus/config.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:45:02.163988 greenlightplus-1.2/GreenLightPlus/core/
--rw-r--r--   0 daidai     (501) staff       (20)    10378 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/core/green_light_model.py
--rw-r--r--   0 daidai     (501) staff       (20)    14630 2024-04-09 21:32:30.000000 greenlightplus-1.2/GreenLightPlus/core/greenhouse_env.py
--rw-r--r--   0 daidai     (501) staff       (20)    61665 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/core/greenhouse_geometry.py
--rw-r--r--   0 daidai     (501) staff       (20)    10309 2024-04-29 09:44:25.000000 greenlightplus-1.2/GreenLightPlus/core/greenlight_energyplus_simulation.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:45:02.169093 greenlightplus-1.2/GreenLightPlus/create_green_light_model/
--rw-r--r--   0 daidai     (501) staff       (20)     5614 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/change_res.py
--rw-r--r--   0 daidai     (501) staff       (20)     2713 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/create_green_light_model.py
--rw-r--r--   0 daidai     (501) staff       (20)     5257 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/ode.py
--rw-r--r--   0 daidai     (501) staff       (20)     3637 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_default_lamp_params.py
--rw-r--r--   0 daidai     (501) staff       (20)     3151 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_dep_params.py
--rw-r--r--   0 daidai     (501) staff       (20)    74154 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_aux.py
--rw-r--r--   0 daidai     (501) staff       (20)     2543 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_control.py
--rw-r--r--   0 daidai     (501) staff       (20)     3639 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_control_init.py
--rw-r--r--   0 daidai     (501) staff       (20)     4083 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_init.py
--rw-r--r--   0 daidai     (501) staff       (20)     5291 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_input.py
--rw-r--r--   0 daidai     (501) staff       (20)    11637 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_odes.py
--rw-r--r--   0 daidai     (501) staff       (20)    19680 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_params.py
--rw-r--r--   0 daidai     (501) staff       (20)     1895 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_states.py
--rw-r--r--   0 daidai     (501) staff       (20)     1307 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_time.py
--rw-r--r--   0 daidai     (501) staff       (20)     3001 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:45:02.169640 greenlightplus-1.2/GreenLightPlus/result_analysis/
--rw-r--r--   0 daidai     (501) staff       (20)     3167 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/result_analysis/energy_analysis.py
--rw-r--r--   0 daidai     (501) staff       (20)     3312 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/result_analysis/energy_yield_analysis.py
--rw-r--r--   0 daidai     (501) staff       (20)     7263 2024-04-16 09:09:37.000000 greenlightplus-1.2/GreenLightPlus/result_analysis/plot_green_light.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:45:02.176105 greenlightplus-1.2/GreenLightPlus/service_functions/
--rw-r--r--   0 daidai     (501) staff       (20)      798 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/co2_dens2ppm.py
--rw-r--r--   0 daidai     (501) staff       (20)      794 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/co2_ppm2dens.py
--rw-r--r--   0 daidai     (501) staff       (20)    15456 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/convert_epw2csv.py
--rw-r--r--   0 daidai     (501) staff       (20)    11525 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/cut_energy_plus_data.py
--rw-r--r--   0 daidai     (501) staff       (20)     9761 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/funcs.py
--rw-r--r--   0 daidai     (501) staff       (20)     3543 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/make_artificial_input.py
--rw-r--r--   0 daidai     (501) staff       (20)     1677 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/rh2vapor_dens.py
--rw-r--r--   0 daidai     (501) staff       (20)     1401 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/vapor_dens2pres.py
--rw-r--r--   0 daidai     (501) staff       (20)     1379 2024-04-09 19:17:21.000000 greenlightplus-1.2/GreenLightPlus/service_functions/vp2dens.py
-drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 09:45:02.176430 greenlightplus-1.2/GreenLightPlus.egg-info/
--rw-r--r--   0 daidai     (501) staff       (20)    10404 2024-04-29 09:45:02.000000 greenlightplus-1.2/GreenLightPlus.egg-info/PKG-INFO
--rw-r--r--   0 daidai     (501) staff       (20)     2006 2024-04-29 09:45:02.000000 greenlightplus-1.2/GreenLightPlus.egg-info/SOURCES.txt
--rw-r--r--   0 daidai     (501) staff       (20)        1 2024-04-29 09:45:02.000000 greenlightplus-1.2/GreenLightPlus.egg-info/dependency_links.txt
--rw-r--r--   0 daidai     (501) staff       (20)       59 2024-04-29 09:45:02.000000 greenlightplus-1.2/GreenLightPlus.egg-info/entry_points.txt
--rw-r--r--   0 daidai     (501) staff       (20)      102 2024-04-29 09:45:02.000000 greenlightplus-1.2/GreenLightPlus.egg-info/requires.txt
--rw-r--r--   0 daidai     (501) staff       (20)       15 2024-04-29 09:45:02.000000 greenlightplus-1.2/GreenLightPlus.egg-info/top_level.txt
--rw-r--r--   0 daidai     (501) staff       (20)    10404 2024-04-29 09:45:02.176859 greenlightplus-1.2/PKG-INFO
--rw-r--r--   0 daidai     (501) staff       (20)     1336 2024-04-29 09:44:52.000000 greenlightplus-1.2/pyproject.toml
--rw-r--r--   0 daidai     (501) staff       (20)       38 2024-04-29 09:45:02.177201 greenlightplus-1.2/setup.cfg
--rw-r--r--   0 daidai     (501) staff       (20)       85 2024-04-29 08:39:56.000000 greenlightplus-1.2/setup.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 11:54:26.848362 greenlightplus-1.3/
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 11:54:26.836826 greenlightplus-1.3/GreenLightPlus/
+-rw-r--r--   0 daidai     (501) staff       (20)     9221 2024-04-09 19:53:32.000000 greenlightplus-1.3/GreenLightPlus/README.md
+-rw-r--r--   0 daidai     (501) staff       (20)      689 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/__init__.py
+-rw-r--r--   0 daidai     (501) staff       (20)        0 2024-04-29 09:33:33.000000 greenlightplus-1.3/GreenLightPlus/config.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 11:54:26.839363 greenlightplus-1.3/GreenLightPlus/core/
+-rw-r--r--   0 daidai     (501) staff       (20)    10378 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/core/green_light_model.py
+-rw-r--r--   0 daidai     (501) staff       (20)    14630 2024-04-09 21:32:30.000000 greenlightplus-1.3/GreenLightPlus/core/greenhouse_env.py
+-rw-r--r--   0 daidai     (501) staff       (20)    61665 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/core/greenhouse_geometry.py
+-rw-r--r--   0 daidai     (501) staff       (20)     9969 2024-04-29 10:54:39.000000 greenlightplus-1.3/GreenLightPlus/core/greenlight_energyplus_simulation.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 11:54:26.843189 greenlightplus-1.3/GreenLightPlus/create_green_light_model/
+-rw-r--r--   0 daidai     (501) staff       (20)     5614 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/change_res.py
+-rw-r--r--   0 daidai     (501) staff       (20)     2713 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/create_green_light_model.py
+-rw-r--r--   0 daidai     (501) staff       (20)     5257 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/ode.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3637 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_default_lamp_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3151 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_dep_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)    74154 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_aux.py
+-rw-r--r--   0 daidai     (501) staff       (20)     2543 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_control.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3639 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_control_init.py
+-rw-r--r--   0 daidai     (501) staff       (20)     4083 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_init.py
+-rw-r--r--   0 daidai     (501) staff       (20)     5291 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_input.py
+-rw-r--r--   0 daidai     (501) staff       (20)    11637 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_odes.py
+-rw-r--r--   0 daidai     (501) staff       (20)    19680 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_params.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1895 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_states.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1307 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_time.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3001 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 11:54:26.843618 greenlightplus-1.3/GreenLightPlus/result_analysis/
+-rw-r--r--   0 daidai     (501) staff       (20)     3167 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/result_analysis/energy_analysis.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3312 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/result_analysis/energy_yield_analysis.py
+-rw-r--r--   0 daidai     (501) staff       (20)     7263 2024-04-16 09:09:37.000000 greenlightplus-1.3/GreenLightPlus/result_analysis/plot_green_light.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 11:54:26.846971 greenlightplus-1.3/GreenLightPlus/service_functions/
+-rw-r--r--   0 daidai     (501) staff       (20)      798 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/co2_dens2ppm.py
+-rw-r--r--   0 daidai     (501) staff       (20)      794 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/co2_ppm2dens.py
+-rw-r--r--   0 daidai     (501) staff       (20)    15456 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/convert_epw2csv.py
+-rw-r--r--   0 daidai     (501) staff       (20)    11525 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/cut_energy_plus_data.py
+-rw-r--r--   0 daidai     (501) staff       (20)     9761 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/funcs.py
+-rw-r--r--   0 daidai     (501) staff       (20)     3543 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/make_artificial_input.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1677 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/rh2vapor_dens.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1401 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/vapor_dens2pres.py
+-rw-r--r--   0 daidai     (501) staff       (20)     1379 2024-04-09 19:17:21.000000 greenlightplus-1.3/GreenLightPlus/service_functions/vp2dens.py
+drwxr-xr-x   0 daidai     (501) staff       (20)        0 2024-04-29 11:54:26.847526 greenlightplus-1.3/GreenLightPlus.egg-info/
+-rw-r--r--   0 daidai     (501) staff       (20)    10404 2024-04-29 11:54:26.000000 greenlightplus-1.3/GreenLightPlus.egg-info/PKG-INFO
+-rw-r--r--   0 daidai     (501) staff       (20)     2006 2024-04-29 11:54:26.000000 greenlightplus-1.3/GreenLightPlus.egg-info/SOURCES.txt
+-rw-r--r--   0 daidai     (501) staff       (20)        1 2024-04-29 11:54:26.000000 greenlightplus-1.3/GreenLightPlus.egg-info/dependency_links.txt
+-rw-r--r--   0 daidai     (501) staff       (20)       59 2024-04-29 11:54:26.000000 greenlightplus-1.3/GreenLightPlus.egg-info/entry_points.txt
+-rw-r--r--   0 daidai     (501) staff       (20)      102 2024-04-29 11:54:26.000000 greenlightplus-1.3/GreenLightPlus.egg-info/requires.txt
+-rw-r--r--   0 daidai     (501) staff       (20)       15 2024-04-29 11:54:26.000000 greenlightplus-1.3/GreenLightPlus.egg-info/top_level.txt
+-rw-r--r--   0 daidai     (501) staff       (20)    10404 2024-04-29 11:54:26.848165 greenlightplus-1.3/PKG-INFO
+-rw-r--r--   0 daidai     (501) staff       (20)     1336 2024-04-29 11:53:55.000000 greenlightplus-1.3/pyproject.toml
+-rw-r--r--   0 daidai     (501) staff       (20)       38 2024-04-29 11:54:26.848668 greenlightplus-1.3/setup.cfg
+-rw-r--r--   0 daidai     (501) staff       (20)       85 2024-04-29 08:39:56.000000 greenlightplus-1.3/setup.py
```

### Comparing `greenlightplus-1.2/GreenLightPlus/README.md` & `greenlightplus-1.3/GreenLightPlus/README.md`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/__init__.py` & `greenlightplus-1.3/GreenLightPlus/__init__.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/core/green_light_model.py` & `greenlightplus-1.3/GreenLightPlus/core/green_light_model.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/core/greenhouse_env.py` & `greenlightplus-1.3/GreenLightPlus/core/greenhouse_env.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/core/greenhouse_geometry.py` & `greenlightplus-1.3/GreenLightPlus/core/greenhouse_geometry.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/core/greenlight_energyplus_simulation.py` & `greenlightplus-1.3/GreenLightPlus/core/greenlight_energyplus_simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-import sys
+
 from ..service_functions.funcs import calculate_energy_consumption, extract_last_value_from_nested_dict
 from .green_light_model import GreenLightModel
 
-class GreenhouseSimulation:
-    def __init__(self, energyplus_path, api, epw_path, idf_path, csv_path, output_directory, first_day, season_length, isMature=False):
-        # 将 EnergyPlus 安装目录添加到 Python 模块搜索路径
-        sys.path.insert(0, energyplus_path)
-
-        # 在设置路径后导入 pyenergyplus 模块
-        from pyenergyplus.plugin import EnergyPlusPlugin
-        from pyenergyplus.api import EnergyPlusAPI
 
-        # 初始化 EnergyPlusPlugin
-        EnergyPlusPlugin.__init__(self)
+class GreenhouseSimulation:
 
+    def __init__(self, api, epw_path, idf_path, csv_path, output_directory, first_day, season_length, isMature=False):
+        super().__init__()
         self.api = api
         self.epw_path = epw_path
         self.idf_path = idf_path
         self.csv_path = csv_path
         self.output_directory = output_directory
         self.last_time_step = None
         self.total_minutes = 0
@@ -40,47 +33,52 @@
         self.total_yield = 0
         self.lampIn = 0
         self.boilIn = 0
         self.current_step = 0
 
         # 创建GreenLight模型实例, 初始状态为未成熟
         self.model = GreenLightModel(
-            first_day=self.first_day, isMature=self.isMature, epw_path=self.epw_path,csv_path=self.csv_path)
+            first_day=self.first_day, isMature=self.isMature, epw_path=self.epw_path, csv_path=self.csv_path)
 
         # 初始化状态参数
         self.init_state = {
             "p": {
                 # Greenhouse structure settings
                 'psi': 22,  # Mean greenhouse cover slope [degrees]
                 'aFlr': 668,  # Floor area [m^2]
-                'aCov': 1405,  # Surface of the cover including side walls [m^2]
+                # Surface of the cover including side walls [m^2]
+                'aCov': 1405,
                 # Height of the main compartment [m] (the ridge height is 6.5, screen is 20 cm below it)
                 'hAir': 6.5,
                 'hGh': 6.905,  # Mean height of the greenhouse [m]
                 'aRoof': 39*2,  # Maximum roof ventilation area
-                'hVent': 1.3,  # Vertical dimension of single ventilation opening [m]
+                # Vertical dimension of single ventilation opening [m]
+                'hVent': 1.3,
                 'cDgh': 0.75,  # Ventilation discharge coefficient [-]
                 'lPipe': 1.25,  # Length of pipe rail system [m m^-2]
                 # Capacity of CO2 injection for the entire greenhouse [mg s^-1]
                 'phiExtCo2': 7.2e4*4e4/1.4e4,
-                'pBoil': 300*668,  # Capacity of boiler for the entire greenhouse [W]
+                # Capacity of boiler for the entire greenhouse [W]
+                'pBoil': 300*668,
 
                 # Control settings
                 'co2SpDay': 1000,  # CO2 setpoint during the light period [ppm]
                 'tSpNight': 18.5,  # temperature set point dark period [°C]
                 'tSpDay': 19.5,  # temperature set point light period [°C]
                 'rhMax': 87,  # maximum relative humidity [%]
                 # P-band for ventilation due to high temperature [°C]
                 'ventHeatPband': 4,
                 # P-band for ventilation due to high relative humidity [% humidity]
                 'ventRhPband': 50,
                 # P-band for screen opening due to high relative humidity [% humidity]
                 'thScrRhPband': 10,
-                'lampsOn': 0,  # time of day (in morning) to switch on lamps [h]
-                'lampsOff': 18,  # time of day (in evening) to switch off lamps [h]
+                # time of day (in morning) to switch on lamps [h]
+                'lampsOn': 0,
+                # time of day (in evening) to switch off lamps [h]
+                'lampsOff': 18,
                 # lamps are switched off if global radiation is above this value [W m^-2]
                 'lampsOffSun': 400,
                 # Predicted daily radiation sum from the sun where lamps are not used that day [MJ m^-2 day^-1]
                 'lampRadSumLimit': 10
             }
         }
 
@@ -176,32 +174,30 @@
             self.init_state = gl
 
             # 使用EnergyPlus输出的数据更新GreenLight模型的状态, 从而实现数据传递
             # print(f"原始温度: {self.init_state['x']['tTop'][-1][-1]}, 原始饱和水蒸气压力: {self.init_state['x']['vpTop'][-1][-1]}")
 
             self.init_state['x']["tTop"][-1][-1] = current_temperature
             self.init_state['x']["vpTop"][-1][-1] = vpTop
-            
-            
+
             # print(f"温度被替换为: {current_temperature}, 饱和水蒸气压力被替换为: {vpTop}")
 
             self.current_step += 1
 
             # 计算水果产量
             dmc = 0.06
             self.total_yield += 1e-6 * \
                 calculate_energy_consumption(gl, "mcFruitHar") / dmc
 
             # 计算照明和加热产生的能耗
             self.lampIn += 1e-6 * \
                 calculate_energy_consumption(gl, "qLampIn", "qIntLampIn")
             self.boilIn += 1e-6 * \
                 calculate_energy_consumption(gl, "hBoilPipe", "hBoilGroPipe")
-                
-                
+
             # print(f"total_yield: {self.total_yield}, lampIn: {self.lampIn}, boilIn: {self.boilIn}")
 
     def run(self):
 
         # 创建新的状态
         state = self.api.state_manager.new_state()
```

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/change_res.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/change_res.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/create_green_light_model.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/create_green_light_model.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/ode.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/ode.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_default_lamp_params.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_default_lamp_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_dep_params.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_dep_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_aux.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_aux.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_control.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_control.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_control_init.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_control_init.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_init.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_init.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_input.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_input.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_odes.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_odes.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_params.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_params.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_states.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_states.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_gl_time.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_gl_time.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py` & `greenlightplus-1.3/GreenLightPlus/create_green_light_model/set_params4ha_world_comparison.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/result_analysis/energy_analysis.py` & `greenlightplus-1.3/GreenLightPlus/result_analysis/energy_analysis.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/result_analysis/energy_yield_analysis.py` & `greenlightplus-1.3/GreenLightPlus/result_analysis/energy_yield_analysis.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/result_analysis/plot_green_light.py` & `greenlightplus-1.3/GreenLightPlus/result_analysis/plot_green_light.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/co2_dens2ppm.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/co2_dens2ppm.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/co2_ppm2dens.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/co2_ppm2dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/convert_epw2csv.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/convert_epw2csv.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/cut_energy_plus_data.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/cut_energy_plus_data.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/funcs.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/funcs.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/make_artificial_input.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/make_artificial_input.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/rh2vapor_dens.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/rh2vapor_dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/vapor_dens2pres.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/vapor_dens2pres.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus/service_functions/vp2dens.py` & `greenlightplus-1.3/GreenLightPlus/service_functions/vp2dens.py`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/GreenLightPlus.egg-info/PKG-INFO` & `greenlightplus-1.3/GreenLightPlus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GreenLightPlus
-Version: 1.2
+Version: 1.3
 Summary: Greenhouse Simulation and Optimization Toolkit
 Author-email: Daidai Qiu <qiu.daidai@outlook.com>
 Project-URL: Homepage, https://github.com/greenpeer/GreenLightPlus
 Project-URL: Bug Reports, https://github.com/greenpeer/GreenLightPlus/issues
 Project-URL: Source, https://github.com/greenpeer/GreenLightPlus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `greenlightplus-1.2/GreenLightPlus.egg-info/SOURCES.txt` & `greenlightplus-1.3/GreenLightPlus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `greenlightplus-1.2/PKG-INFO` & `greenlightplus-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GreenLightPlus
-Version: 1.2
+Version: 1.3
 Summary: Greenhouse Simulation and Optimization Toolkit
 Author-email: Daidai Qiu <qiu.daidai@outlook.com>
 Project-URL: Homepage, https://github.com/greenpeer/GreenLightPlus
 Project-URL: Bug Reports, https://github.com/greenpeer/GreenLightPlus/issues
 Project-URL: Source, https://github.com/greenpeer/GreenLightPlus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `greenlightplus-1.2/pyproject.toml` & `greenlightplus-1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GreenLightPlus"
-version = "1.2"
+version = "1.3"
 authors = [
     {name = "Daidai Qiu", email = "qiu.daidai@outlook.com"}
 ]
 description = "Greenhouse Simulation and Optimization Toolkit"
 readme = "GreenLightPlus/README.md"
 requires-python = ">=3.8"
 classifiers = [
```

