# Comparing `tmp/mesido-0.1.1.tar.gz` & `tmp/mesido-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mesido-0.1.1.tar", last modified: Fri Apr 12 07:34:25 2024, max compression
+gzip compressed data, was "mesido-0.1.2.tar", last modified: Mon Apr 29 12:26:53 2024, max compression
```

## Comparing `mesido-0.1.1.tar` & `mesido-0.1.2.tar`

### file list

```diff
@@ -1,226 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.767841 mesido-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 07:34:21.000000 mesido-0.1.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-12 07:34:21.000000 mesido-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-12 07:34:25.767841 mesido-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-12 07:34:21.000000 mesido-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-12 07:34:25.767841 mesido-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-12 07:34:21.000000 mesido-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.727843 mesido-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.767841 mesido-0.1.1/src/mesido/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/_darcy_weisbach.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/_heat_loss_u_values_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 07:34:25.767841 mesido-0.1.1/src/mesido/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)   104774 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/asset_sizing_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/base_component_type_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/component_type_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/control_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/demand_insulation_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    30118 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/electricity_physics_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.739842 mesido-0.1.1/src/mesido/esdl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   119140 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/_edr_pipes.json
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/_update_edr_pipes_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    45340 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/asset_to_component_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/edr_pipe_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/esdl_additional_vars_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    61654 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/esdl_heat_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    29121 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/esdl_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16311 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/esdl_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/esdl_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/esdl_qth_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    25058 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/esdl/profile_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    62747 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/financial_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    35265 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/gas_physics_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    50797 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/head_loss_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/heat_network_common.py
--rw-r--r--   0 runner    (1001) docker     (127)   180470 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/heat_physics_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.739842 mesido-0.1.1/src/mesido/influxdb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/influxdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/influxdb/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.731842 mesido-0.1.1/src/mesido/modelica/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.739842 mesido-0.1.1/src/mesido/modelica/WarmingUp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.739842 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.743842 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Buffer.mo
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/CheckValve.mo
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/ControlValve.mo
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Demand.mo
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/GeothermalSource.mo
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/HeatPort.mo
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/HeatTwoPort.mo
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Node.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Pipe.mo
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Pump.mo
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Source.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/_NonStorageComponent.mo
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/package.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.747842 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Buffer.mo
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/CheckValve.mo
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/ControlValve.mo
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Demand.mo
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/GeothermalSource.mo
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Node.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Pipe.mo
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Pump.mo
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/QTHPort.mo
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/QTHTwoPort.mo
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Source.mo
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/_FluidPropertiesComponent.mo
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/_NonStorageComponent.mo
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/package.mo
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/package.mo
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/modelica/WarmingUp/package.mo
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/network_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/physics_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pipe_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.747842 mesido-0.1.1/src/mesido/pycml/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.747842 mesido-0.1.1/src/mesido/pycml/component_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.747842 mesido-0.1.1/src/mesido/pycml/component_library/milp/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.747842 mesido-0.1.1/src/mesido/pycml/component_library/milp/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/_internal/electricity_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/_internal/gas_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/_internal/heat_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.747842 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_cable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_demand.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/heat_pump_elec.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/solarpv.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/windpark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.751842 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_demand.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_substation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_tank_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.755842 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/_non_storage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/air_water_heat_pump.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/ates.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/check_valve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/cold_demand.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/control_valve.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/geothermal_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_demand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_exchanger.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_four_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_pump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_two_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/low_temperature_ates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/pump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.755842 mesido-0.1.1/src/mesido/pycml/component_library/milp/multicommodity/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/multicommodity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/milp/multicommodity/electrolyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.755842 mesido-0.1.1/src/mesido/pycml/component_library/qth/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/_fluid_properties_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.755842 mesido-0.1.1/src/mesido/pycml/component_library/qth/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/_internal/qth_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/_non_storage_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/check_valve.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/control_valve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/demand.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/geothermal_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/pump.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/qth_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/qth_two_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/component_library/qth/source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/pycml/pycml_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.759842 mesido-0.1.1/src/mesido/qth_not_maintained/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/qth_not_maintained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/qth_not_maintained/bounds_to_pipe_flow_directions_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    46959 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/qth_not_maintained/head_loss_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/qth_not_maintained/qth_loop_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    56037 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/qth_not_maintained/qth_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/qth_not_maintained/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/techno_economic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.759842 mesido-0.1.1/src/mesido/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.759842 mesido-0.1.1/src/mesido/workflows/goals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/goals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/goals/minimize_tco_goal.py
--rw-r--r--   0 runner    (1001) docker     (127)    23397 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/grow_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.759842 mesido-0.1.1/src/mesido/workflows/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/io/read_files_and_create_influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    62347 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/io/write_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/simulator_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.759842 mesido-0.1.1/src/mesido/workflows/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/utils/adapt_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-12 07:34:21.000000 mesido-0.1.1/src/mesido/workflows/utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.767841 mesido-0.1.1/src/mesido.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-12 07:34:25.000000 mesido-0.1.1/src/mesido.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-04-12 07:34:25.000000 mesido-0.1.1/src/mesido.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:34:25.000000 mesido-0.1.1/src/mesido.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 07:34:25.000000 mesido-0.1.1/src/mesido.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-12 07:34:25.000000 mesido-0.1.1/src/mesido.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 07:34:25.000000 mesido-0.1.1/src/mesido.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:25.763841 mesido-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_absolute_heat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_asset_is_realized.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_ates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_cable_topology_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_cold_demand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_electric_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_electric_source_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_electrolyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_end_scenario_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_end_scenario_sizing_annualized.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_esdl_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_esdl_pycml.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_gas_multi_demand_source_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_gas_pipe_topology_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_gas_source_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)    39312 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_head_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_head_loss_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_heat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_heat_loss_u_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    12734 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_hydraulic_power.py
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_insulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_max_size_and_optional_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_multicommodity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_multiple_carriers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_multiple_in_and_out_port_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_network_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_pipe_diameter_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_producer_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_profile_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_pycml.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_setpoint_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_temperature_ates_hp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_topo_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_varying_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-04-12 07:34:22.000000 mesido-0.1.1/tests/test_warmingup_unit_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    68611 2024-04-12 07:34:22.000000 mesido-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.792005 mesido-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-29 12:26:49.000000 mesido-0.1.2/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-29 12:26:49.000000 mesido-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-29 12:26:53.792005 mesido-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-29 12:26:49.000000 mesido-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 12:26:53.792005 mesido-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 12:26:49.000000 mesido-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.744004 mesido-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.792005 mesido-0.1.2/src/mesido/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/_darcy_weisbach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/_heat_loss_u_values_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 12:26:53.792005 mesido-0.1.2/src/mesido/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106270 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/asset_sizing_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/base_component_type_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/component_type_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/control_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/demand_insulation_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30118 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/electricity_physics_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.760004 mesido-0.1.2/src/mesido/esdl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119140 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/_edr_pipes.json
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/_update_edr_pipes_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47452 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/asset_to_component_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/edr_pipe_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/esdl_additional_vars_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73681 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/esdl_heat_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29121 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/esdl_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18444 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/esdl_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/esdl_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/esdl_qth_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25058 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/esdl/profile_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62633 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/financial_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28588 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/gas_physics_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69003 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/head_loss_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/heat_network_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167904 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/heat_physics_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.760004 mesido-0.1.2/src/mesido/influxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/influxdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/influxdb/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.748004 mesido-0.1.2/src/mesido/modelica/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.760004 mesido-0.1.2/src/mesido/modelica/WarmingUp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.760004 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.760004 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Buffer.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/CheckValve.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/ControlValve.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Demand.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/GeothermalSource.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/HeatPort.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/HeatTwoPort.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Node.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Pipe.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Pump.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Source.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/_NonStorageComponent.mo
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/package.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.764005 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Buffer.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/CheckValve.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/ControlValve.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Demand.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/GeothermalSource.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Node.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Pipe.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Pump.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/QTHPort.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/QTHTwoPort.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Source.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/_FluidPropertiesComponent.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/_NonStorageComponent.mo
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/package.mo
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/package.mo
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/modelica/WarmingUp/package.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/network_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/physics_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pipe_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.764005 mesido-0.1.2/src/mesido/pycml/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.764005 mesido-0.1.2/src/mesido/pycml/component_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.764005 mesido-0.1.2/src/mesido/pycml/component_library/milp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.768005 mesido-0.1.2/src/mesido/pycml/component_library/milp/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/_internal/electricity_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/_internal/gas_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/_internal/heat_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.768005 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_cable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_demand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/heat_pump_elec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/solarpv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/windpark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.768005 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_demand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_substation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_tank_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.772005 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/_non_storage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/air_water_heat_pump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/airco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/ates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/check_valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/cold_demand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/control_valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/geothermal_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_demand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_exchanger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_four_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_pump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_two_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/low_temperature_ates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/pump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.776005 mesido-0.1.2/src/mesido/pycml/component_library/milp/multicommodity/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/multicommodity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/multicommodity/airwater_heat_pump_elec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/multicommodity/electro_boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/multicommodity/electrolyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/milp/multicommodity/gas_boiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.776005 mesido-0.1.2/src/mesido/pycml/component_library/qth/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/_fluid_properties_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.776005 mesido-0.1.2/src/mesido/pycml/component_library/qth/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/_internal/qth_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/_non_storage_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/check_valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/control_valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/demand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/geothermal_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/pump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/qth_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/qth_two_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/component_library/qth/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/pycml/pycml_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.780005 mesido-0.1.2/src/mesido/qth_not_maintained/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/qth_not_maintained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/qth_not_maintained/bounds_to_pipe_flow_directions_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46959 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/qth_not_maintained/head_loss_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/qth_not_maintained/qth_loop_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56037 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/qth_not_maintained/qth_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/qth_not_maintained/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/techno_economic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.780005 mesido-0.1.2/src/mesido/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/emerge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.780005 mesido-0.1.2/src/mesido/workflows/goals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/goals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/goals/minimize_tco_goal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23397 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/grow_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.780005 mesido-0.1.2/src/mesido/workflows/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/io/read_files_and_create_influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62715 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/io/write_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/simulator_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.780005 mesido-0.1.2/src/mesido/workflows/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/utils/adapt_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-29 12:26:49.000000 mesido-0.1.2/src/mesido/workflows/utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.788005 mesido-0.1.2/src/mesido.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-29 12:26:53.000000 mesido-0.1.2/src/mesido.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-29 12:26:53.000000 mesido-0.1.2/src/mesido.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:26:53.000000 mesido-0.1.2/src/mesido.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 12:26:53.000000 mesido-0.1.2/src/mesido.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-29 12:26:53.000000 mesido-0.1.2/src/mesido.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 12:26:53.000000 mesido-0.1.2/src/mesido.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:26:53.788005 mesido-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_absolute_heat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_asset_is_realized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_ates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_cable_topology_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_cold_demand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_elec_boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_electric_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_electric_source_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_electrolyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_emerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_end_scenario_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_end_scenario_sizing_annualized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_esdl_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_esdl_pycml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_gas_boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_gas_multi_demand_source_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_gas_pipe_topology_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_gas_source_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39337 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_head_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_head_loss_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15395 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_heat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_heat_loss_u_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23264 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_hydraulic_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_insulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_max_size_and_optional_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_multicommodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_multiple_carriers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_multiple_in_and_out_port_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_network_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_pipe_diameter_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_producer_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_profile_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_pycml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_setpoint_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_temperature_ates_hp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_topo_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_updated_esdl_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_updated_esdl_pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20164 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_varying_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-29 12:26:49.000000 mesido-0.1.2/tests/test_warmingup_unit_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68611 2024-04-29 12:26:49.000000 mesido-0.1.2/versioneer.py
```

### Comparing `mesido-0.1.1/COPYING.LESSER` & `mesido-0.1.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/PKG-INFO` & `mesido-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesido
-Version: 0.1.1
+Version: 0.1.2
 Summary: Multi Energy System Optimization
 Home-page: https://github.com/Multi-Energy-Systems-Optimization/mesido/
 Author: Jim Rojer
 Author-email: jim.rojer@tno.nl
 Maintainer: Jim Rojer, Kobus van Rooyen, Kelbij Star, Femke Janssen, Jesús Andrés Rodríguez Sarasty, Thijs van der Klauw
 License: LGPLv3
 Keywords: Multi-Energy-Systems,optimization
```

### Comparing `mesido-0.1.1/README.md` & `mesido-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/setup.py` & `mesido-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/_darcy_weisbach.py` & `mesido-0.1.2/src/mesido/_darcy_weisbach.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/_heat_loss_u_values_pipe.py` & `mesido-0.1.2/src/mesido/_heat_loss_u_values_pipe.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/asset_sizing_mixin.py` & `mesido-0.1.2/src/mesido/asset_sizing_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,60 +34,60 @@
         # Boolean variable to switch assets on/off or to increment their size for the entire time
         # horizon.
         self.__asset_aggregation_count_var = {}
         self.__asset_aggregation_count_var_bounds = {}
         self._asset_aggregation_count_var_map = {}
 
         # Variable for the maximum discharge under pipe class optimization
-        self.__pipe_topo_max_discharge_var = {}
-        self._pipe_topo_max_discharge_map = {}
-        self.__pipe_topo_max_discharge_nominals = {}
-        self.__pipe_topo_max_discharge_var_bounds = {}
+        self.__heat_pipe_topo_max_discharge_var = {}
+        self._heat_pipe_topo_max_discharge_map = {}
+        self.__heat_pipe_topo_max_discharge_nominals = {}
+        self.__heat_pipe_topo_max_discharge_var_bounds = {}
 
         # Variable for the diameter of a pipe during pipe-class optimization
-        self.__pipe_topo_diameter_var = {}
-        self.__pipe_topo_diameter_var_bounds = {}
-        self._pipe_topo_diameter_map = {}
-        self.__pipe_topo_diameter_nominals = {}
+        self.__heat_pipe_topo_diameter_var = {}
+        self.__heat_pipe_topo_diameter_var_bounds = {}
+        self._heat_pipe_topo_diameter_map = {}
+        self.__heat_pipe_topo_diameter_nominals = {}
 
         # Variable for the investmentcost in eur/m during pipe-class optimization
-        self.__pipe_topo_cost_var = {}
-        self.__pipe_topo_cost_var_bounds = {}
-        self._pipe_topo_cost_map = {}
-        self.__pipe_topo_cost_nominals = {}
+        self.__heat_pipe_topo_cost_var = {}
+        self.__heat_pipe_topo_cost_var_bounds = {}
+        self._heat_pipe_topo_cost_map = {}
+        self.__heat_pipe_topo_cost_nominals = {}
 
         # Boolean variables for the various pipe class options per pipe
-        # The self._pipe_topo_pipe_class_map is already initiated in the HeatPhysicsMixin
-        self.__pipe_topo_pipe_class_var = {}
-        self.__pipe_topo_pipe_class_var_bounds = {}
-        self.__pipe_topo_pipe_class_result = {}
-
-        self.__pipe_topo_pipe_class_discharge_ordering_var = {}
-        self.__pipe_topo_pipe_class_discharge_ordering_var_bounds = {}
-        self.__pipe_topo_pipe_class_discharge_ordering_map = {}
-
-        self.__pipe_topo_pipe_class_cost_ordering_map = {}
-        self.__pipe_topo_pipe_class_cost_ordering_var = {}
-        self.__pipe_topo_pipe_class_cost_ordering_var_bounds = {}
-
-        self.__pipe_topo_pipe_class_heat_loss_ordering_map = {}
-        self.__pipe_topo_pipe_class_heat_loss_ordering_var = {}
-        self.__pipe_topo_pipe_class_heat_loss_ordering_var_bounds = {}
-
-        self.__pipe_topo_global_pipe_class_count_var = {}
-        self.__pipe_topo_global_pipe_class_count_map = {}
-        self.__pipe_topo_global_pipe_class_count_var_bounds = {}
+        # The self._heat_pipe_topo_pipe_class_map is already initiated in the HeatPhysicsMixin
+        self.__heat_pipe_topo_pipe_class_var = {}
+        self.__heat_pipe_topo_pipe_class_var_bounds = {}
+        self.__heat_pipe_topo_pipe_class_result = {}
+
+        self.__heat_pipe_topo_pipe_class_discharge_ordering_var = {}
+        self.__heat_pipe_topo_pipe_class_discharge_ordering_var_bounds = {}
+        self.__heat_pipe_topo_pipe_class_discharge_ordering_map = {}
+
+        self.__heat_pipe_topo_pipe_class_cost_ordering_map = {}
+        self.__heat_pipe_topo_pipe_class_cost_ordering_var = {}
+        self.__heat_pipe_topo_pipe_class_cost_ordering_var_bounds = {}
+
+        self.__heat_pipe_topo_pipe_class_heat_loss_ordering_map = {}
+        self.__heat_pipe_topo_pipe_class_heat_loss_ordering_var = {}
+        self.__heat_pipe_topo_pipe_class_heat_loss_ordering_var_bounds = {}
+
+        self.__heat_pipe_topo_global_pipe_class_count_var = {}
+        self.__heat_pipe_topo_global_pipe_class_count_map = {}
+        self.__heat_pipe_topo_global_pipe_class_count_var_bounds = {}
 
         # Dict to specifically update the discharge bounds under pipe-class optimization
-        self.__pipe_topo_heat_discharge_bounds = {}
+        self.__heat_pipe_topo_heat_discharge_bounds = {}
 
         # list with entry per ensemble member containing dicts of pipe parameter values for
         # diameter, area and heatloss.
-        self.__pipe_topo_diameter_area_parameters = []
-        self.__pipe_topo_heat_loss_parameters = []
+        self.__heat_pipe_topo_diameter_area_parameters = []
+        self.__heat_pipe_topo_heat_loss_parameters = []
 
         # Gas
         # Variable for the maximum discharge under pipe class optimization
         self.__gas_pipe_topo_max_discharge_var = {}
         self._gas_pipe_topo_max_discharge_map = {}
         self.__gas_pipe_topo_max_discharge_nominals = {}
         self.__gas_pipe_topo_max_discharge_var_bounds = {}
@@ -101,15 +101,15 @@
         # Variable for the investmentcost in eur/m during pipe-class optimization
         self.__gas_pipe_topo_cost_var = {}
         self.__gas_pipe_topo_cost_var_bounds = {}
         self._gas_pipe_topo_cost_map = {}
         self.__gas_pipe_topo_cost_nominals = {}
 
         # Boolean variables for the various pipe class options per pipe
-        # The self._pipe_topo_pipe_class_map is already initiated in the HeatPhysicsMixin
+        # The self._gas_pipe_topo_pipe_class_map is already initiated in the GasPhysicsMixin
         self.__gas_pipe_topo_pipe_class_var = {}
         self.__gas_pipe_topo_pipe_class_var_bounds = {}
         self.__gas_pipe_topo_pipe_class_result = {}
 
         self.__gas_pipe_topo_pipe_class_discharge_ordering_var = {}
         self.__gas_pipe_topo_pipe_class_discharge_ordering_var_bounds = {}
         self.__gas_pipe_topo_pipe_class_discharge_ordering_map = {}
@@ -138,15 +138,16 @@
         # Variable for the investmentcost in eur/m during pipe-class optimization
         self.__electricity_cable_topo_cost_var = {}
         self.__electricity_cable_topo_cost_var_bounds = {}
         self._electricity_cable_topo_cost_map = {}
         self.__electricity_cable_topo_cost_nominals = {}
 
         # Boolean variables for the various pipe class options per pipe
-        # The self._pipe_topo_pipe_class_map is already initiated in the HeatPhysicsMixin
+        # The self._electricity_cable_topo_cable_class_map is already initiated in the
+        # ElectricityPhysicsMixin
         self.__electricity_cable_topo_cable_class_var = {}
         self.__electricity_cable_topo_cable_class_var_bounds = {}
         self.__electricity_cable_topo_cable_class_result = {}
 
         self.__electricity_cable_topo_cable_class_current_ordering_var = {}
         self.__electricity_cable_topo_cable_class_current_ordering_var_bounds = {}
         self.__electricity_cable_topo_cable_class_current_ordering_map = {}
@@ -186,25 +187,25 @@
         # Pipe topology variables
 
         # In case the user overrides the pipe class of the pipe with a single
         # pipe class we update the diameter/area parameters. If there is more
         # than a single pipe class for a certain pipe, we set the diameter
         # and area to NaN to prevent erroneous constraints.
         for _ in range(self.ensemble_size):
-            self.__pipe_topo_diameter_area_parameters.append({})
-            self.__pipe_topo_heat_loss_parameters.append({})
+            self.__heat_pipe_topo_diameter_area_parameters.append({})
+            self.__heat_pipe_topo_heat_loss_parameters.append({})
 
         unique_pipe_classes = self.get_unique_pipe_classes()
         for pc in unique_pipe_classes:
             pipe_class_count = f"{pc.name}__global_pipe_class_count"
-            self.__pipe_topo_global_pipe_class_count_var[pipe_class_count] = ca.MX.sym(
+            self.__heat_pipe_topo_global_pipe_class_count_var[pipe_class_count] = ca.MX.sym(
                 pipe_class_count
             )
-            self.__pipe_topo_global_pipe_class_count_map[f"{pc.name}"] = pipe_class_count
-            self.__pipe_topo_global_pipe_class_count_var_bounds[pipe_class_count] = (
+            self.__heat_pipe_topo_global_pipe_class_count_map[f"{pc.name}"] = pipe_class_count
+            self.__heat_pipe_topo_global_pipe_class_count_var_bounds[pipe_class_count] = (
                 0.0,
                 len(self.energy_system_components.get("heat_pipe", [])),
             )
 
         unique_pipe_classes = self.get_unique_gas_pipe_classes()
         for pc in unique_pipe_classes:
             pipe_class_count = f"{pc.name}__global_gas_pipe_class_count"
@@ -501,91 +502,97 @@
 
             # Note that we always make a diameter symbol, even if the diameter
             # is fixed. This can be convenient when playing around with
             # different pipe class options, and providing a uniform interface
             # to the user. Contrary to that, the pipe class booleans are very
             # much an internal affair.
             diam_var_name = f"{pipe}__hn_diameter"
-            self.__pipe_topo_diameter_var[diam_var_name] = ca.MX.sym(diam_var_name)
-            self._pipe_topo_diameter_map[pipe] = diam_var_name
+            self.__heat_pipe_topo_diameter_var[diam_var_name] = ca.MX.sym(diam_var_name)
+            self._heat_pipe_topo_diameter_map[pipe] = diam_var_name
 
             cost_var_name = f"{pipe}__hn_cost"
-            self.__pipe_topo_cost_var[cost_var_name] = ca.MX.sym(cost_var_name)
-            self._pipe_topo_cost_map[pipe] = cost_var_name
+            self.__heat_pipe_topo_cost_var[cost_var_name] = ca.MX.sym(cost_var_name)
+            self._heat_pipe_topo_cost_map[pipe] = cost_var_name
 
             max_discharge_var_name = f"{pipe}__hn_max_discharge"
             max_discharges = [c.maximum_discharge for c in pipe_classes]
-            self.__pipe_topo_max_discharge_var[max_discharge_var_name] = ca.MX.sym(
+            self.__heat_pipe_topo_max_discharge_var[max_discharge_var_name] = ca.MX.sym(
                 max_discharge_var_name
             )
-            self._pipe_topo_max_discharge_map[pipe] = max_discharge_var_name
+            self._heat_pipe_topo_max_discharge_map[pipe] = max_discharge_var_name
 
             if len(pipe_classes) > 0:
-                self.__pipe_topo_max_discharge_nominals[max_discharge_var_name] = np.median(
+                self.__heat_pipe_topo_max_discharge_nominals[max_discharge_var_name] = np.median(
                     max_discharges
                 )
-                self.__pipe_topo_max_discharge_var_bounds[max_discharge_var_name] = (
+                self.__heat_pipe_topo_max_discharge_var_bounds[max_discharge_var_name] = (
                     -max(max_discharges),
                     max(max_discharges),
                 )
             else:
                 max_velocity = self.heat_network_settings["maximum_velocity"]
-                self.__pipe_topo_max_discharge_nominals[max_discharge_var_name] = (
+                self.__heat_pipe_topo_max_discharge_nominals[max_discharge_var_name] = (
                     parameters[f"{pipe}.area"] * max_velocity
                 )
-                self.__pipe_topo_max_discharge_var_bounds[max_discharge_var_name] = (
+                self.__heat_pipe_topo_max_discharge_var_bounds[max_discharge_var_name] = (
                     -parameters[f"{pipe}.area"] * max_velocity,
                     parameters[f"{pipe}.area"] * max_velocity,
                 )
 
             if not pipe_classes:
                 # No pipe class decision to make for this pipe w.r.t. diameter
                 diameter = parameters[f"{pipe}.diameter"]
                 investment_cost = parameters[f"{pipe}.investment_cost_coefficient"]
-                self.__pipe_topo_diameter_var_bounds[diam_var_name] = (diameter, diameter)
-                self.__pipe_topo_cost_var_bounds[cost_var_name] = (investment_cost, investment_cost)
+                self.__heat_pipe_topo_diameter_var_bounds[diam_var_name] = (diameter, diameter)
+                self.__heat_pipe_topo_cost_var_bounds[cost_var_name] = (
+                    investment_cost,
+                    investment_cost,
+                )
                 if diameter > 0.0:
-                    self.__pipe_topo_diameter_nominals[diam_var_name] = diameter
-                    self.__pipe_topo_cost_nominals[cost_var_name] = max(investment_cost, 1.0)
+                    self.__heat_pipe_topo_diameter_nominals[diam_var_name] = diameter
+                    self.__heat_pipe_topo_cost_nominals[cost_var_name] = max(investment_cost, 1.0)
             elif len(pipe_classes) == 1:
                 # No pipe class decision to make for this pipe w.r.t. diameter
                 diameter = pipe_classes[0].inner_diameter
                 investment_cost = pipe_classes[0].investment_costs
-                self.__pipe_topo_diameter_var_bounds[diam_var_name] = (diameter, diameter)
-                self.__pipe_topo_cost_var_bounds[cost_var_name] = (investment_cost, investment_cost)
+                self.__heat_pipe_topo_diameter_var_bounds[diam_var_name] = (diameter, diameter)
+                self.__heat_pipe_topo_cost_var_bounds[cost_var_name] = (
+                    investment_cost,
+                    investment_cost,
+                )
                 if diameter > 0.0:
-                    self.__pipe_topo_diameter_nominals[diam_var_name] = diameter
-                    self.__pipe_topo_cost_nominals[cost_var_name] = max(investment_cost, 1.0)
+                    self.__heat_pipe_topo_diameter_nominals[diam_var_name] = diameter
+                    self.__heat_pipe_topo_cost_nominals[cost_var_name] = max(investment_cost, 1.0)
                     if investment_cost == 0.0:
                         RuntimeWarning(f"{pipe} has an investment cost of 0. €/m")
 
                 for ensemble_member in range(self.ensemble_size):
-                    d = self.__pipe_topo_diameter_area_parameters[ensemble_member]
+                    d = self.__heat_pipe_topo_diameter_area_parameters[ensemble_member]
 
                     d[f"{pipe}.diameter"] = diameter
                     d[f"{pipe}.area"] = pipe_classes[0].area
             else:
                 diameters = [c.inner_diameter for c in pipe_classes]
-                self.__pipe_topo_diameter_var_bounds[diam_var_name] = (
+                self.__heat_pipe_topo_diameter_var_bounds[diam_var_name] = (
                     min(diameters),
                     max(diameters),
                 )
                 costs = [c.investment_costs for c in pipe_classes]
-                self.__pipe_topo_cost_var_bounds[cost_var_name] = (
+                self.__heat_pipe_topo_cost_var_bounds[cost_var_name] = (
                     min(costs),
                     max(costs),
                 )
-                self.__pipe_topo_cost_nominals[cost_var_name] = np.median(costs)
+                self.__heat_pipe_topo_cost_nominals[cost_var_name] = np.median(costs)
 
-                self.__pipe_topo_diameter_nominals[diam_var_name] = min(
+                self.__heat_pipe_topo_diameter_nominals[diam_var_name] = min(
                     x for x in diameters if x > 0.0
                 )
 
                 for ensemble_member in range(self.ensemble_size):
-                    d = self.__pipe_topo_diameter_area_parameters[ensemble_member]
+                    d = self.__heat_pipe_topo_diameter_area_parameters[ensemble_member]
 
                     d[f"{pipe}.diameter"] = np.nan
                     d[f"{pipe}.area"] = np.nan
 
             # For similar reasons as for the diameter, we always make a milp
             # loss symbol, even if the milp loss is fixed. Note that we also
             # override the .Heat_loss parameter for cold pipes, even though
@@ -612,15 +619,15 @@
                                 self, {"neglect_pipe_heat_losses": False}, parameters, pipe
                             )
                         ),
                         1.0,
                     )
 
                 for ensemble_member in range(self.ensemble_size):
-                    h = self.__pipe_topo_heat_loss_parameters[ensemble_member]
+                    h = self.__heat_pipe_topo_heat_loss_parameters[ensemble_member]
                     h[f"{pipe}.Heat_loss"] = pipe_heat_loss(self, options, parameters, pipe)
 
             elif len(pipe_classes) == 1:
                 # No pipe class decision to make for this pipe w.r.t. milp loss
                 u_values = pipe_classes[0].u_values
                 heat_loss = pipe_heat_loss(self, options, parameters, pipe, u_values)
 
@@ -633,15 +640,15 @@
                 else:
                     self._pipe_heat_loss_nominals[heat_loss_var_name] = max(
                         pipe_heat_loss(self, {"neglect_pipe_heat_losses": False}, parameters, pipe),
                         1.0,
                     )
 
                 for ensemble_member in range(self.ensemble_size):
-                    h = self.__pipe_topo_heat_loss_parameters[ensemble_member]
+                    h = self.__heat_pipe_topo_heat_loss_parameters[ensemble_member]
                     h[f"{pipe}.Heat_loss"] = heat_loss
             else:
                 heat_losses = [
                     pipe_heat_loss(self, options, parameters, pipe, c.u_values)
                     for c in pipe_classes
                 ]
 
@@ -651,28 +658,28 @@
                     max(heat_losses),
                 )
                 self._pipe_heat_loss_nominals[heat_loss_var_name] = np.median(
                     [x for x in heat_losses if x > 0]
                 )
 
                 for ensemble_member in range(self.ensemble_size):
-                    h = self.__pipe_topo_heat_loss_parameters[ensemble_member]
+                    h = self.__heat_pipe_topo_heat_loss_parameters[ensemble_member]
                     h[f"{pipe}.Heat_loss"] = max(
                         pipe_heat_loss(self, options, parameters, pipe), 1.0
                     )
 
             # Pipe class variables.
             if not pipe_classes or len(pipe_classes) == 1:
                 # No pipe class decision to make for this pipe
                 pass
             else:
-                self._pipe_topo_pipe_class_map[pipe] = {}
-                self.__pipe_topo_pipe_class_discharge_ordering_map[pipe] = {}
-                self.__pipe_topo_pipe_class_cost_ordering_map[pipe] = {}
-                self.__pipe_topo_pipe_class_heat_loss_ordering_map[pipe] = {}
+                self._heat_pipe_topo_pipe_class_map[pipe] = {}
+                self.__heat_pipe_topo_pipe_class_discharge_ordering_map[pipe] = {}
+                self.__heat_pipe_topo_pipe_class_cost_ordering_map[pipe] = {}
+                self.__heat_pipe_topo_pipe_class_heat_loss_ordering_map[pipe] = {}
 
                 for c in pipe_classes:
                     neighbour = self.has_related_pipe(pipe)
                     if neighbour and pipe not in self.hot_pipes:
                         cold_pipe = self.cold_to_hot_pipe(pipe)
                         pipe_class_var_name = f"{cold_pipe}__hn_pipe_class_{c.name}"
                         pipe_class_ordering_name = (
@@ -692,73 +699,82 @@
                         pipe_class_cost_ordering_name = (
                             f"{pipe}__hn_pipe_class_{c.name}_cost_ordering"
                         )
                         pipe_class_heat_loss_ordering_name = (
                             f"{pipe}__hn_pipe_class_{c.name}_heat_loss_ordering"
                         )
 
-                    self._pipe_topo_pipe_class_map[pipe][c] = pipe_class_var_name
-                    self.__pipe_topo_pipe_class_var[pipe_class_var_name] = ca.MX.sym(
+                    self._heat_pipe_topo_pipe_class_map[pipe][c] = pipe_class_var_name
+                    self.__heat_pipe_topo_pipe_class_var[pipe_class_var_name] = ca.MX.sym(
                         pipe_class_var_name
                     )
-                    self.__pipe_topo_pipe_class_var_bounds[pipe_class_var_name] = (0.0, 1.0)
+                    self.__heat_pipe_topo_pipe_class_var_bounds[pipe_class_var_name] = (0.0, 1.0)
 
-                    self.__pipe_topo_pipe_class_discharge_ordering_map[pipe][
+                    self.__heat_pipe_topo_pipe_class_discharge_ordering_map[pipe][
                         c
                     ] = pipe_class_ordering_name
-                    self.__pipe_topo_pipe_class_discharge_ordering_var[pipe_class_ordering_name] = (
-                        ca.MX.sym(pipe_class_ordering_name)
-                    )
-                    self.__pipe_topo_pipe_class_discharge_ordering_var_bounds[
+                    self.__heat_pipe_topo_pipe_class_discharge_ordering_var[
+                        pipe_class_ordering_name
+                    ] = ca.MX.sym(pipe_class_ordering_name)
+                    self.__heat_pipe_topo_pipe_class_discharge_ordering_var_bounds[
                         pipe_class_ordering_name
                     ] = (0.0, 1.0)
 
-                    self.__pipe_topo_pipe_class_cost_ordering_map[pipe][
+                    self.__heat_pipe_topo_pipe_class_cost_ordering_map[pipe][
                         c
                     ] = pipe_class_cost_ordering_name
-                    self.__pipe_topo_pipe_class_cost_ordering_var[pipe_class_cost_ordering_name] = (
-                        ca.MX.sym(pipe_class_cost_ordering_name)
-                    )
-                    self.__pipe_topo_pipe_class_cost_ordering_var_bounds[
+                    self.__heat_pipe_topo_pipe_class_cost_ordering_var[
+                        pipe_class_cost_ordering_name
+                    ] = ca.MX.sym(pipe_class_cost_ordering_name)
+                    self.__heat_pipe_topo_pipe_class_cost_ordering_var_bounds[
                         pipe_class_cost_ordering_name
                     ] = (0.0, 1.0)
 
-                    self.__pipe_topo_pipe_class_heat_loss_ordering_map[pipe][
+                    self.__heat_pipe_topo_pipe_class_heat_loss_ordering_map[pipe][
                         c
                     ] = pipe_class_heat_loss_ordering_name
-                    self.__pipe_topo_pipe_class_heat_loss_ordering_var[
+                    self.__heat_pipe_topo_pipe_class_heat_loss_ordering_var[
                         pipe_class_heat_loss_ordering_name
                     ] = ca.MX.sym(pipe_class_heat_loss_ordering_name)
-                    self.__pipe_topo_pipe_class_heat_loss_ordering_var_bounds[
+                    self.__heat_pipe_topo_pipe_class_heat_loss_ordering_var_bounds[
                         pipe_class_heat_loss_ordering_name
                     ] = (0.0, 1.0)
 
         # Update the bounds of the pipes that will have their diameter
         # optimized. Note that the flow direction may have already been fixed
         # based on the original bounds, if that was desired. We can therefore
         # naively override the bounds without taking this into account.
-        for pipe in self._pipe_topo_pipe_class_map:
-            pipe_classes = self._pipe_topo_pipe_class_map[pipe]
+        for pipe in self._heat_pipe_topo_pipe_class_map:
+            pipe_classes = self._heat_pipe_topo_pipe_class_map[pipe]
             max_discharge = max([c.maximum_discharge for c in pipe_classes])
 
-            self.__pipe_topo_heat_discharge_bounds[f"{pipe}.Q"] = (-max_discharge, max_discharge)
+            self.__heat_pipe_topo_heat_discharge_bounds[f"{pipe}.Q"] = (
+                -max_discharge,
+                max_discharge,
+            )
 
             # Heat on cold side is zero, so no change needed
             cp = parameters[f"{pipe}.cp"]
             rho = parameters[f"{pipe}.rho"]
             temperature = parameters[f"{pipe}.temperature"]
 
             # TODO: if temperature is variable these bounds should be set differently
             max_heat = 2.0 * cp * rho * temperature * max_discharge
 
-            self.__pipe_topo_heat_discharge_bounds[f"{pipe}.HeatIn.Heat"] = (-max_heat, max_heat)
-            self.__pipe_topo_heat_discharge_bounds[f"{pipe}.HeatOut.Heat"] = (-max_heat, max_heat)
+            self.__heat_pipe_topo_heat_discharge_bounds[f"{pipe}.HeatIn.Heat"] = (
+                -max_heat,
+                max_heat,
+            )
+            self.__heat_pipe_topo_heat_discharge_bounds[f"{pipe}.HeatOut.Heat"] = (
+                -max_heat,
+                max_heat,
+            )
 
         # When optimizing for pipe size, we do not yet support all options
-        if self._pipe_topo_pipe_class_map:
+        if self._heat_pipe_topo_pipe_class_map:
             if np.isfinite(options["maximum_temperature_der"]) and np.isfinite(
                 options["maximum_flow_der"]
             ):
                 raise Exception(
                     "When optimizing pipe diameters, "
                     "the `maximum_temperature_der` or `maximum_flow_der` should be infinite."
                 )
@@ -786,14 +802,21 @@
                 else bounds[f"{asset_name}.HeatIn.Heat"][1]
             )
             # Note that we only enforce the upper bound in state enabled if it was explicitly
             # specified for the demand
             lb = 0.0 if np.isinf(bounds[f"{asset_name}.Heat_demand"][1]) else ub
             _make_max_size_var(name=asset_name, lb=lb, ub=ub, nominal=ub / 2.0)
 
+        for asset_name in self.energy_system_components.get("airco", []):
+            ub = bounds[f"{asset_name}.Heat_airco"][1]
+            # Note that we only enforce the upper bound in state enabled if it was explicitly
+            # specified for the demand
+            lb = 0.0 if np.isinf(bounds[f"{asset_name}.Heat_airco"][1]) else ub
+            _make_max_size_var(name=asset_name, lb=lb, ub=ub, nominal=ub / 2.0)
+
         for asset_name in self.energy_system_components.get("cold_demand", []):
             ub = (
                 bounds[f"{asset_name}.Cold_demand"][1]
                 if not np.isinf(bounds[f"{asset_name}.Cold_demand"][1])
                 else bounds[f"{asset_name}.HeatIn.Heat"][1]
             )
             # Note that we only enforce the upper bound in state enabled if it was explicitly
@@ -995,57 +1018,57 @@
         return unique_cable_classes
 
     def get_optimized_pipe_class(self, pipe: str) -> PipeClass:
         """
         Return the optimized pipe class for a specific pipe. If no
         optimized pipe class is available (yet), a `KeyError` is returned.
         """
-        return self.__pipe_topo_pipe_class_result[pipe]
+        return self.__heat_pipe_topo_pipe_class_result[pipe]
 
     def get_optimized_deman_insulation_class(self, demand_insulation: str) -> DemandInsulationClass:
         """
         Return the optimized demand_insulation class for a specific pipe. If no
         optimized demand insulation class is available (yet), a `KeyError` is returned.
         """
         return self.__demand_insulation_class_result[demand_insulation]
 
     def pipe_diameter_symbol_name(self, pipe: str) -> str:
         """
         Return the symbol name for the pipe diameter
         """
-        return self._pipe_topo_diameter_map[pipe]
+        return self._heat_pipe_topo_diameter_map[pipe]
 
     def pipe_cost_symbol_name(self, pipe: str) -> str:
         """
         Return the symbol name for the pipe investment cost per meter
         """
-        return self._pipe_topo_cost_map[pipe]
+        return self._heat_pipe_topo_cost_map[pipe]
 
     @property
     def extra_variables(self):
         """
         In this function we add all the variables defined in the HeatMixin to the optimization
         problem. Note that these are only the normal variables not path variables.
         """
         variables = super().extra_variables.copy()
-        variables.extend(self.__pipe_topo_diameter_var.values())
-        variables.extend(self.__pipe_topo_cost_var.values())
-        variables.extend(self.__pipe_topo_pipe_class_var.values())
+        variables.extend(self.__heat_pipe_topo_diameter_var.values())
+        variables.extend(self.__heat_pipe_topo_cost_var.values())
+        variables.extend(self.__heat_pipe_topo_pipe_class_var.values())
         variables.extend(self.__gas_pipe_topo_diameter_var.values())
         variables.extend(self.__gas_pipe_topo_cost_var.values())
         variables.extend(self.__gas_pipe_topo_pipe_class_var.values())
         variables.extend(self.__asset_max_size_var.values())
         variables.extend(self.__asset_aggregation_count_var.values())
         variables.extend(self.__gas_pipe_topo_max_discharge_var.values())
-        variables.extend(self.__pipe_topo_max_discharge_var.values())
-        variables.extend(self.__pipe_topo_global_pipe_class_count_var.values())
+        variables.extend(self.__heat_pipe_topo_max_discharge_var.values())
+        variables.extend(self.__heat_pipe_topo_global_pipe_class_count_var.values())
         variables.extend(self.__gas_pipe_topo_global_pipe_class_count_var.values())
-        variables.extend(self.__pipe_topo_pipe_class_discharge_ordering_var.values())
-        variables.extend(self.__pipe_topo_pipe_class_cost_ordering_var.values())
-        variables.extend(self.__pipe_topo_pipe_class_heat_loss_ordering_var.values())
+        variables.extend(self.__heat_pipe_topo_pipe_class_discharge_ordering_var.values())
+        variables.extend(self.__heat_pipe_topo_pipe_class_cost_ordering_var.values())
+        variables.extend(self.__heat_pipe_topo_pipe_class_heat_loss_ordering_var.values())
         variables.extend(self.__gas_pipe_topo_pipe_class_discharge_ordering_var.values())
         variables.extend(self.__gas_pipe_topo_pipe_class_cost_ordering_var.values())
         variables.extend(self.__electricity_cable_topo_max_current_var.values())
         variables.extend(self.__electricity_cable_topo_resistance_var.values())
         variables.extend(self.__electricity_cable_topo_cost_var.values())
         variables.extend(self.__electricity_cable_topo_cable_class_var.values())
         variables.extend(self.__electricity_cable_topo_cable_class_current_ordering_var.values())
@@ -1065,19 +1088,19 @@
         return variables
 
     def variable_is_discrete(self, variable):
         """
         All variables that only can take integer values should be added to this function.
         """
         if (
-            variable in self.__pipe_topo_pipe_class_var
+            variable in self.__heat_pipe_topo_pipe_class_var
             or variable in self.__asset_aggregation_count_var
-            or variable in self.__pipe_topo_pipe_class_discharge_ordering_var
-            or variable in self.__pipe_topo_pipe_class_cost_ordering_var
-            or variable in self.__pipe_topo_pipe_class_heat_loss_ordering_var
+            or variable in self.__heat_pipe_topo_pipe_class_discharge_ordering_var
+            or variable in self.__heat_pipe_topo_pipe_class_cost_ordering_var
+            or variable in self.__heat_pipe_topo_pipe_class_heat_loss_ordering_var
             or variable in self.__gas_pipe_topo_pipe_class_discharge_ordering_var
             or variable in self.__gas_pipe_topo_pipe_class_cost_ordering_var
             or variable in self.__gas_pipe_topo_pipe_class_var
             or variable in self.__electricity_cable_topo_cable_class_var
             or variable in self.__electricity_cable_topo_cable_class_current_ordering_var
             or variable in self.__electricity_cable_topo_cable_class_cost_ordering_var
         ):
@@ -1085,24 +1108,24 @@
         else:
             return super().variable_is_discrete(variable)
 
     def variable_nominal(self, variable):
         """
         In this function we add all the nominals for the variables defined/added in the HeatMixin.
         """
-        if variable in self.__pipe_topo_diameter_nominals:
-            return self.__pipe_topo_diameter_nominals[variable]
+        if variable in self.__heat_pipe_topo_diameter_nominals:
+            return self.__heat_pipe_topo_diameter_nominals[variable]
         elif variable in self._pipe_heat_loss_nominals:
             return self._pipe_heat_loss_nominals[variable]
-        elif variable in self.__pipe_topo_cost_nominals:
-            return self.__pipe_topo_cost_nominals[variable]
+        elif variable in self.__heat_pipe_topo_cost_nominals:
+            return self.__heat_pipe_topo_cost_nominals[variable]
         elif variable in self.__asset_max_size_nominals:
             return self.__asset_max_size_nominals[variable]
-        elif variable in self.__pipe_topo_max_discharge_nominals:
-            return self.__pipe_topo_max_discharge_nominals[variable]
+        elif variable in self.__heat_pipe_topo_max_discharge_nominals:
+            return self.__heat_pipe_topo_max_discharge_nominals[variable]
         elif variable in self.__gas_pipe_topo_diameter_nominals:
             return self.__gas_pipe_topo_diameter_nominals[variable]
         elif variable in self.__gas_pipe_topo_cost_nominals:
             return self.__gas_pipe_topo_cost_nominals[variable]
         elif variable in self.__gas_pipe_topo_max_discharge_nominals:
             return self.__gas_pipe_topo_max_discharge_nominals[variable]
         elif variable in self.__electricity_cable_topo_resistance_nominals:
@@ -1116,31 +1139,31 @@
 
     def bounds(self):
         """
         In this function we add the bounds to the problem for all the variables defined/added in
         the HeatMixin.
         """
         bounds = super().bounds()
-        bounds.update(self.__pipe_topo_pipe_class_var_bounds)
-        bounds.update(self.__pipe_topo_diameter_var_bounds)
-        bounds.update(self.__pipe_topo_cost_var_bounds)
+        bounds.update(self.__heat_pipe_topo_pipe_class_var_bounds)
+        bounds.update(self.__heat_pipe_topo_diameter_var_bounds)
+        bounds.update(self.__heat_pipe_topo_cost_var_bounds)
         bounds.update(self._pipe_heat_loss_var_bounds)
-        bounds.update(self.__pipe_topo_heat_discharge_bounds)
+        bounds.update(self.__heat_pipe_topo_heat_discharge_bounds)
         bounds.update(self.__gas_pipe_topo_pipe_class_var_bounds)
         bounds.update(self.__gas_pipe_topo_diameter_var_bounds)
         bounds.update(self.__gas_pipe_topo_cost_var_bounds)
         bounds.update(self.__asset_max_size_bounds)
         bounds.update(self.__asset_aggregation_count_var_bounds)
-        bounds.update(self.__pipe_topo_max_discharge_var_bounds)
+        bounds.update(self.__heat_pipe_topo_max_discharge_var_bounds)
         bounds.update(self.__gas_pipe_topo_max_discharge_var_bounds)
-        bounds.update(self.__pipe_topo_global_pipe_class_count_var_bounds)
+        bounds.update(self.__heat_pipe_topo_global_pipe_class_count_var_bounds)
         bounds.update(self.__gas_pipe_topo_global_pipe_class_count_var_bounds)
-        bounds.update(self.__pipe_topo_pipe_class_discharge_ordering_var_bounds)
-        bounds.update(self.__pipe_topo_pipe_class_cost_ordering_var_bounds)
-        bounds.update(self.__pipe_topo_pipe_class_heat_loss_ordering_var_bounds)
+        bounds.update(self.__heat_pipe_topo_pipe_class_discharge_ordering_var_bounds)
+        bounds.update(self.__heat_pipe_topo_pipe_class_cost_ordering_var_bounds)
+        bounds.update(self.__heat_pipe_topo_pipe_class_heat_loss_ordering_var_bounds)
         bounds.update(self.__gas_pipe_topo_pipe_class_discharge_ordering_var_bounds)
         bounds.update(self.__gas_pipe_topo_pipe_class_cost_ordering_var_bounds)
         bounds.update(self.__electricity_cable_topo_max_current_var_bounds)
         bounds.update(self.__electricity_cable_topo_resistance_var_bounds)
         bounds.update(self.__electricity_cable_topo_cost_var_bounds)
         bounds.update(self.__electricity_cable_topo_cable_class_var_bounds)
         bounds.update(self.__electricity_cable_topo_cable_class_current_ordering_var_bounds)
@@ -1155,18 +1178,18 @@
         """
         parameters = super().parameters(ensemble_member)
 
         # To avoid mistakes by accidentally using the `diameter`, `area` and `Heat_loss`
         # parameters in e.g. constraints when those are variable, we set them
         # to NaN in that case. In post(), they are set to their resulting
         # values once again.
-        if self.__pipe_topo_diameter_area_parameters:
-            parameters.update(self.__pipe_topo_diameter_area_parameters[ensemble_member])
-        if self.__pipe_topo_heat_loss_parameters:
-            parameters.update(self.__pipe_topo_heat_loss_parameters[ensemble_member])
+        if self.__heat_pipe_topo_diameter_area_parameters:
+            parameters.update(self.__heat_pipe_topo_diameter_area_parameters[ensemble_member])
+        if self.__heat_pipe_topo_heat_loss_parameters:
+            parameters.update(self.__heat_pipe_topo_heat_loss_parameters[ensemble_member])
 
         return parameters
 
     def __get_maximum_total_head_loss(self):
         """
         Get an upper bound on the maximum total head loss that can be used in
         big-M formulations of e.g. check valves and disconnectable pipes.
@@ -1190,15 +1213,15 @@
         for ensemble_member in range(self.ensemble_size):
             parameters = self.parameters(ensemble_member)
 
             head_loss = 0.0
             # TODO: asset sizing is currently hard coded to use only the milp network settings
             for pipe in components.get("heat_pipe", []):
                 try:
-                    pipe_classes = self._pipe_topo_pipe_class_map[pipe].keys()
+                    pipe_classes = self._heat_pipe_topo_pipe_class_map[pipe].keys()
                     head_loss += max(
                         self._hn_head_loss_class._hn_pipe_head_loss(
                             pipe,
                             self,
                             options,
                             self.heat_network_settings,
                             parameters,
@@ -1257,37 +1280,37 @@
 
         # These are the constraints to count the amount of a certain pipe class
         unique_pipe_classes = self.get_unique_pipe_classes()
         pipe_class_count_sum = {pc.name: 0 for pc in unique_pipe_classes}
 
         for p in self.energy_system_components.get("heat_pipe", []):
             try:
-                pipe_classes = self._pipe_topo_pipe_class_map[p]
+                pipe_classes = self._heat_pipe_topo_pipe_class_map[p]
             except KeyError:
                 pass
             else:
                 for pc in pipe_classes:
                     neighbour = self.has_related_pipe(p)
                     if neighbour and p not in self.hot_pipes:
                         var_name = f"{self.cold_to_hot_pipe(p)}__hn_pipe_class_{pc.name}"
                     else:
                         var_name = f"{p}__hn_pipe_class_{pc.name}"
                     pipe_class_count_sum[pc.name] += self.extra_variable(var_name, ensemble_member)
 
         for pc in unique_pipe_classes:
             var = self.extra_variable(
-                self.__pipe_topo_global_pipe_class_count_map[pc.name], ensemble_member
+                self.__heat_pipe_topo_global_pipe_class_count_map[pc.name], ensemble_member
             )
             constraints.append(((pipe_class_count_sum[pc.name] - var), 0.0, 0.0))
 
         # These are the constraints to order the discharge capabilities of the pipe classes
-        for p, pipe_classes in self.__pipe_topo_pipe_class_discharge_ordering_map.items():
-            max_discharge = self.extra_variable(self._pipe_topo_max_discharge_map[p])
+        for p, pipe_classes in self.__heat_pipe_topo_pipe_class_discharge_ordering_map.items():
+            max_discharge = self.extra_variable(self._heat_pipe_topo_max_discharge_map[p])
             max_discharges = {
-                pc.name: pc.maximum_discharge for pc in self._pipe_topo_pipe_class_map[p]
+                pc.name: pc.maximum_discharge for pc in self._heat_pipe_topo_pipe_class_map[p]
             }
             median_discharge = np.median(list(max_discharges.values()))
 
             big_m = 2.0 * max(max_discharges.values())
             for pc, var_name in pipe_classes.items():
                 pipe_class_discharge_ordering = self.extra_variable(var_name, ensemble_member)
 
@@ -1313,18 +1336,18 @@
                         / median_discharge,
                         -np.inf,
                         0.0,
                     )
                 )
 
         # These are the constraints to order the costs of the pipe classes
-        for p, pipe_classes in self.__pipe_topo_pipe_class_cost_ordering_map.items():
-            cost_sym_name = self._pipe_topo_cost_map[p]
+        for p, pipe_classes in self.__heat_pipe_topo_pipe_class_cost_ordering_map.items():
+            cost_sym_name = self._heat_pipe_topo_cost_map[p]
             cost_sym = self.extra_variable(cost_sym_name, ensemble_member)
-            costs = {pc.name: pc.investment_costs for pc in self._pipe_topo_pipe_class_map[p]}
+            costs = {pc.name: pc.investment_costs for pc in self._heat_pipe_topo_pipe_class_map[p]}
 
             big_m = 2.0 * max(costs.values())
             for pc, var_name in pipe_classes.items():
                 pipe_class_cost_ordering = self.extra_variable(var_name, ensemble_member)
 
                 # should be one if >= than cost_symbol
                 constraints.append(
@@ -1342,15 +1365,18 @@
                         -np.inf,
                         0.0,
                     )
                 )
 
         # These are the constraints to order the milp loss of the pipe classes.
         if not self.energy_system_options()["neglect_pipe_heat_losses"]:
-            for pipe, pipe_classes in self.__pipe_topo_pipe_class_heat_loss_ordering_map.items():
+            for (
+                pipe,
+                pipe_classes,
+            ) in self.__heat_pipe_topo_pipe_class_heat_loss_ordering_map.items():
                 if pipe in self.hot_pipes and self.has_related_pipe(pipe):
                     heat_loss_sym_name = self._pipe_heat_loss_map[pipe]
                     heat_loss_sym = self.extra_variable(heat_loss_sym_name, ensemble_member)
                     cold_name = self._pipe_heat_loss_map[self.hot_to_cold_pipe(pipe)]
                     heat_loss_sym += self.extra_variable(cold_name, ensemble_member)
                     heat_losses = [
                         h1 + h2
@@ -1389,52 +1415,52 @@
                             )
                             / self.variable_nominal(heat_loss_sym_name),
                             -np.inf,
                             0.0,
                         )
                     )
 
-        for p, pipe_classes in self._pipe_topo_pipe_class_map.items():
+        for p, pipe_classes in self._heat_pipe_topo_pipe_class_map.items():
             variables = {
                 pc.name: self.extra_variable(var_name, ensemble_member)
                 for pc, var_name in pipe_classes.items()
             }
 
             # Make sure exactly one indicator is true
             constraints.append((sum(variables.values()), 1.0, 1.0))
 
             # set the max discharge
-            max_discharge = self.extra_variable(self._pipe_topo_max_discharge_map[p])
+            max_discharge = self.extra_variable(self._heat_pipe_topo_max_discharge_map[p])
             max_discharges = {pc.name: pc.maximum_discharge for pc in pipe_classes}
             max_discharge_expr = sum(
                 variables[pc_name] * max_discharges[pc_name] for pc_name in variables
             )
 
             constraints.append(
                 (
                     (max_discharge - max_discharge_expr)
-                    / self.variable_nominal(self._pipe_topo_max_discharge_map[p]),
+                    / self.variable_nominal(self._heat_pipe_topo_max_discharge_map[p]),
                     0.0,
                     0.0,
                 )
             )
 
             # Match the indicators to the diameter symbol
-            diam_sym_name = self._pipe_topo_diameter_map[p]
+            diam_sym_name = self._heat_pipe_topo_diameter_map[p]
             diam_sym = self.extra_variable(diam_sym_name, ensemble_member)
 
             diameters = {pc.name: pc.inner_diameter for pc in pipe_classes}
 
             diam_expr = sum(variables[pc_name] * diameters[pc_name] for pc_name in variables)
 
             constraint_nominal = self.variable_nominal(diam_sym_name)
             constraints.append(((diam_sym - diam_expr) / constraint_nominal, 0.0, 0.0))
 
             # match the indicators to the cost symbol
-            cost_sym_name = self._pipe_topo_cost_map[p]
+            cost_sym_name = self._heat_pipe_topo_cost_map[p]
             cost_sym = self.extra_variable(cost_sym_name, ensemble_member)
 
             investment_costs = {pc.name: pc.investment_costs for pc in pipe_classes}
 
             costs_expr = sum(
                 variables[pc_name] * investment_costs[pc_name] for pc_name in variables
             )
@@ -1735,15 +1761,17 @@
 
         # Clip discharge based on pipe class
         for p in self.energy_system_components.get("heat_pipe", []):
             # Match the indicators to the discharge symbol(s)
             discharge_sym = self.state(f"{p}.Q")
             nominal = self.variable_nominal(f"{p}.Q")
 
-            max_discharge = self.__pipe_topo_max_discharge_var[self._pipe_topo_max_discharge_map[p]]
+            max_discharge = self.__heat_pipe_topo_max_discharge_var[
+                self._heat_pipe_topo_max_discharge_map[p]
+            ]
 
             constraints.append(((max_discharge - discharge_sym) / nominal, 0.0, np.inf))
             constraints.append(((-max_discharge - discharge_sym) / nominal, -np.inf, 0.0))
 
         return constraints
 
     def __gas_pipe_topology_path_constraints(self, ensemble_member):
@@ -2161,46 +2189,46 @@
                 if not pipe_classes:
                     continue
                 elif len(pipe_classes) == 1:
                     pipe_class = pipe_classes[0]
                 else:
                     pipe_class = next(
                         c
-                        for c, s in self._pipe_topo_pipe_class_map[pipe].items()
+                        for c, s in self._heat_pipe_topo_pipe_class_map[pipe].items()
                         if round(results[s][0]) == 1.0
                     )
 
                 for p in [pipe, self.hot_to_cold_pipe(pipe)]:
-                    self.__pipe_topo_pipe_class_result[p] = pipe_class
+                    self.__heat_pipe_topo_pipe_class_result[p] = pipe_class
 
     def _pipe_heat_loss_to_parameters(self):
         """
         This function is used to set the optimized milp losses in the parameters object.
         """
         options = self.energy_system_options()
 
         for ensemble_member in range(self.ensemble_size):
             parameters = self.parameters(ensemble_member)
 
-            h = self.__pipe_topo_heat_loss_parameters[ensemble_member]
+            h = self.__heat_pipe_topo_heat_loss_parameters[ensemble_member]
             for pipe in self._pipe_heat_losses:
                 pipe_class = self.get_optimized_pipe_class(pipe)
 
                 h[f"{pipe}.Heat_loss"] = pipe_heat_loss(
                     self, options, parameters, pipe, pipe_class.u_values
                 )
 
     def __pipe_diameter_to_parameters(self):
         """
         This function is used to update the parameters object with the results of the pipe class
         optimization
         """
         for ensemble_member in range(self.ensemble_size):
-            d = self.__pipe_topo_diameter_area_parameters[ensemble_member]
-            for pipe in self._pipe_topo_pipe_class_map:
+            d = self.__heat_pipe_topo_diameter_area_parameters[ensemble_member]
+            for pipe in self._heat_pipe_topo_pipe_class_map:
                 pipe_class = self.get_optimized_pipe_class(pipe)
 
                 for p in [pipe, self.hot_to_cold_pipe(pipe)]:
                     d[f"{p}.diameter"] = pipe_class.inner_diameter
                     d[f"{p}.area"] = pipe_class.area
 
     def priority_completed(self, priority):
```

### Comparing `mesido-0.1.1/src/mesido/base_component_type_mixin.py` & `mesido-0.1.2/src/mesido/base_component_type_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/component_type_mixin.py` & `mesido-0.1.2/src/mesido/component_type_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/control_variables.py` & `mesido-0.1.2/src/mesido/control_variables.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/demand_insulation_class.py` & `mesido-0.1.2/src/mesido/demand_insulation_class.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/electricity_physics_mixin.py` & `mesido-0.1.2/src/mesido/electricity_physics_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/_edr_pipes.json` & `mesido-0.1.2/src/mesido/esdl/_edr_pipes.json`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/_update_edr_pipes_json.py` & `mesido-0.1.2/src/mesido/esdl/_update_edr_pipes_json.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/asset_to_component_base.py` & `mesido-0.1.2/src/mesido/esdl/asset_to_component_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,28 +68,30 @@
         "DN900": "Steel-S1-DN-900",
         "DN1000": "Steel-S1-DN-1000",
         "DN1100": "Steel-S1-DN-1100",
         "DN1200": "Steel-S1-DN-1200",
     }
     # A map of the esdl assets to the asset types in pycml
     component_map = {
+        "Airco": "airco",
         "ATES": "ates",
         "Battery": "electricity_storage",
         "Bus": "electricity_node",
+        "ElectricBoiler": "elec_boiler",
         "ElectricityCable": "electricity_cable",
         "ElectricityDemand": "electricity_demand",
         "ElectricityProducer": "electricity_source",
         "Electrolyzer": "electrolyzer",
         "Compressor": "compressor",
         "GenericConsumer": "heat_demand",
         "CoolingDemand": "cold_demand",
         "HeatExchange": "heat_exchanger",
         "HeatingDemand": "heat_demand",
         "HeatPump": "heat_pump",
-        "GasHeater": "heat_source",
+        "GasHeater": "gas_boiler",
         "GasProducer": "gas_source",
         "GasDemand": "gas_demand",
         "GasConversion": "gas_substation",
         "GasStorage": "gas_tank_storage",
         "GenericProducer": "heat_source",
         "GeothermalSource": "heat_source",
         "Losses": "heat_demand",
@@ -407,16 +409,23 @@
                 self._set_electricity_current_nominal_and_max(asset, i_max, i_nom)
                 return i_max, i_nom
             else:
                 raise _RetryLaterException(
                     f"Could not determine max and nominal current for {asset.asset_type}"
                     " '{asset.name}'"
                 )
-        elif asset.out_ports is None or asset.asset_type == "Electrolyzer":
-            connected_port = asset.in_ports[0].connectedTo[0]
+        elif (
+            asset.out_ports is None
+            or asset.asset_type == "Electrolyzer"
+            or asset.asset_type == "ElectricBoiler"
+            or asset.asset_type == "HeatPump"
+        ):
+            for port in asset.in_ports:
+                if isinstance(port.carrier, esdl.ElectricityCommodity):
+                    connected_port = port.connectedTo[0]
             i_max = self._port_to_i_max.get(connected_port, None)
             i_nom = self._port_to_i_nominal.get(connected_port, None)
             if i_max is not None:
                 self._set_electricity_current_nominal_and_max(asset, i_max, i_nom)
                 return i_max, i_nom
             else:
                 raise _RetryLaterException(
@@ -500,14 +509,44 @@
             if q_nominal is not None:
                 self._set_q_nominal(asset, q_nominal)
                 return q_nominal
             else:
                 raise _RetryLaterException(
                     f"Could not determine nominal discharge for {asset.asset_type} '{asset.name}'"
                 )
+        elif len(asset.in_ports) == 2 and len(asset.out_ports) == 1:  # for gas_boiler or e_boiler
+            q_nominals = {}
+            try:
+                for port in asset.in_ports:
+                    connected_port = asset.in_ports[0].connectedTo[0]
+                    if isinstance(port.carrier, esdl.GasCommodity):
+                        q_nominals["Q_nominal_gas"] = self._port_to_q_nominal[connected_port]
+                        self._port_to_q_nominal[port] = q_nominals["Q_nominal_gas"]
+                    elif isinstance(port.carrier, esdl.HeatCommodity):
+                        q_nominals["Q_nominal"] = self._port_to_q_nominal[connected_port]
+                        self._port_to_q_nominal[port] = q_nominals["Q_nominal"]
+                    else:
+                        logger.error(
+                            f"{asset.name} should have at least gas or heat specified on"
+                            f"one of the in ports"
+                        )
+            except KeyError:
+                if isinstance(asset.out_ports[0].carrier, esdl.GasCommodity):
+                    connected_port = asset.out_ports[0].connectedTo[0]
+                    q_nominals["Q_nominal"] = self._port_to_q_nominal.get(connected_port, None)
+                else:
+                    logger.error(f"{asset.name} should have a heat carrier on out port")
+
+            if q_nominals["Q_nominal"] is not None:
+                self._port_to_q_nominal[asset.out_ports[0]] = q_nominals["Q_nominal"]
+                return q_nominals
+            else:
+                raise _RetryLaterException(
+                    f"Could not determine nominal discharge for {asset.asset_type} '{asset.name}'"
+                )
         elif len(asset.in_ports) >= 2 and len(asset.out_ports) == 2:
             q_nominals = {}
             for p in asset.in_ports:
                 if isinstance(p.carrier, esdl.HeatCommodity):
                     out_port = None
                     for p2 in asset.out_ports:
                         if p2.carrier.name.replace("_ret", "") == p.carrier.name.replace(
@@ -606,17 +645,19 @@
         asset : The asset object to retrieve port and carrier information from
 
         Returns
         -------
         Tuple with the supply and return temperature.
         """
 
-        assert len(asset.in_ports) == 1 and len(asset.out_ports) == 1
+        assert len(asset.in_ports) <= 2 and len(asset.out_ports) == 1
 
-        in_carrier = asset.global_properties["carriers"][asset.in_ports[0].carrier.id]
+        for port in asset.in_ports:
+            if isinstance(port.carrier, esdl.HeatCommodity):
+                in_carrier = asset.global_properties["carriers"][port.carrier.id]
         out_carrier = asset.global_properties["carriers"][asset.out_ports[0].carrier.id]
 
         if in_carrier["id"] == out_carrier["id"]:
             # these are the pipes, nodes, valves, pumps
             modifiers = {
                 "temperature": in_carrier["temperature"],
                 "carrier_id": in_carrier["id_number_mapping"],
@@ -663,15 +704,15 @@
         asset : Asset object to retrieve carrier temperatures from.
 
         Returns
         -------
         dict with all the temperatures.
         """
 
-        if len(asset.in_ports) == 1 and len(asset.out_ports) == 1:
+        if len(asset.in_ports) <= 2 and len(asset.out_ports) == 1:
             modifiers = self._get_supply_return_temperatures(asset)
             return modifiers
         elif len(asset.in_ports) >= 2 and len(asset.out_ports) == 2:
             prim_return_temperature = None
             sec_return_temperature = None
             for p in asset.in_ports:
                 if isinstance(p.carrier, esdl.HeatCommodity):
```

### Comparing `mesido-0.1.1/src/mesido/esdl/common.py` & `mesido-0.1.2/src/mesido/esdl/common.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/edr_pipe_class.py` & `mesido-0.1.2/src/mesido/esdl/edr_pipe_class.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/esdl_additional_vars_mixin.py` & `mesido-0.1.2/src/mesido/esdl/esdl_additional_vars_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/esdl_heat_model.py` & `mesido-0.1.2/src/mesido/esdl/esdl_heat_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 from mesido.esdl.asset_to_component_base import MODIFIERS, _AssetToComponentBase
 from mesido.esdl.common import Asset
 from mesido.esdl.esdl_model_base import _ESDLModelBase
 from mesido.network_common import NetworkSettings
 from mesido.pycml.component_library.milp import (
     ATES,
     AirWaterHeatPump,
+    AirWaterHeatPumpElec,
+    Airco,
     CheckValve,
     ColdDemand,
     Compressor,
     ControlValve,
+    ElecBoiler,
     ElectricityCable,
     ElectricityDemand,
     ElectricityNode,
     ElectricitySource,
     ElectricityStorage,
     Electrolyzer,
+    GasBoiler,
     GasDemand,
     GasNode,
     GasPipe,
     GasSource,
     GasSubstation,
     GasTankStorage,
     GeothermalSource,
@@ -91,14 +95,44 @@
 
         Returns
         -------
         rho and cp
         """
         return dict(rho=self.rho, cp=self.cp)
 
+    def get_internal_energy(self, asset_name, carrier):
+        # The default of 20°C is also used in the head_loss_class. Thus, when updating ensure it
+        # is also updated in the head_loss_class.
+        temperature = 20.0
+
+        if NetworkSettings.NETWORK_TYPE_GAS in carrier.name:
+            internal_energy = cP.CoolProp.PropsSI(
+                "U",
+                "T",
+                273.15 + temperature,
+                "P",
+                carrier.pressure * 1.0e5,
+                NetworkSettings.NETWORK_COMPOSITION_GAS,
+            )
+        elif NetworkSettings.NETWORK_TYPE_HYDROGEN in carrier.name:
+            internal_energy = cP.CoolProp.PropsSI(
+                "U",
+                "T",
+                273.15 + temperature,
+                "P",
+                carrier.pressure * 1.0e5,
+                str(NetworkSettings.NETWORK_TYPE_HYDROGEN).upper(),
+            )
+        else:
+            logger.warning(
+                f"Neither gas or hydrogen was used in the carrier " f"name of pipe {asset_name}"
+            )
+            internal_energy = 46.0e6  # natural gas at about 8 bar
+        return internal_energy  # we use gram per second and coolprop gives results in kJ per kg
+
     def get_density(self, asset_name, carrier):
         # TODO: gas carrier temperature still needs to be resolved.
         # The default of 20°C is also used in the head_loss_class. Thus, when updating ensure it
         # is also updated in the head_loss_class.
         temperature = 20.0
 
         if NetworkSettings.NETWORK_TYPE_GAS in carrier.name:
@@ -347,14 +381,52 @@
             **self._supply_return_temperature_modifiers(asset),
             **self._rho_cp_modifiers,
             **self._get_cost_figure_modifiers(asset),
         )
 
         return HeatDemand, modifiers
 
+    def convert_airco(self, asset: Asset) -> Tuple[Type[Airco], MODIFIERS]:
+        """
+        This function converts the airco object in esdl to a set of modifiers that can be used in
+        a pycml object. Most important:
+
+        - Setting a cap on the thermal power.
+        - Setting the state (enabled, disabled, optional)
+        - Setting the relevant temperatures.
+        - Setting the relevant cost figures.
+
+        Parameters
+        ----------
+        asset : The asset object with its properties.
+
+        Returns
+        -------
+        Demand class with modifiers
+        """
+        assert asset.asset_type in {"Airco"}
+
+        max_ = asset.attributes["power"] if asset.attributes["power"] else math.inf
+
+        q_nominal = self._get_connected_q_nominal(asset)
+
+        modifiers = dict(
+            Q_nominal=q_nominal,
+            Heat_airco=dict(max=max_, nominal=max_ / 2.0),
+            Heat_flow=dict(max=max_, nominal=max_ / 2.0),
+            HeatIn=dict(Hydraulic_power=dict(nominal=q_nominal * 16.0e5)),
+            HeatOut=dict(Hydraulic_power=dict(nominal=q_nominal * 16.0e5)),
+            state=self.get_state(asset),
+            **self._supply_return_temperature_modifiers(asset),
+            **self._rho_cp_modifiers,
+            **self._get_cost_figure_modifiers(asset),
+        )
+
+        return Airco, modifiers
+
     def convert_cold_demand(self, asset: Asset) -> Tuple[Type[ColdDemand], MODIFIERS]:
         """
         This function converts the demand object in esdl to a set of modifiers that can be used in
         a pycml object. Most important:
         - Setting a cap on the thermal power.
         - Setting the state (enabled, disabled, optional)
         - Setting the relevant temperatures.
@@ -481,14 +553,15 @@
             pressure = asset.in_ports[0].carrier.pressure * 1.0e5
             density = self.get_density(asset.name, asset.in_ports[0].carrier)
             bounds_nominals = dict(
                 Q=dict(min=-q_max, max=q_max, nominal=q_nominal),
                 mass_flow=dict(
                     min=-q_max * density, max=q_max * density, nominal=q_nominal * density
                 ),
+                Hydraulic_power=dict(nominal=q_nominal * pressure),
             )
             modifiers = dict(
                 length=length,
                 density=density,
                 diameter=diameter,
                 pressure=pressure,
                 # disconnectable=self._is_disconnectable_pipe(asset),  # still to be added
@@ -727,15 +800,15 @@
             **self._get_cost_figure_modifiers(asset),
             **params,
         )
         return HeatExchanger, modifiers
 
     def convert_heat_pump(
         self, asset: Asset
-    ) -> Tuple[Union[Type[HeatPump], Type[HeatSource]], MODIFIERS]:
+    ) -> Tuple[Union[Type[HeatPump], Type[HeatSource], Type[AirWaterHeatPumpElec]], MODIFIERS]:
         """
         This function converts the HeatPump object in esdl to a set of modifiers that can be used in
         a pycml object. Most important:
 
         - Setting the COP of the heatpump
         - Setting the cap on the electrical power.
         - Setting a caps on the thermal power on both the primary and secondary side.
@@ -755,14 +828,18 @@
             "HeatPump",
         }
 
         # In this case we only have the secondary side ports, here we assume a air-water HP
         if len(asset.in_ports) == 1 and len(asset.out_ports) == 1:
             _, modifiers = self.convert_heat_source(asset)
             return AirWaterHeatPump, modifiers
+        # In this case we only have the secondary side ports, here we assume a air-water HP elec
+        if len(asset.in_ports) == 2 and len(asset.out_ports) == 1:
+            _, modifiers = self.convert_air_water_heat_pump_elec(asset)
+            return AirWaterHeatPumpElec, modifiers
 
         if not asset.attributes["power"]:
             raise _ESDLInputException(f"{asset.name} has no power specified")
         else:
             power_electrical = asset.attributes["power"]
 
         if not asset.attributes["COP"]:
@@ -849,18 +926,15 @@
 
         if not max_supply:
             logger.error(f"{asset.asset_type} '{asset.name}' has no max power specified. ")
         assert max_supply > 0.0
 
         # get price per unit of energy,
         # assume cost of 1. if nothing is given (effectively milp loss minimization)
-
-        co2_coefficient = 1.0
-        if hasattr(asset.attributes["KPIs"], "kpi"):
-            co2_coefficient = asset.attributes["KPIs"].kpi.items[0].value
+        # TODO: Use an attribute or use and KPI for CO2 coefficient of a source
 
         q_nominal = self._get_connected_q_nominal(asset)
 
         modifiers = dict(
             technical_life=self.get_asset_attribute_value(
                 asset,
                 "technicalLifetime",
@@ -869,15 +943,14 @@
                 max_value=50.0,
             ),
             discount_rate=self.get_asset_attribute_value(
                 asset, "discountRate", default_value=0.0, min_value=0.0, max_value=100.0
             ),
             Q_nominal=q_nominal,
             state=self.get_state(asset),
-            co2_coeff=co2_coefficient,
             Heat_source=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
             Heat_flow=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
             HeatIn=dict(Hydraulic_power=dict(nominal=q_nominal * 16.0e5)),
             HeatOut=dict(Hydraulic_power=dict(nominal=q_nominal * 16.0e5)),
             **self._supply_return_temperature_modifiers(asset),
             **self._rho_cp_modifiers,
             **self._get_cost_figure_modifiers(asset),
@@ -1365,14 +1438,15 @@
 
         id_mapping = asset.global_properties["carriers"][asset.in_ports[0].carrier.id][
             "id_number_mapping"
         ]
         # DO not remove due usage in future
         # hydrogen_specfic_energy = 20.0 / 1.0e6
         density = self.get_density(asset.name, asset.in_ports[0].carrier)
+        pressure = asset.in_ports[0].carrier.pressure * 1.0e5
         q_nominal = self._get_connected_q_nominal(asset)
 
         modifiers = dict(
             Q_nominal=q_nominal,
             id_mapping_carrier=id_mapping,
             # Gas_demand_mass_flow=dict(min=0., max=asset.attributes["power"]
             # *hydrogen_specfic_energy),
@@ -1380,14 +1454,15 @@
             GasIn=dict(
                 Q=dict(
                     min=0.0,
                     max=self._get_connected_q_max(asset),
                     nominal=self._get_connected_q_nominal(asset),
                 ),
                 mass_flow=dict(nominal=density * q_nominal),
+                Hydraulic_power=dict(min=0.0, max=0.0, nominal=q_nominal * pressure),
             ),
             **self._get_cost_figure_modifiers(asset),
         )
 
         return GasDemand, modifiers
 
     def convert_gas_source(self, asset: Asset) -> Tuple[Type[GasSource], MODIFIERS]:
@@ -1405,28 +1480,30 @@
         -------
         GasDemand class with modifiers
         """
         assert asset.asset_type in {"GasProducer"}
 
         q_nominal = self._get_connected_q_nominal(asset)
         density_value = self.get_density(asset.name, asset.out_ports[0].carrier)
+        pressure = asset.out_ports[0].carrier.pressure * 1.0e5
 
         bounds_nominals_mass_flow = dict(
             min=0.0,
             max=self._get_connected_q_max(asset) * density_value,
             nominal=q_nominal * density_value,
         )
 
         modifiers = dict(
             Q_nominal=q_nominal,
             density=density_value,
             Gas_source_mass_flow=bounds_nominals_mass_flow,
             GasOut=dict(
                 Q=dict(nominal=q_nominal),
                 mass_flow=bounds_nominals_mass_flow,
+                Hydraulic_power=dict(nominal=q_nominal * pressure),
             ),
             **self._get_cost_figure_modifiers(asset),
         )
 
         return GasSource, modifiers
 
     def convert_electrolyzer(self, asset: Asset) -> Tuple[Type[Electrolyzer], MODIFIERS]:
@@ -1511,28 +1588,33 @@
         """
         assert asset.asset_type in {"GasStorage"}
 
         # DO not remove due usage in future
         # hydrogen_specific_energy = 20.0 / 1.0e6  # kg/Wh
         q_nominal = self._get_connected_q_nominal(asset)
         density = self.get_density(asset.name, asset.in_ports[0].carrier)
+        pressure = asset.in_ports[0].carrier.pressure * 1.0e5
 
         modifiers = dict(
             Q_nominal=q_nominal,
             density=density,
             volume=asset.attributes["workingVolume"],
             # Gas_tank_flow=dict(min=-hydrogen_specific_energy*asset.attributes["maxDischargeRate"],
             # max=hydrogen_specific_energy*asset.attributes["maxChargeRate"]),
             # TODO: Fix -> Gas network is currenlty non-limiting, mass flow is decoupled from the
             # volumetric flow
             # Gas_tank_flow=dict(
             #     min=-self._get_connected_q_max(asset), max=self._get_connected_q_max(asset),
             #     nominal=self._get_connected_q_nominal(asset),
             # )
-            GasIn=dict(Q=dict(nominal=q_nominal), mass_flow=dict(nominal=q_nominal * density)),
+            GasIn=dict(
+                Q=dict(nominal=q_nominal),
+                mass_flow=dict(nominal=q_nominal * density),
+                Hydraulic_power=dict(nominal=q_nominal * pressure),
+            ),
             **self._get_cost_figure_modifiers(asset),
         )
 
         return GasTankStorage, modifiers
 
     def convert_gas_substation(self, asset: Asset) -> Tuple[Type[GasSubstation], MODIFIERS]:
         """
@@ -1548,24 +1630,34 @@
         GasTankStorage class with modifiers
         """
         assert asset.asset_type in {"GasConversion", "PressureReducingValve"}
 
         q_nom_in, q_nom_out = self._get_connected_q_nominal(asset)
         density_in = self.get_density(asset.name, asset.in_ports[0].carrier)
         density_out = self.get_density(asset.name, asset.out_ports[0].carrier)
+        pressure_in = asset.in_ports[0].carrier.pressure * 1.0e5
+        pressure_out = asset.out_ports[0].carrier.pressure * 1.0e5
 
         assert density_in >= density_out
 
         modifiers = dict(
             Q_nominal_in=q_nom_in,
             Q_nominal_out=q_nom_out,
             density_in=density_in,
             density_out=density_out,
-            GasIn=dict(Q=dict(nominal=q_nom_in), mass_flow=dict(nominal=q_nom_in * density_in)),
-            GasOut=dict(Q=dict(nominal=q_nom_out), mass_flow=dict(nominal=q_nom_out * density_out)),
+            GasIn=dict(
+                Q=dict(nominal=q_nom_in),
+                mass_flow=dict(nominal=q_nom_in * density_in),
+                Hydraulic_power=dict(nominal=q_nom_in * pressure_in),
+            ),
+            GasOut=dict(
+                Q=dict(nominal=q_nom_out),
+                mass_flow=dict(nominal=q_nom_out * density_out),
+                Hydraulic_power=dict(nominal=q_nom_out * pressure_out),
+            ),
             **self._get_cost_figure_modifiers(asset),
         )
 
         return GasSubstation, modifiers
 
     def convert_compressor(self, asset: Asset) -> Tuple[Type[Compressor], MODIFIERS]:
         """
@@ -1574,36 +1666,252 @@
 
         Parameters
         ----------
         asset : The asset object with its properties.
 
         Returns
         -------
-        GasTankStorage class with modifiers
+        Compressor class with modifiers
         """
         assert asset.asset_type in {"Compressor"}
 
         q_nom_in, q_nom_out = self._get_connected_q_nominal(asset)
         density_in = self.get_density(asset.name, asset.in_ports[0].carrier)
         density_out = self.get_density(asset.name, asset.out_ports[0].carrier)
+        pressure_in = asset.in_ports[0].carrier.pressure * 1.0e5
+        pressure_out = asset.out_ports[0].carrier.pressure * 1.0e5
 
         assert density_out >= density_in
 
         modifiers = dict(
             Q_nominal_in=q_nom_in,
             Q_nominal_out=q_nom_out,
             density_in=density_in,
             density_out=density_out,
-            GasIn=dict(Q=dict(nominal=q_nom_in), mass_flow=dict(nominal=q_nom_in * density_in)),
-            GasOut=dict(Q=dict(nominal=q_nom_out), mass_flow=dict(nominal=q_nom_out * density_out)),
+            GasIn=dict(
+                Q=dict(nominal=q_nom_in),
+                mass_flow=dict(nominal=q_nom_in * density_in),
+                Hydraulic_power=dict(nominal=q_nom_in * pressure_in),
+            ),
+            GasOut=dict(
+                Q=dict(nominal=q_nom_out),
+                mass_flow=dict(nominal=q_nom_out * density_out),
+                Hydraulic_power=dict(nominal=q_nom_out * pressure_out),
+            ),
             **self._get_cost_figure_modifiers(asset),
         )
 
         return Compressor, modifiers
 
+    def convert_gas_boiler(self, asset: Asset) -> Tuple[GasBoiler, MODIFIERS]:
+        """
+        This function converts the GasHeater object in esdl to a set of modifiers that can be
+        used in a pycml object.
+
+        Parameters
+        ----------
+        asset : The asset object with its properties.
+
+        Returns
+        -------
+        GasBoiler class with modifiers
+        """
+        assert asset.asset_type in {"GasHeater"}
+
+        max_supply = asset.attributes["power"]
+
+        if not max_supply:
+            logger.error(f"{asset.asset_type} '{asset.name}' has no max power specified. ")
+        assert max_supply > 0.0
+
+        if len(asset.in_ports) == 1:
+            heat_source_object, modifiers = self.convert_heat_source(asset)
+            return heat_source_object, modifiers
+
+        id_mapping = asset.global_properties["carriers"][asset.in_ports[0].carrier.id][
+            "id_number_mapping"
+        ]
+
+        for port in asset.in_ports:
+            if isinstance(port.carrier, esdl.GasCommodity):
+                density = self.get_density(asset.name, port.carrier)
+                internal_energy = self.get_internal_energy(asset.name, port.carrier)
+
+        # TODO: CO2 coefficient
+
+        q_nominals = self._get_connected_q_nominal(asset)
+
+        modifiers = dict(
+            technical_life=self.get_asset_attribute_value(
+                asset,
+                "technicalLifetime",
+                default_value=30.0,
+                min_value=1.0,
+                max_value=50.0,
+            ),
+            discount_rate=self.get_asset_attribute_value(
+                asset, "discountRate", default_value=0.0, min_value=0.0, max_value=100.0
+            ),
+            state=self.get_state(asset),
+            Heat_source=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
+            Heat_flow=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
+            HeatIn=dict(Hydraulic_power=dict(nominal=q_nominals["Q_nominal"] * 16.0e5)),
+            HeatOut=dict(Hydraulic_power=dict(nominal=q_nominals["Q_nominal"] * 16.0e5)),
+            id_mapping_carrier=id_mapping,
+            density=density,
+            internal_energy=internal_energy,
+            GasIn=dict(Q=dict(min=0.0, nominal=q_nominals["Q_nominal_gas"])),
+            **q_nominals,
+            **self._supply_return_temperature_modifiers(asset),
+            **self._rho_cp_modifiers,
+            **self._get_cost_figure_modifiers(asset),
+        )
+
+        return GasBoiler, modifiers
+
+    def convert_elec_boiler(self, asset: Asset) -> Tuple[ElecBoiler, MODIFIERS]:
+        """
+        This function converts the ElectricBoiler object in esdl to a set of modifiers that can be
+        used in a pycml object.
+
+        Parameters
+        ----------
+        asset : The asset object with its properties.
+
+        Returns
+        -------
+        GasBoiler class with modifiers
+        """
+        assert asset.asset_type in {"ElectricBoiler"}
+
+        max_supply = asset.attributes["power"]
+
+        if not max_supply:
+            logger.error(f"{asset.asset_type} '{asset.name}' has no max power specified. ")
+        assert max_supply > 0.0
+
+        if len(asset.in_ports) == 1:
+            heat_source_object, modifiers = self.convert_heat_source(asset)
+            return heat_source_object, modifiers
+
+        id_mapping = asset.global_properties["carriers"][asset.in_ports[0].carrier.id][
+            "id_number_mapping"
+        ]
+
+        # TODO: CO2 coefficient
+
+        q_nominal = self._get_connected_q_nominal(asset)
+        for port in asset.in_ports:
+            if isinstance(port.carrier, esdl.ElectricityCommodity):
+                min_voltage = port.carrier.voltage
+        i_max, i_nom = self._get_connected_i_nominal_and_max(asset)
+        eff = asset.attributes["efficiency"] if asset.attributes["efficiency"] else 1.0
+
+        modifiers = dict(
+            technical_life=self.get_asset_attribute_value(
+                asset,
+                "technicalLifetime",
+                default_value=30.0,
+                min_value=1.0,
+                max_value=50.0,
+            ),
+            discount_rate=self.get_asset_attribute_value(
+                asset, "discountRate", default_value=0.0, min_value=0.0, max_value=100.0
+            ),
+            state=self.get_state(asset),
+            Heat_source=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
+            Heat_flow=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
+            HeatIn=dict(Hydraulic_power=dict(nominal=q_nominal["Q_nominal"] * 16.0e5)),
+            HeatOut=dict(Hydraulic_power=dict(nominal=q_nominal["Q_nominal"] * 16.0e5)),
+            id_mapping_carrier=id_mapping,
+            ElectricityIn=dict(
+                Power=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
+                I=dict(min=0.0, max=i_max, nominal=i_nom),
+                V=dict(min=min_voltage, nominal=min_voltage),
+            ),
+            min_voltage=min_voltage,
+            elec_power_nominal=max_supply,
+            efficiency=eff,
+            **q_nominal,
+            **self._supply_return_temperature_modifiers(asset),
+            **self._rho_cp_modifiers,
+            **self._get_cost_figure_modifiers(asset),
+        )
+
+        return ElecBoiler, modifiers
+
+    def convert_air_water_heat_pump_elec(
+        self, asset: Asset
+    ) -> Tuple[AirWaterHeatPumpElec, MODIFIERS]:
+        """
+        This function converts the ElectricBoiler object in esdl to a set of modifiers that can be
+        used in a pycml object.
+
+        Parameters
+        ----------
+        asset : The asset object with its properties.
+
+        Returns
+        -------
+        AirWaterHeatPumpElec class with modifiers
+        """
+        assert asset.asset_type in {"HeatPump"}
+
+        max_supply = asset.attributes["power"]
+
+        if not max_supply:
+            logger.error(f"{asset.asset_type} '{asset.name}' has no max power specified. ")
+        assert max_supply > 0.0
+
+        id_mapping = asset.global_properties["carriers"][asset.in_ports[0].carrier.id][
+            "id_number_mapping"
+        ]
+
+        # TODO: CO2 coefficient
+
+        q_nominal = self._get_connected_q_nominal(asset)
+        for port in asset.in_ports:
+            if isinstance(port.carrier, esdl.ElectricityCommodity):
+                min_voltage = port.carrier.voltage
+        i_max, i_nom = self._get_connected_i_nominal_and_max(asset)
+        cop = asset.attributes["COP"] if asset.attributes["COP"] else 1.0
+
+        modifiers = dict(
+            technical_life=self.get_asset_attribute_value(
+                asset,
+                "technicalLifetime",
+                default_value=30.0,
+                min_value=1.0,
+                max_value=50.0,
+            ),
+            discount_rate=self.get_asset_attribute_value(
+                asset, "discountRate", default_value=0.0, min_value=0.0, max_value=100.0
+            ),
+            state=self.get_state(asset),
+            Heat_source=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
+            Heat_flow=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
+            HeatIn=dict(Hydraulic_power=dict(nominal=q_nominal["Q_nominal"] * 16.0e5)),
+            HeatOut=dict(Hydraulic_power=dict(nominal=q_nominal["Q_nominal"] * 16.0e5)),
+            id_mapping_carrier=id_mapping,
+            ElectricityIn=dict(
+                Power=dict(min=0.0, max=max_supply, nominal=max_supply / 2.0),
+                I=dict(min=0.0, max=i_max, nominal=i_nom),
+                V=dict(min=min_voltage, nominal=min_voltage),
+            ),
+            min_voltage=min_voltage,
+            elec_power_nominal=max_supply,
+            cop=cop,
+            **q_nominal,
+            **self._supply_return_temperature_modifiers(asset),
+            **self._rho_cp_modifiers,
+            **self._get_cost_figure_modifiers(asset),
+        )
+
+        return AirWaterHeatPumpElec, modifiers
+
 
 class ESDLHeatModel(_ESDLModelBase):
     """
     This class is used to convert the esdl Assets to PyCML assets this class only exists to specify
     the specific objects used in the conversion step. Note there is no __init__ in the base class.
     This probably could be standardized in that case this class would become obsolete.
     """
```

### Comparing `mesido-0.1.1/src/mesido/esdl/esdl_mixin.py` & `mesido-0.1.2/src/mesido/esdl/esdl_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/esdl_model_base.py` & `mesido-0.1.2/src/mesido/esdl/esdl_model_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Dict
 
 import esdl
-from esdl import InPort
+from esdl import InPort, OutPort
 
 from mesido.esdl.asset_to_component_base import _AssetToComponentBase
 from mesido.pycml import Model as _Model
 
 from ._exceptions import _RetryLaterException, _SkipAssetException
 
 logger = logging.getLogger("mesido")
@@ -188,36 +188,76 @@
                             p_elec += 1
                         else:
                             raise Exception(
                                 f"{asset.name} has total of 5 ports, but no proper split between "
                                 f"milp(4) and electricity (1) ports"
                             )
                 elif (
-                    len(asset.in_ports) == 1
+                    asset.asset_type == "HeatPump"
                     and len(asset.out_ports) == 1
-                    and asset.asset_type == "HeatPump"
+                    and len(asset.in_ports) in [1, 2]
                 ):
                     for p in [*asset.in_ports, *asset.out_ports]:
-                        if isinstance(p.carrier, esdl.HeatCommodity):
-                            if isinstance(p, InPort):
-                                port_map[p.id] = getattr(component, in_suf)
-                            else:  # OutPort
-                                port_map[p.id] = getattr(component, out_suf)
+
+                        if isinstance(p, InPort) and isinstance(
+                            p.carrier, esdl.ElectricityCommodity
+                        ):
+                            port_map[p.id] = getattr(component, elec_in_suf)
+                        elif isinstance(p, InPort) and isinstance(p.carrier, esdl.HeatCommodity):
+                            port_map[p.id] = getattr(component, in_suf)
+                        elif isinstance(p, OutPort):  # OutPort
+                            port_map[p.id] = getattr(component, out_suf)
                         else:
                             raise Exception(
-                                f"{asset.name} has does not have 1 Heat in_ports and 1 Heat "
-                                f"out_ports "
+                                f"{asset.name} has does not have (1 electricity in_port) 1 heat "
+                                f"in port and 1 Heat out_ports "
                             )
                 else:
                     raise Exception(
                         f"{asset.name} has incorrect number of in/out ports. HeatPumps are allows "
                         f"to have 1 in and 1 out port for air-water HP, 2 in ports and 2 out ports "
                         f"when modelling a water-water HP, or 3 in ports and 2 out ports when the "
                         f"electricity connection of the water-water HP is modelled."
                     )
+            elif (
+                asset.asset_type == "GasHeater"
+                and len(asset.out_ports) == 1
+                and len(asset.in_ports) == 2
+            ):
+                for p in [*asset.in_ports, *asset.out_ports]:
+
+                    if isinstance(p, InPort) and isinstance(p.carrier, esdl.GasCommodity):
+                        port_map[p.id] = getattr(component, gas_in_suf)
+                    elif isinstance(p, InPort) and isinstance(p.carrier, esdl.HeatCommodity):
+                        port_map[p.id] = getattr(component, in_suf)
+                    elif isinstance(p, OutPort):  # OutPort
+                        port_map[p.id] = getattr(component, out_suf)
+                    else:
+                        raise Exception(
+                            f"{asset.name} has does not have 1 Heat in_port 1 gas in port and 1"
+                            f"Heat out_ports "
+                        )
+            elif (
+                asset.asset_type == "ElectricBoiler"
+                and len(asset.out_ports) == 1
+                and len(asset.in_ports) == 2
+            ):
+                for p in [*asset.in_ports, *asset.out_ports]:
+
+                    if isinstance(p, InPort) and isinstance(p.carrier, esdl.ElectricityCommodity):
+                        port_map[p.id] = getattr(component, elec_in_suf)
+                    elif isinstance(p, InPort) and isinstance(p.carrier, esdl.HeatCommodity):
+                        port_map[p.id] = getattr(component, in_suf)
+                    elif isinstance(p, OutPort):  # OutPort
+                        port_map[p.id] = getattr(component, out_suf)
+                    else:
+                        raise Exception(
+                            f"{asset.name} has does not have 1 electricity in_port 1 gas in port "
+                            f"and 1 Heat out_ports "
+                        )
             elif asset.asset_type == "Electrolyzer":
                 if len(asset.out_ports) == 1 and len(asset.in_ports) == 1:
                     if isinstance(asset.out_ports[0].carrier, esdl.GasCommodity):
                         port_map[asset.out_ports[0].id] = getattr(component, gas_out_suf)
                     else:
                         raise Exception(f"{asset.name} must have a gas commodity on the outport")
                     if isinstance(asset.in_ports[0].carrier, esdl.ElectricityCommodity):
```

### Comparing `mesido-0.1.1/src/mesido/esdl/esdl_parser.py` & `mesido-0.1.2/src/mesido/esdl/esdl_parser.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/esdl_qth_model.py` & `mesido-0.1.2/src/mesido/esdl/esdl_qth_model.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/esdl/profile_parser.py` & `mesido-0.1.2/src/mesido/esdl/profile_parser.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/financial_mixin.py` & `mesido-0.1.2/src/mesido/financial_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1062,33 +1062,29 @@
         and the investments made at timestep i are sufficient the asset also is realized (becomes
         available) in that same timestep.
         """
         constraints = []
         options = self.energy_system_options()
         if options["include_asset_is_realized"]:
             for asset in [
-                *self.energy_system_components.get("heat_demand", []),
+                # *self.energy_system_components.get("heat_demand", []),
                 *self.energy_system_components.get("heat_source", []),
                 *self.energy_system_components.get("ates", []),
                 *self.energy_system_components.get("low_temperature_ates", []),
                 *self.energy_system_components.get("heat_buffer", []),
                 *self.energy_system_components.get("heat_exchanger", []),
                 *self.energy_system_components.get("heat_pump", []),
             ]:
                 var_name = self.__cumulative_investments_made_in_eur_map[asset]
                 cumulative_investments_made = self.state(var_name)
                 nominal = self.variable_nominal(var_name)
                 var_name = self.__asset_is_realized_map[asset]
                 asset_is_realized = self.state(var_name)
-                installation_cost_sym = self.__asset_installation_cost_var[
-                    self._asset_installation_cost_map[asset]
-                ]
-                investment_cost_sym = self.__asset_investment_cost_var[
-                    self._asset_investment_cost_map[asset]
-                ]
+                installation_cost_sym = self.variable(self._asset_installation_cost_map[asset])
+                investment_cost_sym = self.variable(self._asset_investment_cost_map[asset])
                 # TODO: add insulation class cost to the investments made.
                 # if asset in self.heat_network_components.get("demand", []):
                 #     for insulation_class in self.__get_insulation_classes(asset):
                 #         insulation_class_active
                 #         insulation_class_cost
                 #         investment_cost_sym += insulation_class_active * insulation_class_cost
                 big_m = (
```

### Comparing `mesido-0.1.1/src/mesido/gas_physics_mixin.py` & `mesido-0.1.2/src/mesido/gas_physics_mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         }
         self._gn_head_loss_class = HeadLossClass(self.gas_network_settings)
         self.__gas_pipe_head_bounds = {}
         self.__gas_pipe_head_loss_var = {}
         self.__gas_pipe_head_loss_bounds = {}
         self.__gas_pipe_head_loss_nominals = {}
         self.__gas_pipe_head_loss_zero_bounds = {}
-        self._hn_gas_pipe_to_head_loss_map = {}
+        self._gn_pipe_to_head_loss_map = {}
 
         # Boolean path-variable for the direction of the flow, inport to outport is positive flow.
         self.__gas_flow_direct_var = {}
         self.__gas_flow_direct_bounds = {}
         self._gas_pipe_to_flow_direct_map = {}
 
         # Still to be implemented
@@ -128,14 +128,18 @@
         self.__gas_pipe_linear_line_segment_var_bounds = {}
         self._gas_pipe_linear_line_segment_map = {}
 
         super().__init__(*args, **kwargs)
 
         self._gas_pipe_topo_pipe_class_map = {}
 
+        # self.__gas_pipe_disconnect_var = {}
+        # self.__gas_pipe_disconnect_var_bounds = {}
+        self._gas_pipe_disconnect_map = {}
+
     def gas_carriers(self):
         """
         This function should be overwritten by the problem and should give a dict with the
         carriers as keys and a list of temperatures as values.
         """
         return {}
 
@@ -179,15 +183,15 @@
             if initialized_vars[1] != {}:
                 self.__gas_pipe_head_bounds[
                     f"{pipe_name}.{NetworkSettings.NETWORK_TYPE_GAS}Out.H"
                 ] = initialized_vars[1]
             if initialized_vars[2] != {}:
                 self.__gas_pipe_head_loss_zero_bounds[f"{pipe_name}.dH"] = initialized_vars[2]
             if initialized_vars[3] != {}:
-                self._hn_gas_pipe_to_head_loss_map[pipe_name] = initialized_vars[3]
+                self._gn_pipe_to_head_loss_map[pipe_name] = initialized_vars[3]
             if initialized_vars[4] != {}:
                 self.__gas_pipe_head_loss_var[head_loss_var] = initialized_vars[4]
             if initialized_vars[5] != {}:
                 self.__gas_pipe_head_loss_nominals[f"{pipe_name}.dH"] = initialized_vars[5]
             if initialized_vars[6] != {}:
                 self.__gas_pipe_head_loss_nominals[head_loss_var] = initialized_vars[6]
             if initialized_vars[7] != {}:
@@ -229,15 +233,15 @@
             if (q_in_lb >= 0.0 and q_in_ub >= 0.0) or (q_out_lb >= 0.0 and q_out_ub >= 0.0):
                 self.__gas_flow_direct_bounds[flow_dir_var] = (1.0, 1.0)
             elif (q_in_lb <= 0.0 and q_in_ub <= 0.0) or (q_out_lb <= 0.0 and q_out_ub <= 0.0):
                 self.__gas_flow_direct_bounds[flow_dir_var] = (0.0, 0.0)
             else:
                 self.__gas_flow_direct_bounds[flow_dir_var] = (0.0, 1.0)
 
-            # Still to be added in the future
+            # # Still to be added in the future
             # if parameters[f"{pipe_name}.disconnectable"]:
             #     disconnected_var = f"{pipe_name}__is_disconnected"
             #     self._gas_pipe_disconnect_map[pipe_name] = disconnected_var
             #     self.__gas_pipe_disconnect_var[disconnected_var] = ca.MX.sym(disconnected_var)
             #     self.__gas_pipe_disconnect_var_bounds[disconnected_var] = (0.0, 1.0)
 
         self.__maximum_total_head_loss = self.__get_maximum_total_head_loss()
@@ -332,14 +336,26 @@
             and self.gas_network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS
         ):
             g.append(
                 self._gn_head_loss_class._hn_minimization_goal_class(
                     self, self.gas_network_settings
                 )
             )
+            if (
+                self.gas_network_settings["head_loss_option"]
+                == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY
+                or self.gas_network_settings["head_loss_option"]
+                == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
+            ):
+                g.append(
+                    self._gn_head_loss_class._hpwr_minimization_goal_class(
+                        self,
+                        self.gas_network_settings,
+                    )
+                )
 
         return g
 
     def __get_maximum_total_head_loss(self):
         """
         Get an upper bound on the maximum total head loss that can be used in
         big-M formulations of e.g. check valves and disconnectable pipes.
@@ -371,15 +387,15 @@
                 head_loss += self._gn_head_loss_class._hn_pipe_head_loss(
                     pipe,
                     self,
                     options,
                     self.gas_network_settings,
                     parameters,
                     max_discharge,
-                    network_type=self.gas_network_settings["network_type"],
+                    # network_type=self.gas_network_settings["network_type"],
                     pressure=parameters[f"{pipe}.pressure"],
                 )
 
             head_loss += options["minimum_pressure_far_point"] * 10.2
 
             max_sum_dh_pipes = max(max_sum_dh_pipes, head_loss)
 
@@ -420,14 +436,36 @@
                 q_nominals.append(self.variable_nominal(gas_conn))
 
             q_nominal = np.median(q_nominals)
             constraints.append((q_sum / q_nominal, 0.0, 0.0))
 
         return constraints
 
+    def __gas_node_hydraulic_power_mixing_path_constraints(self, ensemble_member):
+        """
+        This function adds constraints to ensure that the incoming hydraulic power equals the
+        outgoing hydraulic power. We assume constant density throughout a hydraulically coupled
+        system and thus these constraints are needed for mass conservation.
+        """
+        constraints = []
+
+        for node, connected_pipes in self.energy_system_topology.gas_nodes.items():
+            q_sum = 0.0
+            q_nominals = []
+
+            for i_conn, (_pipe, orientation) in connected_pipes.items():
+                q_conn = f"{node}.GasConn[{i_conn + 1}].Hydraulic_power"
+                q_sum += orientation * self.state(q_conn)
+                q_nominals.append(self.variable_nominal(q_conn))
+
+            q_nominal = np.median(q_nominals)
+            constraints.append((q_sum / q_nominal, 0.0, 0.0))
+
+        return constraints
+
     def __state_vector_scaled(self, variable, ensemble_member):
         """
         This functions returns the casadi symbols scaled with their nominal for the entire time
         horizon.
         """
         canonical, sign = self.alias_relation.canonical_signed(variable)
         return (
@@ -492,202 +530,14 @@
 
             for p in pipes[1:]:
                 flow_dir_var = self.state(self._gas_pipe_to_flow_direct_map[p])
                 constraints.append((base_flow_dir_var - flow_dir_var, 0.0, 0.0))
 
         return constraints
 
-    def _hn_gas_pipe_head_loss_constraints(self, ensemble_member):
-        """
-        This function adds the head loss constraints for pipes. There are two options namely with
-        and without pipe class optimization. In both cases we assume that disconnected pipes, pipes
-        without flow have no head loss.
-
-        Under pipe-class optimization the head loss constraints per pipe class are added and
-        applied with the big_m method (is_topo_disconnected) to only activate the correct
-        constraints.
-
-        Under constant pipe class constraints for only one diameter are added.
-        """
-        constraints = []
-
-        options = self.energy_system_options()
-        parameters = self.parameters(ensemble_member)
-        components = self.energy_system_components
-        # Set the head loss according to the direction in the pipes. Note that
-        # the `.__head_loss` symbol is always positive by definition, but that
-        # `.dH` is not (positive when flow is negative, and vice versa).
-        # If the pipe is disconnected, we leave the .__head_loss symbol free
-        # (and it has no physical meaning). We also do not set any discharge
-        # relationship in this case (but dH is still equal to Out - In of
-        # course).
-
-        for pipe in components.get("gas_pipe", []):
-            if parameters[f"{pipe}.length"] == 0.0:
-                # If the pipe does not have a control valve, the head loss is
-                # forced to zero via bounds. If the pipe _does_ have a control
-                # valve, then there still is no relationship between the
-                # discharge and the head loss/dH.
-                continue
-
-            head_loss_sym = self._hn_gas_pipe_to_head_loss_map[pipe]
-
-            dh = self.__state_vector_scaled(f"{pipe}.dH", ensemble_member)
-            head_loss = self.__state_vector_scaled(head_loss_sym, ensemble_member)
-            discharge = self.__state_vector_scaled(f"{pipe}.Q", ensemble_member)
-
-            # We need to make sure the dH is decoupled from the discharge when
-            # the pipe is disconnected. Simply put, this means making the
-            # below constraints trivial.
-
-            # Still to be implemented
-            # is_disconnected_var = self._gas_pipe_disconnect_map.get(pipe)
-            is_disconnected_var = None
-
-            if is_disconnected_var is None:
-                is_disconnected = 0.0
-            else:
-                is_disconnected = self.__state_vector_scaled(is_disconnected_var, ensemble_member)
-
-            max_discharge = None
-            max_head_loss = -np.inf
-
-            if pipe in self._gas_pipe_topo_pipe_class_map:
-                # Multiple diameter options for this pipe
-                pipe_classes = self._gas_pipe_topo_pipe_class_map[pipe]
-                max_discharge = max(c.maximum_discharge for c in pipe_classes)
-
-                for pc, pc_var_name in pipe_classes.items():
-                    if pc.inner_diameter == 0.0:
-                        continue
-
-                    head_loss_max_discharge = self._gn_head_loss_class._hn_pipe_head_loss(
-                        pipe,
-                        self,
-                        options,
-                        self.gas_network_settings,
-                        parameters,
-                        max_discharge,
-                        pipe_class=pc,
-                        network_type=self.gas_network_settings["network_type"],
-                        pressure=parameters[f"{pipe}.pressure"],
-                    )
-
-                    big_m = max(
-                        2.0 * 2.0 * self.__maximum_total_head_loss, 2 * head_loss_max_discharge
-                    )
-
-                    is_topo_disconnected = 1 - self.extra_variable(pc_var_name, ensemble_member)
-                    is_topo_disconnected = ca.repmat(is_topo_disconnected, dh.size1())
-
-                    # Note that we add the two booleans `is_disconnected` and
-                    # `is_topo_disconnected`. This is allowed because of the way the
-                    # resulting expression is used in the Big-M formulation. We only care
-                    # that the expression (i.e. a single boolean or the sum of the two
-                    # booleans) is either 0 when the pipe is connected, or >= 1 when it
-                    # is disconnected.
-                    constraints.extend(
-                        self._gn_head_loss_class._hn_pipe_head_loss(
-                            pipe,
-                            self,
-                            options,
-                            self.gas_network_settings,
-                            parameters,
-                            discharge,
-                            head_loss,
-                            dh,
-                            is_disconnected + is_topo_disconnected,
-                            big_m,
-                            pc,
-                            network_type=self.gas_network_settings["network_type"],
-                            pressure=parameters[f"{pipe}.pressure"],
-                        )
-                    )
-
-                    # Contrary to the Big-M calculation above, the relation
-                    # between dH and the head loss symbol requires the
-                    # maximum head loss that can be realized effectively. So
-                    # we pass the current pipe class's maximum discharge.
-                    max_head_loss = max(
-                        max_head_loss,
-                        self._gn_head_loss_class._hn_pipe_head_loss(
-                            pipe,
-                            self,
-                            options,
-                            self.gas_network_settings,
-                            parameters,
-                            pc.maximum_discharge,
-                            pipe_class=pc,
-                            network_type=self.gas_network_settings["network_type"],
-                            pressure=parameters[f"{pipe}.pressure"],
-                        ),
-                    )
-            else:
-                # Only a single diameter for this pipe. Note that we rely on
-                # the diameter parameter being overridden automatically if a
-                # single pipe class is set by the user.
-                area = parameters[f"{pipe}.area"]
-                max_discharge = self.gas_network_settings["maximum_velocity"] * area
-
-                is_topo_disconnected = int(parameters[f"{pipe}.diameter"] == 0.0)
-
-                constraints.extend(
-                    self._gn_head_loss_class._hn_pipe_head_loss(
-                        pipe,
-                        self,
-                        options,
-                        self.gas_network_settings,
-                        parameters,
-                        discharge,
-                        head_loss,
-                        dh,
-                        is_disconnected + is_topo_disconnected,
-                        2.0 * 2.0 * self.__maximum_total_head_loss,
-                        network_type=self.gas_network_settings["network_type"],
-                        pressure=parameters[f"{pipe}.pressure"],
-                    )
-                )
-
-                max_head_loss = self._gn_head_loss_class._hn_pipe_head_loss(
-                    pipe,
-                    self,
-                    options,
-                    self.gas_network_settings,
-                    parameters,
-                    max_discharge,
-                    network_type=self.gas_network_settings["network_type"],
-                    pressure=parameters[f"{pipe}.pressure"],
-                )
-
-            # Relate the head loss symbol to the pipe's dH symbol.
-
-            # FIXME: Ugly hack. Cold pipes should be modelled completely with
-            # their own integers as well.
-            flow_dir = self.__state_vector_scaled(
-                self._gas_pipe_to_flow_direct_map[pipe], ensemble_member
-            )
-
-            # Note that the Big-M should _at least_ cover the maximum
-            # distance between `head_loss` and `dh`. If `head_loss` can be at
-            # most 1.0 (= `max_head_loss`), that means our Big-M should be at
-            # least double (i.e. >= 2.0). And because we do not want Big-Ms to
-            # be overly tight, we include an additional factor of 2.
-            big_m = 2.0 * 2.0 * max_head_loss
-
-            constraints.append(
-                (
-                    (-dh - head_loss + (1 - flow_dir) * big_m) / big_m,
-                    0.0,
-                    np.inf,
-                )
-            )
-            constraints.append(((dh - head_loss + flow_dir * big_m) / big_m, 0.0, np.inf))
-
-        return constraints
-
     def path_constraints(self, ensemble_member):
         """
         Here we add all the path constraints to the optimization problem. Please note that the
         path constraints are the constraints that are applied to each time-step in the problem.
         """
 
         constraints = super().path_constraints(ensemble_member)
@@ -695,30 +545,39 @@
         constraints.extend(self.__gas_node_mixing_path_constraints(ensemble_member))
 
         # Add source/demand head loss constrains only if head loss is non-zero
         if self.gas_network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
             constraints.extend(
                 self._gn_head_loss_class._pipe_head_loss_path_constraints(self, ensemble_member)
             )
-
+        constraints.extend(
+            self._gn_head_loss_class._pipe_hydraulic_power_path_constraints(
+                self, self.__maximum_total_head_loss, ensemble_member
+            )
+        )
         constraints.extend(self.__flow_direction_path_constraints(ensemble_member))
+        constraints.extend(self.__gas_node_hydraulic_power_mixing_path_constraints(ensemble_member))
 
         return constraints
 
     def constraints(self, ensemble_member):
         """
         This function adds the normal constraints to the problem. Unlike the path constraints these
         are not applied to every time-step in the problem. Meaning that these constraints either
         consider global variables that are independent of time-step or that the relevant time-steps
         are indexed within the constraint formulation.
         """
         constraints = super().constraints(ensemble_member)
 
         if self.gas_network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
-            constraints.extend(self._hn_gas_pipe_head_loss_constraints(ensemble_member))
+            constraints.extend(
+                self._gn_head_loss_class._pipe_head_loss_constraints(
+                    self, self.__maximum_total_head_loss, ensemble_member
+                )
+            )
 
         return constraints
 
     def goal_programming_options(self):
         """
         Here we set the goal programming configuration. We use soft constraints for consecutive
         goals.
@@ -789,24 +648,24 @@
                         pipe,
                         self,
                         options,
                         self.gas_network_settings,
                         parameters,
                         q,
                         None,
-                        network_type=self.gas_network_settings["network_type"],
+                        # network_type=self.gas_network_settings["network_type"],
                         pressure=parameters[f"{pipe}.pressure"],
                     )
                     if (
                         self.gas_network_settings["head_loss_option"]
                         == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY
                     ):
                         head_loss = np.abs(results[f"{pipe}.dH"][inds])
                     else:
-                        head_loss = results[self._hn_gas_pipe_to_head_loss_map[pipe]][inds]
+                        head_loss = results[self._gn_pipe_to_head_loss_map[pipe]][inds]
 
                     if not np.allclose(head_loss, head_loss_target, rtol=rtol, atol=atol):
                         logger.warning(
                             f"Pipe {pipe} has artificial head loss; "
                             f"at least one more control valve should be added to the network."
                         )
```

### Comparing `mesido-0.1.1/src/mesido/head_loss_class.py` & `mesido-0.1.2/src/mesido/qth_not_maintained/head_loss_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 from abc import abstractmethod
 from enum import IntEnum
 from typing import List, Optional, Tuple, Type, Union
 
 import casadi as ca
 
 import mesido._darcy_weisbach as darcy_weisbach
-from mesido.constants import GRAVITATIONAL_CONSTANT
-from mesido.network_common import NetworkSettings
-from mesido.pipe_class import PipeClass
+from mesido.base_component_type_mixin import BaseComponentTypeMixin
 
 import numpy as np
 
-from rtctools.optimization.goal_programming_mixin_base import Goal
-from rtctools.optimization.optimization_problem import BT
+from rtctools._internal.alias_tools import AliasDict
+from rtctools.optimization.goal_programming_mixin_base import Goal, _GoalProgrammingMixinBase
+from rtctools.optimization.optimization_problem import BT, OptimizationProblem
+
+from ..constants import GRAVITATIONAL_CONSTANT
+from ..pipe_class import PipeClass
 
 
 logger = logging.getLogger("mesido")
 
 
 class HeadLossOption(IntEnum):
     r"""
     Enumeration for the possible options to take head loss in pipes into account.
-    Also see :py:meth:`._HeadLossMixin.energy_system_options` for related options.
+    Also see :py:meth:`._HeadLossMixin.heat_network_options` for related options.
 
     .. note::
         Not all options are supported by :py:class:`.HeatMixin`, due to the focus
         on MILP formulations.
 
     NO_HEADLOSS
        The NO_HEADLOSS option assumes that there is no headloss in the pipelines.
@@ -63,15 +65,15 @@
            \Delta H \ge \vec{a} \cdot Q + \vec{b}
 
         with :math:`\vec{a}` and :math:`\vec{b}` the linearization coefficients.
 
         This approach can more easily be explain with a plot, showing the Darcy-Weisbach
         head loss, and the linear lines approximating it. Note that the number of
         supporting lines is an option that can be set by the user by overriding
-        :py:meth:`._HeadLossMixin.energy_system_options`. Also note that, just like
+        :py:meth:`._HeadLossMixin.heat_network_options`. Also note that, just like
         ``CQ2_INEQUALITY``, a boolean is needed when flow directions are not fixed.
 
            .. image:: /images/DWlinearization.PNG
 
     LINEARIZED_ONE_LINE_EQUALITY
         This option uses a linear head loss formulation.
         A single constraint of the type
@@ -81,15 +83,15 @@
            H_{up} - H_{down} = dH = C \cdot Q
 
         is added.
         Note that no boolean are required to support the case where flow directions
         are not fixed yet, at the cost of reduced fidelity in the head-loss relationship.
 
         The exact velocity to use to linearize can be set by overriding
-        :py:meth:`._HeadLossMixin.energy_system_options`.
+        :py:meth:`._HeadLossMixin.heat_network_options`.
 
     CQ2_EQUALITY
         This option adds **equality** constraints of the type:
 
          .. math::
 
            dH = C \cdot Q^2
@@ -98,204 +100,240 @@
     """
 
     NO_HEADLOSS = 1
     CQ2_INEQUALITY = 2
     LINEARIZED_N_LINES_WEAK_INEQUALITY = 3
     LINEARIZED_ONE_LINE_EQUALITY = 4
     CQ2_EQUALITY = 5
-    LINEARIZED_N_LINES_EQUALITY = 6
 
 
 class _MinimizeHeadLosses(Goal):
     order = 1
 
-    priority = 2**31 - 2
+    priority = 2**31 - 1
 
-    def __init__(self, optimization_problem, input_network_settings, *args, **kwargs):
+    def __init__(self, optimization_problem: "_HeadLossMixin", *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.optimization_problem = optimization_problem
-        self.network_settings = input_network_settings
         self.function_nominal = len(optimization_problem.times())
 
-    def function(self, optimization_problem, ensemble_member):
+    def function(self, optimization_problem: "_HeadLossMixin", ensemble_member):
         """
         This function returns the summed head loss of all pipes and pumps.
         """
         sum_ = 0.0
 
         parameters = optimization_problem.parameters(ensemble_member)
+        options = optimization_problem.heat_network_options()
 
         pumps = optimization_problem.energy_system_components.get("pump", [])
         sources = optimization_problem.energy_system_components.get("heat_source", [])
 
         for p in pumps:
             sum_ += optimization_problem.state(f"{p}.dH")
 
         # If sources have an accompanying pump, we prefer the produced head to
         # be shifted to that pump. We therefore penalize the head of the
         # sources twice as much.
         for s in sources:
             sum_ += 2 * optimization_problem.state(f"{s}.dH")
 
-        assert self.network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS
+        assert options["head_loss_option"] != HeadLossOption.NO_HEADLOSS
 
-        if self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_HEAT:
-            for p in optimization_problem.energy_system_components.get("heat_pipe", []):
-                if (
-                    not parameters[f"{p}.has_control_valve"]
-                    and not parameters[f"{p}.length"] == 0.0
-                ):
-                    sym_name = optimization_problem._hn_pipe_to_head_loss_map[p]
-                    sum_ += optimization_problem.state(sym_name)
-        elif self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_GAS:
-            for p in optimization_problem.energy_system_components.get("gas_pipe", []):
-                if not parameters[f"{p}.length"] == 0.0:
-                    sym_name = optimization_problem._hn_gas_pipe_to_head_loss_map[p]
-                    sum_ += optimization_problem.state(sym_name)
+        for p in optimization_problem.energy_system_components["pipe"]:
+            if not parameters[f"{p}.has_control_valve"] and not parameters[f"{p}.length"] == 0.0:
+                sym_name = optimization_problem._hn_pipe_to_head_loss_map[p]
+                sum_ += optimization_problem.state(sym_name)
 
         return sum_
 
 
 class _MinimizeHydraulicPower(Goal):
     order = 1
 
     priority = 2**31 - 1
 
     def __init__(
         self,
-        optimization_problem,
-        input_network_settings,
+        optimization_problem: "_HeadLossMixin",
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.optimization_problem = optimization_problem
-        self.network_settings = input_network_settings
 
-    def function(self, optimization_problem, ensemble_member):
+    def function(self, optimization_problem: "_HeadLossMixin", ensemble_member):
         """
         This function returns the summed hydraulic power of all pipes
         """
         sum_ = 0.0
 
         parameters = optimization_problem.parameters(ensemble_member)
+        options = optimization_problem.heat_network_options()
 
-        assert self.network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS
+        assert options["head_loss_option"] != HeadLossOption.NO_HEADLOSS
 
-        for pipe in optimization_problem.energy_system_components.get("heat_pipe", []):
+        for pipe in optimization_problem.energy_system_components.get("pipe", []):
             if (
                 not parameters[f"{pipe}.has_control_valve"]
                 and not parameters[f"{pipe}.length"] == 0.0
             ):
                 sum_ += optimization_problem.state(f"{pipe}.Hydraulic_power")
 
         return sum_
 
 
-class HeadLossClass:
+class _HeadLossMixin(BaseComponentTypeMixin, _GoalProgrammingMixinBase, OptimizationProblem):
     """
-    For handling of discharge - head (loss) relationship to the model.
+    Adds handling of discharge - head (loss) relationship to the model.
     """
 
-    def __init__(self, input_network_settings, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
         self.__pipe_head_bounds = {}
 
         self.__pipe_head_loss_var = {}
         self.__pipe_head_loss_bounds = {}
         self.__pipe_head_loss_nominals = {}
         self.__pipe_head_loss_zero_bounds = {}
         self._hn_pipe_to_head_loss_map = {}
 
-        # Kvr
-        # Boolean variables for the linear line segment options per pipe.
-        self.__pipe_linear_line_segment_var = {}  # value 0/1: line segment - not active/active
-        self.__pipe_linear_line_segment_var_bounds = {}
-        self._pipe_linear_line_segment_map = {}
-
         self.__priority = None
 
-        self.network_settings = input_network_settings
-
     def pre(self):
         """
         Some checks to avoid that different pipes have different head_loss options in case one
         has the No_HeadLoss option.
         """
         super().pre()
 
         self.__initialize_nominals_and_bounds()
 
+        options = self.heat_network_options()
         parameters = self.parameters(0)
 
         # It is not allowed to mix NO_HEADLOSS with other head loss options as
         # that just leads to weird and undefined behavior.
         head_loss_values = {
-            self.network_settings["head_loss_option"],
+            options["head_loss_option"],
         }
-
-        pipe_type = "heat_pipe"
-        if len(self.energy_system_components.get("heat_pipe", [])) == 0:
-            pipe_type = "gas_pipe"
-
-        for p in self.energy_system_components.get(pipe_type, []):
-            head_loss_values.add(
-                self._hn_get_pipe_head_loss_option(p, self.network_settings, parameters)
-            )
+        for p in self.energy_system_components.get("pipe", []):
+            head_loss_values.add(self._hn_get_pipe_head_loss_option(p, options, parameters))
 
         if HeadLossOption.NO_HEADLOSS in head_loss_values and len(head_loss_values) > 1:
             raise Exception(
                 "Mixing .NO_HEADLOSS with other head loss options is not allowed. "
                 "Either all pipes should have .NO_HEADLOSS set, or none. "
-                "The global value returned by energy_system_options() also need to match."
+                "The global value returned by heat_network_options() also need to match."
             )
 
-    def head_loss_network_options(self):
+    def heat_network_options(self):
         r"""
         Returns a dictionary of milp network specific options.
 
         +--------------------------------+-----------+-----------------------------------+
         | Option                         | Type      | Default value                     |
         +================================+===========+===================================+
         | ``minimum_pressure_far_point`` | ``float`` | ``1.0`` bar                       |
         +--------------------------------+-----------+-----------------------------------+
         | ``wall_roughness``             | ``float`` | ``0.0002`` m                      |
         +--------------------------------+-----------+-----------------------------------+
+        | ``head_loss_option``           | ``enum``  | ``HeadLossOption.CQ2_INEQUALITY`` |
+        +--------------------------------+-----------+-----------------------------------+
         | ``estimated_velocity``         | ``float`` | ``1.0`` m/s (CQ2_* &              |
         |                                |           |LINEARIZED_ONE_LINE_EQUALITY)      |
         +--------------------------------+-----------+-----------------------------------+
+        | ``maximum_velocity``           | ``float`` | ``2.5`` m/s                       |
+        |                                |           |LINEARIZED_N_LINES_WEAK_INEQUALITY |
+        +--------------------------------+-----------+-----------------------------------+
+        | ``n_linearization_lines``      | ``int``   | ``5``                             |
+        |                                |           |LINEARIZED_N_LINES_WEAK_INEQUALITY |
+        +--------------------------------+-----------+-----------------------------------+
+        | ``minimize_head_losses``       | ``bool``  | ``True``                          |
+        +--------------------------------+-----------+-----------------------------------+
+        | ``pipe_minimum_pressure``      | ``float`` | ``-np.inf``                       |
+        +--------------------------------+-----------+-----------------------------------+
+        | ``pipe_maximum_pressure``      | ``float`` | ``np.inf``                        |
+        +--------------------------------+-----------+-----------------------------------+
 
         The ``minimum_pressure_far_point`` gives the minimum pressure
         requirement at any demand node, which means that the pressure at the
         furthest point is also satisfied without inspecting the topology.
 
         The ``wall_roughness`` of the pipes plays a role in determining the
         resistance of the pipes.
+
+        To model the head loss in pipes, the ``head_loss_option`` refers to
+        one of the ways this can be done. See :class:`HeadLossOption` for more
+        explanation on what each option entails. Note that some options model
+        the head loss as an inequality, i.e. :math:`\Delta H \ge f(Q)`, whereas
+        others model it as an equality.
+
+        When ``HeadLossOption.CQ2_INEQUALITY`` is used, the wall roughness at
+        ``estimated_velocity`` determines the `C` in :math:`\Delta H \ge C
+        \cdot Q^2`.
+
+        When ``HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY`` is used, the
+        ``maximum_velocity`` needs to be set. The Darcy-Weisbach head loss
+        relationship from :math:`v = 0` until :math:`v = \text{maximum_velocity}`
+        will then be linearized using ``n_linearization`` lines.
+
+        When ``HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY`` is used, the wall roughness at
+        ``estimated_velocity`` determines the `C` in :math:`\Delta H = C \cdot
+        Q`. For pipes that contain a control valve, the formulation of
+        ``HeadLossOption.CQ2_INEQUALITY`` is used.
+
+        When ``HeadLossOption.CQ2_EQUALITY`` is used, the wall roughness at
+        ``estimated_velocity`` determines the `C` in :math:`\Delta H = C \cdot
+        Q^2`. Note that this formulation is non-convex. At `theta < 1` we
+        therefore use the formulation ``HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY``. For pipes
+        that contain a control valve, the formulation of
+        ``HeadLossOption.CQ2_INEQUALITY`` is used.
+
+
+        When ``minimize_head_losses`` is set to True (default), a last
+        priority is inserted where the head losses and hydraulic power in the system are
+        minimized if the ``head_loss_option`` is not `NO_HEADLOSS`.
+        This is related to the assumption that control valves are
+        present in the system to steer water in the right direction the case
+        of multiple routes. If such control valves are not present, enabling
+        this option will give warnings in case the found solution is not
+        feasible. In case the option is False, both the minimization and
+        checks are skipped.
+
+        The ``pipe_minimum_pressure`` is the global minimum pressured allowed
+        in the network. Similarly, ``pipe_maximum_pressure`` is the maximum
+        one.
         """
 
         options = {}
 
         options["minimum_pressure_far_point"] = 1.0
         options["wall_roughness"] = 2e-4
+        options["head_loss_option"] = HeadLossOption.CQ2_INEQUALITY
         options["estimated_velocity"] = 1.0
+        options["maximum_velocity"] = 2.5
+        options["n_linearization_lines"] = 5
+        options["minimize_head_losses"] = True
 
         return options
 
     @abstractmethod
     def _hn_get_pipe_head_loss_option(
-        self, pipe, network_settings, parameters, **kwargs
+        self, pipe, heat_network_options, parameters, **kwargs
     ) -> HeadLossOption:
         """
         The global user head loss option is not necessarily the same as the
         head loss option for a specific pipe. For example, when a control
         valve is present, a .LINEARIZED_ONE_LINE_EQUALITY global head loss option could mean a
         .CQ2_INEQUALITY formulation should be used instead.
 
         See also the explanation of `head_loss_option` (and its values) in
-        :py:meth:`.energy_system_options`.
+        :py:meth:`.heat_network_options`.
         """
         raise NotImplementedError
 
     @abstractmethod
     def _hn_pipe_head_loss_constraints(self, ensemble_member) -> List[Tuple[ca.MX, float, float]]:
         """
         This method should be implemented to relate the three variables:
@@ -320,187 +358,86 @@
     @property
     def _hpwr_minimization_goal_class(self) -> Type[Goal]:
         """
         This function returns the minimize hydraulic power goal
         """
         return _MinimizeHydraulicPower
 
-    def initialize_variables_nominals_and_bounds(
-        self, optimization_problem, commodity_type, pipe_name, network_settings
-    ):
+    def __initialize_nominals_and_bounds(self):
         """
         This function computes and sets the bounds and nominals for the head loss of all the pipes
         as well as the minimum and maximum pipe pressure.
         """
-        options = optimization_problem.energy_system_options()
-        parameters = optimization_problem.parameters(0)
+        self.__pipe_head_loss_nominals = AliasDict(self.alias_relation)
 
-        min_pressure = network_settings["pipe_minimum_pressure"]
-        max_pressure = network_settings["pipe_maximum_pressure"]
+        options = self.heat_network_options()
+        parameters = self.parameters(0)
+
+        min_pressure = options["pipe_minimum_pressure"]
+        max_pressure = options["pipe_maximum_pressure"]
         assert (
             max_pressure > min_pressure
         ), "The global maximum pressure must be larger than the minimum one."
         if np.isfinite(min_pressure) or np.isfinite(max_pressure):
-            # No elevation data available yet. Assume 0 mDAT for now.
-            pipe_elevation = 0.0
-            min_head = min_pressure * 10.2 + pipe_elevation
-            max_head = max_pressure * 10.2 + pipe_elevation
-            self.__pipe_head_bounds[f"{pipe_name}.{commodity_type}In.H"] = (min_head, max_head)
-            self.__pipe_head_bounds[f"{pipe_name}.{commodity_type}Out.H"] = (min_head, max_head)
+            for p in self.energy_system_components["pipe"]:
+                # No elevation data available yet. Assume 0 mDAT for now.
+                pipe_elevation = 0.0
+                min_head = min_pressure * 10.2 + pipe_elevation
+                max_head = max_pressure * 10.2 + pipe_elevation
+                self.__pipe_head_bounds[f"{p}.HeatIn.H"] = (min_head, max_head)
+                self.__pipe_head_bounds[f"{p}.HeatOut.H"] = (min_head, max_head)
 
-        head_loss_option = network_settings["head_loss_option"]
+        head_loss_option = options["head_loss_option"]
         if head_loss_option not in HeadLossOption.__members__.values():
             raise Exception(f"Head loss option '{head_loss_option}' does not exist")
 
-        length = parameters[f"{pipe_name}.length"]
-        if length < 0.0:
-            raise ValueError("Pipe length has to be larger than or equal to zero")
+        for p in self.energy_system_components.get("pipe", []):
+            length = parameters[f"{p}.length"]
+            if length < 0.0:
+                raise ValueError("Pipe length has to be larger than or equal to zero")
 
-        if head_loss_option == HeadLossOption.NO_HEADLOSS or (
-            length == 0.0 and not parameters[f"{pipe_name}.has_control_valve"]
-        ):
-            self.__pipe_head_loss_zero_bounds[f"{pipe_name}.dH"] = (0.0, 0.0)
-            head_loss_var = ""  # Required for checking if the keys exist in the return past below
-        else:
-            q_nominal = self._hn_pipe_nominal_discharge(options, parameters, pipe_name)
-            head_loss_nominal = self._hn_pipe_head_loss(
-                pipe_name,
-                optimization_problem,
-                options,
-                network_settings,
-                parameters,
-                q_nominal,
-                network_type=self.network_settings["network_type"],
-                pressure=parameters[f"{pipe_name}.pressure"],
-            )
+            head_loss_option = self._hn_get_pipe_head_loss_option(p, options, parameters)
+
+            if head_loss_option == HeadLossOption.NO_HEADLOSS or (
+                length == 0.0 and not parameters[f"{p}.has_control_valve"]
+            ):
+                self.__pipe_head_loss_zero_bounds[f"{p}.dH"] = (0.0, 0.0)
+            else:
+                q_nominal = self._hn_pipe_nominal_discharge(options, parameters, p)
+                head_loss_nominal = self._hn_pipe_head_loss(p, options, parameters, q_nominal)
 
-            self.__pipe_head_loss_nominals[f"{pipe_name}.dH"] = head_loss_nominal
+                self.__pipe_head_loss_nominals[f"{p}.dH"] = head_loss_nominal
 
-            # The .dH is by definition "Out - In". The .__head_loss is by
-            # definition larger than or equal to the absolute value of dH.
-            head_loss_var = f"{pipe_name}.__head_loss"
-
-            self._hn_pipe_to_head_loss_map[pipe_name] = head_loss_var
-            self.__pipe_head_loss_var[head_loss_var] = ca.MX.sym(head_loss_var)
-
-            self.__pipe_head_loss_nominals[head_loss_var] = head_loss_nominal
-            self.__pipe_head_loss_bounds[head_loss_var] = (0.0, np.inf)
-
-            if head_loss_option == HeadLossOption.LINEARIZED_N_LINES_EQUALITY:
-                # Add pipe head loss linear line segment variables
-                self._pipe_linear_line_segment_map[pipe_name] = {}
-                self.__pipe_linear_line_segment_var[pipe_name] = {}
-                self.__pipe_linear_line_segment_var_bounds[pipe_name] = {}
-                # We need to creat linear line segments for the - and + volumetric flow rate
-                # possibilites. Line number 1, 2, N for the - & + side is created
-                discharge_type = ["neg_discharge", "pos_discharge"]
-                line_number = 0
-                for dtype in discharge_type:
-                    for ii_line in range(network_settings["n_linearization_lines"] * 2):
-                        if ii_line < network_settings["n_linearization_lines"]:
-                            dtype = discharge_type[0]
-                            line_number = ii_line + 1
-                        else:
-                            dtype = discharge_type[1]
-                            line_number = ii_line + 1 - network_settings["n_linearization_lines"]
-
-                        # start line segment numbering from 1 up to "n_linearization_lines"
-                        pipe_linear_line_segment_var_name = (
-                            f"{pipe_name}__pipe_linear_line_segment_num_{line_number}_{dtype}"
-                        )
+                # The .dH is by definition "Out - In". The .__head_loss is by
+                # definition larger than or equal to the absolute value of dH.
+                head_loss_var = f"{p}.__head_loss"
 
-                        self._pipe_linear_line_segment_map[pipe_name][
-                            ii_line
-                        ] = pipe_linear_line_segment_var_name
-                        self.__pipe_linear_line_segment_var[pipe_name][
-                            pipe_linear_line_segment_var_name
-                        ] = ca.MX.sym(pipe_linear_line_segment_var_name)
-                        self.__pipe_linear_line_segment_var_bounds[pipe_name][
-                            pipe_linear_line_segment_var_name
-                        ] = (0.0, 1.0)
-
-        return (
-            (
-                self.__pipe_head_bounds[f"{pipe_name}.{commodity_type}In.H"]
-                if self.__pipe_head_bounds.get(f"{pipe_name}.{commodity_type}In.H") is not None
-                else self.__pipe_head_bounds
-            ),
-            (
-                self.__pipe_head_bounds[f"{pipe_name}.{commodity_type}Out.H"]
-                if self.__pipe_head_bounds.get(f"{pipe_name}.{commodity_type}Out.H") is not None
-                else self.__pipe_head_bounds
-            ),
-            (
-                self.__pipe_head_loss_zero_bounds[f"{pipe_name}.dH"]
-                if self.__pipe_head_loss_zero_bounds.get(f"{pipe_name}.dH") is not None
-                else self.__pipe_head_loss_zero_bounds
-            ),
-            (
-                self._hn_pipe_to_head_loss_map[pipe_name]
-                if self._hn_pipe_to_head_loss_map.get(pipe_name) is not None
-                else self._hn_pipe_to_head_loss_map
-            ),
-            (
-                self.__pipe_head_loss_var[head_loss_var]
-                if self.__pipe_head_loss_var.get(head_loss_var) is not None
-                else self.__pipe_head_loss_var
-            ),
-            (
-                self.__pipe_head_loss_nominals[f"{pipe_name}.dH"]
-                if self.__pipe_head_loss_nominals.get(f"{pipe_name}.dH") is not None
-                else self.__pipe_head_loss_nominals
-            ),
-            (
-                self.__pipe_head_loss_nominals[head_loss_var]
-                if self.__pipe_head_loss_nominals.get(head_loss_var) is not None
-                else self.__pipe_head_loss_nominals
-            ),
-            (
-                self.__pipe_head_loss_bounds[head_loss_var]
-                if self.__pipe_head_loss_bounds.get(head_loss_var) is not None
-                else self.__pipe_head_loss_bounds
-            ),
-            (
-                self._pipe_linear_line_segment_map[pipe_name]
-                if self._pipe_linear_line_segment_map.get(pipe_name) is not None
-                else self._pipe_linear_line_segment_map
-            ),
-            (
-                self.__pipe_linear_line_segment_var[pipe_name]
-                if self.__pipe_linear_line_segment_var.get(pipe_name) is not None
-                else self.__pipe_linear_line_segment_var
-            ),
-            (
-                self.__pipe_linear_line_segment_var_bounds[pipe_name]
-                if self.__pipe_linear_line_segment_var_bounds.get(pipe_name) is not None
-                else self.__pipe_linear_line_segment_var_bounds
-            ),
-        )
+                self._hn_pipe_to_head_loss_map[p] = head_loss_var
+                self.__pipe_head_loss_var[head_loss_var] = ca.MX.sym(head_loss_var)
+
+                self.__pipe_head_loss_nominals[head_loss_var] = head_loss_nominal
+                self.__pipe_head_loss_bounds[head_loss_var] = (0.0, np.inf)
 
-    def _hn_pipe_nominal_discharge(self, energy_system_options, parameters, pipe: str) -> float:
+    def _hn_pipe_nominal_discharge(self, heat_network_options, parameters, pipe: str) -> float:
         """
         This function returns the nominal volumetric flow (m^3/s) through the pipe.
         """
-        return parameters[f"{pipe}.area"] * energy_system_options["estimated_velocity"]
+        return parameters[f"{pipe}.area"] * heat_network_options["estimated_velocity"]
 
     def _hn_pipe_head_loss(
         self,
         pipe: str,
-        optimization_problem,
-        energy_system_options,
-        network_settings,
+        heat_network_options,
         parameters,
         discharge: Union[ca.MX, float, np.ndarray],
         head_loss: Optional[ca.MX] = None,
         dh: Optional[ca.MX] = None,
         is_disconnected: Union[ca.MX, int] = 0,
         big_m: Optional[float] = None,
         pipe_class: Optional[PipeClass] = None,
-        network_type: NetworkSettings = NetworkSettings.NETWORK_TYPE_HEAT,
-        pressure: float = 0.0,
     ) -> Union[List[Tuple[ca.MX, BT, BT]], float, np.ndarray]:
         """
         This function has two purposes:
         - return the head loss constraint expression(s) or
         - compute the head loss numerically (always positive).
 
         Note that there are different head loss formulations (see
@@ -523,15 +460,17 @@
         """
 
         if head_loss is None and dh is None:
             symbolic = False
         else:
             symbolic = True
 
-        head_loss_option = network_settings["head_loss_option"]
+        head_loss_option = self._hn_get_pipe_head_loss_option(
+            pipe, heat_network_options, parameters
+        )
         assert (
             head_loss_option != HeadLossOption.NO_HEADLOSS
         ), "This method should be skipped when NO_HEADLOSS is set."
 
         length = parameters[f"{pipe}.length"]
 
         if length == 0.0:
@@ -558,71 +497,46 @@
                 return 0.0
 
         if big_m is None:
             assert is_disconnected == 0.0
         else:
             assert big_m != 0.0
 
-        wall_roughness = energy_system_options["wall_roughness"]
+        wall_roughness = heat_network_options["wall_roughness"]
+
         if pipe_class is not None:
             diameter = pipe_class.inner_diameter
             area = pipe_class.area
             maximum_velocity = pipe_class.maximum_velocity
         else:
             diameter = parameters[f"{pipe}.diameter"]
             area = parameters[f"{pipe}.area"]
-            maximum_velocity = network_settings["maximum_velocity"]
-
-        try:
-            # Only milp networks have a temperature attribute in the pipes, otherwise we will use
-            # a default temperature for gas networks
-            temperature = parameters[f"{pipe}.temperature"]
-            for _id, attr in optimization_problem.temperature_carriers().items():
-                if (
-                    parameters[f"{pipe}.carrier_id"] == attr["id_number_mapping"]
-                    and len(
-                        optimization_problem.temperature_regimes(parameters[f"{pipe}.carrier_id"])
-                    )
-                    > 0
-                ):
-                    temperature = min(
-                        optimization_problem.temperature_regimes(parameters[f"{pipe}.carrier_id"])
-                    )
-        except KeyError:
-            # A default temperature of 20 degrees celcius is used for gas networks.
-            temperature = 20.0
+            maximum_velocity = heat_network_options["maximum_velocity"]
 
-        try:
-            has_control_valve = parameters[f"{pipe}.has_control_valve"]
-        except KeyError:
-            has_control_valve = False
+        temperature = parameters[f"{pipe}.temperature"]
+        has_control_valve = parameters[f"{pipe}.has_control_valve"]
 
         if head_loss_option == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY:
             assert not has_control_valve
 
             ff = darcy_weisbach.friction_factor(
-                maximum_velocity,
-                diameter,
-                wall_roughness,
-                temperature,
-                network_type=network_type,
-                pressure=pressure,
+                heat_network_options["maximum_velocity"], diameter, wall_roughness, temperature
             )
 
             # Compute c_v constant (where |dH| ~ c_v * v^2)
             c_v = length * ff / (2 * GRAVITATIONAL_CONSTANT) / diameter
 
-            linearization_velocity = maximum_velocity
+            linearization_velocity = heat_network_options["maximum_velocity"]
             linearization_head_loss = c_v * linearization_velocity**2
             linearization_discharge = linearization_velocity * area
 
             expr = linearization_head_loss * discharge / linearization_discharge
 
             if symbolic:
-                constraint_nominal = c_v * maximum_velocity**2
+                constraint_nominal = c_v * heat_network_options["estimated_velocity"] ** 2
                 # Interior point solvers, like IPOPT, do not like linearly dependent
                 # tight inequality constraints. For this reason, we split the
                 # constraints depending whether the Big-M formulation is used or not.
                 if big_m is None:
                     return [((-1 * dh - expr) / constraint_nominal, 0.0, 0.0)]
                 else:
                     constraint_nominal = (constraint_nominal * big_m) ** 0.5
@@ -643,20 +557,15 @@
                 return expr * np.sign(discharge)
 
         elif head_loss_option in {
             HeadLossOption.CQ2_INEQUALITY,
             HeadLossOption.CQ2_EQUALITY,
         }:
             ff = darcy_weisbach.friction_factor(
-                energy_system_options["estimated_velocity"],
-                diameter,
-                wall_roughness,
-                temperature,
-                network_type=network_type,
-                pressure=pressure,
+                heat_network_options["estimated_velocity"], diameter, wall_roughness, temperature
             )
 
             # Compute c_v constant (where |dH| ~ c_v * v^2)
             c_v = length * ff / (2 * GRAVITATIONAL_CONSTANT) / diameter
 
             v = discharge / area
             expr = c_v * v**2
@@ -694,192 +603,85 @@
                                 0.0,
                             ),
                         )
                 return equations
             else:
                 return expr
 
-        elif (
-            head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
-            or head_loss_option == HeadLossOption.LINEARIZED_N_LINES_EQUALITY
-        ):
-            n_linear_lines = network_settings["n_linearization_lines"]
-            n_timesteps = len(optimization_problem.times())
+        elif head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY:
+            n_lines = heat_network_options["n_linearization_lines"]
 
             a, b = darcy_weisbach.get_linear_pipe_dh_vs_q_fit(
                 diameter,
                 length,
                 wall_roughness,
                 temperature=temperature,
-                n_lines=n_linear_lines,
+                n_lines=n_lines,
                 v_max=maximum_velocity,
-                network_type=self.network_settings["network_type"],
-                pressure=parameters[f"{pipe}.pressure"],
             )
 
             # The function above only gives result in the positive quadrant
             # (positive head loss, positive discharge). We also need a
             # positive head loss for _negative_ discharges.
             a = np.hstack([-a, a])
             b = np.hstack([b, b])
 
             # Vectorize constraint for speed
             if symbolic:
-                q_nominal = optimization_problem.variable_nominal(f"{pipe}.Q")
-                head_loss_nominal = optimization_problem.variable_nominal(f"{pipe}.dH")
+                q_nominal = self.variable_nominal(f"{pipe}.Q")
+                head_loss_nominal = self.variable_nominal(f"{pipe}.dH")
                 head_loss_vec = ca.repmat(head_loss, len(a))
                 discharge_vec = ca.repmat(discharge, len(a))
-
                 if isinstance(is_disconnected, ca.MX):
                     is_disconnected_vec = ca.repmat(is_disconnected, len(a))
                 else:
-                    # is_disconnected_vec = is_disconnected
-                    is_disconnected_vec = (
-                        np.ones((len(a) * discharge.size1(), 1), dtype=float) * is_disconnected
-                    )
+                    is_disconnected_vec = is_disconnected
 
                 a_vec = np.repeat(a, discharge.size1())
                 b_vec = np.repeat(b, discharge.size1())
-
                 constraint_nominal = np.abs(head_loss_nominal * a_vec * q_nominal) ** 0.5
 
                 if big_m is None:
                     # We write the equation such that big_m is always used, even if
                     # it is None (i.e. not used). We do have to be sure to set it to 0,
                     # because we cannot multiple with "None".
                     big_m_lin = 0.0
                 else:
                     big_m_lin = big_m
                     constraint_nominal = (constraint_nominal * big_m_lin) ** 0.5
-
-                constraints = []
-
-                # Add weak inequality constraint, value >= 0.0 for all linear lines
-                constraints.append(
+                return [
                     (
                         (
                             head_loss_vec
                             - (a_vec * discharge_vec + b_vec)
                             + is_disconnected_vec * big_m_lin
                         )
                         / constraint_nominal,
                         0.0,
                         np.inf,
-                    ),
-                )
-                if head_loss_option == HeadLossOption.LINEARIZED_N_LINES_EQUALITY:
-                    # Add constraints for piece-wise linear equality
-
-                    # Populate variable indicating if a linear line segment is active (1) or not (0)
-                    # pipe_linear_line_segment: will contain variables of negative and positive
-                    # discharge possibilites for the pipe. This implies if a pipe is linearized
-                    # with N = 2 linear lines then pipe_linear_line_segment will have 2 * 2
-                    # variables
-                    # Order of linear line variables:
-                    #  - negative discharge line_1, line_2
-                    #  - positve discharge line_1, line_2
-                    pipe_linear_line_segment = self._pipe_linear_line_segment_map[pipe]
-                    is_line_segment_active = []
-
-                    for _, ii_line_var in pipe_linear_line_segment.items():
-                        # Create integer variable to activate/deactivate (1/0) a linear line
-                        # segment
-                        is_line_segment_active_var = optimization_problem.state_vector(ii_line_var)
-
-                        # Linear line segment activation variable for each time step of demand
-                        # profile
-                        is_line_segment_active.append(is_line_segment_active_var)
-
-                    # Calculate constraint to enforce that only 1 linear line segment can be active
-                    # per time step for the current pipe for the entire time horizon
-                    for itstep in range(n_timesteps):
-                        is_line_segment_active_sum_per_timestep = 0.0
-                        for ii_line in range(len(pipe_linear_line_segment)):
-
-                            is_line_segment_active_sum_per_timestep = (
-                                is_line_segment_active_sum_per_timestep
-                                + is_line_segment_active[ii_line][itstep]
-                            )
-                        constraints.append(
-                            (is_line_segment_active_sum_per_timestep, 1.0, 1.0),
-                        )
-
-                    # Add equality constraint, value == 0.0 for all linear lines
-                    # Loop twice due to linear lines exsiting for negative and positive discharge
-                    # ii==0: this is the linear lines for the negative discharge possibility
-                    # ii==1: this is the linear lines for the postive discharge possibility
-                    for ii in range(2):
-                        for ii_line in range(n_linear_lines):
-                            ii_line_used = (ii * 2) + ii_line
-
-                            ii_start = (ii_line + 2 * ii) * n_timesteps
-                            ii_end = ii_start + n_timesteps
-                            constraints.append(
-                                (
-                                    (
-                                        head_loss_vec[ii_start:ii_end]
-                                        - (
-                                            a_vec[ii_start:ii_end] * discharge_vec[ii_start:ii_end]
-                                            + b_vec[ii_start:ii_end]
-                                        )
-                                        + is_disconnected_vec[ii_start:ii_end] * big_m_lin
-                                        + big_m_lin
-                                        * (1 - is_line_segment_active[ii_line_used][0:n_timesteps])
-                                    )
-                                    / constraint_nominal[ii_start:ii_end],
-                                    0.0,
-                                    np.inf,
-                                ),
-                            )
-                    for ii in range(2):
-                        for ii_line in range(n_linear_lines):
-                            ii_line_used = (ii * 2) + ii_line
-
-                            ii_start = (ii_line + 2 * ii) * n_timesteps
-                            ii_end = ii_start + n_timesteps
-                            constraints.append(
-                                (
-                                    (
-                                        head_loss_vec[ii_start:ii_end]
-                                        - (
-                                            a_vec[ii_start:ii_end] * discharge_vec[ii_start:ii_end]
-                                            + b_vec[ii_start:ii_end]
-                                        )
-                                        - is_disconnected_vec[ii_start:ii_end] * big_m_lin
-                                        - big_m_lin
-                                        * (1 - is_line_segment_active[ii_line_used][0:n_timesteps])
-                                    )
-                                    / constraint_nominal[ii_start:ii_end],
-                                    -np.inf,
-                                    0.0,
-                                ),
-                            )
-                return constraints
+                    )
+                ]
             else:
                 ret = np.amax(a * np.tile(discharge, (len(a), 1)).transpose() + b, axis=1)
                 if isinstance(discharge, float):
                     ret = ret[0]
                 return ret
 
     def _hydraulic_power(
         self,
         pipe: str,
-        optimization_problem,
-        energy_system_options,
-        network_settings,
+        heat_network_options,
         parameters,
         discharge: Union[ca.MX, float, np.ndarray],
         hydraulic_power: Optional[Union[ca.MX, float, np.ndarray]] = None,
         dh: Optional[ca.MX] = None,
         is_disconnected: Union[ca.MX, int] = 0,
         big_m: Optional[float] = None,
         pipe_class: Optional[PipeClass] = None,
         flow_dir: Union[ca.MX, int] = 0,
-        network_type: NetworkSettings = NetworkSettings.NETWORK_TYPE_HEAT,
-        pressure: float = 0.0,
     ) -> Union[List[Tuple[ca.MX, BT, BT]], float, np.ndarray]:
         """
         This function has two purposes:
         - return the hydraulic power constraint expression(s) or
         - compute the hydraulic power numerically (always positive).
 
         Note: the discharge value can be negative. In such a case the hydraulic_power in the
@@ -905,15 +707,17 @@
         """
 
         if hydraulic_power is None:
             symbolic = False
         else:
             symbolic = True
 
-        head_loss_option = network_settings["head_loss_option"]
+        head_loss_option = self._hn_get_pipe_head_loss_option(
+            pipe, heat_network_options, parameters
+        )
         assert (
             head_loss_option != HeadLossOption.NO_HEADLOSS
         ), "This method should be skipped when NO_HEADLOSS is set."
 
         length = parameters[f"{pipe}.length"]
 
         if length == 0.0:
@@ -938,53 +742,39 @@
                 return 0.0
 
         if big_m is None:
             assert is_disconnected == 0.0
         else:
             assert big_m != 0.0
 
-        wall_roughness = energy_system_options["wall_roughness"]
+        wall_roughness = heat_network_options["wall_roughness"]
         temperature = parameters[f"{pipe}.temperature"]
-        for _id, attr in optimization_problem.temperature_carriers().items():
-            if (
-                parameters[f"{pipe}.carrier_id"] == attr["id_number_mapping"]
-                and len(optimization_problem.temperature_regimes(parameters[f"{pipe}.carrier_id"]))
-                > 0
-            ):
-                temperature = min(
-                    optimization_problem.temperature_regimes(parameters[f"{pipe}.carrier_id"])
-                )
         rho = parameters[f"{pipe}.rho"]
 
         if pipe_class is not None:
             diameter = pipe_class.inner_diameter
             area = pipe_class.area
             maximum_velocity = pipe_class.maximum_velocity
         else:
             diameter = parameters[f"{pipe}.diameter"]
             area = parameters[f"{pipe}.area"]
-            maximum_velocity = network_settings["maximum_velocity"]
+            maximum_velocity = heat_network_options["maximum_velocity"]
 
         constraint_nominal = abs(
             parameters[f"{pipe}.rho"]
             * GRAVITATIONAL_CONSTANT
-            * optimization_problem.variable_nominal(f"{pipe}.dH")
-            * optimization_problem.variable_nominal(f"{pipe}.Q")
+            * self.variable_nominal(f"{pipe}.dH")
+            * self.variable_nominal(f"{pipe}.Q")
         )
 
         if head_loss_option == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY:
             # Uitlized maximum_velocity instead of estimated_velocity (used in head loss linear
             # calc)
             ff = darcy_weisbach.friction_factor(
-                maximum_velocity,
-                diameter,
-                wall_roughness,
-                temperature,
-                network_type=network_type,
-                pressure=pressure,
+                maximum_velocity, diameter, wall_roughness, temperature
             )
             # Compute c_k constant (where |hydraulic power| ~ c_k * v^3)
             c_k = rho * ff * length * area / 2.0 / diameter
             # Compute linearized value
             max_hydraulic_power = c_k * maximum_velocity**3
             maximum_discharge = maximum_velocity * area
             hydraulic_power_linearized = max_hydraulic_power * discharge / maximum_discharge
@@ -1046,29 +836,24 @@
                             -np.inf,
                             0.0,
                         ),
                     ]
             else:
                 return abs(hydraulic_power_linearized)
 
-        elif (
-            head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
-            or HeadLossOption.LINEARIZED_N_LINES_EQUALITY
-        ):
-            n_lines = network_settings["n_linearization_lines"]
+        elif head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY:
+            n_lines = heat_network_options["n_linearization_lines"]
             a_coef, b_coef = darcy_weisbach.get_linear_pipe_power_hydraulic_vs_q_fit(
                 rho,
                 diameter,
                 length,
                 wall_roughness,
                 temperature=temperature,
                 n_lines=n_lines,
                 v_max=maximum_velocity,
-                network_type=self.network_settings["network_type"],
-                pressure=parameters[f"{pipe}.pressure"],
             )
             discharge_vec = ca.repmat(discharge, len(a_coef))
             hydraulic_power_linearized_vec = a_coef * discharge_vec + b_coef
 
             if symbolic:
                 hydraulic_power_vec = ca.repmat(hydraulic_power, len(a_coef))
 
@@ -1118,63 +903,211 @@
                 if isinstance(discharge, float):
                     max_hydraulic_power_linearized = max_hydraulic_power_linearized[0]
                 return abs(max_hydraulic_power_linearized)
         else:
             assert (
                 head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
                 or head_loss_option == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY
-                or head_loss_option == HeadLossOption.LINEARIZED_N_LINES_EQUALITY
-            ), "This method only caters for head_loss_option: "
-            "LINEARIZED_ONE_LINE_EQUALITY & LINEARIZED_N_LINES_WEAK_INEQUALITY."
+            ), "This method only caters for head_loss_option: LINEARIZED_ONE_LINE_EQUALITY &"
+            "LINEARIZED_N_LINES_WEAK_INEQUALITY."
 
-    def _pipe_head_loss_path_constraints(self, optimization_problem, _ensemble_member):
+    def __pipe_head_loss_path_constraints(self, _ensemble_member):
         """
         We set this constraint relating .dH to the upstream and downstream
         heads here in the Mixin for scaling purposes (dH nominal is
         calculated in pre()).
         """
         constraints = []
 
-        pipe_type = "heat_pipe"
-        commodity = "Heat"
-        if len(optimization_problem.energy_system_components.get(pipe_type, [])) == 0:
-            pipe_type = "gas_pipe"
-            commodity = NetworkSettings.NETWORK_TYPE_GAS
-
-        for pipe in optimization_problem.energy_system_components.get(pipe_type, []):
-            dh = optimization_problem.state(f"{pipe}.dH")
-            h_down = optimization_problem.state(f"{pipe}.{commodity}Out.H")
-            h_up = optimization_problem.state(f"{pipe}.{commodity}In.H")
+        for pipe in self.energy_system_components.get("pipe", []):
+            dh = self.state(f"{pipe}.dH")
+            h_down = self.state(f"{pipe}.HeatOut.H")
+            h_up = self.state(f"{pipe}.HeatIn.H")
 
             constraint_nominal = (
-                optimization_problem.variable_nominal(f"{pipe}.dH")
-                * optimization_problem.variable_nominal(f"{pipe}.{commodity}In.H")
+                self.variable_nominal(f"{pipe}.dH") * self.variable_nominal(f"{pipe}.HeatIn.H")
             ) ** 0.5
             constraints.append(((dh - (h_down - h_up)) / constraint_nominal, 0.0, 0.0))
 
         return constraints
 
-    def _demand_head_loss_path_constraints(self, optimization_problem, _ensemble_member):
+    def __demand_head_loss_path_constraints(self, _ensemble_member):
         """
         This function adds constraints for a minimum pressure drop at demands. This minimum
         pressure drop is often required in practice to guarantee that it is possible to increase
         the flow rate at that specific demand, if needed, by opening the control valve.
         """
         constraints = []
 
-        options = optimization_problem.energy_system_options()
-        components = optimization_problem.energy_system_components
+        options = self.heat_network_options()
+        components = self.energy_system_components
 
         # Convert minimum pressure at far point from bar to meter (water) head
         min_head_loss = options["minimum_pressure_far_point"] * 10.2
 
-        for d in components.get("heat_demand", []):
+        for d in components.get("demand", []):
             constraints.append(
                 (
-                    optimization_problem.state(f"{d}.HeatIn.H")
-                    - optimization_problem.state(f"{d}.HeatOut.H"),
+                    self.state(f"{d}.HeatIn.H") - self.state(f"{d}.HeatOut.H"),
                     min_head_loss,
                     np.inf,
                 )
             )
 
         return constraints
+
+    def constraints(self, ensemble_member):
+        """
+        Here we add the pipe head loss constraints
+        """
+        constraints = super().constraints(ensemble_member)
+
+        if self.heat_network_options()["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
+            constraints.extend(self._hn_pipe_head_loss_constraints(ensemble_member))
+
+        return constraints
+
+    def path_constraints(self, ensemble_member):
+        """
+        Here we add the path constraints for the head in pipes and minimum pressure drop at demands.
+        """
+        constraints = super().path_constraints(ensemble_member).copy()
+
+        options = self.heat_network_options()
+
+        # Add source/demand head loss constrains only if head loss is non-zero
+        if options["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
+            constraints.extend(self.__pipe_head_loss_path_constraints(ensemble_member))
+            constraints.extend(self.__demand_head_loss_path_constraints(ensemble_member))
+
+        return constraints
+
+    def priority_started(self, priority):
+        """
+        Keeping track of the priority in the optimization
+        """
+        super().priority_started(priority)
+        self.__priority = priority
+
+    def priority_completed(self, priority):
+        """
+        In this funtion we check whether there is still artificial head loss in pipes after the
+        head loss minimization goal. This can happen when there are multiple routes without control
+        valves towards a single consumer.In this case the optimization can create non-physical
+        solutions for the inequality head loss options where it favours one route above another.
+        This favoured route would also have a head loss which would not possible in practice and
+        could not be compensated for by a control valve along the route.
+        """
+        super().priority_completed(priority)
+
+        options = self.heat_network_options()
+
+        if (
+            options["minimize_head_losses"]
+            and options["head_loss_option"] != HeadLossOption.NO_HEADLOSS
+            and priority == self._hn_minimization_goal_class.priority
+        ):
+            components = self.energy_system_components
+
+            rtol = 1e-5
+            atol = 1e-4
+
+            for ensemble_member in range(self.ensemble_size):
+                parameters = self.parameters(ensemble_member)
+                results = self.extract_results(ensemble_member)
+
+                for pipe in components["pipe"]:
+                    if parameters[f"{pipe}.has_control_valve"]:
+                        continue
+
+                    # Just like with a control valve, if pipe is disconnected
+                    # there is nothing to check.
+                    q_full = results[f"{pipe}.Q"]
+                    if parameters[f"{pipe}.disconnectable"]:
+                        inds = q_full != 0.0
+                    else:
+                        inds = np.arange(len(q_full), dtype=int)
+
+                    if parameters[f"{pipe}.diameter"] == 0.0:
+                        # Pipe is disconnected. Head loss is free, so nothing to check.
+                        continue
+
+                    q = results[f"{pipe}.Q"][inds]
+                    head_loss_target = self._hn_pipe_head_loss(pipe, options, parameters, q, None)
+                    if options["head_loss_option"] == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY:
+                        head_loss = np.abs(results[f"{pipe}.dH"][inds])
+                    else:
+                        head_loss = results[self._hn_pipe_to_head_loss_map[pipe]][inds]
+
+                    if not np.allclose(head_loss, head_loss_target, rtol=rtol, atol=atol):
+                        logger.warning(
+                            f"Pipe {pipe} has artificial head loss; "
+                            f"at least one more control valve should be added to the network."
+                        )
+
+                min_head_loss_target = options["minimum_pressure_far_point"] * 10.2
+                min_head_loss = None
+
+                for demand in components["demand"]:
+                    head_loss = results[f"{demand}.HeatIn.H"] - results[f"{demand}.HeatOut.H"]
+                    if min_head_loss is None:
+                        min_head_loss = head_loss
+                    else:
+                        min_head_loss = np.minimum(min_head_loss, head_loss)
+
+                if not np.allclose(min_head_loss, min_head_loss_target, rtol=rtol, atol=atol):
+                    logger.warning("Minimum head at demands is higher than target minimum.")
+
+    def path_goals(self):
+        """
+        Here we add the goals for minimizing the head loss and hydraulic power depending on the
+        configuration. Please note that we only do hydraulic power for the MILP problem thus only
+        for the linearized head_loss options.
+        """
+        g = super().path_goals().copy()
+
+        options = self.heat_network_options()
+        if (
+            options["minimize_head_losses"]
+            and options["head_loss_option"] != HeadLossOption.NO_HEADLOSS
+        ):
+            g.append(self._hn_minimization_goal_class(self))
+
+            if (
+                options["head_loss_option"] == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY
+                or options["head_loss_option"] == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
+            ):
+                g.append(self._hpwr_minimization_goal_class(self))
+
+        return g
+
+    @property
+    def path_variables(self):
+        """
+        Here we add the pipe head loss path-variables to the problem.
+        """
+        variables = super().path_variables.copy()
+        variables.extend(self.__pipe_head_loss_var.values())
+        return variables
+
+    def variable_nominal(self, variable):
+        """
+        Here we add the nominal for the head loss path-variable to the problem.
+        """
+        try:
+            return self.__pipe_head_loss_nominals[variable]
+        except KeyError:
+            return super().variable_nominal(variable)
+
+    def bounds(self):
+        """
+        Here we add the bounds for the head loss variable to the problem.
+        """
+        bounds = super().bounds().copy()
+
+        bounds.update(self.__pipe_head_loss_bounds)
+        bounds.update(self.__pipe_head_loss_zero_bounds)
+
+        for k, v in self.__pipe_head_bounds.items():
+            bounds[k] = self.merge_bounds(bounds[k], v)
+
+        return bounds
```

### Comparing `mesido-0.1.1/src/mesido/heat_network_common.py` & `mesido-0.1.2/src/mesido/heat_network_common.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/heat_physics_mixin.py` & `mesido-0.1.2/src/mesido/heat_physics_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import math
 from typing import List
 
 import casadi as ca
 
 from mesido._heat_loss_u_values_pipe import pipe_heat_loss
 from mesido.base_component_type_mixin import BaseComponentTypeMixin
-from mesido.constants import GRAVITATIONAL_CONSTANT
 from mesido.demand_insulation_class import DemandInsulationClass
 from mesido.head_loss_class import HeadLossClass, HeadLossOption
 from mesido.network_common import NetworkSettings
 
 import numpy as np
 
 from rtctools.optimization.collocated_integrated_optimization_problem import (
@@ -113,22 +112,22 @@
         self.__pipe_head_loss_var = {}
         self.__pipe_head_loss_bounds = {}
         self.__pipe_head_loss_nominals = {}
         self.__pipe_head_loss_zero_bounds = {}
         self._hn_pipe_to_head_loss_map = {}
 
         # Boolean path-variable for the direction of the flow, inport to outport is positive flow.
-        self.__flow_direct_var = {}
-        self.__flow_direct_bounds = {}
-        self._pipe_to_flow_direct_map = {}
+        self.__heat_flow_direct_var = {}
+        self.__heat_flow_direct_bounds = {}
+        self._heat_pipe_to_flow_direct_map = {}
 
         # Boolean path-variable to determine whether flow is going through a pipe.
-        self.__pipe_disconnect_var = {}
-        self.__pipe_disconnect_var_bounds = {}
-        self._pipe_disconnect_map = {}
+        self.__heat_pipe_disconnect_var = {}
+        self.__heat_pipe_disconnect_var_bounds = {}
+        self._heat_pipe_disconnect_map = {}
 
         # Boolean path-variable for the status of the check valve
         self.__check_valve_status_var = {}
         self.__check_valve_status_var_bounds = {}
         self.__check_valve_status_map = {}
 
         # Boolean path-variable for the status of the control valve
@@ -196,15 +195,15 @@
         # Dict to write the heat loss in the parameters
         self.__pipe_heat_loss_parameters = []
 
         # Part of the physics constraints are inherently linked to the sizing optimization. Since
         # these variables do not exist here, we instead only instantiate the maps to allow the
         # physics mixin to have the logic in place. The creation of the actual variables and filling
         # of these maps is in the AssetSizingMixin.
-        self._pipe_topo_pipe_class_map = {}
+        self._heat_pipe_topo_pipe_class_map = {}
 
         super().__init__(*args, **kwargs)
 
     def temperature_carriers(self):
         """
         This function should be overwritten by the problem and should give a dict with the
         carriers as keys and a list of temperatures as values.
@@ -292,47 +291,47 @@
 
             neighbour = self.has_related_pipe(pipe_name)
             if neighbour and pipe_name not in self.hot_pipes:
                 flow_dir_var = f"{self.cold_to_hot_pipe(pipe_name)}__flow_direct_var"
             else:
                 flow_dir_var = f"{pipe_name}__flow_direct_var"
 
-            self._pipe_to_flow_direct_map[pipe_name] = flow_dir_var
-            self.__flow_direct_var[flow_dir_var] = ca.MX.sym(flow_dir_var)
+            self._heat_pipe_to_flow_direct_map[pipe_name] = flow_dir_var
+            self.__heat_flow_direct_var[flow_dir_var] = ca.MX.sym(flow_dir_var)
 
             # Fix the directions that are already implied by the bounds on heat
             # Nonnegative heat implies that flow direction Boolean is equal to one.
             # Nonpositive heat implies that flow direction Boolean is equal to zero.
 
             heat_in_lb = _get_min_bound(bounds[f"{pipe_name}.HeatIn.Heat"][0])
             heat_in_ub = _get_max_bound(bounds[f"{pipe_name}.HeatIn.Heat"][1])
             heat_out_lb = _get_min_bound(bounds[f"{pipe_name}.HeatOut.Heat"][0])
             heat_out_ub = _get_max_bound(bounds[f"{pipe_name}.HeatOut.Heat"][1])
 
             if (heat_in_lb >= 0.0 and heat_in_ub >= 0.0) or (
                 heat_out_lb >= 0.0 and heat_out_ub >= 0.0
             ):
-                self.__flow_direct_bounds[flow_dir_var] = (1.0, 1.0)
+                self.__heat_flow_direct_bounds[flow_dir_var] = (1.0, 1.0)
             elif (heat_in_lb <= 0.0 and heat_in_ub <= 0.0) or (
                 heat_out_lb <= 0.0 and heat_out_ub <= 0.0
             ):
-                self.__flow_direct_bounds[flow_dir_var] = (0.0, 0.0)
+                self.__heat_flow_direct_bounds[flow_dir_var] = (0.0, 0.0)
             else:
-                self.__flow_direct_bounds[flow_dir_var] = (0.0, 1.0)
+                self.__heat_flow_direct_bounds[flow_dir_var] = (0.0, 1.0)
 
             if parameters[f"{pipe_name}.disconnectable"]:
                 neighbour = self.has_related_pipe(pipe_name)
                 if neighbour and pipe_name not in self.hot_pipes:
                     disconnected_var = f"{self.cold_to_hot_pipe(pipe_name)}__is_disconnected"
                 else:
                     disconnected_var = f"{pipe_name}__is_disconnected"
 
-                self._pipe_disconnect_map[pipe_name] = disconnected_var
-                self.__pipe_disconnect_var[disconnected_var] = ca.MX.sym(disconnected_var)
-                self.__pipe_disconnect_var_bounds[disconnected_var] = (0.0, 1.0)
+                self._heat_pipe_disconnect_map[pipe_name] = disconnected_var
+                self.__heat_pipe_disconnect_var[disconnected_var] = ca.MX.sym(disconnected_var)
+                self.__heat_pipe_disconnect_var_bounds[disconnected_var] = (0.0, 1.0)
 
             if heat_in_ub <= 0.0 and heat_out_lb >= 0.0:
                 raise Exception(f"Heat flow rate in/out of pipe '{pipe_name}' cannot be zero.")
 
         # Integers for disabling the HEX temperature constraints
         for hex in [
             *self.energy_system_components.get("heat_exchanger", []),
@@ -632,16 +631,16 @@
         """
         In this function we add all the path variables defined in the HeatMixin to the
         optimization problem. Note that path_variables are variables that are created for each
         time-step.
         """
         variables = super().path_variables.copy()
         variables.extend(self.__pipe_head_loss_var.values())
-        variables.extend(self.__flow_direct_var.values())
-        variables.extend(self.__pipe_disconnect_var.values())
+        variables.extend(self.__heat_flow_direct_var.values())
+        variables.extend(self.__heat_pipe_disconnect_var.values())
         variables.extend(self.__check_valve_status_var.values())
         variables.extend(self.__control_valve_direction_var.values())
         variables.extend(self.__demand_insulation_class_var.values())
         variables.extend(self.__pipe_linear_line_segment_var.values())
         variables.extend(self.__temperature_regime_var.values())
         variables.extend(self.__carrier_selected_var.values())
         variables.extend(self.__ates_temperature_disc_var.values())
@@ -654,16 +653,16 @@
         return variables
 
     def variable_is_discrete(self, variable):
         """
         All variables that only can take integer values should be added to this function.
         """
         if (
-            variable in self.__flow_direct_var
-            or variable in self.__pipe_disconnect_var
+            variable in self.__heat_flow_direct_var
+            or variable in self.__heat_pipe_disconnect_var
             or variable in self.__check_valve_status_var
             or variable in self.__control_valve_direction_var
             or variable in self.__demand_insulation_class_var
             or variable in self.__pipe_linear_line_segment_var
             or variable in self.__carrier_selected_var
             or variable in self.__ates_temperature_selected_var
             or variable in self.__disabled_hex_var
@@ -690,16 +689,16 @@
 
     def bounds(self):
         """
         In this function we add the bounds to the problem for all the variables defined/added in
         the HeatMixin.
         """
         bounds = super().bounds()
-        bounds.update(self.__flow_direct_bounds)
-        bounds.update(self.__pipe_disconnect_var_bounds)
+        bounds.update(self.__heat_flow_direct_bounds)
+        bounds.update(self.__heat_pipe_disconnect_var_bounds)
         bounds.update(self.__check_valve_status_var_bounds)
         bounds.update(self.__control_valve_direction_var_bounds)
         bounds.update(self.__buffer_t0_bounds)
         bounds.update(self.__demand_insulation_class_var_bounds)
         bounds.update(self.__pipe_linear_line_segment_var_bounds)
         bounds.update(self._pipe_heat_loss_var_bounds)
         bounds.update(self.__temperature_regime_var_bounds)
@@ -987,15 +986,15 @@
         hn_options = self.energy_system_options()
 
         t_change = hn_options["maximum_temperature_der"]
         q_change = hn_options["maximum_flow_der"]
 
         if np.isfinite(t_change) and np.isfinite(q_change):
             assert (
-                not self._pipe_topo_pipe_class_map
+                not self._heat_pipe_topo_pipe_class_map
             ), "heat rate change constraints not allowed with topology optimization"
 
         for p in self.energy_system_components.get("heat_pipe", []):
             variable = f"{p}.HeatIn.Heat"
             dt = np.diff(self.times(variable))
 
             canonical, sign = self.alias_relation.canonical_signed(variable)
@@ -1132,15 +1131,15 @@
                     (
                         *self.bounds()[f"{p}.HeatIn.Heat"],
                         *self.bounds()[f"{p}.HeatOut.Heat"],
                     )
                 )
             )
 
-            is_disconnected_var = self._pipe_disconnect_map.get(p)
+            is_disconnected_var = self._heat_pipe_disconnect_map.get(p)
 
             if is_disconnected_var is None:
                 is_disconnected = 0.0
             else:
                 is_disconnected = self.state(is_disconnected_var)
 
             if p in self._pipe_heat_loss_map:
@@ -1221,32 +1220,32 @@
         parameters = self.parameters(ensemble_member)
 
         minimum_velocity = self.heat_network_settings["minimum_velocity"]
         maximum_velocity = self.heat_network_settings["maximum_velocity"]
 
         # Also ensure that the discharge has the same sign as the heat.
         for p in self.energy_system_components.get("heat_pipe", []):
-            flow_dir_var = self._pipe_to_flow_direct_map[p]
+            flow_dir_var = self._heat_pipe_to_flow_direct_map[p]
             flow_dir = self.state(flow_dir_var)
 
-            is_disconnected_var = self._pipe_disconnect_map.get(p)
+            is_disconnected_var = self._heat_pipe_disconnect_map.get(p)
 
             if is_disconnected_var is None:
                 is_disconnected = 0.0
             else:
                 is_disconnected = self.state(is_disconnected_var)
 
             q_pipe = self.state(f"{p}.Q")
             heat_in = self.state(f"{p}.HeatIn.Heat")
             heat_out = self.state(f"{p}.HeatOut.Heat")
 
             try:
-                pipe_classes = self._pipe_topo_pipe_class_map[p].keys()
+                pipe_classes = self._heat_pipe_topo_pipe_class_map[p].keys()
                 maximum_discharge = max([c.maximum_discharge for c in pipe_classes])
-                var_names = self._pipe_topo_pipe_class_map[p].values()
+                var_names = self._heat_pipe_topo_pipe_class_map[p].values()
                 dn_none = 0.0
                 for i, pc in enumerate(pipe_classes):
                     if pc.inner_diameter == 0.0:
                         dn_none = self.variable(list(var_names)[i])
                 minimum_discharge = min(
                     [c.area * minimum_velocity for c in pipe_classes if c.area > 0.0]
                 )
@@ -1348,18 +1347,18 @@
             if len(pipes) <= 1:
                 continue
 
             assert (
                 len({p for p in pipes if self.is_cold_pipe(p)}) == 0
             ), "Pipe series for Heat models should only contain hot pipes"
 
-            base_flow_dir_var = self.state(self._pipe_to_flow_direct_map[pipes[0]])
+            base_flow_dir_var = self.state(self._heat_pipe_to_flow_direct_map[pipes[0]])
 
             for p in pipes[1:]:
-                flow_dir_var = self.state(self._pipe_to_flow_direct_map[p])
+                flow_dir_var = self.state(self._heat_pipe_to_flow_direct_map[p])
                 constraints.append((base_flow_dir_var - flow_dir_var, 0.0, 0.0))
 
         return constraints
 
     def __demand_heat_to_discharge_path_constraints(self, ensemble_member):
         """
         This function adds constraints linking the flow to the thermal power at the demand assets.
@@ -1368,15 +1367,18 @@
         in the pipes. This means that the heat can decrease in the network to compensate losses,
         but that the losses and thus flow will always be over-estimated with the temperature for
         which no temperature drops are modelled.
         """
         constraints = []
         parameters = self.parameters(ensemble_member)
 
-        for d in self.energy_system_components.get("heat_demand", []):
+        for d in [
+            *self.energy_system_components.get("heat_demand", []),
+            *self.energy_system_components.get("airco", []),
+        ]:
             heat_nominal = parameters[f"{d}.Heat_nominal"]
             cp = parameters[f"{d}.cp"]
             rho = parameters[f"{d}.rho"]
             discharge = self.state(f"{d}.Q")
             heat_out = self.state(f"{d}.HeatOut.Heat")
 
             ret_carrier = parameters[f"{d}.T_return_id"]
@@ -1553,123 +1555,14 @@
                             -np.inf,
                             0.0,
                         )
                     )
 
         return constraints
 
-    def __pipe_hydraulic_power_path_constraints(self, ensemble_member):
-        """
-        This function adds constraints to compute the hydraulic power that is needed to realize the
-        flow, compensating the pressure drop through the pipe. Similar to the head loss constraints
-        we allow two supported methods. 1) a single linear line between 0 to max velocity. 2) A
-        multiple line inequality approach where one can use the minimize_head_losses == True option
-        to drag down the solution to the actual physical solution.
-
-        Note that the linearizations are made separately from the pressure drop constraints, this is
-        done to avoid "stacked" overestimations.
-        """
-        constraints = []
-        options = self.energy_system_options()
-
-        if self.heat_network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
-            parameters = self.parameters(ensemble_member)
-            components = self.energy_system_components
-
-            for pipe in components.get("heat_pipe", []):
-                if parameters[f"{pipe}.length"] == 0.0:
-                    # If the pipe does not have a control valve, the head loss is
-                    # forced to zero via bounds. If the pipe _does_ have a control
-                    # valve, then there still is no relationship between the
-                    # discharge and the hydraulic_power.
-                    continue
-
-                head_loss_option = self._hn_get_pipe_head_loss_option(
-                    pipe, self.heat_network_settings, parameters
-                )
-                assert (
-                    head_loss_option != HeadLossOption.NO_HEADLOSS
-                ), "This method should be skipped when NO_HEADLOSS is set."
-
-                discharge = self.state(f"{pipe}.Q")
-                hydraulic_power = self.state(f"{pipe}.Hydraulic_power")
-                rho = parameters[f"{pipe}.rho"]
-
-                # 0: pipe is connected, 1: pipe is disconnected
-                is_disconnected_var = self._pipe_disconnect_map.get(pipe)
-                if is_disconnected_var is None:
-                    is_disconnected = 0.0
-                else:
-                    is_disconnected = self.state(is_disconnected_var)
-
-                flow_dir_var = self._pipe_to_flow_direct_map[pipe]
-                flow_dir = self.state(flow_dir_var)  # 0/1: negative/positive flow direction
-
-                if pipe in self._pipe_topo_pipe_class_map:
-                    # Multiple diameter options for this pipe
-                    pipe_classes = self._pipe_topo_pipe_class_map[pipe]
-                    max_discharge = max(c.maximum_discharge for c in pipe_classes)
-                    for pc, pc_var_name in pipe_classes.items():
-                        if pc.inner_diameter == 0.0:
-                            continue
-
-                        # Calc max hydraulic power based on maximum_total_head_loss =
-                        # f(max_sum_dh_pipes, max_dh_network_options)
-                        max_total_hydraulic_power = 2.0 * (
-                            rho
-                            * GRAVITATIONAL_CONSTANT
-                            * self.__maximum_total_head_loss
-                            * max_discharge
-                        )
-
-                        # is_topo_disconnected - 0: pipe selected, 1: pipe disconnected/not selected
-                        # self.__pipe_topo_pipe_class_var - value 0: pipe is not selected, 1: pipe
-                        # is selected
-                        is_topo_disconnected = 1 - self.variable(pc_var_name)
-
-                        constraints.extend(
-                            self._hn_head_loss_class._hydraulic_power(
-                                pipe,
-                                self,
-                                options,
-                                self.heat_network_settings,
-                                parameters,
-                                discharge,
-                                hydraulic_power,
-                                is_disconnected=is_topo_disconnected + is_disconnected,
-                                big_m=max_total_hydraulic_power,
-                                pipe_class=pc,
-                                flow_dir=flow_dir,
-                            )
-                        )
-                else:
-                    is_topo_disconnected = int(parameters[f"{pipe}.diameter"] == 0.0)
-                    max_total_hydraulic_power = 2.0 * (
-                        rho
-                        * GRAVITATIONAL_CONSTANT
-                        * self.__maximum_total_head_loss
-                        * parameters[f"{pipe}.area"]
-                        * self.heat_network_settings["maximum_velocity"]
-                    )
-                    constraints.extend(
-                        self._hn_head_loss_class._hydraulic_power(
-                            pipe,
-                            self,
-                            options,
-                            self.heat_network_settings,
-                            parameters,
-                            discharge,
-                            hydraulic_power,
-                            is_disconnected=is_disconnected + is_topo_disconnected,
-                            big_m=max_total_hydraulic_power,
-                            flow_dir=flow_dir,
-                        )
-                    )
-        return constraints
-
     def __pipe_heat_to_discharge_path_constraints(self, ensemble_member):
         """
         This function adds constraints linking the flow to the thermal power at the pipe assets.
         We use an equality constraint on the outgoing flow for every non-pipe asset. Meaning that we
         equate Q * rho * cp * T == Heat for outgoing flows, and inequalities for the heat carried
         in the pipes. This means that the heat can decrease in the network to compensate losses,
         but that the losses and thus flow will always be over-estimated with the temperature for
@@ -1698,15 +1591,15 @@
             cp = parameters[f"{p}.cp"]
             rho = parameters[f"{p}.rho"]
             # Note that during cold delivery the line can be colder than the ground temperature.
             # In this case we have to bound the heat flowing in the line with the ground
             # temperature instead, as the line can heat up to at maximum the ground temperature.
             temp = max(parameters[f"{p}.temperature"], parameters[f"{p}.T_ground"])
 
-            flow_dir_var = self._pipe_to_flow_direct_map[p]
+            flow_dir_var = self._heat_pipe_to_flow_direct_map[p]
             flow_dir = self.state(flow_dir_var)
             scaled_heat_in = self.state(f"{p}.HeatIn.Heat")  # * heat_to_discharge_fac
             scaled_heat_out = self.state(f"{p}.HeatOut.Heat")  # * heat_to_discharge_fac
             pipe_q = self.state(f"{p}.Q")
             heat_nominal = self.variable_nominal(f"{p}.HeatIn.Heat")
 
             # We do not want Big M to be too tight in this case, as it results
@@ -1861,15 +1754,15 @@
             (hot_pipe, _hot_pipe_orientation),
             (_cold_pipe, _cold_pipe_orientation),
         ) in {**self.energy_system_topology.ates}.items():
 
             if ates_asset in self.energy_system_components.get("low_temperature_ates", []):
                 continue
 
-            flow_dir_var = self._pipe_to_flow_direct_map[hot_pipe]
+            flow_dir_var = self._heat_pipe_to_flow_direct_map[hot_pipe]
             is_buffer_charging = self.state(flow_dir_var) * _hot_pipe_orientation
 
             sup_carrier = parameters[f"{ates_asset}.T_supply_id"]
             supply_temperatures = self.temperature_regimes(sup_carrier)
             ates_temperature = self.state(f"{ates_asset}.Temperature_ates")
             ates_temperature_disc = self.state(f"{ates_asset}__temperature_ates_disc")
 
@@ -2145,15 +2038,15 @@
             if options["include_ates_temperature_options"] and len(supply_temperatures) != 0:
                 soil_temperature = parameters[f"{ates}.T_amb"]
                 ates_temperature_loss_nominal = self.variable_nominal(f"{ates}.Temperature_loss")
                 ates_dt_charging_nominal = self.variable_nominal(
                     f"{ates}.Temperature_change_charging"
                 )
 
-                flow_dir_var = self._pipe_to_flow_direct_map[hot_pipe]
+                flow_dir_var = self._heat_pipe_to_flow_direct_map[hot_pipe]
                 is_buffer_charging = self.state(flow_dir_var) * _hot_pipe_orientation
                 heat_stored_max = bounds[f"{ates}.Stored_heat"][1]
                 heat_ates_max = bounds[f"{ates}.Heat_ates"][1]
                 heat_ates = self.state(f"{ates}.Heat_ates")
                 stored_heat = self.state(f"{ates}.Stored_heat")
 
                 big_m = 2.0 * max(bounds[f"{ates}.Temperature_change_charging"][1], 1e-5)
@@ -2388,15 +2281,15 @@
 
             # We want an _equality_ constraint between discharge and heat if the buffer is
             # consuming (i.e. behaving like a "demand"). We want an _inequality_
             # constraint (`|heat| >= |f(Q)|`) just like a "heat_source" component if heat is
             # extracted from the buffer. We accomplish this by disabling one of
             # the constraints with a boolean. Note that `discharge` and `heat_hot`
             # are guaranteed to have the same sign.
-            flow_dir_var = self._pipe_to_flow_direct_map[hot_pipe]
+            flow_dir_var = self._heat_pipe_to_flow_direct_map[hot_pipe]
             is_buffer_charging = self.state(flow_dir_var)
 
             big_m = 2.0 * np.max(
                 np.abs((*self.bounds()[f"{b}.HeatIn.Heat"], *self.bounds()[f"{b}.HeatOut.Heat"]))
             )
 
             sup_carrier = parameters[f"{b}.T_supply_id"]
@@ -2872,15 +2765,15 @@
         )
 
     def _hn_pipe_nominal_discharge(self, energy_system_options, parameters, pipe: str) -> float:
         """
         This functions returns a nominal for the discharge of pipes under topology optimization.
         """
         try:
-            pipe_classes = self._pipe_topo_pipe_class_map[pipe].keys()
+            pipe_classes = self._heat_pipe_topo_pipe_class_map[pipe].keys()
             area = np.median(c.area for c in pipe_classes)
         except KeyError:
             area = parameters[f"{pipe}.area"]
 
         return area * energy_system_options["estimated_velocity"]
 
     @staticmethod
@@ -2897,182 +2790,14 @@
         ):
             # If there is a control valve present, we use the more accurate
             # Darcy-Weisbach inequality formulation.
             head_loss_option = HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
 
         return head_loss_option
 
-    def _hn_pipe_head_loss_constraints(self, ensemble_member):
-        """
-        This function adds the head loss constraints for pipes. There are two options namely with
-        and without pipe class optimization. In both cases we assume that disconnected pipes, pipes
-        without flow have no head loss.
-
-        Under pipe-class optimization the head loss constraints per pipe class are added and
-        applied with the big_m method (is_topo_disconnected) to only activate the correct
-        constraints.
-
-        Under constant pipe class constraints for only one diameter are added.
-        """
-        constraints = []
-
-        options = self.energy_system_options()
-        parameters = self.parameters(ensemble_member)
-        components = self.energy_system_components
-        # Set the head loss according to the direction in the pipes. Note that
-        # the `.__head_loss` symbol is always positive by definition, but that
-        # `.dH` is not (positive when flow is negative, and vice versa).
-        # If the pipe is disconnected, we leave the .__head_loss symbol free
-        # (and it has no physical meaning). We also do not set any discharge
-        # relationship in this case (but dH is still equal to Out - In of
-        # course).
-
-        for pipe in components.get("heat_pipe", []):
-            if parameters[f"{pipe}.length"] == 0.0:
-                # If the pipe does not have a control valve, the head loss is
-                # forced to zero via bounds. If the pipe _does_ have a control
-                # valve, then there still is no relationship between the
-                # discharge and the head loss/dH.
-                continue
-
-            head_loss_sym = self._hn_pipe_to_head_loss_map[pipe]
-
-            dh = self.__state_vector_scaled(f"{pipe}.dH", ensemble_member)
-            head_loss = self.__state_vector_scaled(head_loss_sym, ensemble_member)
-            discharge = self.__state_vector_scaled(f"{pipe}.Q", ensemble_member)
-
-            # We need to make sure the dH is decoupled from the discharge when
-            # the pipe is disconnected. Simply put, this means making the
-            # below constraints trivial.
-            is_disconnected_var = self._pipe_disconnect_map.get(pipe)
-
-            if is_disconnected_var is None:
-                is_disconnected = 0.0
-            else:
-                is_disconnected = self.__state_vector_scaled(is_disconnected_var, ensemble_member)
-
-            max_discharge = None
-            max_head_loss = -np.inf
-
-            if pipe in self._pipe_topo_pipe_class_map:
-                # Multiple diameter options for this pipe
-                pipe_classes = self._pipe_topo_pipe_class_map[pipe]
-                max_discharge = max(c.maximum_discharge for c in pipe_classes)
-
-                for pc, pc_var_name in pipe_classes.items():
-                    if pc.inner_diameter == 0.0:
-                        continue
-
-                    head_loss_max_discharge = self._hn_head_loss_class._hn_pipe_head_loss(
-                        pipe,
-                        self,
-                        options,
-                        self.heat_network_settings,
-                        parameters,
-                        max_discharge,
-                        pipe_class=pc,
-                    )
-
-                    big_m = max(1.1 * self.__maximum_total_head_loss, 2 * head_loss_max_discharge)
-
-                    is_topo_disconnected = 1 - self.extra_variable(pc_var_name, ensemble_member)
-                    is_topo_disconnected = ca.repmat(is_topo_disconnected, dh.size1())
-
-                    # Note that we add the two booleans `is_disconnected` and
-                    # `is_topo_disconnected`. This is allowed because of the way the
-                    # resulting expression is used in the Big-M formulation. We only care
-                    # that the expression (i.e. a single boolean or the sum of the two
-                    # booleans) is either 0 when the pipe is connected, or >= 1 when it
-                    # is disconnected.
-                    constraints.extend(
-                        self._hn_head_loss_class._hn_pipe_head_loss(
-                            pipe,
-                            self,
-                            options,
-                            self.heat_network_settings,
-                            parameters,
-                            discharge,
-                            head_loss,
-                            dh,
-                            is_disconnected + is_topo_disconnected,
-                            big_m,
-                            pc,
-                        )
-                    )
-
-                    # Contrary to the Big-M calculation above, the relation
-                    # between dH and the head loss symbol requires the
-                    # maximum head loss that can be realized effectively. So
-                    # we pass the current pipe class's maximum discharge.
-                    max_head_loss = max(
-                        max_head_loss,
-                        self._hn_head_loss_class._hn_pipe_head_loss(
-                            pipe,
-                            self,
-                            options,
-                            self.heat_network_settings,
-                            parameters,
-                            pc.maximum_discharge,
-                            pipe_class=pc,
-                        ),
-                    )
-            else:
-                # Only a single diameter for this pipe. Note that we rely on
-                # the diameter parameter being overridden automatically if a
-                # single pipe class is set by the user.
-                area = parameters[f"{pipe}.area"]
-                max_discharge = self.heat_network_settings["maximum_velocity"] * area
-
-                is_topo_disconnected = int(parameters[f"{pipe}.diameter"] == 0.0)
-
-                constraints.extend(
-                    self._hn_head_loss_class._hn_pipe_head_loss(
-                        pipe,
-                        self,
-                        options,
-                        self.heat_network_settings,
-                        parameters,
-                        discharge,
-                        head_loss,
-                        dh,
-                        is_disconnected + is_topo_disconnected,
-                        1.1 * self.__maximum_total_head_loss,
-                    )
-                )
-
-                max_head_loss = self._hn_head_loss_class._hn_pipe_head_loss(
-                    pipe, self, options, self.heat_network_settings, parameters, max_discharge
-                )
-
-            # Relate the head loss symbol to the pipe's dH symbol.
-
-            # FIXME: Ugly hack. Cold pipes should be modelled completely with
-            # their own integers as well.
-            flow_dir = self.__state_vector_scaled(
-                self._pipe_to_flow_direct_map[pipe], ensemble_member
-            )
-
-            # Note that the Big-M should _at least_ cover the maximum
-            # distance between `head_loss` and `dh`. If `head_loss` can be at
-            # most 1.0 (= `max_head_loss`), that means our Big-M should be at
-            # least double (i.e. >= 2.0). And because we do not want Big-Ms to
-            # be overly tight, we include an additional factor of 2.
-            big_m = 2 * 2 * max_head_loss
-
-            constraints.append(
-                (
-                    (-dh - head_loss + (1 - flow_dir) * big_m) / big_m,
-                    0.0,
-                    np.inf,
-                )
-            )
-            constraints.append(((dh - head_loss + flow_dir * big_m) / big_m, 0.0, np.inf))
-
-        return constraints
-
     def __check_valve_head_discharge_path_constraints(self, ensemble_member):
         """
         This function adds constraints for the check valve functionality. Meaning that the flow can
         only go in positive direction of the valve. Depending on the status of the valve the flow is
         set to zero or bounded between zero and the maximum discharge.
 
         The head loss is also bounded to only act in one direction.
@@ -3095,15 +2820,15 @@
             q_aliases = self.alias_relation.aliases(q.name())
             connected_pipes = {p for p in all_pipes if f"{p}.Q" in q_aliases}
 
             maximum_discharge = 0.0
 
             for p in connected_pipes:
                 try:
-                    pipe_classes = self._pipe_topo_pipe_class_map[p].keys()
+                    pipe_classes = self._heat_pipe_topo_pipe_class_map[p].keys()
                     max_discharge_pipe = max(c.maximum_discharge for c in pipe_classes)
                 except KeyError:
                     max_discharge_pipe = maximum_velocity * parameters[f"{p}.area"]
 
                 maximum_discharge = max(maximum_discharge, max_discharge_pipe)
 
             maximum_head_loss = self.__maximum_total_head_loss
@@ -3142,15 +2867,15 @@
             q_aliases = self.alias_relation.aliases(q.name())
             connected_pipes = {p for p in all_pipes if f"{p}.Q" in q_aliases}
 
             maximum_discharge = 0.0
 
             for p in connected_pipes:
                 try:
-                    pipe_classes = self._pipe_topo_pipe_class_map[p].keys()
+                    pipe_classes = self._heat_pipe_topo_pipe_class_map[p].keys()
                     max_discharge_pipe = max(c.maximum_discharge for c in pipe_classes)
                 except KeyError:
                     max_discharge_pipe = maximum_velocity * parameters[f"{p}.area"]
 
                 maximum_discharge = max(maximum_discharge, max_discharge_pipe)
 
             maximum_head_loss = self.__maximum_total_head_loss
@@ -3193,15 +2918,15 @@
             carrier = self.parameters(ensemble_member)[f"{p}.carrier_id"]
             temperatures = self.temperature_regimes(carrier)
 
             if len(temperatures) == 0:
                 heat_loss_sym = self.extra_variable(heat_loss_sym_name, ensemble_member)
                 try:
                     heat_losses = self._pipe_heat_losses[p]
-                    pipe_classes = self._pipe_topo_pipe_class_map[p]
+                    pipe_classes = self._heat_pipe_topo_pipe_class_map[p]
                     variables = [
                         self.extra_variable(var_name, ensemble_member)
                         for pc, var_name in pipe_classes.items()
                     ]
                     heat_loss_expr = 0.0
                     for i in range(len(heat_losses)):
                         heat_loss_expr = heat_loss_expr + variables[i] * heat_losses[i]
@@ -3499,15 +3224,15 @@
         ) in {**self.energy_system_topology.buffers, **self.energy_system_topology.ates}.items():
             discharge = self.state(f"{b}.HeatIn.Q")
             hp_in = self.state(f"{b}.HeatIn.Hydraulic_power")
             hp_out = self.state(f"{b}.HeatOut.Hydraulic_power")
             pump_power = self.state(f"{b}.Pump_power")
             min_dp = parameters[f"{b}.minimum_pressure_drop"]
 
-            flow_dir_var = self._pipe_to_flow_direct_map[hot_pipe]
+            flow_dir_var = self._heat_pipe_to_flow_direct_map[hot_pipe]
             is_buffer_charging = self.state(flow_dir_var) * hot_pipe_orientation
 
             big_m = (
                 2.0
                 * self.bounds()[f"{b}.HeatIn.Q"][1]
                 * self.__maximum_total_head_loss
                 * 10.2
@@ -3574,15 +3299,19 @@
             constraints.extend(
                 self._hn_head_loss_class._pipe_head_loss_path_constraints(self, ensemble_member)
             )
             constraints.extend(
                 self._hn_head_loss_class._demand_head_loss_path_constraints(self, ensemble_member)
             )
 
-        constraints.extend(self.__pipe_hydraulic_power_path_constraints(ensemble_member))
+        constraints.extend(
+            self._hn_head_loss_class._pipe_hydraulic_power_path_constraints(
+                self, self.__maximum_total_head_loss, ensemble_member
+            )
+        )
         constraints.extend(self.__flow_direction_path_constraints(ensemble_member))
         constraints.extend(self.__node_heat_mixing_path_constraints(ensemble_member))
         constraints.extend(self.__node_hydraulic_power_mixing_path_constraints(ensemble_member))
         constraints.extend(self.__heat_loss_path_constraints(ensemble_member))
         constraints.extend(self.__node_discharge_mixing_path_constraints(ensemble_member))
         constraints.extend(self.__demand_heat_to_discharge_path_constraints(ensemble_member))
         constraints.extend(self.__cold_demand_heat_to_discharge_path_constraints(ensemble_member))
@@ -3610,15 +3339,20 @@
         are not applied to every time-step in the problem. Meaning that these constraints either
         consider global variables that are independent of time-step or that the relevant time-steps
         are indexed within the constraint formulation.
         """
         constraints = super().constraints(ensemble_member)
 
         if self.heat_network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
-            constraints.extend(self._hn_pipe_head_loss_constraints(ensemble_member))
+            # constraints.extend(self._hn_pipe_head_loss_constraints(ensemble_member))
+            constraints.extend(
+                self._hn_head_loss_class._pipe_head_loss_constraints(
+                    self, self.__maximum_total_head_loss, ensemble_member
+                )
+            )
 
         constraints.extend(self.__heat_loss_variable_constraints(ensemble_member))
         constraints.extend(self.__pipe_rate_heat_change_constraints(ensemble_member))
 
         if self.energy_system_options()["include_demand_insulation_options"]:
             constraints.extend(self.__heat_matching_demand_insulation_constraints(ensemble_member))
 
@@ -3786,15 +3520,15 @@
                 if parameters[f"{p}.length"] == 0.0 and not parameters[f"{p}.has_control_valve"]:
                     atol = self.variable_nominal(f"{p}.HeatIn.H") * 1e-5
                     assert np.allclose(head_diff, 0.0, atol=atol)
                 else:
                     q = results[f"{p}.Q"]
 
                     try:
-                        is_disconnected = np.round(results[self._pipe_disconnect_map[p]])
+                        is_disconnected = np.round(results[self._heat_pipe_disconnect_map[p]])
                     except KeyError:
                         is_disconnected = np.zeros_like(q)
 
                     q_nominal = self.variable_nominal(
                         self.alias_relation.canonical_signed(f"{p}.Q")[0]
                     )
                     inds = (np.abs(q) / q_nominal > 1e-4) & (is_disconnected == 0)
@@ -3806,17 +3540,17 @@
             area = parameters[f"{p}.area"]
 
             if area == 0.0:
                 continue
 
             q = results[f"{p}.Q"]
             v = q / area
-            flow_dir = np.round(results[self._pipe_to_flow_direct_map[p]])
+            flow_dir = np.round(results[self._heat_pipe_to_flow_direct_map[p]])
             try:
-                is_disconnected = np.round(results[self._pipe_disconnect_map[p]])
+                is_disconnected = np.round(results[self._heat_pipe_disconnect_map[p]])
             except KeyError:
                 is_disconnected = np.zeros_like(q)
 
             inds_disconnected = is_disconnected == 1
             inds_positive = (flow_dir == 1) & ~inds_disconnected
             inds_negative = (flow_dir == 0) & ~inds_disconnected
```

### Comparing `mesido-0.1.1/src/mesido/influxdb/profile.py` & `mesido-0.1.2/src/mesido/influxdb/profile.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Buffer.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Buffer.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Demand.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Demand.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Node.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Node.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Pipe.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Pipe.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Source.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/Source.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/_NonStorageComponent.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/Heat/_NonStorageComponent.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Buffer.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Buffer.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Node.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Node.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Pipe.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Pipe.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Source.mo` & `mesido-0.1.2/src/mesido/modelica/WarmingUp/HeatNetwork/QTH/Source.mo`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/network_common.py` & `mesido-0.1.2/src/mesido/network_common.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/physics_mixin.py` & `mesido-0.1.2/src/mesido/physics_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pipe_class.py` & `mesido-0.1.2/src/mesido/pipe_class.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/__init__.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .gas.gas_demand import GasDemand
 from .gas.gas_node import GasNode
 from .gas.gas_pipe import GasPipe
 from .gas.gas_source import GasSource
 from .gas.gas_substation import GasSubstation
 from .gas.gas_tank_storage import GasTankStorage
 from .heat.air_water_heat_pump import AirWaterHeatPump
+from .heat.airco import Airco
 from .heat.ates import ATES
 from .heat.check_valve import CheckValve
 from .heat.cold_demand import ColdDemand
 from .heat.control_valve import ControlValve
 from .heat.geothermal_source import GeothermalSource
 from .heat.heat_buffer import HeatBuffer
 from .heat.heat_demand import HeatDemand
@@ -28,31 +29,38 @@
 from .heat.heat_port import HeatPort
 from .heat.heat_pump import HeatPump
 from .heat.heat_source import HeatSource
 from .heat.heat_two_port import HeatTwoPort
 from .heat.low_temperature_ates import LowTemperatureATES
 from .heat.node import Node
 from .heat.pump import Pump
+from .multicommodity.airwater_heat_pump_elec import AirWaterHeatPumpElec
+from .multicommodity.electro_boiler import ElecBoiler
 from .multicommodity.electrolyzer import Electrolyzer
+from .multicommodity.gas_boiler import GasBoiler
 
 __all__ = [
+    "Airco",
     "AirWaterHeatPump",
+    "AirWaterHeatPumpElec",
     "ATES",
     "HeatBuffer",
     "CheckValve",
     "ColdDemand",
     "Compressor",
     "ControlValve",
     "HeatDemand",
+    "ElecBoiler",
     "ElectricityCable",
     "ElectricityDemand",
     "ElectricityNode",
     "ElectricitySource",
     "ElectricityStorage",
     "Electrolyzer",
+    "GasBoiler",
     "GasDemand",
     "GasNode",
     "GasPipe",
     "GasSource",
     "GasSubstation",
     "GasTankStorage",
     "GeothermalSource",
```

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/_internal/heat_component.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/_internal/heat_component.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_base.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_base.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_cable.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_cable.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_demand.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_demand.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_node.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_node.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_source.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_source.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/electricity_storage.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/electricity_storage.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/heat_pump_elec.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/heat_pump_elec.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/electricity/transformer.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/electricity/transformer.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/compressor.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/compressor.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_base.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         super().__init__(name, **modifiers)
         # TODO: think of more elegant approach for Q_shadow, currently required to ensure that
         #  every port has a unique variable to make the correct port mapping
         self.add_variable(Variable, "Q")  # [m3/s]
         self.add_variable(Variable, "Q_shadow")
         self.add_variable(Variable, "mass_flow")  # [g/s]
         self.add_variable(Variable, "H")  # [m]
+        self.add_variable(Variable, "Hydraulic_power")  # [W]
 
 
 class GasTwoPort(GasComponent):
     """
     For gas components that transport flow we have a two port component.
     """
```

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_demand.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_demand.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_node.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_node.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_pipe.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_tank_storage.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 from mesido.pycml import Variable
+from mesido.pycml.component_library.milp._internal import BaseAsset
 
-from numpy import nan, pi
+from numpy import nan
 
-from .gas_base import GasTwoPort
-from .._internal import BaseAsset
+from .gas_base import GasPort
+from .._internal.gas_component import GasComponent
 
 
-class GasPipe(GasTwoPort, BaseAsset):
+class GasTankStorage(GasComponent, BaseAsset):
     """
-    The gas_pipe component is used to model head loss through the pipe. At the moment we only have
-    a placeholder linear head loss formulation in place.
+    ...
     """
 
     def __init__(self, name, **modifiers):
         super().__init__(name, **modifiers)
 
-        self.component_type = "gas_pipe"
-        self.disconnectable = False
+        self.component_type = "gas_tank_storage"
 
-        self.v_max = 15.0
-        self.density = 2.5e3  # [g/m3]
-        self.diameter = nan
-        self.area = 0.25 * pi * self.diameter**2
-        self.Q_nominal = self.v_max / 2.0 * self.area
-        self.pressure = 16.0e5
-
-        self.nominal_head = 30.0
-        self.length = nan
-        self.r = 1.0e-6 * self.length  # TODO: temporary value
-        self.nominal_head_loss = (self.Q_nominal * self.r * self.nominal_head) ** 0.5
-
-        self.add_variable(Variable, "dH", nominal=self.Q_nominal * self.r)
-        self.add_variable(Variable, "Q", nominal=self.Q_nominal)
-
-        # Flow should be preserved
-        self.add_equation(((self.GasIn.Q - self.GasOut.Q) / self.Q_nominal))
-        self.add_equation(((self.Q - self.GasOut.Q) / self.Q_nominal))
-        self.add_equation(((self.GasIn.Q - self.GasIn.mass_flow / self.density) / self.Q_nominal))
+        self.min_head = 30.0
+        self.density = 2.5e3  # H2 density [g/m3] at 30bar
+        self.density_max_storage = 23.715e3  # H2 density [g/m3] at 350bar
+        self.volume = nan
+        self.Q_nominal = nan
+
+        self.add_variable(GasPort, "GasIn")
+        self.add_variable(Variable, "Gas_tank_flow", nominal=self.Q_nominal * self.density)
+
+        self._typical_fill_time = 3600.0
+        self._nominal_stored_gas = (
+            self.Q_nominal * self.density_max_storage * self._typical_fill_time
+        )
+        self.add_variable(
+            Variable,
+            "Stored_gas_mass",
+            min=0.0,
+            max=self.density_max_storage * self.volume,
+            nominal=self._nominal_stored_gas,
+        )
+
+        self.add_equation(
+            ((self.GasIn.mass_flow - self.Gas_tank_flow) / (self.Q_nominal * self.density))
+        )
 
-        # Flow should be preserved
         self.add_equation(
-            ((self.GasIn.mass_flow - self.GasOut.mass_flow) / (self.Q_nominal * self.density))
+            (
+                (self.der(self.Stored_gas_mass) - (self.Gas_tank_flow))
+                / (self._nominal_stored_gas * self.Q_nominal * self.density) ** 0.5
+            )
         )
-        # # shadow Q for aliases
-        self.add_equation(((self.GasOut.Q_shadow - (self.GasIn.Q_shadow - 1.0e-3))))
+
+        self.add_initial_equation((self.Stored_gas_mass / self._nominal_stored_gas))
```

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_source.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_source.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_substation.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/gas/gas_substation.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/gas/gas_tank_storage.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/multicommodity/electrolyzer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 from mesido.pycml import Variable
 from mesido.pycml.component_library.milp._internal import BaseAsset
+from mesido.pycml.component_library.milp._internal.electricity_component import (
+    ElectricityComponent,
+)
+from mesido.pycml.component_library.milp.electricity.electricity_base import (
+    ElectricityPort,
+)
+from mesido.pycml.component_library.milp.gas.gas_base import (
+    GasPort,
+)
 
 from numpy import nan
 
-from .gas_base import GasPort
-from .._internal.gas_component import GasComponent
 
-
-class GasTankStorage(GasComponent, BaseAsset):
+class Electrolyzer(ElectricityComponent, BaseAsset):
     """
-    ...
+    An electrolyzer consumes electricity and produces hydrogen
     """
 
     def __init__(self, name, **modifiers):
-        super().__init__(name, **modifiers)
+        super().__init__(
+            name,
+            **self.merge_modifiers(
+                dict(),
+                modifiers,
+            ),
+        )
 
-        self.component_type = "gas_tank_storage"
+        self.component_type = "electrolyzer"
 
-        self.min_head = 30.0
-        self.density = 2.5e3  # H2 density [g/m3] at 30bar
-        self.density_max_storage = 23.715e3  # H2 density [g/m3] at 350bar
-        self.volume = nan
-        self.Q_nominal = nan
+        self.a_eff_coefficient = nan
+        self.b_eff_coefficient = nan
+        self.c_eff_coefficient = nan
 
-        self.add_variable(GasPort, "GasIn")
-        self.add_variable(Variable, "Gas_tank_flow", nominal=self.Q_nominal * self.density)
+        self.minimum_load = nan
 
-        self._typical_fill_time = 3600.0
-        self._nominal_stored_gas = (
-            self.Q_nominal * self.density_max_storage * self._typical_fill_time
-        )
-        self.add_variable(
-            Variable,
-            "Stored_gas_mass",
-            min=0.0,
-            max=self.density_max_storage * self.volume,
-            nominal=self._nominal_stored_gas,
-        )
+        self.density = 2.5  # H2 density [kg/m3] at 30bar
 
+        self.Q_nominal = nan
+        self.min_voltage = nan
+
+        self.nominal_gass_mass_out = self.Q_nominal * self.density
+        self.nominal_power_consumed = nan
+
+        self.add_variable(ElectricityPort, "ElectricityIn")  # [W]
+        self.add_variable(Variable, "Power_consumed", min=0.0, nominal=self.nominal_power_consumed)
         self.add_equation(
-            ((self.GasIn.mass_flow - self.Gas_tank_flow) / (self.Q_nominal * self.density))
-        )
+            (self.ElectricityIn.Power - self.Power_consumed) / self.nominal_power_consumed
+        )  # [W]
 
+        self.add_variable(GasPort, "GasOut")
+        self.add_variable(
+            Variable, "Gas_mass_flow_out", min=0.0, nominal=self.nominal_gass_mass_out
+        )  # [kg/hr]
         self.add_equation(
-            (
-                (self.der(self.Stored_gas_mass) - (self.Gas_tank_flow))
-                / (self._nominal_stored_gas * self.Q_nominal * self.density) ** 0.5
-            )
+            (self.GasOut.mass_flow - self.Gas_mass_flow_out) / self.nominal_gass_mass_out
         )
-
-        self.add_initial_equation((self.Stored_gas_mass / self._nominal_stored_gas))
```

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/__init__.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .air_water_heat_pump import AirWaterHeatPump
+from .airco import Airco
 from .ates import ATES
 from .check_valve import CheckValve
 from .cold_demand import ColdDemand
 from .control_valve import ControlValve
 from .geothermal_source import GeothermalSource
 from .heat_buffer import HeatBuffer
 from .heat_demand import HeatDemand
@@ -14,14 +15,15 @@
 from .heat_source import HeatSource
 from .heat_two_port import HeatTwoPort
 from .low_temperature_ates import LowTemperatureATES
 from .node import Node
 from .pump import Pump
 
 __all__ = [
+    "Airco",
     "AirWaterHeatPump",
     "ATES",
     "HeatBuffer",
     "CheckValve",
     "ColdDemand",
     "ControlValve",
     "HeatDemand",
```

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/_non_storage_component.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/_non_storage_component.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/ates.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/ates.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/check_valve.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/check_valve.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/cold_demand.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/cold_demand.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/control_valve.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/control_valve.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/geothermal_source.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/geothermal_source.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_buffer.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_buffer.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_demand.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_demand.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_exchanger.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_exchanger.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_four_port.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_four_port.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_pipe.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_pipe.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_port.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_port.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_pump.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_pump.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_source.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_source.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/heat_two_port.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/heat_two_port.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/low_temperature_ates.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/low_temperature_ates.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/node.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/node.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/milp/heat/pump.py` & `mesido-0.1.2/src/mesido/pycml/component_library/milp/heat/pump.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/__init__.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/__init__.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/_non_storage_component.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/_non_storage_component.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/buffer.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/buffer.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/check_valve.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/check_valve.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/demand.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/demand.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/node.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/node.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/pipe.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/pipe.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/pump.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/pump.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/component_library/qth/source.py` & `mesido-0.1.2/src/mesido/pycml/component_library/qth/source.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/model_base.py` & `mesido-0.1.2/src/mesido/pycml/model_base.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/pycml/pycml_mixin.py` & `mesido-0.1.2/src/mesido/pycml/pycml_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/qth_not_maintained/bounds_to_pipe_flow_directions_mixin.py` & `mesido-0.1.2/src/mesido/qth_not_maintained/bounds_to_pipe_flow_directions_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/qth_not_maintained/head_loss_mixin.py` & `mesido-0.1.2/src/mesido/head_loss_class.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,33 +2,44 @@
 from abc import abstractmethod
 from enum import IntEnum
 from typing import List, Optional, Tuple, Type, Union
 
 import casadi as ca
 
 import mesido._darcy_weisbach as darcy_weisbach
-from mesido.base_component_type_mixin import BaseComponentTypeMixin
+from mesido.constants import GRAVITATIONAL_CONSTANT
+from mesido.network_common import NetworkSettings
+from mesido.pipe_class import PipeClass
 
 import numpy as np
 
-from rtctools._internal.alias_tools import AliasDict
-from rtctools.optimization.goal_programming_mixin_base import Goal, _GoalProgrammingMixinBase
-from rtctools.optimization.optimization_problem import BT, OptimizationProblem
-
-from ..constants import GRAVITATIONAL_CONSTANT
-from ..pipe_class import PipeClass
+from rtctools.optimization.goal_programming_mixin_base import Goal
+from rtctools.optimization.optimization_problem import BT
 
 
 logger = logging.getLogger("mesido")
 
 
+def _state_vector_scaled(optimization_problem, variable, ensemble_member):
+    """
+    This functions returns the casadi symbols scaled with their nominal for the entire time
+    horizon.
+    """
+    canonical, sign = optimization_problem.alias_relation.canonical_signed(variable)
+    return (
+        optimization_problem.state_vector(canonical, ensemble_member)
+        * optimization_problem.variable_nominal(canonical)
+        * sign
+    )
+
+
 class HeadLossOption(IntEnum):
     r"""
     Enumeration for the possible options to take head loss in pipes into account.
-    Also see :py:meth:`._HeadLossMixin.heat_network_options` for related options.
+    Also see :py:meth:`._HeadLossMixin.energy_system_options` for related options.
 
     .. note::
         Not all options are supported by :py:class:`.HeatMixin`, due to the focus
         on MILP formulations.
 
     NO_HEADLOSS
        The NO_HEADLOSS option assumes that there is no headloss in the pipelines.
@@ -65,15 +76,15 @@
            \Delta H \ge \vec{a} \cdot Q + \vec{b}
 
         with :math:`\vec{a}` and :math:`\vec{b}` the linearization coefficients.
 
         This approach can more easily be explain with a plot, showing the Darcy-Weisbach
         head loss, and the linear lines approximating it. Note that the number of
         supporting lines is an option that can be set by the user by overriding
-        :py:meth:`._HeadLossMixin.heat_network_options`. Also note that, just like
+        :py:meth:`._HeadLossMixin.energy_system_options`. Also note that, just like
         ``CQ2_INEQUALITY``, a boolean is needed when flow directions are not fixed.
 
            .. image:: /images/DWlinearization.PNG
 
     LINEARIZED_ONE_LINE_EQUALITY
         This option uses a linear head loss formulation.
         A single constraint of the type
@@ -83,15 +94,15 @@
            H_{up} - H_{down} = dH = C \cdot Q
 
         is added.
         Note that no boolean are required to support the case where flow directions
         are not fixed yet, at the cost of reduced fidelity in the head-loss relationship.
 
         The exact velocity to use to linearize can be set by overriding
-        :py:meth:`._HeadLossMixin.heat_network_options`.
+        :py:meth:`._HeadLossMixin.energy_system_options`.
 
     CQ2_EQUALITY
         This option adds **equality** constraints of the type:
 
          .. math::
 
            dH = C \cdot Q^2
@@ -100,240 +111,204 @@
     """
 
     NO_HEADLOSS = 1
     CQ2_INEQUALITY = 2
     LINEARIZED_N_LINES_WEAK_INEQUALITY = 3
     LINEARIZED_ONE_LINE_EQUALITY = 4
     CQ2_EQUALITY = 5
+    LINEARIZED_N_LINES_EQUALITY = 6
 
 
 class _MinimizeHeadLosses(Goal):
     order = 1
 
-    priority = 2**31 - 1
+    priority = 2**31 - 2
 
-    def __init__(self, optimization_problem: "_HeadLossMixin", *args, **kwargs):
+    def __init__(self, optimization_problem, input_network_settings, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.optimization_problem = optimization_problem
+        self.network_settings = input_network_settings
         self.function_nominal = len(optimization_problem.times())
 
-    def function(self, optimization_problem: "_HeadLossMixin", ensemble_member):
+    def function(self, optimization_problem, ensemble_member):
         """
         This function returns the summed head loss of all pipes and pumps.
         """
         sum_ = 0.0
 
         parameters = optimization_problem.parameters(ensemble_member)
-        options = optimization_problem.heat_network_options()
 
         pumps = optimization_problem.energy_system_components.get("pump", [])
         sources = optimization_problem.energy_system_components.get("heat_source", [])
 
         for p in pumps:
             sum_ += optimization_problem.state(f"{p}.dH")
 
         # If sources have an accompanying pump, we prefer the produced head to
         # be shifted to that pump. We therefore penalize the head of the
         # sources twice as much.
         for s in sources:
             sum_ += 2 * optimization_problem.state(f"{s}.dH")
 
-        assert options["head_loss_option"] != HeadLossOption.NO_HEADLOSS
+        assert self.network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS
 
-        for p in optimization_problem.energy_system_components["pipe"]:
-            if not parameters[f"{p}.has_control_valve"] and not parameters[f"{p}.length"] == 0.0:
-                sym_name = optimization_problem._hn_pipe_to_head_loss_map[p]
-                sum_ += optimization_problem.state(sym_name)
+        if self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_HEAT:
+            for p in optimization_problem.energy_system_components.get("heat_pipe", []):
+                if (
+                    not parameters[f"{p}.has_control_valve"]
+                    and not parameters[f"{p}.length"] == 0.0
+                ):
+                    sym_name = optimization_problem._hn_pipe_to_head_loss_map[p]
+                    sum_ += optimization_problem.state(sym_name)
+        elif self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_GAS:
+            for p in optimization_problem.energy_system_components.get("gas_pipe", []):
+                if not parameters[f"{p}.length"] == 0.0:
+                    sym_name = optimization_problem._gn_pipe_to_head_loss_map[p]
+                    sum_ += optimization_problem.state(sym_name)
 
         return sum_
 
 
 class _MinimizeHydraulicPower(Goal):
     order = 1
 
     priority = 2**31 - 1
 
     def __init__(
         self,
-        optimization_problem: "_HeadLossMixin",
+        optimization_problem,
+        input_network_settings,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.optimization_problem = optimization_problem
+        self.network_settings = input_network_settings
 
-    def function(self, optimization_problem: "_HeadLossMixin", ensemble_member):
+    def function(self, optimization_problem, ensemble_member):
         """
         This function returns the summed hydraulic power of all pipes
         """
         sum_ = 0.0
 
         parameters = optimization_problem.parameters(ensemble_member)
-        options = optimization_problem.heat_network_options()
 
-        assert options["head_loss_option"] != HeadLossOption.NO_HEADLOSS
+        assert self.network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS
 
-        for pipe in optimization_problem.energy_system_components.get("pipe", []):
+        for pipe in optimization_problem.energy_system_components.get("heat_pipe", []):
             if (
                 not parameters[f"{pipe}.has_control_valve"]
                 and not parameters[f"{pipe}.length"] == 0.0
             ):
                 sum_ += optimization_problem.state(f"{pipe}.Hydraulic_power")
 
         return sum_
 
 
-class _HeadLossMixin(BaseComponentTypeMixin, _GoalProgrammingMixinBase, OptimizationProblem):
+class HeadLossClass:
     """
-    Adds handling of discharge - head (loss) relationship to the model.
+    For handling of discharge - head (loss) relationship to the model.
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, input_network_settings, *args, **kwargs):
 
         self.__pipe_head_bounds = {}
 
         self.__pipe_head_loss_var = {}
         self.__pipe_head_loss_bounds = {}
         self.__pipe_head_loss_nominals = {}
         self.__pipe_head_loss_zero_bounds = {}
         self._hn_pipe_to_head_loss_map = {}
 
+        # Kvr
+        # Boolean variables for the linear line segment options per pipe.
+        self.__pipe_linear_line_segment_var = {}  # value 0/1: line segment - not active/active
+        self.__pipe_linear_line_segment_var_bounds = {}
+        self._pipe_linear_line_segment_map = {}
+
         self.__priority = None
 
+        self.network_settings = input_network_settings
+
     def pre(self):
         """
         Some checks to avoid that different pipes have different head_loss options in case one
         has the No_HeadLoss option.
         """
         super().pre()
 
         self.__initialize_nominals_and_bounds()
 
-        options = self.heat_network_options()
         parameters = self.parameters(0)
 
         # It is not allowed to mix NO_HEADLOSS with other head loss options as
         # that just leads to weird and undefined behavior.
         head_loss_values = {
-            options["head_loss_option"],
+            self.network_settings["head_loss_option"],
         }
-        for p in self.energy_system_components.get("pipe", []):
-            head_loss_values.add(self._hn_get_pipe_head_loss_option(p, options, parameters))
+
+        pipe_type = "heat_pipe"
+        if len(self.energy_system_components.get("heat_pipe", [])) == 0:
+            pipe_type = "gas_pipe"
+
+        for p in self.energy_system_components.get(pipe_type, []):
+            head_loss_values.add(
+                self._hn_get_pipe_head_loss_option(p, self.network_settings, parameters)
+            )
 
         if HeadLossOption.NO_HEADLOSS in head_loss_values and len(head_loss_values) > 1:
             raise Exception(
                 "Mixing .NO_HEADLOSS with other head loss options is not allowed. "
                 "Either all pipes should have .NO_HEADLOSS set, or none. "
-                "The global value returned by heat_network_options() also need to match."
+                "The global value returned by energy_system_options() also need to match."
             )
 
-    def heat_network_options(self):
+    def head_loss_network_options(self):
         r"""
         Returns a dictionary of milp network specific options.
 
         +--------------------------------+-----------+-----------------------------------+
         | Option                         | Type      | Default value                     |
         +================================+===========+===================================+
         | ``minimum_pressure_far_point`` | ``float`` | ``1.0`` bar                       |
         +--------------------------------+-----------+-----------------------------------+
         | ``wall_roughness``             | ``float`` | ``0.0002`` m                      |
         +--------------------------------+-----------+-----------------------------------+
-        | ``head_loss_option``           | ``enum``  | ``HeadLossOption.CQ2_INEQUALITY`` |
-        +--------------------------------+-----------+-----------------------------------+
         | ``estimated_velocity``         | ``float`` | ``1.0`` m/s (CQ2_* &              |
         |                                |           |LINEARIZED_ONE_LINE_EQUALITY)      |
         +--------------------------------+-----------+-----------------------------------+
-        | ``maximum_velocity``           | ``float`` | ``2.5`` m/s                       |
-        |                                |           |LINEARIZED_N_LINES_WEAK_INEQUALITY |
-        +--------------------------------+-----------+-----------------------------------+
-        | ``n_linearization_lines``      | ``int``   | ``5``                             |
-        |                                |           |LINEARIZED_N_LINES_WEAK_INEQUALITY |
-        +--------------------------------+-----------+-----------------------------------+
-        | ``minimize_head_losses``       | ``bool``  | ``True``                          |
-        +--------------------------------+-----------+-----------------------------------+
-        | ``pipe_minimum_pressure``      | ``float`` | ``-np.inf``                       |
-        +--------------------------------+-----------+-----------------------------------+
-        | ``pipe_maximum_pressure``      | ``float`` | ``np.inf``                        |
-        +--------------------------------+-----------+-----------------------------------+
 
         The ``minimum_pressure_far_point`` gives the minimum pressure
         requirement at any demand node, which means that the pressure at the
         furthest point is also satisfied without inspecting the topology.
 
         The ``wall_roughness`` of the pipes plays a role in determining the
         resistance of the pipes.
-
-        To model the head loss in pipes, the ``head_loss_option`` refers to
-        one of the ways this can be done. See :class:`HeadLossOption` for more
-        explanation on what each option entails. Note that some options model
-        the head loss as an inequality, i.e. :math:`\Delta H \ge f(Q)`, whereas
-        others model it as an equality.
-
-        When ``HeadLossOption.CQ2_INEQUALITY`` is used, the wall roughness at
-        ``estimated_velocity`` determines the `C` in :math:`\Delta H \ge C
-        \cdot Q^2`.
-
-        When ``HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY`` is used, the
-        ``maximum_velocity`` needs to be set. The Darcy-Weisbach head loss
-        relationship from :math:`v = 0` until :math:`v = \text{maximum_velocity}`
-        will then be linearized using ``n_linearization`` lines.
-
-        When ``HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY`` is used, the wall roughness at
-        ``estimated_velocity`` determines the `C` in :math:`\Delta H = C \cdot
-        Q`. For pipes that contain a control valve, the formulation of
-        ``HeadLossOption.CQ2_INEQUALITY`` is used.
-
-        When ``HeadLossOption.CQ2_EQUALITY`` is used, the wall roughness at
-        ``estimated_velocity`` determines the `C` in :math:`\Delta H = C \cdot
-        Q^2`. Note that this formulation is non-convex. At `theta < 1` we
-        therefore use the formulation ``HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY``. For pipes
-        that contain a control valve, the formulation of
-        ``HeadLossOption.CQ2_INEQUALITY`` is used.
-
-
-        When ``minimize_head_losses`` is set to True (default), a last
-        priority is inserted where the head losses and hydraulic power in the system are
-        minimized if the ``head_loss_option`` is not `NO_HEADLOSS`.
-        This is related to the assumption that control valves are
-        present in the system to steer water in the right direction the case
-        of multiple routes. If such control valves are not present, enabling
-        this option will give warnings in case the found solution is not
-        feasible. In case the option is False, both the minimization and
-        checks are skipped.
-
-        The ``pipe_minimum_pressure`` is the global minimum pressured allowed
-        in the network. Similarly, ``pipe_maximum_pressure`` is the maximum
-        one.
         """
 
         options = {}
 
         options["minimum_pressure_far_point"] = 1.0
         options["wall_roughness"] = 2e-4
-        options["head_loss_option"] = HeadLossOption.CQ2_INEQUALITY
         options["estimated_velocity"] = 1.0
-        options["maximum_velocity"] = 2.5
-        options["n_linearization_lines"] = 5
-        options["minimize_head_losses"] = True
 
         return options
 
     @abstractmethod
     def _hn_get_pipe_head_loss_option(
-        self, pipe, heat_network_options, parameters, **kwargs
+        self, pipe, network_settings, parameters, **kwargs
     ) -> HeadLossOption:
         """
         The global user head loss option is not necessarily the same as the
         head loss option for a specific pipe. For example, when a control
         valve is present, a .LINEARIZED_ONE_LINE_EQUALITY global head loss option could mean a
         .CQ2_INEQUALITY formulation should be used instead.
 
         See also the explanation of `head_loss_option` (and its values) in
-        :py:meth:`.heat_network_options`.
+        :py:meth:`.energy_system_options`.
         """
         raise NotImplementedError
 
     @abstractmethod
     def _hn_pipe_head_loss_constraints(self, ensemble_member) -> List[Tuple[ca.MX, float, float]]:
         """
         This method should be implemented to relate the three variables:
@@ -358,86 +333,187 @@
     @property
     def _hpwr_minimization_goal_class(self) -> Type[Goal]:
         """
         This function returns the minimize hydraulic power goal
         """
         return _MinimizeHydraulicPower
 
-    def __initialize_nominals_and_bounds(self):
+    def initialize_variables_nominals_and_bounds(
+        self, optimization_problem, commodity_type, pipe_name, network_settings
+    ):
         """
         This function computes and sets the bounds and nominals for the head loss of all the pipes
         as well as the minimum and maximum pipe pressure.
         """
-        self.__pipe_head_loss_nominals = AliasDict(self.alias_relation)
-
-        options = self.heat_network_options()
-        parameters = self.parameters(0)
+        options = optimization_problem.energy_system_options()
+        parameters = optimization_problem.parameters(0)
 
-        min_pressure = options["pipe_minimum_pressure"]
-        max_pressure = options["pipe_maximum_pressure"]
+        min_pressure = network_settings["pipe_minimum_pressure"]
+        max_pressure = network_settings["pipe_maximum_pressure"]
         assert (
             max_pressure > min_pressure
         ), "The global maximum pressure must be larger than the minimum one."
         if np.isfinite(min_pressure) or np.isfinite(max_pressure):
-            for p in self.energy_system_components["pipe"]:
-                # No elevation data available yet. Assume 0 mDAT for now.
-                pipe_elevation = 0.0
-                min_head = min_pressure * 10.2 + pipe_elevation
-                max_head = max_pressure * 10.2 + pipe_elevation
-                self.__pipe_head_bounds[f"{p}.HeatIn.H"] = (min_head, max_head)
-                self.__pipe_head_bounds[f"{p}.HeatOut.H"] = (min_head, max_head)
+            # No elevation data available yet. Assume 0 mDAT for now.
+            pipe_elevation = 0.0
+            min_head = min_pressure * 10.2 + pipe_elevation
+            max_head = max_pressure * 10.2 + pipe_elevation
+            self.__pipe_head_bounds[f"{pipe_name}.{commodity_type}In.H"] = (min_head, max_head)
+            self.__pipe_head_bounds[f"{pipe_name}.{commodity_type}Out.H"] = (min_head, max_head)
 
-        head_loss_option = options["head_loss_option"]
+        head_loss_option = network_settings["head_loss_option"]
         if head_loss_option not in HeadLossOption.__members__.values():
             raise Exception(f"Head loss option '{head_loss_option}' does not exist")
 
-        for p in self.energy_system_components.get("pipe", []):
-            length = parameters[f"{p}.length"]
-            if length < 0.0:
-                raise ValueError("Pipe length has to be larger than or equal to zero")
-
-            head_loss_option = self._hn_get_pipe_head_loss_option(p, options, parameters)
-
-            if head_loss_option == HeadLossOption.NO_HEADLOSS or (
-                length == 0.0 and not parameters[f"{p}.has_control_valve"]
-            ):
-                self.__pipe_head_loss_zero_bounds[f"{p}.dH"] = (0.0, 0.0)
-            else:
-                q_nominal = self._hn_pipe_nominal_discharge(options, parameters, p)
-                head_loss_nominal = self._hn_pipe_head_loss(p, options, parameters, q_nominal)
+        length = parameters[f"{pipe_name}.length"]
+        if length < 0.0:
+            raise ValueError("Pipe length has to be larger than or equal to zero")
 
-                self.__pipe_head_loss_nominals[f"{p}.dH"] = head_loss_nominal
+        if head_loss_option == HeadLossOption.NO_HEADLOSS or (
+            length == 0.0 and not parameters[f"{pipe_name}.has_control_valve"]
+        ):
+            self.__pipe_head_loss_zero_bounds[f"{pipe_name}.dH"] = (0.0, 0.0)
+            head_loss_var = ""  # Required for checking if the keys exist in the return past below
+        else:
+            q_nominal = self._hn_pipe_nominal_discharge(options, parameters, pipe_name)
+            head_loss_nominal = self._hn_pipe_head_loss(
+                pipe_name,
+                optimization_problem,
+                options,
+                network_settings,
+                parameters,
+                q_nominal,
+                # network_type=self.network_settings["network_type"],
+                pressure=parameters[f"{pipe_name}.pressure"],
+            )
 
-                # The .dH is by definition "Out - In". The .__head_loss is by
-                # definition larger than or equal to the absolute value of dH.
-                head_loss_var = f"{p}.__head_loss"
+            self.__pipe_head_loss_nominals[f"{pipe_name}.dH"] = head_loss_nominal
 
-                self._hn_pipe_to_head_loss_map[p] = head_loss_var
-                self.__pipe_head_loss_var[head_loss_var] = ca.MX.sym(head_loss_var)
+            # The .dH is by definition "Out - In". The .__head_loss is by
+            # definition larger than or equal to the absolute value of dH.
+            head_loss_var = f"{pipe_name}.__head_loss"
+
+            self._hn_pipe_to_head_loss_map[pipe_name] = head_loss_var
+            self.__pipe_head_loss_var[head_loss_var] = ca.MX.sym(head_loss_var)
+
+            self.__pipe_head_loss_nominals[head_loss_var] = head_loss_nominal
+            self.__pipe_head_loss_bounds[head_loss_var] = (0.0, np.inf)
+
+            if head_loss_option == HeadLossOption.LINEARIZED_N_LINES_EQUALITY:
+                # Add pipe head loss linear line segment variables
+                self._pipe_linear_line_segment_map[pipe_name] = {}
+                self.__pipe_linear_line_segment_var[pipe_name] = {}
+                self.__pipe_linear_line_segment_var_bounds[pipe_name] = {}
+                # We need to creat linear line segments for the - and + volumetric flow rate
+                # possibilites. Line number 1, 2, N for the - & + side is created
+                discharge_type = ["neg_discharge", "pos_discharge"]
+                line_number = 0
+                for dtype in discharge_type:
+                    for ii_line in range(network_settings["n_linearization_lines"] * 2):
+                        if ii_line < network_settings["n_linearization_lines"]:
+                            dtype = discharge_type[0]
+                            line_number = ii_line + 1
+                        else:
+                            dtype = discharge_type[1]
+                            line_number = ii_line + 1 - network_settings["n_linearization_lines"]
+
+                        # start line segment numbering from 1 up to "n_linearization_lines"
+                        pipe_linear_line_segment_var_name = (
+                            f"{pipe_name}__pipe_linear_line_segment_num_{line_number}_{dtype}"
+                        )
 
-                self.__pipe_head_loss_nominals[head_loss_var] = head_loss_nominal
-                self.__pipe_head_loss_bounds[head_loss_var] = (0.0, np.inf)
+                        self._pipe_linear_line_segment_map[pipe_name][
+                            ii_line
+                        ] = pipe_linear_line_segment_var_name
+                        self.__pipe_linear_line_segment_var[pipe_name][
+                            pipe_linear_line_segment_var_name
+                        ] = ca.MX.sym(pipe_linear_line_segment_var_name)
+                        self.__pipe_linear_line_segment_var_bounds[pipe_name][
+                            pipe_linear_line_segment_var_name
+                        ] = (0.0, 1.0)
+
+        return (
+            (
+                self.__pipe_head_bounds[f"{pipe_name}.{commodity_type}In.H"]
+                if self.__pipe_head_bounds.get(f"{pipe_name}.{commodity_type}In.H") is not None
+                else self.__pipe_head_bounds
+            ),
+            (
+                self.__pipe_head_bounds[f"{pipe_name}.{commodity_type}Out.H"]
+                if self.__pipe_head_bounds.get(f"{pipe_name}.{commodity_type}Out.H") is not None
+                else self.__pipe_head_bounds
+            ),
+            (
+                self.__pipe_head_loss_zero_bounds[f"{pipe_name}.dH"]
+                if self.__pipe_head_loss_zero_bounds.get(f"{pipe_name}.dH") is not None
+                else self.__pipe_head_loss_zero_bounds
+            ),
+            (
+                self._hn_pipe_to_head_loss_map[pipe_name]
+                if self._hn_pipe_to_head_loss_map.get(pipe_name) is not None
+                else self._hn_pipe_to_head_loss_map
+            ),
+            (
+                self.__pipe_head_loss_var[head_loss_var]
+                if self.__pipe_head_loss_var.get(head_loss_var) is not None
+                else self.__pipe_head_loss_var
+            ),
+            (
+                self.__pipe_head_loss_nominals[f"{pipe_name}.dH"]
+                if self.__pipe_head_loss_nominals.get(f"{pipe_name}.dH") is not None
+                else self.__pipe_head_loss_nominals
+            ),
+            (
+                self.__pipe_head_loss_nominals[head_loss_var]
+                if self.__pipe_head_loss_nominals.get(head_loss_var) is not None
+                else self.__pipe_head_loss_nominals
+            ),
+            (
+                self.__pipe_head_loss_bounds[head_loss_var]
+                if self.__pipe_head_loss_bounds.get(head_loss_var) is not None
+                else self.__pipe_head_loss_bounds
+            ),
+            (
+                self._pipe_linear_line_segment_map[pipe_name]
+                if self._pipe_linear_line_segment_map.get(pipe_name) is not None
+                else self._pipe_linear_line_segment_map
+            ),
+            (
+                self.__pipe_linear_line_segment_var[pipe_name]
+                if self.__pipe_linear_line_segment_var.get(pipe_name) is not None
+                else self.__pipe_linear_line_segment_var
+            ),
+            (
+                self.__pipe_linear_line_segment_var_bounds[pipe_name]
+                if self.__pipe_linear_line_segment_var_bounds.get(pipe_name) is not None
+                else self.__pipe_linear_line_segment_var_bounds
+            ),
+        )
 
-    def _hn_pipe_nominal_discharge(self, heat_network_options, parameters, pipe: str) -> float:
+    def _hn_pipe_nominal_discharge(self, energy_system_options, parameters, pipe: str) -> float:
         """
         This function returns the nominal volumetric flow (m^3/s) through the pipe.
         """
-        return parameters[f"{pipe}.area"] * heat_network_options["estimated_velocity"]
+        return parameters[f"{pipe}.area"] * energy_system_options["estimated_velocity"]
 
     def _hn_pipe_head_loss(
         self,
         pipe: str,
-        heat_network_options,
+        optimization_problem,
+        energy_system_options,
+        network_settings,
         parameters,
         discharge: Union[ca.MX, float, np.ndarray],
         head_loss: Optional[ca.MX] = None,
         dh: Optional[ca.MX] = None,
         is_disconnected: Union[ca.MX, int] = 0,
         big_m: Optional[float] = None,
         pipe_class: Optional[PipeClass] = None,
+        # network_type: NetworkSettings = NetworkSettings.NETWORK_TYPE_HEAT,
+        pressure: float = 0.0,
     ) -> Union[List[Tuple[ca.MX, BT, BT]], float, np.ndarray]:
         """
         This function has two purposes:
         - return the head loss constraint expression(s) or
         - compute the head loss numerically (always positive).
 
         Note that there are different head loss formulations (see
@@ -455,22 +531,22 @@
 
         `is_disconnected` can be used to specify whether a pipe is
         disconnected or not. This is most useful if a (boolean) ca.MX symbol
         is passed, which can then be used with a big-M formulation. The big-M
         itself then also needs to be passed via the `big_m` keyword argument.
         """
 
+        network_type = network_settings["network_type"]
+
         if head_loss is None and dh is None:
             symbolic = False
         else:
             symbolic = True
 
-        head_loss_option = self._hn_get_pipe_head_loss_option(
-            pipe, heat_network_options, parameters
-        )
+        head_loss_option = network_settings["head_loss_option"]
         assert (
             head_loss_option != HeadLossOption.NO_HEADLOSS
         ), "This method should be skipped when NO_HEADLOSS is set."
 
         length = parameters[f"{pipe}.length"]
 
         if length == 0.0:
@@ -497,46 +573,71 @@
                 return 0.0
 
         if big_m is None:
             assert is_disconnected == 0.0
         else:
             assert big_m != 0.0
 
-        wall_roughness = heat_network_options["wall_roughness"]
-
+        wall_roughness = energy_system_options["wall_roughness"]
         if pipe_class is not None:
             diameter = pipe_class.inner_diameter
             area = pipe_class.area
             maximum_velocity = pipe_class.maximum_velocity
         else:
             diameter = parameters[f"{pipe}.diameter"]
             area = parameters[f"{pipe}.area"]
-            maximum_velocity = heat_network_options["maximum_velocity"]
+            maximum_velocity = network_settings["maximum_velocity"]
+
+        try:
+            # Only heat networks have a temperature attribute in the pipes, otherwise we will use
+            # a default temperature for gas networks
+            temperature = parameters[f"{pipe}.temperature"]
+            for _id, attr in optimization_problem.temperature_carriers().items():
+                if (
+                    parameters[f"{pipe}.carrier_id"] == attr["id_number_mapping"]
+                    and len(
+                        optimization_problem.temperature_regimes(parameters[f"{pipe}.carrier_id"])
+                    )
+                    > 0
+                ):
+                    temperature = min(
+                        optimization_problem.temperature_regimes(parameters[f"{pipe}.carrier_id"])
+                    )
+        except KeyError:
+            # A default temperature of 20 degrees celcius is used for gas networks.
+            temperature = 20.0
 
-        temperature = parameters[f"{pipe}.temperature"]
-        has_control_valve = parameters[f"{pipe}.has_control_valve"]
+        try:
+            has_control_valve = parameters[f"{pipe}.has_control_valve"]
+        except KeyError:
+            has_control_valve = False
 
         if head_loss_option == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY:
             assert not has_control_valve
 
             ff = darcy_weisbach.friction_factor(
-                heat_network_options["maximum_velocity"], diameter, wall_roughness, temperature
+                maximum_velocity,
+                diameter,
+                wall_roughness,
+                temperature,
+                network_type=network_type,
+                pressure=pressure,
             )
 
             # Compute c_v constant (where |dH| ~ c_v * v^2)
             c_v = length * ff / (2 * GRAVITATIONAL_CONSTANT) / diameter
 
-            linearization_velocity = heat_network_options["maximum_velocity"]
+            linearization_velocity = maximum_velocity
             linearization_head_loss = c_v * linearization_velocity**2
             linearization_discharge = linearization_velocity * area
 
             expr = linearization_head_loss * discharge / linearization_discharge
 
             if symbolic:
-                constraint_nominal = c_v * heat_network_options["estimated_velocity"] ** 2
+                constraint_nominal = c_v * maximum_velocity**2
                 # Interior point solvers, like IPOPT, do not like linearly dependent
                 # tight inequality constraints. For this reason, we split the
                 # constraints depending whether the Big-M formulation is used or not.
                 if big_m is None:
                     return [((-1 * dh - expr) / constraint_nominal, 0.0, 0.0)]
                 else:
                     constraint_nominal = (constraint_nominal * big_m) ** 0.5
@@ -557,15 +658,20 @@
                 return expr * np.sign(discharge)
 
         elif head_loss_option in {
             HeadLossOption.CQ2_INEQUALITY,
             HeadLossOption.CQ2_EQUALITY,
         }:
             ff = darcy_weisbach.friction_factor(
-                heat_network_options["estimated_velocity"], diameter, wall_roughness, temperature
+                energy_system_options["estimated_velocity"],
+                diameter,
+                wall_roughness,
+                temperature,
+                network_type=network_type,
+                pressure=pressure,
             )
 
             # Compute c_v constant (where |dH| ~ c_v * v^2)
             c_v = length * ff / (2 * GRAVITATIONAL_CONSTANT) / diameter
 
             v = discharge / area
             expr = c_v * v**2
@@ -603,85 +709,191 @@
                                 0.0,
                             ),
                         )
                 return equations
             else:
                 return expr
 
-        elif head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY:
-            n_lines = heat_network_options["n_linearization_lines"]
+        elif (
+            head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
+            or head_loss_option == HeadLossOption.LINEARIZED_N_LINES_EQUALITY
+        ):
+            n_linear_lines = network_settings["n_linearization_lines"]
+            n_timesteps = len(optimization_problem.times())
 
             a, b = darcy_weisbach.get_linear_pipe_dh_vs_q_fit(
                 diameter,
                 length,
                 wall_roughness,
                 temperature=temperature,
-                n_lines=n_lines,
+                n_lines=n_linear_lines,
                 v_max=maximum_velocity,
+                network_type=self.network_settings["network_type"],
+                pressure=parameters[f"{pipe}.pressure"],
             )
 
             # The function above only gives result in the positive quadrant
             # (positive head loss, positive discharge). We also need a
             # positive head loss for _negative_ discharges.
             a = np.hstack([-a, a])
             b = np.hstack([b, b])
 
             # Vectorize constraint for speed
             if symbolic:
-                q_nominal = self.variable_nominal(f"{pipe}.Q")
-                head_loss_nominal = self.variable_nominal(f"{pipe}.dH")
+                q_nominal = optimization_problem.variable_nominal(f"{pipe}.Q")
+                head_loss_nominal = optimization_problem.variable_nominal(f"{pipe}.dH")
                 head_loss_vec = ca.repmat(head_loss, len(a))
                 discharge_vec = ca.repmat(discharge, len(a))
+
                 if isinstance(is_disconnected, ca.MX):
                     is_disconnected_vec = ca.repmat(is_disconnected, len(a))
                 else:
-                    is_disconnected_vec = is_disconnected
+                    # is_disconnected_vec = is_disconnected
+                    is_disconnected_vec = (
+                        np.ones((len(a) * discharge.size1(), 1), dtype=float) * is_disconnected
+                    )
 
                 a_vec = np.repeat(a, discharge.size1())
                 b_vec = np.repeat(b, discharge.size1())
+
                 constraint_nominal = np.abs(head_loss_nominal * a_vec * q_nominal) ** 0.5
 
                 if big_m is None:
                     # We write the equation such that big_m is always used, even if
                     # it is None (i.e. not used). We do have to be sure to set it to 0,
                     # because we cannot multiple with "None".
                     big_m_lin = 0.0
                 else:
                     big_m_lin = big_m
                     constraint_nominal = (constraint_nominal * big_m_lin) ** 0.5
-                return [
+
+                constraints = []
+
+                # Add weak inequality constraint, value >= 0.0 for all linear lines
+                constraints.append(
                     (
                         (
                             head_loss_vec
                             - (a_vec * discharge_vec + b_vec)
                             + is_disconnected_vec * big_m_lin
                         )
                         / constraint_nominal,
                         0.0,
                         np.inf,
-                    )
-                ]
+                    ),
+                )
+                if head_loss_option == HeadLossOption.LINEARIZED_N_LINES_EQUALITY:
+                    # Add constraints for piece-wise linear equality
+
+                    # Populate variable indicating if a linear line segment is active (1) or not (0)
+                    # pipe_linear_line_segment: will contain variables of negative and positive
+                    # discharge possibilites for the pipe. This implies if a pipe is linearized
+                    # with N = 2 linear lines then pipe_linear_line_segment will have 2 * 2
+                    # variables
+                    # Order of linear line variables:
+                    #  - negative discharge line_1, line_2
+                    #  - positve discharge line_1, line_2
+                    pipe_linear_line_segment = self._pipe_linear_line_segment_map[pipe]
+                    is_line_segment_active = []
+
+                    for _, ii_line_var in pipe_linear_line_segment.items():
+                        # Create integer variable to activate/deactivate (1/0) a linear line
+                        # segment
+                        is_line_segment_active_var = optimization_problem.state_vector(ii_line_var)
+
+                        # Linear line segment activation variable for each time step of demand
+                        # profile
+                        is_line_segment_active.append(is_line_segment_active_var)
+
+                    # Calculate constraint to enforce that only 1 linear line segment can be active
+                    # per time step for the current pipe for the entire time horizon
+                    for itstep in range(n_timesteps):
+                        is_line_segment_active_sum_per_timestep = 0.0
+                        for ii_line in range(len(pipe_linear_line_segment)):
+
+                            is_line_segment_active_sum_per_timestep = (
+                                is_line_segment_active_sum_per_timestep
+                                + is_line_segment_active[ii_line][itstep]
+                            )
+                        constraints.append(
+                            (is_line_segment_active_sum_per_timestep, 1.0, 1.0),
+                        )
+
+                    # Add equality constraint, value == 0.0 for all linear lines
+                    # Loop twice due to linear lines exsiting for negative and positive discharge
+                    # ii==0: this is the linear lines for the negative discharge possibility
+                    # ii==1: this is the linear lines for the postive discharge possibility
+                    for ii in range(2):
+                        for ii_line in range(n_linear_lines):
+                            ii_line_used = (ii * 2) + ii_line
+
+                            ii_start = (ii_line + 2 * ii) * n_timesteps
+                            ii_end = ii_start + n_timesteps
+                            constraints.append(
+                                (
+                                    (
+                                        head_loss_vec[ii_start:ii_end]
+                                        - (
+                                            a_vec[ii_start:ii_end] * discharge_vec[ii_start:ii_end]
+                                            + b_vec[ii_start:ii_end]
+                                        )
+                                        + is_disconnected_vec[ii_start:ii_end] * big_m_lin
+                                        + big_m_lin
+                                        * (1 - is_line_segment_active[ii_line_used][0:n_timesteps])
+                                    )
+                                    / constraint_nominal[ii_start:ii_end],
+                                    0.0,
+                                    np.inf,
+                                ),
+                            )
+                    for ii in range(2):
+                        for ii_line in range(n_linear_lines):
+                            ii_line_used = (ii * 2) + ii_line
+
+                            ii_start = (ii_line + 2 * ii) * n_timesteps
+                            ii_end = ii_start + n_timesteps
+                            constraints.append(
+                                (
+                                    (
+                                        head_loss_vec[ii_start:ii_end]
+                                        - (
+                                            a_vec[ii_start:ii_end] * discharge_vec[ii_start:ii_end]
+                                            + b_vec[ii_start:ii_end]
+                                        )
+                                        - is_disconnected_vec[ii_start:ii_end] * big_m_lin
+                                        - big_m_lin
+                                        * (1 - is_line_segment_active[ii_line_used][0:n_timesteps])
+                                    )
+                                    / constraint_nominal[ii_start:ii_end],
+                                    -np.inf,
+                                    0.0,
+                                ),
+                            )
+                return constraints
             else:
                 ret = np.amax(a * np.tile(discharge, (len(a), 1)).transpose() + b, axis=1)
                 if isinstance(discharge, float):
                     ret = ret[0]
                 return ret
 
     def _hydraulic_power(
         self,
         pipe: str,
-        heat_network_options,
+        optimization_problem,
+        energy_system_options,
+        network_settings,
         parameters,
         discharge: Union[ca.MX, float, np.ndarray],
         hydraulic_power: Optional[Union[ca.MX, float, np.ndarray]] = None,
         dh: Optional[ca.MX] = None,
         is_disconnected: Union[ca.MX, int] = 0,
         big_m: Optional[float] = None,
         pipe_class: Optional[PipeClass] = None,
         flow_dir: Union[ca.MX, int] = 0,
+        pressure: float = 0.0,
     ) -> Union[List[Tuple[ca.MX, BT, BT]], float, np.ndarray]:
         """
         This function has two purposes:
         - return the hydraulic power constraint expression(s) or
         - compute the hydraulic power numerically (always positive).
 
         Note: the discharge value can be negative. In such a case the hydraulic_power in the
@@ -702,22 +914,22 @@
 
         `is_disconnected` can be used to specify whether a pipe is
         disconnected or not. This is most useful if a (boolean) ca.MX symbol
         is passed, which can then be used with a big-M formulation. The big-M
         itself then also needs to be passed via the `big_m` keyword argument.
         """
 
+        network_type = network_settings["network_type"]
+
         if hydraulic_power is None:
             symbolic = False
         else:
             symbolic = True
 
-        head_loss_option = self._hn_get_pipe_head_loss_option(
-            pipe, heat_network_options, parameters
-        )
+        head_loss_option = network_settings["head_loss_option"]
         assert (
             head_loss_option != HeadLossOption.NO_HEADLOSS
         ), "This method should be skipped when NO_HEADLOSS is set."
 
         length = parameters[f"{pipe}.length"]
 
         if length == 0.0:
@@ -742,39 +954,59 @@
                 return 0.0
 
         if big_m is None:
             assert is_disconnected == 0.0
         else:
             assert big_m != 0.0
 
-        wall_roughness = heat_network_options["wall_roughness"]
-        temperature = parameters[f"{pipe}.temperature"]
+        wall_roughness = energy_system_options["wall_roughness"]
+        if network_type == NetworkSettings.NETWORK_TYPE_HEAT:
+            temperature = parameters[f"{pipe}.temperature"]
+            for _id, attr in optimization_problem.temperature_carriers().items():
+                if (
+                    parameters[f"{pipe}.carrier_id"] == attr["id_number_mapping"]
+                    and len(
+                        optimization_problem.temperature_regimes(parameters[f"{pipe}.carrier_id"])
+                    )
+                    > 0
+                ):
+                    temperature = min(
+                        optimization_problem.temperature_regimes(parameters[f"{pipe}.carrier_id"])
+                    )
+        else:
+            # A default temperature of 20 degrees celcius is used for gas networks.
+            temperature = 20.0
         rho = parameters[f"{pipe}.rho"]
 
         if pipe_class is not None:
             diameter = pipe_class.inner_diameter
             area = pipe_class.area
             maximum_velocity = pipe_class.maximum_velocity
         else:
             diameter = parameters[f"{pipe}.diameter"]
             area = parameters[f"{pipe}.area"]
-            maximum_velocity = heat_network_options["maximum_velocity"]
+            maximum_velocity = network_settings["maximum_velocity"]
 
         constraint_nominal = abs(
             parameters[f"{pipe}.rho"]
             * GRAVITATIONAL_CONSTANT
-            * self.variable_nominal(f"{pipe}.dH")
-            * self.variable_nominal(f"{pipe}.Q")
+            * optimization_problem.variable_nominal(f"{pipe}.dH")
+            * optimization_problem.variable_nominal(f"{pipe}.Q")
         )
 
         if head_loss_option == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY:
             # Uitlized maximum_velocity instead of estimated_velocity (used in head loss linear
             # calc)
             ff = darcy_weisbach.friction_factor(
-                maximum_velocity, diameter, wall_roughness, temperature
+                maximum_velocity,
+                diameter,
+                wall_roughness,
+                temperature,
+                network_type=network_type,
+                pressure=pressure,
             )
             # Compute c_k constant (where |hydraulic power| ~ c_k * v^3)
             c_k = rho * ff * length * area / 2.0 / diameter
             # Compute linearized value
             max_hydraulic_power = c_k * maximum_velocity**3
             maximum_discharge = maximum_velocity * area
             hydraulic_power_linearized = max_hydraulic_power * discharge / maximum_discharge
@@ -836,24 +1068,29 @@
                             -np.inf,
                             0.0,
                         ),
                     ]
             else:
                 return abs(hydraulic_power_linearized)
 
-        elif head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY:
-            n_lines = heat_network_options["n_linearization_lines"]
+        elif (
+            head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
+            or HeadLossOption.LINEARIZED_N_LINES_EQUALITY
+        ):
+            n_lines = network_settings["n_linearization_lines"]
             a_coef, b_coef = darcy_weisbach.get_linear_pipe_power_hydraulic_vs_q_fit(
                 rho,
                 diameter,
                 length,
                 wall_roughness,
                 temperature=temperature,
                 n_lines=n_lines,
                 v_max=maximum_velocity,
+                network_type=self.network_settings["network_type"],
+                pressure=parameters[f"{pipe}.pressure"],
             )
             discharge_vec = ca.repmat(discharge, len(a_coef))
             hydraulic_power_linearized_vec = a_coef * discharge_vec + b_coef
 
             if symbolic:
                 hydraulic_power_vec = ca.repmat(hydraulic_power, len(a_coef))
 
@@ -903,211 +1140,431 @@
                 if isinstance(discharge, float):
                     max_hydraulic_power_linearized = max_hydraulic_power_linearized[0]
                 return abs(max_hydraulic_power_linearized)
         else:
             assert (
                 head_loss_option == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
                 or head_loss_option == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY
-            ), "This method only caters for head_loss_option: LINEARIZED_ONE_LINE_EQUALITY &"
-            "LINEARIZED_N_LINES_WEAK_INEQUALITY."
+                or head_loss_option == HeadLossOption.LINEARIZED_N_LINES_EQUALITY
+            ), "This method only caters for head_loss_option: "
+            "LINEARIZED_ONE_LINE_EQUALITY & LINEARIZED_N_LINES_WEAK_INEQUALITY."
 
-    def __pipe_head_loss_path_constraints(self, _ensemble_member):
+    def _pipe_head_loss_path_constraints(self, optimization_problem, _ensemble_member):
         """
         We set this constraint relating .dH to the upstream and downstream
         heads here in the Mixin for scaling purposes (dH nominal is
         calculated in pre()).
         """
         constraints = []
 
-        for pipe in self.energy_system_components.get("pipe", []):
-            dh = self.state(f"{pipe}.dH")
-            h_down = self.state(f"{pipe}.HeatOut.H")
-            h_up = self.state(f"{pipe}.HeatIn.H")
+        if self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_HEAT:
+            commodity = "Heat"
+            pipe_type = "heat_pipe"
+        elif self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_GAS:
+            commodity = "Gas"
+            pipe_type = "gas_pipe"
+        else:
+            raise Exception(
+                f"hydraulic power can not be calculated for network type of "
+                f"{self.network_settings['network_type']}"
+            )
+
+        for pipe in optimization_problem.energy_system_components.get(pipe_type, []):
+            dh = optimization_problem.state(f"{pipe}.dH")
+            h_down = optimization_problem.state(f"{pipe}.{commodity}Out.H")
+            h_up = optimization_problem.state(f"{pipe}.{commodity}In.H")
 
             constraint_nominal = (
-                self.variable_nominal(f"{pipe}.dH") * self.variable_nominal(f"{pipe}.HeatIn.H")
+                optimization_problem.variable_nominal(f"{pipe}.dH")
+                * optimization_problem.variable_nominal(f"{pipe}.{commodity}In.H")
             ) ** 0.5
             constraints.append(((dh - (h_down - h_up)) / constraint_nominal, 0.0, 0.0))
 
         return constraints
 
-    def __demand_head_loss_path_constraints(self, _ensemble_member):
+    def _demand_head_loss_path_constraints(self, optimization_problem, _ensemble_member):
         """
         This function adds constraints for a minimum pressure drop at demands. This minimum
         pressure drop is often required in practice to guarantee that it is possible to increase
         the flow rate at that specific demand, if needed, by opening the control valve.
         """
         constraints = []
 
-        options = self.heat_network_options()
-        components = self.energy_system_components
+        options = optimization_problem.energy_system_options()
+        components = optimization_problem.energy_system_components
 
         # Convert minimum pressure at far point from bar to meter (water) head
         min_head_loss = options["minimum_pressure_far_point"] * 10.2
 
-        for d in components.get("demand", []):
+        for d in components.get("heat_demand", []):
             constraints.append(
                 (
-                    self.state(f"{d}.HeatIn.H") - self.state(f"{d}.HeatOut.H"),
+                    optimization_problem.state(f"{d}.HeatIn.H")
+                    - optimization_problem.state(f"{d}.HeatOut.H"),
                     min_head_loss,
                     np.inf,
                 )
             )
 
         return constraints
 
-    def constraints(self, ensemble_member):
-        """
-        Here we add the pipe head loss constraints
+    def _pipe_head_loss_constraints(
+        self, optimization_problem, _maximum_total_head_loss, ensemble_member
+    ):
         """
-        constraints = super().constraints(ensemble_member)
+        This function adds the head loss constraints for pipes. There are two options namely with
+        and without pipe class optimization. In both cases we assume that disconnected pipes, pipes
+        without flow have no head loss.
+
+        Under pipe-class optimization the head loss constraints per pipe class are added and
+        applied with the big_m method (is_topo_disconnected) to only activate the correct
+        constraints.
 
-        if self.heat_network_options()["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
-            constraints.extend(self._hn_pipe_head_loss_constraints(ensemble_member))
-
-        return constraints
-
-    def path_constraints(self, ensemble_member):
+        Under constant pipe class constraints for only one diameter are added.
         """
-        Here we add the path constraints for the head in pipes and minimum pressure drop at demands.
-        """
-        constraints = super().path_constraints(ensemble_member).copy()
-
-        options = self.heat_network_options()
-
-        # Add source/demand head loss constrains only if head loss is non-zero
-        if options["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
-            constraints.extend(self.__pipe_head_loss_path_constraints(ensemble_member))
-            constraints.extend(self.__demand_head_loss_path_constraints(ensemble_member))
-
-        return constraints
+        constraints = []
 
-    def priority_started(self, priority):
-        """
-        Keeping track of the priority in the optimization
-        """
-        super().priority_started(priority)
-        self.__priority = priority
+        options = optimization_problem.energy_system_options()
+        parameters = optimization_problem.parameters(ensemble_member)
+        components = optimization_problem.energy_system_components
+        # Set the head loss according to the direction in the pipes. Note that
+        # the `.__head_loss` symbol is always positive by definition, but that
+        # `.dH` is not (positive when flow is negative, and vice versa).
+        # If the pipe is disconnected, we leave the .__head_loss symbol free
+        # (and it has no physical meaning). We also do not set any discharge
+        # relationship in this case (but dH is still equal to Out - In of
+        # course).
+
+        if self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_HEAT:
+            commodity = "heat"
+            n_type = "hn"
+        elif self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_GAS:
+            commodity = "gas"
+            n_type = "gn"
+        else:
+            raise Exception(
+                f"hydraulic power can not be calculated for network type of "
+                f"{self.network_settings['network_type']}"
+            )
+        pipe_type = f"{commodity}_pipe"
 
-    def priority_completed(self, priority):
-        """
-        In this funtion we check whether there is still artificial head loss in pipes after the
-        head loss minimization goal. This can happen when there are multiple routes without control
-        valves towards a single consumer.In this case the optimization can create non-physical
-        solutions for the inequality head loss options where it favours one route above another.
-        This favoured route would also have a head loss which would not possible in practice and
-        could not be compensated for by a control valve along the route.
-        """
-        super().priority_completed(priority)
+        pipe_head_loss_map = getattr(optimization_problem, f"_{n_type}_pipe_to_head_loss_map")
+        is_disconnected_map = getattr(optimization_problem, f"_{commodity}_pipe_disconnect_map")
+        pipe_topo_class_map = getattr(
+            optimization_problem, f"_{commodity}_pipe_topo_pipe_class_map"
+        )
+        pipe_to_flow_direct_map = getattr(
+            optimization_problem, f"_{commodity}_pipe_to_flow_direct_map"
+        )
 
-        options = self.heat_network_options()
+        for pipe in components.get(pipe_type, []):
+            if parameters[f"{pipe}.length"] == 0.0:
+                # If the pipe does not have a control valve, the head loss is
+                # forced to zero via bounds. If the pipe _does_ have a control
+                # valve, then there still is no relationship between the
+                # discharge and the head loss/dH.
+                continue
+
+            head_loss_sym = pipe_head_loss_map[pipe]
+
+            dh = _state_vector_scaled(optimization_problem, f"{pipe}.dH", ensemble_member)
+            head_loss = _state_vector_scaled(optimization_problem, head_loss_sym, ensemble_member)
+            discharge = _state_vector_scaled(optimization_problem, f"{pipe}.Q", ensemble_member)
+
+            # We need to make sure the dH is decoupled from the discharge when
+            # the pipe is disconnected. Simply put, this means making the
+            # below constraints trivial.
+            is_disconnected_var = is_disconnected_map.get(pipe)
 
-        if (
-            options["minimize_head_losses"]
-            and options["head_loss_option"] != HeadLossOption.NO_HEADLOSS
-            and priority == self._hn_minimization_goal_class.priority
-        ):
-            components = self.energy_system_components
+            if is_disconnected_var is None:
+                is_disconnected = 0.0
+            else:
+                is_disconnected = _state_vector_scaled(
+                    optimization_problem, is_disconnected_var, ensemble_member
+                )
 
-            rtol = 1e-5
-            atol = 1e-4
+            max_discharge = None
+            max_head_loss = -np.inf
 
-            for ensemble_member in range(self.ensemble_size):
-                parameters = self.parameters(ensemble_member)
-                results = self.extract_results(ensemble_member)
+            if pipe in pipe_topo_class_map:
+                # Multiple diameter options for this pipe
+                pipe_classes = pipe_topo_class_map[pipe]
+                max_discharge = max(c.maximum_discharge for c in pipe_classes)
 
-                for pipe in components["pipe"]:
-                    if parameters[f"{pipe}.has_control_valve"]:
+                for pc, pc_var_name in pipe_classes.items():
+                    if pc.inner_diameter == 0.0:
                         continue
 
-                    # Just like with a control valve, if pipe is disconnected
-                    # there is nothing to check.
-                    q_full = results[f"{pipe}.Q"]
-                    if parameters[f"{pipe}.disconnectable"]:
-                        inds = q_full != 0.0
-                    else:
-                        inds = np.arange(len(q_full), dtype=int)
-
-                    if parameters[f"{pipe}.diameter"] == 0.0:
-                        # Pipe is disconnected. Head loss is free, so nothing to check.
-                        continue
+                    head_loss_max_discharge = self._hn_pipe_head_loss(
+                        pipe,
+                        optimization_problem,
+                        options,
+                        self.network_settings,
+                        parameters,
+                        max_discharge,
+                        pipe_class=pc,
+                        pressure=parameters[f"{pipe}.pressure"],
+                    )
 
-                    q = results[f"{pipe}.Q"][inds]
-                    head_loss_target = self._hn_pipe_head_loss(pipe, options, parameters, q, None)
-                    if options["head_loss_option"] == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY:
-                        head_loss = np.abs(results[f"{pipe}.dH"][inds])
+                    if self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_HEAT:
+                        big_m = max(1.1 * _maximum_total_head_loss, 2 * head_loss_max_discharge)
+                    elif self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_GAS:
+                        big_m = max(
+                            2.0 * 2.0 * _maximum_total_head_loss, 2 * head_loss_max_discharge
+                        )
                     else:
-                        head_loss = results[self._hn_pipe_to_head_loss_map[pipe]][inds]
+                        raise RuntimeError(
+                            f"{self.network_settings['network_type']} is not of type Gas or Heat "
+                            f"thus no maximum total headloss is given"
+                        )
+
+                    is_topo_disconnected = 1 - optimization_problem.extra_variable(
+                        pc_var_name, ensemble_member
+                    )
+                    is_topo_disconnected = ca.repmat(is_topo_disconnected, dh.size1())
 
-                    if not np.allclose(head_loss, head_loss_target, rtol=rtol, atol=atol):
-                        logger.warning(
-                            f"Pipe {pipe} has artificial head loss; "
-                            f"at least one more control valve should be added to the network."
+                    # Note that we add the two booleans `is_disconnected` and
+                    # `is_topo_disconnected`. This is allowed because of the way the
+                    # resulting expression is used in the Big-M formulation. We only care
+                    # that the expression (i.e. a single boolean or the sum of the two
+                    # booleans) is either 0 when the pipe is connected, or >= 1 when it
+                    # is disconnected.
+                    constraints.extend(
+                        self._hn_pipe_head_loss(
+                            pipe,
+                            optimization_problem,
+                            options,
+                            self.network_settings,
+                            parameters,
+                            discharge,
+                            head_loss,
+                            dh,
+                            is_disconnected + is_topo_disconnected,
+                            big_m,
+                            pc,
+                            pressure=parameters[f"{pipe}.pressure"],
                         )
+                    )
 
-                min_head_loss_target = options["minimum_pressure_far_point"] * 10.2
-                min_head_loss = None
+                    # Contrary to the Big-M calculation above, the relation
+                    # between dH and the head loss symbol requires the
+                    # maximum head loss that can be realized effectively. So
+                    # we pass the current pipe class's maximum discharge.
+                    max_head_loss = max(
+                        max_head_loss,
+                        self._hn_pipe_head_loss(
+                            pipe,
+                            optimization_problem,
+                            options,
+                            self.network_settings,
+                            parameters,
+                            pc.maximum_discharge,
+                            pipe_class=pc,
+                            pressure=parameters[f"{pipe}.pressure"],
+                        ),
+                    )
+            else:
+                # Only a single diameter for this pipe. Note that we rely on
+                # the diameter parameter being overridden automatically if a
+                # single pipe class is set by the user.
+                area = parameters[f"{pipe}.area"]
+                max_discharge = self.network_settings["maximum_velocity"] * area
+
+                is_topo_disconnected = int(parameters[f"{pipe}.diameter"] == 0.0)
+
+                if self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_HEAT:
+                    big_m = 1.1 * _maximum_total_head_loss
+                elif self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_GAS:
+                    big_m = 2.0 * 2.0 * _maximum_total_head_loss
+                else:
+                    raise RuntimeError(
+                        f"{self.network_settings['network_type']} is not of type Gas or Heat thus "
+                        f"no maximum total headloss is given"
+                    )
 
-                for demand in components["demand"]:
-                    head_loss = results[f"{demand}.HeatIn.H"] - results[f"{demand}.HeatOut.H"]
-                    if min_head_loss is None:
-                        min_head_loss = head_loss
-                    else:
-                        min_head_loss = np.minimum(min_head_loss, head_loss)
+                constraints.extend(
+                    self._hn_pipe_head_loss(
+                        pipe,
+                        optimization_problem,
+                        options,
+                        self.network_settings,
+                        parameters,
+                        discharge,
+                        head_loss,
+                        dh,
+                        is_disconnected + is_topo_disconnected,
+                        big_m=big_m,
+                        pressure=parameters[f"{pipe}.pressure"],
+                    )
+                )
 
-                if not np.allclose(min_head_loss, min_head_loss_target, rtol=rtol, atol=atol):
-                    logger.warning("Minimum head at demands is higher than target minimum.")
+                max_head_loss = self._hn_pipe_head_loss(
+                    pipe,
+                    optimization_problem,
+                    options,
+                    self.network_settings,
+                    parameters,
+                    max_discharge,
+                    pressure=parameters[f"{pipe}.pressure"],
+                )
 
-    def path_goals(self):
-        """
-        Here we add the goals for minimizing the head loss and hydraulic power depending on the
-        configuration. Please note that we only do hydraulic power for the MILP problem thus only
-        for the linearized head_loss options.
-        """
-        g = super().path_goals().copy()
+            # Relate the head loss symbol to the pipe's dH symbol.
 
-        options = self.heat_network_options()
-        if (
-            options["minimize_head_losses"]
-            and options["head_loss_option"] != HeadLossOption.NO_HEADLOSS
-        ):
-            g.append(self._hn_minimization_goal_class(self))
+            # FIXME: Ugly hack. Cold pipes should be modelled completely with
+            # their own integers as well.
+            flow_dir = _state_vector_scaled(
+                optimization_problem, pipe_to_flow_direct_map[pipe], ensemble_member
+            )
 
-            if (
-                options["head_loss_option"] == HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY
-                or options["head_loss_option"] == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
-            ):
-                g.append(self._hpwr_minimization_goal_class(self))
+            # Note that the Big-M should _at least_ cover the maximum
+            # distance between `head_loss` and `dh`. If `head_loss` can be at
+            # most 1.0 (= `max_head_loss`), that means our Big-M should be at
+            # least double (i.e. >= 2.0). And because we do not want Big-Ms to
+            # be overly tight, we include an additional factor of 2.
+            big_m = 2 * 2 * max_head_loss
 
-        return g
+            constraints.append(
+                (
+                    (-dh - head_loss + (1 - flow_dir) * big_m) / big_m,
+                    0.0,
+                    np.inf,
+                )
+            )
+            constraints.append(((dh - head_loss + flow_dir * big_m) / big_m, 0.0, np.inf))
 
-    @property
-    def path_variables(self):
-        """
-        Here we add the pipe head loss path-variables to the problem.
-        """
-        variables = super().path_variables.copy()
-        variables.extend(self.__pipe_head_loss_var.values())
-        return variables
+        return constraints
 
-    def variable_nominal(self, variable):
-        """
-        Here we add the nominal for the head loss path-variable to the problem.
+    def _pipe_hydraulic_power_path_constraints(
+        self, optimization_problem, _maximum_total_head_loss, ensemble_member
+    ):
         """
-        try:
-            return self.__pipe_head_loss_nominals[variable]
-        except KeyError:
-            return super().variable_nominal(variable)
+        This function adds constraints to compute the hydraulic power that is needed to realize the
+        flow, compensating the pressure drop through the pipe. Similar to the head loss constraints
+        we allow two supported methods. 1) a single linear line between 0 to max velocity. 2) A
+        multiple line inequality approach where one can use the minimize_head_losses == True option
+        to drag down the solution to the actual physical solution.
 
-    def bounds(self):
+        Note that the linearizations are made separately from the pressure drop constraints, this is
+        done to avoid "stacked" overestimations.
         """
-        Here we add the bounds for the head loss variable to the problem.
-        """
-        bounds = super().bounds().copy()
+        constraints = []
+        options = optimization_problem.energy_system_options()
+
+        if self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_HEAT:
+            commodity = "heat"
+        elif self.network_settings["network_type"] == NetworkSettings.NETWORK_TYPE_GAS:
+            commodity = "gas"
+        else:
+            raise Exception(
+                f"hydraulic power can not be calculated for network type of "
+                f"{self.network_settings['network_type']}"
+            )
+        pipe_type = f"{commodity}_pipe"
 
-        bounds.update(self.__pipe_head_loss_bounds)
-        bounds.update(self.__pipe_head_loss_zero_bounds)
+        pipe_topo_class_map = getattr(
+            optimization_problem, f"_{commodity}_pipe_topo_pipe_class_map"
+        )
 
-        for k, v in self.__pipe_head_bounds.items():
-            bounds[k] = self.merge_bounds(bounds[k], v)
+        if self.network_settings["head_loss_option"] != HeadLossOption.NO_HEADLOSS:
+            parameters = optimization_problem.parameters(ensemble_member)
+            components = optimization_problem.energy_system_components
+
+            for pipe in components.get(pipe_type, []):
+                if parameters[f"{pipe}.length"] == 0.0:
+                    # If the pipe does not have a control valve, the head loss is
+                    # forced to zero via bounds. If the pipe _does_ have a control
+                    # valve, then there still is no relationship between the
+                    # discharge and the hydraulic_power.
+                    continue
+
+                # TODO: I think the upcomming 8 lines can be removed (e.g. head_loss_option)
+                if pipe_type == "heat_pipe":
+                    head_loss_option = optimization_problem._hn_get_pipe_head_loss_option(
+                        pipe, self.network_settings, parameters
+                    )
+                else:
+                    head_loss_option = self.network_settings["head_loss_option"]
+                assert (
+                    head_loss_option != HeadLossOption.NO_HEADLOSS
+                ), "This method should be skipped when NO_HEADLOSS is set."
+
+                discharge = optimization_problem.state(f"{pipe}.Q")
+                hydraulic_power = optimization_problem.state(f"{pipe}.Hydraulic_power")
+                rho = parameters[f"{pipe}.rho"]
+
+                # 0: pipe is connected, 1: pipe is disconnected
+                is_disconnected_var = getattr(
+                    optimization_problem, f"_{commodity}_pipe_disconnect_map"
+                ).get(pipe)
+                # optimization_problem._pipe_disconnect_map.get(pipe)
+                if is_disconnected_var is None:
+                    is_disconnected = 0.0
+                else:
+                    is_disconnected = optimization_problem.state(is_disconnected_var)
 
-        return bounds
+                flow_dir_var = getattr(
+                    optimization_problem, f"_{commodity}_pipe_to_flow_direct_map"
+                ).get(pipe)
+                flow_dir = optimization_problem.state(
+                    flow_dir_var
+                )  # 0/1: negative/positive flow direction
+
+                if pipe in pipe_topo_class_map:
+                    # Multiple diameter options for this pipe
+                    pipe_classes = pipe_topo_class_map[pipe]
+                    max_discharge = max(c.maximum_discharge for c in pipe_classes)
+                    for pc, pc_var_name in pipe_classes.items():
+                        if pc.inner_diameter == 0.0:
+                            continue
+
+                        # Calc max hydraulic power based on maximum_total_head_loss =
+                        # f(max_sum_dh_pipes, max_dh_network_options)
+                        max_total_hydraulic_power = 2.0 * (
+                            rho * GRAVITATIONAL_CONSTANT * _maximum_total_head_loss * max_discharge
+                        )
+
+                        # is_topo_disconnected - 0: pipe selected, 1: pipe disconnected/not selected
+                        # self.__pipe_topo_pipe_class_var - value 0: pipe is not selected, 1: pipe
+                        # is selected
+                        is_topo_disconnected = 1 - optimization_problem.variable(pc_var_name)
+
+                        constraints.extend(
+                            self._hydraulic_power(
+                                pipe,
+                                optimization_problem,
+                                options,
+                                self.network_settings,
+                                parameters,
+                                discharge,
+                                hydraulic_power,
+                                is_disconnected=is_topo_disconnected + is_disconnected,
+                                big_m=max_total_hydraulic_power,
+                                pipe_class=pc,
+                                flow_dir=flow_dir,
+                                pressure=parameters[f"{pipe}.pressure"],
+                            )
+                        )
+                else:
+                    is_topo_disconnected = int(parameters[f"{pipe}.diameter"] == 0.0)
+                    max_total_hydraulic_power = 2.0 * (
+                        rho
+                        * GRAVITATIONAL_CONSTANT
+                        * _maximum_total_head_loss
+                        * parameters[f"{pipe}.area"]
+                        * self.network_settings["maximum_velocity"]
+                    )
+                    constraints.extend(
+                        self._hydraulic_power(
+                            pipe,
+                            optimization_problem,
+                            options,
+                            self.network_settings,
+                            parameters,
+                            discharge,
+                            hydraulic_power,
+                            is_disconnected=is_disconnected + is_topo_disconnected,
+                            big_m=max_total_hydraulic_power,
+                            flow_dir=flow_dir,
+                            pressure=parameters[f"{pipe}.pressure"],
+                        )
+                    )
+        return constraints
```

### Comparing `mesido-0.1.1/src/mesido/qth_not_maintained/qth_loop_mixin.py` & `mesido-0.1.2/src/mesido/qth_not_maintained/qth_loop_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/qth_not_maintained/qth_mixin.py` & `mesido-0.1.2/src/mesido/qth_not_maintained/qth_mixin.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/qth_not_maintained/util.py` & `mesido-0.1.2/src/mesido/qth_not_maintained/util.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/techno_economic_mixin.py` & `mesido-0.1.2/src/mesido/techno_economic_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,24 +50,24 @@
             self._asset_aggregation_count_var_map[asset_name], ensemble_member
         )
 
     def get_aggregation_count_max(self, asset_name):
         return self.bounds()[self._asset_aggregation_count_var_map[asset_name]][1]
 
     def get_pipe_class_map(self):
-        return self._pipe_topo_pipe_class_map
+        return self._heat_pipe_topo_pipe_class_map
 
     def get_gas_pipe_class_map(self):
         return self._gas_pipe_topo_pipe_class_map
 
     def get_electricity_cable_class_map(self):
         return self._electricity_cable_topo_cable_class_map
 
     def get_pipe_investment_cost_coefficient(self, asset_name, ensemble_member):
-        return self.extra_variable(self._pipe_topo_cost_map[asset_name], ensemble_member)
+        return self.extra_variable(self._heat_pipe_topo_cost_map[asset_name], ensemble_member)
 
     def get_electricity_carriers(self):
         return self.electricity_carriers()
 
     def get_gas_carriers(self):
         return self.gas_carriers()
```

### Comparing `mesido-0.1.1/src/mesido/topology.py` & `mesido-0.1.2/src/mesido/topology.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/workflows/__init__.py` & `mesido-0.1.2/src/mesido/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/workflows/goals/minimize_tco_goal.py` & `mesido-0.1.2/src/mesido/workflows/goals/minimize_tco_goal.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/workflows/grow_workflow.py` & `mesido-0.1.2/src/mesido/workflows/grow_workflow.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/workflows/io/read_files_and_create_influxdb.py` & `mesido-0.1.2/src/mesido/workflows/io/read_files_and_create_influxdb.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/workflows/io/write_output.py` & `mesido-0.1.2/src/mesido/workflows/io/write_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,14 +483,17 @@
                 name="Energy production [Wh]",
                 distribution=esdl.StringLabelDistribution(
                     stringItem=[
                         esdl.StringItem(label=key, value=value)
                         for key, value in heat_source_energy_wh.items()
                     ]
                 ),
+                quantityAndUnit=esdl.esdl.QuantityAndUnitType(
+                    physicalQuantity=esdl.PhysicalQuantityEnum.ENERGY, unit=esdl.UnitEnum.WATTHOUR
+                ),
             )
         )
         energy_system.instance[0].area.KPIs = kpis_top_level
         # ------------------------------------------------------------------------------------------
         # Cost breakdowns per polygon areas (can consist of several assets of differents types)
         # Notes:
         # - OPEX KPIs are taken into account for energy sources only.
@@ -894,61 +897,63 @@
                 *self.energy_system_components.get("heat_demand", []),
                 *self.energy_system_components.get("heat_pipe", []),
                 *self.energy_system_components.get("heat_buffer", []),
                 *self.energy_system_components.get("ates", []),
                 *self.energy_system_components.get("heat_exchanger", []),
                 *self.energy_system_components.get("heat_pump", []),
             ]:
-                # Note: when adding new variables to variables_one_hydraulic_system or"
-                # variables_two_hydraulic_system also add quantity and units to the ESDL for the new
-                # variables in the code lower down
-                # These variables exist for all the assets. Variables that only exist for specific
-                # assets are only added later, like Pump_power
-                variables_one_hydraulic_system = ["HeatIn.Q", "Heat_flow"]
-                variables_two_hydraulic_system = [
-                    "Primary.HeatIn.Q",
-                    "Secondary.HeatIn.Q",
-                    "Heat_flow",
-                ]
-
-                # Update/overwrite each asset variable list due to:
-                # - the addition of head loss minimization: head variable and pump power
-                # - only a specific variable required for a specific asset: pump power
-                # - addition of post processed variables: pipe velocity
-                if self.heat_network_settings["minimize_head_losses"]:
-                    variables_one_hydraulic_system.append("HeatIn.H")
-                    variables_two_hydraulic_system.append("Primary.HeatIn.H")
-                    variables_two_hydraulic_system.append("Secondary.HeatIn.H")
-                    if asset_name in [
-                        *self.energy_system_components.get("heat_source", []),
-                        *self.energy_system_components.get("heat_buffer", []),
-                        *self.energy_system_components.get("ates", []),
-                        *self.energy_system_components.get("heat_exchanger", []),
-                        *self.energy_system_components.get("heat_pump", []),
-                    ]:
-                        variables_one_hydraulic_system.append("Pump_power")
-                        variables_two_hydraulic_system.append("Pump_power")
-                    elif asset_name in [*self.energy_system_components.get("pump", [])]:
-                        variables_one_hydraulic_system = ["Pump_power"]
-                        variables_two_hydraulic_system = ["Pump_power"]
-                if asset_name in [*self.energy_system_components.get("heat_pipe", [])]:
-                    variables_one_hydraulic_system.append("PostProc.Velocity")
-                    variables_two_hydraulic_system.append("PostProc.Velocity")
-                    # Velocity at the pipe outlet [m/s]
-                    post_processed_velocity = (
-                        results[f"{asset_name}.HeatOut.Q"] / parameters[f"{asset_name}.area"]
-                    )
-
-                profiles = ProfileManager()
-                profiles.profile_type = "DATETIME_LIST"
-                profiles.profile_header = ["datetime"]
                 try:
                     # If the asset has been placed
                     asset = _name_to_asset(asset_name)
 
+                    # Note: when adding new variables to variables_one_hydraulic_system or"
+                    # variables_two_hydraulic_system also add quantity and units to the ESDL for
+                    # the new variables in the code lower down
+                    # These variables exist for all the assets. Variables that only exist for
+                    # specific
+                    # assets are only added later, like Pump_power
+                    variables_one_hydraulic_system = ["HeatIn.Q", "Heat_flow"]
+                    variables_two_hydraulic_system = [
+                        "Primary.HeatIn.Q",
+                        "Secondary.HeatIn.Q",
+                        "Heat_flow",
+                    ]
+
+                    # Update/overwrite each asset variable list due to:
+                    # - the addition of head loss minimization: head variable and pump power
+                    # - only a specific variable required for a specific asset: pump power
+                    # - addition of post processed variables: pipe velocity
+                    if self.heat_network_settings["minimize_head_losses"]:
+                        variables_one_hydraulic_system.append("HeatIn.H")
+                        variables_two_hydraulic_system.append("Primary.HeatIn.H")
+                        variables_two_hydraulic_system.append("Secondary.HeatIn.H")
+                        if asset_name in [
+                            *self.energy_system_components.get("heat_source", []),
+                            *self.energy_system_components.get("heat_buffer", []),
+                            *self.energy_system_components.get("ates", []),
+                            *self.energy_system_components.get("heat_exchanger", []),
+                            *self.energy_system_components.get("heat_pump", []),
+                        ]:
+                            variables_one_hydraulic_system.append("Pump_power")
+                            variables_two_hydraulic_system.append("Pump_power")
+                        elif asset_name in [*self.energy_system_components.get("pump", [])]:
+                            variables_one_hydraulic_system = ["Pump_power"]
+                            variables_two_hydraulic_system = ["Pump_power"]
+                    if asset_name in [*self.energy_system_components.get("heat_pipe", [])]:
+                        variables_one_hydraulic_system.append("PostProc.Velocity")
+                        variables_two_hydraulic_system.append("PostProc.Velocity")
+                        # Velocity at the pipe outlet [m/s]
+                        post_processed_velocity = (
+                            results[f"{asset_name}.HeatOut.Q"] / parameters[f"{asset_name}.area"]
+                        )
+
+                    profiles = ProfileManager()
+                    profiles.profile_type = "DATETIME_LIST"
+                    profiles.profile_header = ["datetime"]
+
                     # Get index of outport which will be used to assign the profile data to
                     index_outport = -1
                     for ip in range(len(asset.port)):
                         if isinstance(asset.port[ip], esdl.OutPort):
                             if index_outport == -1:
                                 index_outport = ip
                             else:
```

### Comparing `mesido-0.1.1/src/mesido/workflows/simulator_workflow.py` & `mesido-0.1.2/src/mesido/workflows/simulator_workflow.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/workflows/utils/adapt_profiles.py` & `mesido-0.1.2/src/mesido/workflows/utils/adapt_profiles.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido/workflows/utils/helpers.py` & `mesido-0.1.2/src/mesido/workflows/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/src/mesido.egg-info/PKG-INFO` & `mesido-0.1.2/src/mesido.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesido
-Version: 0.1.1
+Version: 0.1.2
 Summary: Multi Energy System Optimization
 Home-page: https://github.com/Multi-Energy-Systems-Optimization/mesido/
 Author: Jim Rojer
 Author-email: jim.rojer@tno.nl
 Maintainer: Jim Rojer, Kobus van Rooyen, Kelbij Star, Femke Janssen, Jesús Andrés Rodríguez Sarasty, Thijs van der Klauw
 License: LGPLv3
 Keywords: Multi-Energy-Systems,optimization
```

### Comparing `mesido-0.1.1/src/mesido.egg-info/SOURCES.txt` & `mesido-0.1.2/src/mesido.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/mesido/heat_network_common.py
 src/mesido/heat_physics_mixin.py
 src/mesido/network_common.py
 src/mesido/physics_mixin.py
 src/mesido/pipe_class.py
 src/mesido/techno_economic_mixin.py
 src/mesido/topology.py
+src/mesido/util.py
 src/mesido.egg-info/PKG-INFO
 src/mesido.egg-info/SOURCES.txt
 src/mesido.egg-info/dependency_links.txt
 src/mesido.egg-info/entry_points.txt
 src/mesido.egg-info/requires.txt
 src/mesido.egg-info/top_level.txt
 src/mesido/esdl/__init__.py
@@ -104,14 +105,15 @@
 src/mesido/pycml/component_library/milp/gas/gas_pipe.py
 src/mesido/pycml/component_library/milp/gas/gas_source.py
 src/mesido/pycml/component_library/milp/gas/gas_substation.py
 src/mesido/pycml/component_library/milp/gas/gas_tank_storage.py
 src/mesido/pycml/component_library/milp/heat/__init__.py
 src/mesido/pycml/component_library/milp/heat/_non_storage_component.py
 src/mesido/pycml/component_library/milp/heat/air_water_heat_pump.py
+src/mesido/pycml/component_library/milp/heat/airco.py
 src/mesido/pycml/component_library/milp/heat/ates.py
 src/mesido/pycml/component_library/milp/heat/check_valve.py
 src/mesido/pycml/component_library/milp/heat/cold_demand.py
 src/mesido/pycml/component_library/milp/heat/control_valve.py
 src/mesido/pycml/component_library/milp/heat/geothermal_source.py
 src/mesido/pycml/component_library/milp/heat/heat_buffer.py
 src/mesido/pycml/component_library/milp/heat/heat_demand.py
@@ -122,15 +124,18 @@
 src/mesido/pycml/component_library/milp/heat/heat_pump.py
 src/mesido/pycml/component_library/milp/heat/heat_source.py
 src/mesido/pycml/component_library/milp/heat/heat_two_port.py
 src/mesido/pycml/component_library/milp/heat/low_temperature_ates.py
 src/mesido/pycml/component_library/milp/heat/node.py
 src/mesido/pycml/component_library/milp/heat/pump.py
 src/mesido/pycml/component_library/milp/multicommodity/__init__.py
+src/mesido/pycml/component_library/milp/multicommodity/airwater_heat_pump_elec.py
+src/mesido/pycml/component_library/milp/multicommodity/electro_boiler.py
 src/mesido/pycml/component_library/milp/multicommodity/electrolyzer.py
+src/mesido/pycml/component_library/milp/multicommodity/gas_boiler.py
 src/mesido/pycml/component_library/qth/__init__.py
 src/mesido/pycml/component_library/qth/_fluid_properties_component.py
 src/mesido/pycml/component_library/qth/_non_storage_component.py
 src/mesido/pycml/component_library/qth/buffer.py
 src/mesido/pycml/component_library/qth/check_valve.py
 src/mesido/pycml/component_library/qth/control_valve.py
 src/mesido/pycml/component_library/qth/demand.py
@@ -146,14 +151,15 @@
 src/mesido/qth_not_maintained/__init__.py
 src/mesido/qth_not_maintained/bounds_to_pipe_flow_directions_mixin.py
 src/mesido/qth_not_maintained/head_loss_mixin.py
 src/mesido/qth_not_maintained/qth_loop_mixin.py
 src/mesido/qth_not_maintained/qth_mixin.py
 src/mesido/qth_not_maintained/util.py
 src/mesido/workflows/__init__.py
+src/mesido/workflows/emerge.py
 src/mesido/workflows/grow_workflow.py
 src/mesido/workflows/simulator_workflow.py
 src/mesido/workflows/goals/__init__.py
 src/mesido/workflows/goals/minimize_tco_goal.py
 src/mesido/workflows/io/__init__.py
 src/mesido/workflows/io/read_files_and_create_influxdb.py
 src/mesido/workflows/io/write_output.py
@@ -161,22 +167,25 @@
 src/mesido/workflows/utils/adapt_profiles.py
 src/mesido/workflows/utils/helpers.py
 tests/test_absolute_heat.py
 tests/test_asset_is_realized.py
 tests/test_ates.py
 tests/test_cable_topology_optimization.py
 tests/test_cold_demand.py
+tests/test_elec_boiler.py
 tests/test_electric_bus.py
 tests/test_electric_source_sink.py
 tests/test_electrolyzer.py
+tests/test_emerge.py
 tests/test_end_scenario_sizing.py
 tests/test_end_scenario_sizing_annualized.py
 tests/test_esdl_parsing.py
 tests/test_esdl_pycml.py
 tests/test_examples.py
+tests/test_gas_boiler.py
 tests/test_gas_multi_demand_source_node.py
 tests/test_gas_pipe_topology_optimization.py
 tests/test_gas_source_sink.py
 tests/test_head_loss.py
 tests/test_head_loss_class.py
 tests/test_heat.py
 tests/test_heat_loss_u_values.py
@@ -190,9 +199,11 @@
 tests/test_pipe_diameter_sizing.py
 tests/test_producer_profiles.py
 tests/test_profile_parsing.py
 tests/test_pycml.py
 tests/test_setpoint_constraints.py
 tests/test_temperature_ates_hp.py
 tests/test_topo_constraints.py
+tests/test_updated_esdl_post_process.py
+tests/test_updated_esdl_pre_process.py
 tests/test_varying_temperature.py
 tests/test_warmingup_unit_cases.py
```

### Comparing `mesido-0.1.1/tests/test_absolute_heat.py` & `mesido-0.1.2/tests/test_absolute_heat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
-
-from rtctools.util import run_optimization_problem
+from mesido.util import run_esdl_mesido_optimization
 
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestAbsoluteHeat(TestCase):
     def test_absolute_heat(self):
         """
@@ -23,15 +22,15 @@
 
         """
         import models.absolute_heat.src.example as example
         from models.absolute_heat.src.example import HeatProblem
 
         base_folder = Path(example.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="absolute_heat.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_asset_is_realized.py` & `mesido-0.1.2/tests/test_asset_is_realized.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 
 class TestAssetIsRealized(TestCase):
     def test_asset_is_realized(self):
         r"""
         This is a test to check the behaviour of the cumulative investments made and the
         asset is realized variable. We want the asset only to become available once sufficient
         investments are made.
@@ -32,15 +31,15 @@
             HeatProblemPlacingOverTime,
         )
 
         base_folder = Path(run_ates.__file__).resolve().parent.parent
 
         # This is an optimization done over 25 timesteps with a cap on how quickly the cost
         # for the 2 producers can be realized
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblemPlacingOverTime,
             base_folder=base_folder,
             esdl_file_name="test_case_small_network_with_ates.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="Warmte_test.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_ates.py` & `mesido-0.1.2/tests/test_ates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestAtes(TestCase):
     def test_ates(self):
         """
         Checks the constraints concerning the milp to discharge and energy conservation
@@ -29,15 +28,15 @@
         from models.test_case_small_network_with_ates.src.run_ates import (
             HeatProblem,
         )
 
         base_folder = Path(run_ates.__file__).resolve().parent.parent
 
         # This is an optimization done over a full year with 365 day timesteps
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="test_case_small_network_with_ates.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="Warmte_test.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_cable_topology_optimization.py` & `mesido-0.1.2/tests/test_cable_topology_optimization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 
 class TestElectricityTopo(TestCase):
     def test_electricity_network_topology(self):
         """
         This test checks the functioning of topology optimization of electricity cables. It uses
         a symmetrical network where the left side should stay in as those cables are shorter.
 
@@ -21,15 +20,15 @@
 
         """
         import models.electricity_cable_topology.src.example as example
         from models.electricity_cable_topology.src.example import HeatProblem
 
         base_folder = Path(example.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="enettopology.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_cold_demand.py` & `mesido-0.1.2/tests/test_cold_demand.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
-
-from rtctools.util import run_optimization_problem
+from mesido.util import run_esdl_mesido_optimization
 
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestColdDemand(TestCase):
     def test_cold_demand(self):
         """
@@ -23,23 +22,53 @@
 
         """
         import models.wko.src.example as example
         from models.wko.src.example import HeatProblem
 
         base_folder = Path(example.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="LT_wko.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
 
         demand_matching_test(heat_problem, heat_problem.extract_results())
         energy_conservation_test(heat_problem, heat_problem.extract_results())
+        heat_to_discharge_test(heat_problem, heat_problem.extract_results())
+
+    def test_airco(self):
+        """
+        This test is to check the basic physics for a network which includes an airco. In this
+        case we have a network with an air-water hp, a low temperature ates and both hot and cold
+        demand. In this case the demands are matched and the low temperature ates is utilized.
+
+        Checks:
+        1. demand is matched
+        2. energy conservation in the network
+        3. heat to discharge
+
+        """
+        import models.wko.src.example as example
+        from models.wko.src.example import HeatProblem
+
+        base_folder = Path(example.__file__).resolve().parent.parent
+
+        heat_problem = run_esdl_mesido_optimization(
+            HeatProblem,
+            base_folder=base_folder,
+            esdl_file_name="airco.esdl",
+            esdl_parser=ESDLFileParser,
+            profile_reader=ProfileReaderFromFile,
+            input_timeseries_file="timeseries.csv",
+        )
+
+        demand_matching_test(heat_problem, heat_problem.extract_results())
+        energy_conservation_test(heat_problem, heat_problem.extract_results())
         heat_to_discharge_test(heat_problem, heat_problem.extract_results())
 
 
 if __name__ == "__main__":
     a = 1
```

### Comparing `mesido-0.1.1/tests/test_electric_bus.py` & `mesido-0.1.2/tests/test_electric_bus.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 """
 
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
 
-from rtctools.util import run_optimization_problem
-
-
 class TestMILPbus(TestCase):
     def test_voltages_and_power_network1(self):
         """
         Checks the behaviour of electricity networks with a bus asset. A bus asset is the
         only asset that is allowed to have more than one electricity port.
 
         Checks:
@@ -35,15 +33,15 @@
         """
         import models.unit_cases_electricity.bus_networks.src.example as example
         from models.unit_cases_electricity.bus_networks.src.example import ElectricityProblem
 
         base_folder = Path(example.__file__).resolve().parent.parent
 
         # Run the problem
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             ElectricityProblem,
             base_folder=base_folder,
             esdl_file_name="Electric_bus3.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_electric_source_sink.py` & `mesido-0.1.2/tests/test_electric_source_sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 
 # TODO: still have to make test where elecitricity direction is switched:
 # e.g. 2 nodes, with at each node a producer and consumer, first one node medium demand, second
 # small demand and then increase the demand of the second node such that direction changes
 
 
 class TestMILPElectricSourceSink(TestCase):
@@ -32,15 +31,15 @@
 
         import models.unit_cases_electricity.source_sink_cable.src.example as example
         from models.unit_cases_electricity.source_sink_cable.src.example import ElectricityProblem
 
         base_folder = Path(example.__file__).resolve().parent.parent
         tol = 1e-10
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             ElectricityProblem,
             base_folder=base_folder,
             esdl_file_name="case1_elec.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
@@ -119,15 +118,15 @@
         import models.unit_cases_electricity.source_sink_cable.src.example as example
         from models.unit_cases_electricity.source_sink_cable.src.example import (
             ElectricityProblemMaxCurr,
         )
 
         base_folder = Path(example.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             ElectricityProblemMaxCurr,
             base_folder=base_folder,
             esdl_file_name="case1_elec.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
@@ -215,15 +214,15 @@
         import models.unit_cases_electricity.source_sink_cable.src.example as example
         from models.unit_cases_electricity.source_sink_cable.src.example import (
             ElectricityProblem,
         )
 
         base_folder = Path(example.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             ElectricityProblem,
             base_folder=base_folder,
             esdl_file_name="transformer.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_electrolyzer.py` & `mesido-0.1.2/tests/test_electrolyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 
 # from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestElectrolyzer(TestCase):
     def test_electrolyzer(self):
         """
@@ -34,15 +33,15 @@
         class MILPProblemSolve(MILPProblem):
             def energy_system_options(self):
                 options = super().energy_system_options()
                 self.gas_network_settings["pipe_maximum_pressure"] = 100.0  # [bar]
                 self.gas_network_settings["pipe_minimum_pressure"] = 0.0
                 return options
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             MILPProblem,
             base_folder=base_folder,
             esdl_file_name="h2.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_end_scenario_sizing.py` & `mesido-0.1.2/tests/test_end_scenario_sizing.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_end_scenario_sizing_annualized.py` & `mesido-0.1.2/tests/test_end_scenario_sizing_annualized.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_esdl_parsing.py` & `mesido-0.1.2/tests/test_esdl_parsing.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_esdl_pycml.py` & `mesido-0.1.2/tests/test_esdl_pycml.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_examples.py` & `mesido-0.1.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_gas_multi_demand_source_node.py` & `mesido-0.1.2/tests/test_gas_multi_demand_source_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
 
-from rtctools.util import run_optimization_problem
-
-
 class TestMILPGasMultiDemandSourceNode(TestCase):
     def test_multi_demand_source_node(self):
         """
         Test a network consisting out of 2 demands, 2 sources and a node. Verify that the head is
         equal for all ports at a node, and throughout the network that the flow (mass) balance is
         maintained.
 
@@ -31,15 +29,15 @@
         class TestGasProblem(GasProblem):
             def energy_system_options(self):
                 options = super().energy_system_options()
                 self.gas_network_settings["pipe_maximum_pressure"] = 100.0  # [bar]
                 self.gas_network_settings["pipe_minimum_pressure"] = 0.0
                 return options
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             GasProblem,
             base_folder=base_folder,
             esdl_file_name="test.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_gas_pipe_topology_optimization.py` & `mesido-0.1.2/tests/test_gas_pipe_topology_optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
 from mesido.head_loss_class import HeadLossOption
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 
 class TestGasNetwork(TestCase):
     def test_gas_pipe_top(self):
         """
         This test checks the functioning of topology optimization of gas pipes. It uses
         a symmetrical network where the left side should stay in as those pipes are shorter.
 
@@ -32,31 +31,31 @@
                 options = super().energy_system_options()
                 self.gas_network_settings["head_loss_option"] = (
                     HeadLossOption.LINEARIZED_ONE_LINE_EQUALITY
                 )
                 self.gas_network_settings["minimize_head_losses"] = True
                 return options
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             GasNetworkProblem,
             base_folder=base_folder,
             esdl_file_name="2a_gas.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
 
         results = solution.extract_results()
 
         for demand in solution.energy_system_components.get("gas_demand", []):
             target = solution.get_timeseries(f"{demand}.target_gas_demand").values
             np.testing.assert_allclose(target, results[f"{demand}.Gas_demand_mass_flow"])
 
-        removed_pipes = ["Pipe_a718", "Pipe_9a6f", "Pipe_2927"]
-        remained_pipes = ["Pipe_51e4", "Pipe_6b39", "Pipe_f9b0"]
+        removed_pipes = ["Pipe_a718", "Pipe_9a6f", "Pipe_2927", "Pipe_8592"]
+        remained_pipes = ["Pipe_51e4", "Pipe_6b39", "Pipe_f9b0", "Pipe_96bc"]
         for pipe in removed_pipes:
             np.testing.assert_allclose(results[f"{pipe}__gn_diameter"], 0.0, atol=1.0e-6)
             np.testing.assert_allclose(results[f"{pipe}__investment_cost"], 0.0, atol=1.0e-6)
             np.testing.assert_allclose(results[f"{pipe}__gn_max_discharge"], 0.0, atol=1.0e-6)
         for pipe in remained_pipes:
             np.testing.assert_array_less(0.0, results[f"{pipe}__gn_diameter"])
             np.testing.assert_array_less(0.0, results[f"{pipe}__investment_cost"])
```

### Comparing `mesido-0.1.1/tests/test_gas_source_sink.py` & `mesido-0.1.2/tests/test_gas_source_sink.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
 from mesido.head_loss_class import HeadLossOption
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
 
-from rtctools.util import run_optimization_problem
-
-
 class TestMILPGasSourceSink(TestCase):
     def test_source_sink(self):
         """
         Test case for a network consisting out of a source, pipes and a sink
 
         Checks:
         - That flow is maintained.
@@ -36,15 +34,15 @@
                 self.heat_network_settings["n_linearization_lines"] = 5
                 self.heat_network_settings["minimize_head_losses"] = True
 
                 self.heat_network_settings["pipe_maximum_pressure"] = 100.0  # [bar]
                 self.heat_network_settings["pipe_minimum_pressure"] = 0.0
                 return options
 
-        soltion = run_optimization_problem(
+        soltion = run_esdl_mesido_optimization(
             GasProblem,
             base_folder=base_folder,
             esdl_file_name="source_sink.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_head_loss.py` & `mesido-0.1.2/tests/test_head_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 import mesido._darcy_weisbach as darcy_weisbach
 from mesido.constants import GRAVITATIONAL_CONSTANT
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
 from mesido.head_loss_class import HeadLossOption
 from mesido.network_common import NetworkSettings
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test
 
 
 class TestHeadLoss(TestCase):
     """
     Test case for a heat network and a gas network consisting out of a source, pipe(s) and a sink
     """
@@ -84,15 +83,15 @@
                 "influxdb_port": 8086,
                 "influxdb_username": None,
                 "influxdb_password": None,
                 "influxdb_ssl": False,
                 "influxdb_verify_ssl": False,
             }
 
-            solution = run_optimization_problem(
+            solution = run_esdl_mesido_optimization(
                 SourcePipeSinkDW,
                 base_folder=base_folder,
                 esdl_file_name="sourcesink.esdl",
                 esdl_parser=ESDLFileParser,
                 profile_reader=ProfileReaderFromFile,
                 input_timeseries_file="timeseries_import.csv",
                 **kwargs,
@@ -260,15 +259,15 @@
 
                     self.heat_network_settings["n_linearization_lines"] = 2
                     self.heat_network_settings["minimum_velocity"] = 0.0
                     self.heat_network_settings["minimize_head_losses"] = True
 
                     return options
 
-            solution = run_optimization_problem(
+            solution = run_esdl_mesido_optimization(
                 SourcePipeSinkDW,
                 base_folder=base_folder,
                 esdl_file_name="sourcesink.esdl",
                 esdl_parser=ESDLFileParser,
                 profile_reader=ProfileReaderFromFile,
                 input_timeseries_file="timeseries_import.csv",
             )
@@ -437,15 +436,15 @@
                     if head_loss_option_setting == HeadLossOption.LINEARIZED_N_LINES_EQUALITY:
                         self.gas_network_settings["n_linearization_lines"] = 2
                         self.gas_network_settings["minimize_head_losses"] = True
                         self.gas_network_settings["minimum_velocity"] = 0.0
 
                     return options
 
-            solution = run_optimization_problem(
+            solution = run_esdl_mesido_optimization(
                 TestSourceSink,
                 base_folder=base_folder,
                 esdl_file_name="source_sink.esdl",
                 esdl_parser=ESDLFileParser,
                 profile_reader=ProfileReaderFromFile,
                 input_timeseries_file="timeseries.csv",
             )
@@ -589,15 +588,15 @@
                         == HeadLossOption.LINEARIZED_N_LINES_WEAK_INEQUALITY
                     ):
                         self.gas_network_settings["n_linearization_lines"] = 2
                         self.gas_network_settings["minimize_head_losses"] = True
 
                     return options
 
-            solution = run_optimization_problem(
+            solution = run_esdl_mesido_optimization(
                 TestSourceSink,
                 base_folder=base_folder,
                 esdl_file_name="source_sink.esdl",
                 esdl_parser=ESDLFileParser,
                 profile_reader=ProfileReaderFromFile,
                 input_timeseries_file="timeseries.csv",
             )
@@ -725,15 +724,15 @@
         _ That the pipes have the expected head loss given their reference pressures
         """
         import models.multiple_gas_carriers.src.run_multiple_gas_carriers as example
         from models.multiple_gas_carriers.src.run_multiple_gas_carriers import GasProblem
 
         base_folder = Path(example.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             GasProblem,
             base_folder=base_folder,
             esdl_file_name="multiple_carriers.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
@@ -774,15 +773,15 @@
         _ That the pipes have the expected head loss given their reference pressures
         """
         import models.multiple_gas_carriers.src.run_multiple_gas_carriers as example
         from models.multiple_gas_carriers.src.run_multiple_gas_carriers import GasProblem
 
         base_folder = Path(example.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             GasProblem,
             base_folder=base_folder,
             esdl_file_name="compressor.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_head_loss_class.py` & `mesido-0.1.2/tests/test_head_loss_class.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_heat.py` & `mesido-0.1.2/tests/test_heat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
 from mesido.head_loss_class import HeadLossOption
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestHeat(TestCase):
     def test_heat_loss(self):
         """
         This is a test to check whether the network (pipes) are dissipating milp as we expect.
@@ -23,15 +22,15 @@
 
         """
         import models.source_pipe_sink.src.double_pipe_heat as double_pipe_heat
         from models.source_pipe_sink.src.double_pipe_heat import SourcePipeSink
 
         base_folder = Path(double_pipe_heat.__file__).resolve().parent.parent
 
-        case = run_optimization_problem(
+        case = run_esdl_mesido_optimization(
             SourcePipeSink,
             base_folder=base_folder,
             esdl_file_name="sourcesink.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.csv",
         )
@@ -65,15 +64,15 @@
                 options = super().energy_system_options()
                 options["neglect_pipe_heat_losses"] = True
 
                 return options
 
         base_folder = Path(double_pipe_heat.__file__).resolve().parent.parent
 
-        case = run_optimization_problem(
+        case = run_esdl_mesido_optimization(
             Model,
             base_folder=base_folder,
             esdl_file_name="sourcesink.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.csv",
         )
@@ -156,39 +155,39 @@
 
         Checks:
         - unbounded problem has requires more pressure drop than allowed by the min and max pressure
         - min pressure
         - max pressure
 
         """
-        case_default = run_optimization_problem(
+        case_default = run_esdl_mesido_optimization(
             self.SmallerPipes,
             base_folder=self.base_folder,
             esdl_file_name=self.esdl_file,
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file=self.input_time_series_file,
         )
-        case_min_pressure = run_optimization_problem(
+        case_min_pressure = run_esdl_mesido_optimization(
             self.MinPressure,
             base_folder=self.base_folder,
             esdl_file_name=self.esdl_file,
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file=self.input_time_series_file,
         )
-        case_max_pressure = run_optimization_problem(
+        case_max_pressure = run_esdl_mesido_optimization(
             self.MaxPressure,
             base_folder=self.base_folder,
             esdl_file_name=self.esdl_file,
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file=self.input_time_series_file,
         )
-        case_min_max_pressure = run_optimization_problem(
+        case_min_max_pressure = run_esdl_mesido_optimization(
             self.MinMaxPressure,
             base_folder=self.base_folder,
             esdl_file_name=self.esdl_file,
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file=self.input_time_series_file,
         )
@@ -289,26 +288,26 @@
 
         Checks:
         - Sanity check that min velocity is >0
         - Check that pipe stays connected when flow is not forced to zero
         - Check that pipe becomes disconnected when flow is forced to zero
 
         """
-        case_connected = run_optimization_problem(
+        case_connected = run_esdl_mesido_optimization(
             self.ModelConnected,
             base_folder=self.base_folder,
             esdl_file_name="sourcesink.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.csv",
         )
         results_connected = case_connected.extract_results()
         q_connected = results_connected["Pipe1.Q"]
 
-        case_disconnected = run_optimization_problem(
+        case_disconnected = run_esdl_mesido_optimization(
             self.ModelDisconnected,
             base_folder=self.base_folder,
             esdl_file_name="sourcesink.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.csv",
         )
@@ -342,26 +341,26 @@
 
         Checks:
         - That the flow is equal for both types of head loss constraint settings.
         - Check that is_disconnected is set correctly.
 
         """
 
-        case_linear = run_optimization_problem(
+        case_linear = run_esdl_mesido_optimization(
             self.ModelDisconnected,
             base_folder=self.base_folder,
             esdl_file_name="sourcesink.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.csv",
         )
         results_linear = case_linear.extract_results()
         q_linear = results_linear["Pipe1.Q"]
 
-        case_dw = run_optimization_problem(
+        case_dw = run_esdl_mesido_optimization(
             self.ModelDisconnectedDarcyWeisbach,
             base_folder=self.base_folder,
             esdl_file_name="sourcesink.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_heat_loss_u_values.py` & `mesido-0.1.2/tests/test_heat_loss_u_values.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_insulation.py` & `mesido-0.1.2/tests/test_insulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 
 class TestInsulation(TestCase):
     """
     This testcase class should contain the following tests:
     1. Test to select the lowest heating demands (best insulation level), check that the
      resulting demands are the same as the original demand (input file) * insulation factor for the
      best insulation level and that the source is sufficient for the demands
@@ -57,15 +56,15 @@
         - Energy conservation and heat to discharge (replace current check of sufficient heat)
 
         """
         import models.insulation.src.run_insulation as run_insulation
         from models.insulation.src.run_insulation import HeatProblem
 
         base_folder = Path(run_insulation.__file__).resolve().parent.parent
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="Insulation.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -137,15 +136,15 @@
         - Check that the other insulation classes are not selected
 
         """
         import models.insulation.src.run_insulation as run_insulation
         from models.insulation.src.run_insulation import HeatProblemB
 
         base_folder = Path(run_insulation.__file__).resolve().parent.parent
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblemB,
             base_folder=base_folder,
             esdl_file_name="Insulation.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
```

### Comparing `mesido-0.1.1/tests/test_max_size_and_optional_assets.py` & `mesido-0.1.2/tests/test_max_size_and_optional_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestMaxSizeAggregationCount(TestCase):
     def test_max_size_and_aggr_count(self):
         """
         Check the behaviour of the asset sizing, asset placement and the cost
@@ -41,15 +40,15 @@
         from models.test_case_small_network_with_ates_with_buffer.src.run_ates import (
             HeatProblem,
         )
 
         base_folder = Path(run_ates.__file__).resolve().parent.parent
 
         # This is an optimization done over a few days
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="test_case_small_network_with_ates_with_buffer.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="Warmte_test.csv",
         )
@@ -141,15 +140,15 @@
         )
 
         base_folder = Path(run_ates.__file__).resolve().parent.parent
 
         # This is the same problem, but now with the buffer and ates also optional.
         # Therefore, we expect that the ates and buffer are no longer placed to avoid their heat
         # losses. This allows us to check if their placement constraints are proper.
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="test_case_small_network_with_ates_with_buffer_all_optional.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="Warmte_test.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_multicommodity.py` & `mesido-0.1.2/tests/test_multicommodity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestMultiCommodityHeatPump(TestCase):
     """Test to verify that the optimisation problem can handle multicommodity problems, relating
     electricity and heat"""
 
@@ -30,15 +28,15 @@
 
         """
         import models.unit_cases_electricity.heat_pump_elec.src.run_hp_elec as run_hp_elec
         from models.unit_cases_electricity.heat_pump_elec.src.run_hp_elec import HeatProblem2
 
         base_folder = Path(run_hp_elec.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblem2,
             base_folder=base_folder,
             esdl_file_name="heat_pump_elec.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -100,15 +98,15 @@
 
         """
         import models.unit_cases_electricity.heat_pump_elec.src.run_hp_elec as run_hp_elec
         from models.unit_cases_electricity.heat_pump_elec.src.run_hp_elec import HeatProblem
 
         base_folder = Path(run_hp_elec.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="heat_pump_elec.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -172,15 +170,15 @@
         import models.unit_cases_electricity.heat_pump_elec.src.run_hp_elec as run_hp_elec
         from models.unit_cases_electricity.heat_pump_elec.src.run_hp_elec import (
             ElectricityProblem,
         )
 
         base_folder = Path(run_hp_elec.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             ElectricityProblem,
             base_folder=base_folder,
             esdl_file_name="heat_pump_elec.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
```

### Comparing `mesido-0.1.1/tests/test_multiple_carriers.py` & `mesido-0.1.2/tests/test_multiple_carriers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
-
-from rtctools.util import run_optimization_problem
+from mesido.util import run_esdl_mesido_optimization
 
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestMultipleCarriers(TestCase):
     def test_multiple_carriers(self):
         """
@@ -22,15 +21,15 @@
         import models.multiple_carriers.src.run_multiple_carriers as run_multiple_carriers
         from models.multiple_carriers.src.run_multiple_carriers import (
             HeatProblem,
         )
 
         base_folder = Path(run_multiple_carriers.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="MultipleCarrierTest.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
```

### Comparing `mesido-0.1.1/tests/test_multiple_in_and_out_port_components.py` & `mesido-0.1.2/tests/test_multiple_in_and_out_port_components.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestHEX(TestCase):
     def test_heat_exchanger(self):
         """
         Check the modelling of the heat exchanger component which allows two hydraulically
@@ -56,15 +55,15 @@
             "influxdb_username": None,
             "influxdb_password": None,
             "influxdb_ssl": False,
             "influxdb_verify_ssl": False,
         }
         # -----------------------------------------------------------------------------------------
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblemPost,
             base_folder=base_folder,
             esdl_file_name="heat_exchanger.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
             **kwargs,
@@ -149,15 +148,15 @@
             "influxdb_username": None,
             "influxdb_password": None,
             "influxdb_ssl": False,
             "influxdb_verify_ssl": False,
         }
         # -----------------------------------------------------------------------------------------
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblemPost,
             base_folder=base_folder,
             esdl_file_name="heat_pump.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
             **kwargs,
```

### Comparing `mesido-0.1.1/tests/test_network_simulator.py` & `mesido-0.1.2/tests/test_network_simulator.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_pipe_diameter_sizing.py` & `mesido-0.1.2/tests/test_pipe_diameter_sizing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import sys
 from pathlib import Path
 from unittest import TestCase
 
 from mesido._darcy_weisbach import friction_factor
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestPipeDiameterSizingExample(TestCase):
     def test_half_network_gone(self):
         """
         This test is to check if the optimization behaves as expected under pipe class optimization.
@@ -45,23 +44,26 @@
         base_folder = (
             Path(examples.pipe_diameter_sizing.src.example.__file__).resolve().parent.parent
         )
 
         del root_folder
         sys.path.pop(1)
 
-        problem = run_optimization_problem(
+        problem = run_esdl_mesido_optimization(
             PipeDiameterSizingProblem,
             base_folder=base_folder,
             esdl_file_name="2a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
 
+        feasibility = problem.solver_stats["return_status"]
+        self.assertTrue((feasibility == "Optimal"))
+
         parameters = problem.parameters(0)
         diameters = {p: parameters[f"{p}.diameter"] for p in problem.hot_pipes}
         results = problem.extract_results()
 
         # Check that half the network is removed, i.e. 4 pipes. Note that it
         # is equally possible for the left or right side of the network to be
         # removed.
```

### Comparing `mesido-0.1.1/tests/test_producer_profiles.py` & `mesido-0.1.2/tests/test_producer_profiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
-
-from rtctools.util import run_optimization_problem
+from mesido.util import run_esdl_mesido_optimization
 
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestProducerMaxProfile(TestCase):
     """
     A test to verify that the producer can have a given scaled profile, where the producer will
@@ -24,15 +23,15 @@
 
     def test_max_producer_profile(self):
         import models.unit_cases.case_3a.src.run_3a as run_3a
         from models.unit_cases.case_3a.src.run_3a import HeatProblemProdProfile
 
         base_folder = Path(run_3a.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblemProdProfile,
             base_folder=base_folder,
             esdl_file_name="3a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
```

### Comparing `mesido-0.1.1/tests/test_profile_parsing.py` & `mesido-0.1.2/tests/test_profile_parsing.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_pycml.py` & `mesido-0.1.2/tests/test_pycml.py`

 * *Files identical despite different names*

### Comparing `mesido-0.1.1/tests/test_setpoint_constraints.py` & `mesido-0.1.2/tests/test_setpoint_constraints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
 import pytest
 
-from rtctools.util import run_optimization_problem
-
 
 class TestSetpointConstraints(TestCase):
     @pytest.mark.first
     def test_setpoint_constraints(self):
         """
         his function checks the working of the setpoint constraints for a few cases to ensure the
         behaviour is as expected. The setpoint constraints are used to enforce a maximum number of
@@ -27,26 +26,26 @@
 
         """
         import models.unit_cases.case_3a.src.run_3a as run_3a
         from models.unit_cases.case_3a.src.run_3a import HeatProblemSetPointConstraints
 
         base_folder = Path(run_3a.__file__).resolve().parent.parent
 
-        _heat_problem_3 = run_optimization_problem(
+        _heat_problem_3 = run_esdl_mesido_optimization(
             HeatProblemSetPointConstraints,
             base_folder=base_folder,
             esdl_file_name="3a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
             **{"timed_setpoints": {"GeothermalSource_b702": (45, 1)}},
         )
         results_3 = _heat_problem_3.extract_results()
 
-        _heat_problem_4 = run_optimization_problem(
+        _heat_problem_4 = run_esdl_mesido_optimization(
             HeatProblemSetPointConstraints,
             base_folder=base_folder,
             esdl_file_name="3a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
             **{"timed_setpoints": {"GeothermalSource_b702": (45, 0)}},
@@ -56,15 +55,15 @@
         # Here we check whehter the ESDLAdditionalVarsMixin is working as intended when
         # a constraint for the setpoints is specified
         import models.unit_cases.case_3a_setpoint.src.run_3a as run_3a
         from models.unit_cases.case_3a_setpoint.src.run_3a import HeatProblem
 
         base_folder = Path(run_3a.__file__).resolve().parent.parent
 
-        sol_esdl_setpoints = run_optimization_problem(
+        sol_esdl_setpoints = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="3a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -110,15 +109,15 @@
 
         """
         import models.test_case_small_network_with_ates.src.run_ates as run_ates
         from models.test_case_small_network_with_ates.src.run_ates import HeatProblemSetPoints
 
         base_folder = Path(run_ates.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblemSetPoints,
             base_folder=base_folder,
             esdl_file_name="test_case_small_network_with_ates.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="Warmte_test.csv",
             **{"timed_setpoints": {"HeatProducer_1": (24 * 365, 2)}},
@@ -146,28 +145,28 @@
 
         """
         import models.test_case_small_network_with_ates.src.run_ates as run_ates
         from models.test_case_small_network_with_ates.src.run_ates import HeatProblemSetPoints
 
         base_folder = Path(run_ates.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblemSetPoints,
             base_folder=base_folder,
             esdl_file_name="test_case_small_network_with_ates.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="Warmte_test.csv",
             **{"timed_setpoints": {"HeatProducer_1": (24 * 365, 0)}},  # not change at all - works
         )
         results = solution.extract_results()
         check = abs(
             results["HeatProducer_1.Heat_source"][2:] - results["HeatProducer_1.Heat_source"][1:-1]
         )
-        np.testing.assert_array_less(check, 1.0e-6)
+        np.testing.assert_array_less(check, 1.0e-5)
 
     @pytest.mark.fourth
     def test_run_small_ates_timed_setpoints_multiple_constraints(self):
         """
         Run the small network with ATES and check that the setpoint changes as specified.
         The heat source for producer_1 changes 8 times (consecutively) when no timed_setpoints are
         specified. The 1 year heat demand profiles contains demand values: hourly (peak day), weekly
@@ -182,15 +181,15 @@
         """
         import models.test_case_small_network_with_ates.src.run_ates as run_ates
         from models.test_case_small_network_with_ates.src.run_ates import HeatProblemSetPoints
 
         base_folder = Path(run_ates.__file__).resolve().parent.parent
 
         for ihrs in range(119, 122):
-            solution = run_optimization_problem(
+            solution = run_esdl_mesido_optimization(
                 HeatProblemSetPoints,
                 base_folder=base_folder,
                 esdl_file_name="test_case_small_network_with_ates.esdl",
                 esdl_parser=ESDLFileParser,
                 profile_reader=ProfileReaderFromFile,
                 input_timeseries_file="Warmte_test.csv",
                 **{"timed_setpoints": {"HeatProducer_1": (ihrs, 1)}},
```

### Comparing `mesido-0.1.1/tests/test_temperature_ates_hp.py` & `mesido-0.1.2/tests/test_temperature_ates_hp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestAtesTemperature(TestCase):
     """
     Checks the constraints concerning the temperature changes in the ates as a result of heat
     loss and charging
@@ -38,15 +37,15 @@
         - heat loss ates>= relation of heat loss
         """
         import models.ates_temperature.src.run_ates_temperature as run_ates_temperature
         from models.ates_temperature.src.run_ates_temperature import HeatProblem
 
         basefolder = Path(run_ates_temperature.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=basefolder,
             esdl_file_name="HP_ATES with return network.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="Warmte_test_3.csv",
         )
@@ -92,18 +91,14 @@
             )
             + sum(
                 parameters["GenericProducer_4dfe.variable_operational_cost_coefficient"]
                 * results["GenericProducer_4dfe.Heat_source"]
             )
         )
 
-        feasibility = solution.solver_stats["return_status"]
-
-        self.assertTrue((feasibility == "Optimal"))
-
         np.testing.assert_allclose(objective_calc / 1e4, objective)
 
         np.testing.assert_array_less(ates_temperature_disc - tol, ates_temperature)
         np.testing.assert_array_less(
             ates_temperature_disc - tol,
             sum(
                 [
@@ -156,15 +151,15 @@
         """
 
         import models.ates_temperature.src.run_ates_temperature as run_ates_temperature
         from models.ates_temperature.src.run_ates_temperature import HeatProblemMaxFlow
 
         basefolder = Path(run_ates_temperature.__file__).resolve().parent.parent
 
-        solution = run_optimization_problem(
+        solution = run_esdl_mesido_optimization(
             HeatProblemMaxFlow,
             base_folder=basefolder,
             esdl_file_name="HP_ATES with return network.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="Warmte_test_3.csv",
         )
```

### Comparing `mesido-0.1.1/tests/test_topo_constraints.py` & `mesido-0.1.2/tests/test_topo_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 from unittest import TestCase
 
 from mesido._heat_loss_u_values_pipe import pipe_heat_loss
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
 from mesido.pipe_class import PipeClass
 from mesido.techno_economic_mixin import TechnoEconomicMixin
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 import numpy.testing
 
-from rtctools.util import run_optimization_problem
-
-
 MIP_TOLERANCE = 1e-8
 
 
 class TestTopoConstraintsOnPipeDiameterSizingExample(TestCase):
     """
     Tests the topo variables and constraints of heat_mixin on the Pipe Diameter Sizing example.
     """
@@ -39,15 +37,15 @@
         base_folder = (
             Path(examples.pipe_diameter_sizing.src.example.__file__).resolve().parent.parent
         )
 
         del root_folder
         sys.path.pop(1)
 
-        cls.problem = run_optimization_problem(
+        cls.problem = run_esdl_mesido_optimization(
             PipeDiameterSizingProblem,
             base_folder=base_folder,
             esdl_file_name="2a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
```

### Comparing `mesido-0.1.1/tests/test_varying_temperature.py` & `mesido-0.1.2/tests/test_varying_temperature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido._heat_loss_u_values_pipe import pipe_heat_loss
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestVaryingTemperature(TestCase):
     def test_1a_temperature_variation(self):
         """
         This test is to check if the varying network temperature works as expected on a simple
@@ -29,15 +28,15 @@
 
         """
         import models.unit_cases.case_1a.src.run_1a as run_1a
         from models.unit_cases.case_1a.src.run_1a import HeatProblemTvar
 
         base_folder = Path(run_1a.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblemTvar,
             base_folder=base_folder,
             esdl_file_name="1a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -93,15 +92,15 @@
 
         """
         import models.unit_cases.case_3a.src.run_3a as run_3a
         from models.unit_cases.case_3a.src.run_3a import HeatProblemTvarsup
 
         base_folder = Path(run_3a.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblemTvarsup,
             base_folder=base_folder,
             esdl_file_name="3a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -165,15 +164,15 @@
 
         """
         import models.unit_cases.case_3a.src.run_3a as run_3a
         from models.unit_cases.case_3a.src.run_3a import HeatProblemTvarret
 
         base_folder = Path(run_3a.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblemTvarret,
             base_folder=base_folder,
             esdl_file_name="3a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -229,15 +228,15 @@
 
         """
         import models.heat_exchange.src.run_heat_exchanger as run_heat_exchanger
         from models.heat_exchange.src.run_heat_exchanger import HeatProblemTvar
 
         base_folder = Path(run_heat_exchanger.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblemTvar,
             base_folder=base_folder,
             esdl_file_name="heat_exchanger.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -295,15 +294,15 @@
 
         """
         import models.heat_exchange.src.run_heat_exchanger as run_heat_exchanger
         from models.heat_exchange.src.run_heat_exchanger import HeatProblemTvarDisableHEX
 
         base_folder = Path(run_heat_exchanger.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblemTvarDisableHEX,
             base_folder=base_folder,
             esdl_file_name="heat_exchanger.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -337,15 +336,15 @@
 
         """
         import models.heat_exchange.src.run_heat_exchanger as run_heat_exchanger
         from models.heat_exchange.src.run_heat_exchanger import HeatProblemTvarSecondary
 
         base_folder = Path(run_heat_exchanger.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblemTvarSecondary,
             base_folder=base_folder,
             esdl_file_name="heat_exchanger.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -375,15 +374,15 @@
 
         """
         import models.heatpump.src.run_heat_pump as run_heat_pump
         from models.heatpump.src.run_heat_pump import HeatProblemTvar
 
         base_folder = Path(run_heat_pump.__file__).resolve().parent.parent
 
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblemTvar,
             base_folder=base_folder,
             esdl_file_name="heat_pump.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
```

### Comparing `mesido-0.1.1/tests/test_warmingup_unit_cases.py` & `mesido-0.1.2/tests/test_warmingup_unit_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from mesido.esdl.esdl_parser import ESDLFileParser
 from mesido.esdl.profile_parser import ProfileReaderFromFile
+from mesido.util import run_esdl_mesido_optimization
 
 import numpy as np
 
-from rtctools.util import run_optimization_problem
-
 from utils_tests import demand_matching_test, energy_conservation_test, heat_to_discharge_test
 
 
 class TestWarmingUpUnitCases(TestCase):
     def test_1a(self):
         """
         This is the most basic check where we have a simple network and check for the basic physics.
@@ -30,15 +29,15 @@
         """
         import models.unit_cases.case_1a.src.run_1a as run_1a
         from models.unit_cases.case_1a.src.run_1a import HeatProblem
 
         base_folder = Path(run_1a.__file__).resolve().parent.parent
 
         # Just a "problem is not infeasible"
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="1a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -99,15 +98,15 @@
         """
         import models.unit_cases.case_2a.src.run_2a as run_2a
         from models.unit_cases.case_2a.src.run_2a import HeatProblem
 
         base_folder = Path(run_2a.__file__).resolve().parent.parent
 
         # Just a "problem is not infeasible"
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="2a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
@@ -135,15 +134,15 @@
         """
         import models.unit_cases.case_3a.src.run_3a as run_3a
         from models.unit_cases.case_3a.src.run_3a import HeatProblem
 
         base_folder = Path(run_3a.__file__).resolve().parent.parent
 
         # Just a "problem is not infeasible"
-        heat_problem = run_optimization_problem(
+        heat_problem = run_esdl_mesido_optimization(
             HeatProblem,
             base_folder=base_folder,
             esdl_file_name="3a.esdl",
             esdl_parser=ESDLFileParser,
             profile_reader=ProfileReaderFromFile,
             input_timeseries_file="timeseries_import.xml",
         )
```

### Comparing `mesido-0.1.1/versioneer.py` & `mesido-0.1.2/versioneer.py`

 * *Files identical despite different names*

