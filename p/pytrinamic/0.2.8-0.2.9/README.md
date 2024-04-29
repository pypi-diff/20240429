# Comparing `tmp/pytrinamic-0.2.8.tar.gz` & `tmp/pytrinamic-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrinamic-0.2.8.tar", last modified: Mon Jan 15 12:35:53 2024, max compression
+gzip compressed data, was "pytrinamic-0.2.9.tar", last modified: Mon Apr 29 07:18:35 2024, max compression
```

## Comparing `pytrinamic-0.2.8.tar` & `pytrinamic-0.2.9.tar`

### file list

```diff
@@ -1,176 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.214512 pytrinamic-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-01-15 12:35:53.214512 pytrinamic-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.182512 pytrinamic-0.2.8/pytrinamic/
--rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/RAMDebug.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.186512 pytrinamic-0.2.8/pytrinamic/connections/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.186512 pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/can_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15837 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/dummy_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/serial_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/uart_ic_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/connections/usb_tmcl_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.194512 pytrinamic-0.2.8/pytrinamic/evalboards/
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/MAX22216_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2100_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2130_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2160_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2208_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2209_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2224_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2225_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2240_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2300_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2590_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC2660_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC4361_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC4671_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5031_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5041_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5062_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5072_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5130_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5160_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5160_shield.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5240_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC5272_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC6100_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC6140_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC6200_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC6300_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/TMC7300_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/evalboards/tmcl_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.198512 pytrinamic-0.2.8/pytrinamic/features/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/abn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/abn_encoder_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/absolute_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/absolute_encoder_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/coolstep.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/coolstep_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/current.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/current_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/current_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/digital_hall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/digital_hall_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/drive_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17239 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/drive_setting_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/linear_ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/linear_ramp_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/linear_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/motor_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/motor_control_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/motor_control_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/pid_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/ramp_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/ramp_settings_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/s_ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/s_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/six_point_ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/six_point_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/solenoid.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/solenoid_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/solenoid_control_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/solenoid_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/stallguard2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/stallguard2_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/features/stallguard2_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.206512 pytrinamic-0.2.8/pytrinamic/ic/
--rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/MAX22216.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2100.py
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2130.py
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2160.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2208.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2209.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2224.py
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2225.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2240.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2300.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2590.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC2660.py
--rw-r--r--   0 runner    (1001) docker     (127)    38601 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC4361.py
--rw-r--r--   0 runner    (1001) docker     (127)    49444 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC4671.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC5031.py
--rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC5041.py
--rw-r--r--   0 runner    (1001) docker     (127)    14668 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC5062.py
--rw-r--r--   0 runner    (1001) docker     (127)    26092 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC5072.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC5130.py
--rw-r--r--   0 runner    (1001) docker     (127)    34406 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC5160.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC5240.py
--rw-r--r--   0 runner    (1001) docker     (127)    23692 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC5272.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC6100.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC6140.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC6200.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC6300.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/TMC7300.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/ic/tmc_ic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.210512 pytrinamic-0.2.8/pytrinamic/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/Landungsbruecke.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCC160.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1021.py
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1111.py
--rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1140.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1141.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1160.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1161.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM123x_0_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1240.py
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1260.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1270.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1276.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1370.py
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1617.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1630.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1633.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1636.py
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1637.py
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1638.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1640.py
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM1670.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM3110.py
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM3312.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM3351.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM6110.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM6212.py
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM6214.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/TMCM_Python.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/canopen_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/tmc_eval_shield.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/modules/tmcl_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.210512 pytrinamic-0.2.8/pytrinamic/referencedesigns/
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/referencedesigns/TMC4671_LEV_REF.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/referencedesigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/tmcl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.214512 pytrinamic-0.2.8/pytrinamic/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/tools/velocity_ramp_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/pytrinamic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.214512 pytrinamic-0.2.8/pytrinamic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-01-15 12:35:53.000000 pytrinamic-0.2.8/pytrinamic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-01-15 12:35:53.000000 pytrinamic-0.2.8/pytrinamic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 12:35:53.000000 pytrinamic-0.2.8/pytrinamic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 12:35:53.000000 pytrinamic-0.2.8/pytrinamic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-15 12:35:53.000000 pytrinamic-0.2.8/pytrinamic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-15 12:35:53.000000 pytrinamic-0.2.8/pytrinamic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-15 12:35:53.214512 pytrinamic-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:35:53.214512 pytrinamic-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/tests/test_can_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-01-15 12:35:45.000000 pytrinamic-0.2.8/tests/test_interface_timeouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.274637 pytrinamic-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 07:18:35.274637 pytrinamic-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.242637 pytrinamic-0.2.9/pytrinamic/
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/RAMDebug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.246637 pytrinamic-0.2.9/pytrinamic/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.246637 pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/can_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15837 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/dummy_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/serial_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/uart_ic_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/connections/usb_tmcl_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.254637 pytrinamic-0.2.9/pytrinamic/evalboards/
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/MAX22216_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2100_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2130_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2160_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2208_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2209_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2224_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2225_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2240_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2590_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC2660_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC4361_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC4671_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5031_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5041_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5062_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5072_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5130_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5160_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5160_shield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5240_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5262_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5271_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC5272_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC6100_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC6140_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC6200_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC6300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/TMC7300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/evalboards/tmcl_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.258637 pytrinamic-0.2.9/pytrinamic/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/abn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/abn_encoder_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/absolute_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/absolute_encoder_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/coolstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/coolstep_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/current_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/current_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/digital_hall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/digital_hall_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/drive_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17239 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/drive_setting_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/linear_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/linear_ramp_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/linear_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/motor_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/motor_control_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/motor_control_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/pid_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/ramp_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/ramp_settings_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/s_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/s_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/six_point_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/six_point_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/solenoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/solenoid_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/solenoid_control_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/solenoid_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/stallguard2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/stallguard2_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/features/stallguard2_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.266637 pytrinamic-0.2.9/pytrinamic/ic/
+-rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/MAX22216.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2130.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2160.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2208.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2209.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2224.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2225.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2240.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2300.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2590.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC2660.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38601 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC4361.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49444 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC4671.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5031.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5041.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14668 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5062.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26092 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5072.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5130.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34406 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5160.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5240.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5262.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5271.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31406 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC5272.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC6100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC6140.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC6200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC6300.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/TMC7300.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/ic/tmc_ic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.270637 pytrinamic-0.2.9/pytrinamic/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/Landungsbruecke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCC160.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1021.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1140.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1141.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1160.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1161.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM123x_0_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1240.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1260.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1270.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1276.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1370.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1617.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1630.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1633.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1636.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1637.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1638.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1640.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM1670.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM2611.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM3110.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM3312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM3351.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM6110.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM6212.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM6214.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/TMCM_Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/canopen_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/tmc_eval_shield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/modules/tmcl_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.270637 pytrinamic-0.2.9/pytrinamic/referencedesigns/
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/referencedesigns/TMC4671_LEV_REF.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/referencedesigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/tmcl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.270637 pytrinamic-0.2.9/pytrinamic/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/tools/velocity_ramp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/pytrinamic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.274637 pytrinamic-0.2.9/pytrinamic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 07:18:35.000000 pytrinamic-0.2.9/pytrinamic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-29 07:18:35.000000 pytrinamic-0.2.9/pytrinamic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:18:35.000000 pytrinamic-0.2.9/pytrinamic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:18:35.000000 pytrinamic-0.2.9/pytrinamic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 07:18:35.000000 pytrinamic-0.2.9/pytrinamic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 07:18:35.000000 pytrinamic-0.2.9/pytrinamic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 07:18:35.274637 pytrinamic-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:18:35.274637 pytrinamic-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/tests/test_can_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-29 07:18:31.000000 pytrinamic-0.2.9/tests/test_interface_timeouts.py
```

### Comparing `pytrinamic-0.2.8/LICENSE` & `pytrinamic-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/MANIFEST.in` & `pytrinamic-0.2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/PKG-INFO` & `pytrinamic-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrinamic
-Version: 0.2.8
+Version: 0.2.9
 Summary: TRINAMIC's Python Technology Access Package.
 Home-page: https://github.com/trinamic/PyTrinamic
 Author: Trinamic Software Team
 Author-email: tmc_info@trinamic.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrinamic-0.2.8/README.md` & `pytrinamic-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/RAMDebug.py` & `pytrinamic-0.2.9/pytrinamic/RAMDebug.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         channel_type = RAMDebug_Channel.CHANNEL_SYSTICK
         value = 0
         return cls(channel_type, value)
 
     @classmethod
     def axis_parameter(cls, motor, parameter_nr, eval_channel=0):
         channel_type = RAMDebug_Channel.CHANNEL_AXIS_PARAMETER
-        value = ((motor << 24) & 0xFF00_0000) | ((eval_channel << 16) & 0x0001_0000) | (parameter_nr & 0x0000_00FF)
+        value = ((motor << 24) & 0xFF00_0000) | ((eval_channel << 16) & 0x0001_0000) | (parameter_nr & 0x0000_0FFF)
         # Error if value is bigger than 8 bits
         return cls(channel_type, value)
 
     @classmethod
     def register(cls, motor, address, signed=False, eval_channel=0):
         channel_type = RAMDebug_Channel.CHANNEL_REGISTER
         value = ((motor << 24) & 0xFF00_0000) | ((eval_channel << 16) & 0x0001_0000) | (address & 0x0000_FFFF)
@@ -133,15 +133,15 @@
 
         # Error if value is bigger than 8 bits
         return cls(channel_type, number)
 
     @classmethod
     def global_parameter(cls, bank, parameter_nr, eval_channel=0):
         channel_type = RAMDebug_Channel.CHANNEL_GLOBAL_PARAMETER
-        value = ((motor << 24) & 0xFF00_0000) | ((eval_channel << 16) & 0x0001_0000) | (parameter_nr & 0x0000_00FF)
+        value = ((bank << 24) & 0xFF00_0000) | ((eval_channel << 16) & 0x0001_0000) | (parameter_nr & 0x0000_00FF)
         # Error if value is bigger than 8 bits
         return cls(channel_type, value)
 
 
 class RAMDebug():
     def __init__(self, connection):
         self._connection = connection
```

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/__init__.py` & `pytrinamic-0.2.9/pytrinamic/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/can_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/can_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/connection_manager.py` & `pytrinamic-0.2.9/pytrinamic/connections/connection_manager.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/dummy_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/dummy_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/serial_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/serial_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/tmcl_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,16 @@
         reply = TMCLReply.from_buffer(self._recv(self._host_id, request.moduleAddress))
 
         self.logger.debug("Rx: %s", reply)
 
         self._reply_check(reply)
 
         # Status codes below 100 indicate an error response.
-        if reply.status < 100:
+        # Ignore status when reading TMCL memory. 
+        if reply.status < 100 and request.command != TMCLCommand.READ_TMCL_MEMORY:
             raise TMCLReplyStatusError(reply)
 
         return reply
 
     def send(self, opcode, op_type, motor, value, module_id=None):
         """
         Send a TMCL datagram and read back a reply. This function blocks until
@@ -221,17 +222,25 @@
     def write_mc(self, register_address, value, module_id=None):
         return self.write_register(register_address, TMCLCommand.WRITE_MC, 0, value, module_id)
 
     def read_mc(self, register_address, module_id=None, signed=False):
         return self.read_register(register_address, TMCLCommand.READ_MC, 0, module_id, signed)
 
     def write_mc_by_id(self, ic_id, register_address, value, module_id=None):
+        """
+        .. deprecated:: 0.2.8
+        """
+        warnings.warn("Function write_mc_by_id() is going te be removed in future versions of pytrinamic!", DeprecationWarning)
         return self.write_register(register_address, TMCLCommand.WRITE_MC, ic_id, value, module_id)
 
     def read_mc_by_id(self, ic_id, register_address, module_id=None, signed=False):
+        """
+        .. deprecated:: 0.2.8
+        """
+        warnings.warn("Function read_mc_by_id() is going te be removed in future versions of pytrinamic!", DeprecationWarning)
         return self.read_register(register_address, TMCLCommand.READ_MC, ic_id, module_id, signed)
 
     def write_drv(self, register_address, value, module_id=None):
         return self.write_register(register_address, TMCLCommand.WRITE_DRV, 1, value, module_id)
 
     def read_drv(self, register_address, module_id=None, signed=False):
         return self.read_register(register_address, TMCLCommand.READ_DRV, 1, module_id, signed)
```

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/uart_ic_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/uart_ic_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/connections/usb_tmcl_interface.py` & `pytrinamic-0.2.9/pytrinamic/connections/usb_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/MAX22216_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/MAX22216_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2100_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2100_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2130_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2130_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2160_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2160_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2208_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2208_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2209_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2209_eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             module_id:
                 Type: int, optional, default value: 1
                 The TMCL module ID of the TMC2209. This ID is used as a
                 parameter for the writeDRV and readDRV functions.
         """
         TMCLEval.__init__(self, connection, module_id)
         self.motors = [self._MotorTypeA(self, 0)]
-        self.ics = [TMC2209()]
+        self.ics = [TMC2209(self)]
 
     # Use the driver controller functions for register access
 
     def write_register(self, register_address, value):
         return self._connection.write_drv(register_address, value, self._module_id)
 
     def read_register(self, register_address, signed=False):
```

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2224_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2224_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2225_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2225_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2240_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2240_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2300_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2590_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2590_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC2660_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC2660_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC4361_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC4361_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC4671_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC4671_eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,22 +44,33 @@
 
 
         class AP:
             MaxVelocity                    = 4
             MaxAcceleration                = 11
             EnableRamp                     = 12
             RampVelocity                   = 13
+            LinearScaler                   = 20
+            LinearMaxVelocity              = 21
+            LinearMaxAcceleration          = 22
             LinearTargetPosition           = 25
             TargetTorque                   = 171
             PID_FLUX_TARGET                = 172
             PID_VELOCITY_TARGET            = 173
             TargetPosition                 = 174
             ActualTorque                   = 176
             ActualVelocity                 = 178
             ActualPosition                 = 179
             TargetTorqueRaw                = 189
             PIDIN_TARGET_FLUX              = 191
             TargetVelocity                 = 192
+
+            DebugMaxVelocity               = 240
+            DebugMaxAcceleration           = 241
+            DebugTargetVelocity            = 242
+            DebugRampVelocity              = 243
+            DebugTargetPosition            = 244
+            DebugRampPosition              = 245
+
             torqueMeasurementFactor        = 251
             StartEncoderInitialization     = 252
             EncoderInitState               = 253
             ActualEncoderWaitTime          = 254
```

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5031_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5031_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5041_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5041_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5062_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5062_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5072_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5072_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5130_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5130_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5160_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5160_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5160_shield.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5160_shield.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5240_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5240_eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 ################################################################################
-# Copyright © 2019 TRINAMIC Motion Control GmbH & Co. KG
-# (now owned by Analog Devices Inc.),
-#
 # Copyright © 2023 Analog Devices Inc. All Rights Reserved. This software is
 # proprietary & confidential to Analog Devices, Inc. and its licensors.
 ################################################################################
 
 from pytrinamic.evalboards import TMCLEval
 from pytrinamic.ic import TMC5240
 from pytrinamic.features import MotorControlModule
```

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC5272_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC5272_eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 ################################################################################
-# Copyright © 2019 TRINAMIC Motion Control GmbH & Co. KG
-# (now owned by Analog Devices Inc.),
-#
-# Copyright © 2023 Analog Devices Inc. All Rights Reserved. This software is
+# Copyright © 2024 Analog Devices Inc. All Rights Reserved. This software is
 # proprietary & confidential to Analog Devices, Inc. and its licensors.
 ################################################################################
 
 from pytrinamic.evalboards import TMCLEval
 from pytrinamic.ic import TMC5272
 from pytrinamic.features import MotorControlModule
 
@@ -32,24 +29,26 @@
                 for writing/reading to register of the TMC5272.
             module_id:
                 Type: int, optional, default value: 1
                 The TMCL module ID of the TMC5272. This ID is used as a
                 parameter for the writeDRV and readDRV functions.
         """
         TMCLEval.__init__(self, connection, module_id)
-        self.motors = [self._MotorTypeA(self, 0)]
-        self.ics = [TMC5272()]
+        self.motors = [self._MotorTypeA(self, 0),
+                       self._MotorTypeA(self, 1)]
+
+        self.ics = [TMC5272(self)]
 
     # Use the driver controller functions for register access
 
     def write_register(self, register_address, value):
-        return self._connection.write_drv(register_address, value, self._module_id)
+        return self._connection.write_mc(register_address, value, self._module_id)
 
     def read_register(self, register_address, signed=False):
-        return self._connection.read_drv(register_address, self._module_id, signed)
+        return self._connection.read_mc(register_address, self._module_id, signed)
 
     # Motion control functions
 
     def rotate(self, motor, value):
         self._connection.rotate(motor, value)
 
     def stop(self, motor):
```

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC6100_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC6100_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC6140_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC6140_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC6200_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC6200_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC6300_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC6300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/TMC7300_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/TMC7300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/__init__.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,7 +23,9 @@
 from .TMC5240_eval import TMC5240_eval
 from .TMC6100_eval import TMC6100_eval
 from .TMC6140_eval import TMC6140_eval
 from .TMC6200_eval import TMC6200_eval
 from .TMC6300_eval import TMC6300_eval
 from .TMC7300_eval import TMC7300_eval
 from .TMC5272_eval import TMC5272_eval
+from .TMC5271_eval import TMC5271_eval
+from .TMC5262_eval import TMC5262_eval
```

### Comparing `pytrinamic-0.2.8/pytrinamic/evalboards/tmcl_eval.py` & `pytrinamic-0.2.9/pytrinamic/evalboards/tmcl_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/abn_encoder.py` & `pytrinamic-0.2.9/pytrinamic/features/abn_encoder.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/abn_encoder_module.py` & `pytrinamic-0.2.9/pytrinamic/features/abn_encoder_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/absolute_encoder.py` & `pytrinamic-0.2.9/pytrinamic/features/absolute_encoder.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/absolute_encoder_module.py` & `pytrinamic-0.2.9/pytrinamic/features/absolute_encoder_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/coolstep.py` & `pytrinamic-0.2.9/pytrinamic/features/coolstep.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/coolstep_module.py` & `pytrinamic-0.2.9/pytrinamic/features/coolstep_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/current.py` & `pytrinamic-0.2.9/pytrinamic/features/current.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/current_ic.py` & `pytrinamic-0.2.9/pytrinamic/features/current_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/current_module.py` & `pytrinamic-0.2.9/pytrinamic/features/current_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/digital_hall.py` & `pytrinamic-0.2.9/pytrinamic/features/digital_hall.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/digital_hall_module.py` & `pytrinamic-0.2.9/pytrinamic/features/digital_hall_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/drive_setting.py` & `pytrinamic-0.2.9/pytrinamic/features/drive_setting.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/drive_setting_module.py` & `pytrinamic-0.2.9/pytrinamic/features/drive_setting_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/linear_ramp.py` & `pytrinamic-0.2.9/pytrinamic/features/linear_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/linear_ramp_ic.py` & `pytrinamic-0.2.9/pytrinamic/features/linear_ramp_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/linear_ramp_module.py` & `pytrinamic-0.2.9/pytrinamic/features/linear_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/motor_control.py` & `pytrinamic-0.2.9/pytrinamic/features/motor_control.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/motor_control_ic.py` & `pytrinamic-0.2.9/pytrinamic/features/motor_control_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/motor_control_module.py` & `pytrinamic-0.2.9/pytrinamic/features/motor_control_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/pid.py` & `pytrinamic-0.2.9/pytrinamic/features/pid.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/pid_module.py` & `pytrinamic-0.2.9/pytrinamic/features/pid_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/ramp_settings.py` & `pytrinamic-0.2.9/pytrinamic/features/ramp_settings.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/ramp_settings_module.py` & `pytrinamic-0.2.9/pytrinamic/features/ramp_settings_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/s_ramp.py` & `pytrinamic-0.2.9/pytrinamic/features/s_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/s_ramp_module.py` & `pytrinamic-0.2.9/pytrinamic/features/s_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/six_point_ramp.py` & `pytrinamic-0.2.9/pytrinamic/features/six_point_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/six_point_ramp_module.py` & `pytrinamic-0.2.9/pytrinamic/features/six_point_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/solenoid.py` & `pytrinamic-0.2.9/pytrinamic/features/solenoid.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/solenoid_control.py` & `pytrinamic-0.2.9/pytrinamic/features/solenoid_control.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/solenoid_control_ic.py` & `pytrinamic-0.2.9/pytrinamic/features/solenoid_control_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/solenoid_ic.py` & `pytrinamic-0.2.9/pytrinamic/features/solenoid_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/stallguard2.py` & `pytrinamic-0.2.9/pytrinamic/features/stallguard2.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/stallguard2_ic.py` & `pytrinamic-0.2.9/pytrinamic/features/stallguard2_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/features/stallguard2_module.py` & `pytrinamic-0.2.9/pytrinamic/features/stallguard2_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/helpers.py` & `pytrinamic-0.2.9/pytrinamic/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,25 @@
 
     @staticmethod
     def field_set(data, mask, shift, value):
         return (data & (~mask)) | ((value << shift) & mask)
 
 
 def to_signed_32(x):
+    """Convert any unsigned integer to a 32 bit signed integer."""
     m = x & 0xffffffff
     return (m ^ 0x80000000) - 0x80000000
 
 
+def to_signed_16(x):
+    """Convert any unsigned integer to a 16 bit signed integer."""
+    m = x & 0x0000ffff
+    return (m ^ 0x00008000) - 0x00008000
+
+
 class EEPROM:
     """
     This class provides basic access to an EEPROM.
 
     All accesses are in little-endian byte order. No alignment of addresses is
     required.
```

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/MAX22216.py` & `pytrinamic-0.2.9/pytrinamic/ic/MAX22216.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2100.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2100.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2130.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2130.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2160.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2208.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2208.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2209.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2209.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,33 @@
 # (now owned by Analog Devices Inc.),
 #
 # Copyright © 2023 Analog Devices Inc. All Rights Reserved. This software is
 # proprietary & confidential to Analog Devices, Inc. and its licensors.
 ################################################################################
 
 from ..ic.tmc_ic import TMCIc
+from ..features.motor_control_ic import MotorControlIc
 
 
 class TMC2209(TMCIc):
     """
     The TMC2209 is an ultra-silent motor driver IC for two phase stepper motors. TMC2209 pinning is compatible to a
     number of legacy drivers as well as to the TMC2208. Supply voltage is 4,75 - 29V.
     """
-    def __init__(self):
-        super().__init__("TMC2209", self.__doc__)
+    def __init__(self, parent_eval):
+        super().__init__(self.__class__.__name__, self.__doc__)
+        self._parent = parent_eval
+        self.motors = [self.MotorTypeA(parent_eval, self, 0)]
+
+    class MotorTypeA(MotorControlIc):
+        """
+        Motor class for the generic motor.
+        """
+        def __init__(self, parent_eval, ic, axis):
+            MotorControlIc.__init__(self, parent_eval, ic, axis)
 
     class REG:
         """
         Define all registers of the TMC2209.
         """
         GCONF        = 0x00
         GSTAT        = 0x01
```

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2224.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2224.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2225.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2225.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2240.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2240.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2300.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2300.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2590.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2590.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC2660.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC2660.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC4361.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC4361.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC4671.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC4671.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC5031.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC5031.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC5041.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC5041.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC5062.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC5062.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC5072.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC5072.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC5130.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC5130.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC5160.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC5160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC5240.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC5240.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 ################################################################################
-# Copyright © 2019 TRINAMIC Motion Control GmbH & Co. KG
-# (now owned by Analog Devices Inc.),
-#
 # Copyright © 2023 Analog Devices Inc. All Rights Reserved. This software is
 # proprietary & confidential to Analog Devices, Inc. and its licensors.
 ################################################################################
 
 from ..ic.tmc_ic import TMCIc
 from ..features.motor_control_ic import MotorControlIc
```

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC6100.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC6100.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC6140.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC6140.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC6200.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC6200.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC6300.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC6300.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/TMC7300.py` & `pytrinamic-0.2.9/pytrinamic/ic/TMC7300.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/__init__.py` & `pytrinamic-0.2.9/pytrinamic/ic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 from .TMC5240 import TMC5240
 from .TMC6100 import TMC6100
 from .TMC6140 import TMC6140
 from .TMC6200 import TMC6200
 from .TMC6300 import TMC6300
 from .TMC7300 import TMC7300
 from .TMC5272 import TMC5272
+from .TMC5271 import TMC5271
+from .TMC5262 import TMC5262
+
```

### Comparing `pytrinamic-0.2.8/pytrinamic/ic/tmc_ic.py` & `pytrinamic-0.2.9/pytrinamic/ic/tmc_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/Landungsbruecke.py` & `pytrinamic-0.2.9/pytrinamic/modules/Landungsbruecke.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCC160.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCC160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1021.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1021.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1111.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1111.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1140.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1140.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1141.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1141.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1160.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1161.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1161.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM123x_0_1.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM123x_0_1.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1240.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1240.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1260.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1260.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1270.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1270.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1276.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1276.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1370.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1370.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1617.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1617.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ################################################################################
 
 from ..modules import TMCLModule
 from ..ic import TMC4671, TMC6200
 from ..features import MotorControlModule, DriveSettingModule, LinearRampModule
 from ..features import ABNEncoderModule, DigitalHallModule, PIDModule
 from ..helpers import BitField
+from ..tmcl import TMCLCommand
 
 
 class TMCM1617(TMCLModule):
     """
     The TMCM-1617 is a single axis servo drive platform for 3-phase BLDC motors and DC motors.
         * Supply Voltage: 8 - 28V
     """
@@ -39,18 +40,18 @@
 
     def move_by(self, axis, difference, velocity=None):
         if velocity:
             self.motors[axis].linear_ramp.max_velocity = velocity
         self.connection.move_by(axis, difference, self.module_id)
 
     def write_register(self, ic_id, register_address, value):
-        return self.connection.write_mc_by_id(ic_id, register_address, value, self.module_id)
+        return self.connection.write_register(register_address, TMCLCommand.WRITE_MC, ic_id, value, self.module_id)
 
     def read_register(self, ic_id, register_address, signed=False):
-        return self.connection.read_mc_by_id(ic_id, register_address, self.module_id, signed)
+        return self.connection.read_register(register_address, TMCLCommand.READ_MC, ic_id, self.module_id, signed)
 
     def write_register_field(self, ic_id, field, value):
         return self.write_register(ic_id, field[0], BitField.field_set(self.read_register(ic_id, field[0]),
                                                                        field[1], field[2], value))
 
     def read_register_field(self, ic_id, field):
         return BitField.field_get(self.read_register(ic_id, field[0]), field[1], field[2])
```

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1630.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1630.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1633.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1633.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1636.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1636.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1637.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1637.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1638.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1638.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1640.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1640.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM1670.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM1670.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM3110.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM3110.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM3312.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM3312.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM3351.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM3351.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM6110.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM6110.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,7 +186,8 @@
         IN1    = 1
         IN2    = 2
         IN3    = 3
         AIN4   = 4
         IN5    = 5
         IN6    = 6
         IN7    = 7
+        VIN    = 8
```

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM6212.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM6212.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM6214.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM6214.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/TMCM_Python.py` & `pytrinamic-0.2.9/pytrinamic/modules/TMCM_Python.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/__init__.py` & `pytrinamic-0.2.9/pytrinamic/modules/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .TMCM1141 import TMCM1141
 from .TMCM1160 import TMCM1160
 from .TMCM1161 import TMCM1161
 from .TMCM1240 import TMCM1240
 from .TMCM1260 import TMCM1260
 from .TMCM1270 import TMCM1270
 from .TMCM1276 import TMCM1276
+from .TMCM1311 import TMCM1311
 from .TMCM1370 import TMCM1370
 from .TMCM1617 import TMCM1617
 from .TMCM1630 import TMCM1630
 from .TMCM1633 import TMCM1633
 from .TMCM1636 import TMCM1636
 from .TMCM1637 import TMCM1637
 from .TMCM1638 import TMCM1638
@@ -22,7 +23,8 @@
 from .TMCM3110 import TMCM3110
 from .TMCM3312 import TMCM3312
 from .TMCM3351 import TMCM3351
 from .TMCM6110 import TMCM6110
 from .TMCM6212 import TMCM6212
 from .TMCM6214 import TMCM6214
 from .TMCM123x_0_1 import TMCM123x_0_1
+from .TMCM2611 import TMCM2611
```

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/canopen_node.py` & `pytrinamic-0.2.9/pytrinamic/modules/canopen_node.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/tmc_eval_shield.py` & `pytrinamic-0.2.9/pytrinamic/modules/tmc_eval_shield.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/modules/tmcl_module.py` & `pytrinamic-0.2.9/pytrinamic/modules/tmcl_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/referencedesigns/TMC4671_LEV_REF.py` & `pytrinamic-0.2.9/pytrinamic/referencedesigns/TMC4671_LEV_REF.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic/tmcl.py` & `pytrinamic-0.2.9/pytrinamic/tmcl.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,80 +32,103 @@
         for d in data:
             checksum += d
         checksum &= 0xFF
         return checksum
 
 
 class TMCLCommand:
-    ROR                         = 1
-    ROL                         = 2
-    MST                         = 3
+
+    ROR                        = 1
+    ROL                        = 2
+    MST                        = 3
     MVP                         = 4
-    SAP                         = 5
-    GAP                         = 6
-    STAP                        = 7
-    RSAP                        = 8
-    SGP                         = 9
-    GGP                         = 10
-    STGP                        = 11
-    RSGP                        = 12
+    SAP                        = 5
+    GAP                        = 6
+    STAP                       = 7
+    RSAP                       = 8
+    SGP                        = 9
+    GGP                        = 10
+    STGP                       = 11
+    RSGP                       = 12
     RFS                         = 13
-    SIO                         = 14
-    GIO                         = 15
-    CALC                        = 19
-    COMP                        = 20
-    JC                          = 21
-    JA                          = 22
-    CSUB                        = 23
-    RSUB                        = 24
-    WAIT                        = 27
-    STOP                        = 28
-    SAC                         = 29
-    SCO                         = 30
-    GCO                         = 31
-    CCO                         = 32
-    CALCX                       = 33
-    AAP                         = 34
-    AGP                         = 35
-    CLE                         = 36
-    TMCL_UF0                    = 64
-    TMCL_UF1                    = 65
-    TMCL_UF2                    = 66
-    TMCL_UF3                    = 67
-    TMCL_UF4                    = 68
-    TMCL_UF5                    = 69
-    TMCL_UF6                    = 70
-    TMCL_UF7                    = 71
-    STOP_APPLICATION            = 128
-    RUN_APPLICATION             = 129
-    STEP_APPLICATION            = 130
-    RESET_APPLICATION           = 131
-    START_DOWNLOAD_MODE         = 132
-    QUIT_DOWNLOAD_MODE          = 133
-    READ_TMCL_MEMORY            = 134
-    GET_APPLICATION_STATUS      = 135
-    GET_FIRMWARE_VERSION        = 136
-    RESTORE_FACTORY_SETTINGS    = 137
-    TARGET_POSITION_REACHED     = 138
-    RAMDEBUG                    = 142
-    ASSIGNMENT                  = 143
-    WRITE_MC                    = 146
-    WRITE_DRV                   = 147
-    READ_MC                     = 148
-    READ_DRV                    = 149
-
-    BOOT_ERASE_ALL              = 200
-    BOOT_WRITE_BUFFER           = 201
-    BOOT_WRITE_PAGE             = 202
-    BOOT_GET_CHECKSUM           = 203
-    BOOT_READ_MEMORY            = 204
-    BOOT_START_APPL             = 205
-    BOOT_GET_INFO               = 206
-    BOOT_WRITE_LENGTH           = 208
-    BOOT                        = 242
+    SIO                        = 14
+    GIO                        = 15
+    CALC                       = 19
+    COMP                       = 20
+    JC                         = 21
+    JA                         = 22
+    CSUB                       = 23
+    RSUB                       = 24
+    EI                         = 25
+    DI                         = 26
+    WAIT                       = 27
+    STOP                       = 28
+    SAC                        = 29
+    SCO                        = 30
+    GCO                        = 31
+    CCO                        = 32
+    CALCX                      = 33
+    AAP                        = 34
+    AGP                        = 35
+    CLE                        = 36
+    VECT                       = 37
+    RETI                       = 38
+    ACO                        = 39
+    CALCVV                     = 40
+    CALCVA                     = 41
+    CALCAV                     = 42
+    CALCVX                     = 43
+    CALCXV                     = 44
+    CALCV                      = 45
+    MVPA                       = 46
+    RST                        = 48
+    DJNZ                       = 49
+    ROLA                       = 50
+    RORA                       = 51
+    SIV                        = 55
+    GIV                        = 56
+    AIV                        = 57
+    TMCL_UF0                   = 64
+    TMCL_UF1                   = 65
+    TMCL_UF2                   = 66
+    TMCL_UF3                   = 67
+    TMCL_UF4                   = 68
+    TMCL_UF5                   = 69
+    TMCL_UF6                   = 70
+    TMCL_UF7                   = 71
+    CALL                       = 80
+
+    STOP_APPLICATION           = 128
+    RUN_APPLICATION            = 129
+    STEP_APPLICATION           = 130
+    RESET_APPLICATION          = 131
+    START_DOWNLOAD_MODE        = 132
+    QUIT_DOWNLOAD_MODE         = 133
+    READ_TMCL_MEMORY           = 134
+    GET_APPLICATION_STATUS     = 135
+    GET_FIRMWARE_VERSION       = 136
+    RESTORE_FACTORY_SETTINGS   = 137
+    TARGET_POSITION_REACHED    = 138
+    RAMDEBUG                   = 142
+    ASSIGNMENT                 = 143
+    WRITE_MC                   = 146
+    WRITE_DRV                  = 147
+    READ_MC                    = 148
+    READ_DRV                   = 149
+    GET_INFO                   = 157
+
+    BOOT_ERASE_ALL             = 200
+    BOOT_WRITE_BUFFER          = 201
+    BOOT_WRITE_PAGE            = 202
+    BOOT_GET_CHECKSUM          = 203
+    BOOT_READ_MEMORY           = 204
+    BOOT_START_APPL            = 205
+    BOOT_GET_INFO              = 206
+    BOOT_WRITE_LENGTH          = 208
+    BOOT                       = 242
 
 
 class TMCLStatus:
     SUCCESS               = 100
     COMMAND_LOADED        = 101
     WRONG_CHECKSUM        = 1
     INVALID_COMMAND       = 2
```

### Comparing `pytrinamic-0.2.8/pytrinamic/tools/velocity_ramp_runner.py` & `pytrinamic-0.2.9/pytrinamic/tools/velocity_ramp_runner.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/pytrinamic.egg-info/PKG-INFO` & `pytrinamic-0.2.9/pytrinamic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrinamic
-Version: 0.2.8
+Version: 0.2.9
 Summary: TRINAMIC's Python Technology Access Package.
 Home-page: https://github.com/trinamic/PyTrinamic
 Author: Trinamic Software Team
 Author-email: tmc_info@trinamic.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrinamic-0.2.8/pytrinamic.egg-info/SOURCES.txt` & `pytrinamic-0.2.9/pytrinamic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 pytrinamic/evalboards/TMC5041_eval.py
 pytrinamic/evalboards/TMC5062_eval.py
 pytrinamic/evalboards/TMC5072_eval.py
 pytrinamic/evalboards/TMC5130_eval.py
 pytrinamic/evalboards/TMC5160_eval.py
 pytrinamic/evalboards/TMC5160_shield.py
 pytrinamic/evalboards/TMC5240_eval.py
+pytrinamic/evalboards/TMC5262_eval.py
+pytrinamic/evalboards/TMC5271_eval.py
 pytrinamic/evalboards/TMC5272_eval.py
 pytrinamic/evalboards/TMC6100_eval.py
 pytrinamic/evalboards/TMC6140_eval.py
 pytrinamic/evalboards/TMC6200_eval.py
 pytrinamic/evalboards/TMC6300_eval.py
 pytrinamic/evalboards/TMC7300_eval.py
 pytrinamic/evalboards/__init__.py
@@ -110,14 +112,16 @@
 pytrinamic/ic/TMC5031.py
 pytrinamic/ic/TMC5041.py
 pytrinamic/ic/TMC5062.py
 pytrinamic/ic/TMC5072.py
 pytrinamic/ic/TMC5130.py
 pytrinamic/ic/TMC5160.py
 pytrinamic/ic/TMC5240.py
+pytrinamic/ic/TMC5262.py
+pytrinamic/ic/TMC5271.py
 pytrinamic/ic/TMC5272.py
 pytrinamic/ic/TMC6100.py
 pytrinamic/ic/TMC6140.py
 pytrinamic/ic/TMC6200.py
 pytrinamic/ic/TMC6300.py
 pytrinamic/ic/TMC7300.py
 pytrinamic/ic/__init__.py
@@ -131,23 +135,25 @@
 pytrinamic/modules/TMCM1160.py
 pytrinamic/modules/TMCM1161.py
 pytrinamic/modules/TMCM123x_0_1.py
 pytrinamic/modules/TMCM1240.py
 pytrinamic/modules/TMCM1260.py
 pytrinamic/modules/TMCM1270.py
 pytrinamic/modules/TMCM1276.py
+pytrinamic/modules/TMCM1311.py
 pytrinamic/modules/TMCM1370.py
 pytrinamic/modules/TMCM1617.py
 pytrinamic/modules/TMCM1630.py
 pytrinamic/modules/TMCM1633.py
 pytrinamic/modules/TMCM1636.py
 pytrinamic/modules/TMCM1637.py
 pytrinamic/modules/TMCM1638.py
 pytrinamic/modules/TMCM1640.py
 pytrinamic/modules/TMCM1670.py
+pytrinamic/modules/TMCM2611.py
 pytrinamic/modules/TMCM3110.py
 pytrinamic/modules/TMCM3312.py
 pytrinamic/modules/TMCM3351.py
 pytrinamic/modules/TMCM6110.py
 pytrinamic/modules/TMCM6212.py
 pytrinamic/modules/TMCM6214.py
 pytrinamic/modules/TMCM_Python.py
```

### Comparing `pytrinamic-0.2.8/setup.py` & `pytrinamic-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/tests/test_can_adapters.py` & `pytrinamic-0.2.9/tests/test_can_adapters.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.8/tests/test_interface_timeouts.py` & `pytrinamic-0.2.9/tests/test_interface_timeouts.py`

 * *Files identical despite different names*

