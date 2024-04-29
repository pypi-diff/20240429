# Comparing `tmp/uav_collision_avoidance-0.6.4-py3-none-any.whl.zip` & `tmp/uav_collision_avoidance-0.6.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,128 +1,178 @@
-Zip file size: 176631 bytes, number of entries: 126
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+Zip file size: 236136 bytes, number of entries: 176
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
+-rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
+-rw-r--r--  2.0 unx     9540 b- defN 24-Apr-11 18:19 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+-rw-r--r--  2.0 unx     8671 b- defN 24-Apr-16 07:07 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     6057 b- defN 24-Apr-11 11:29 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
+-rw-r--r--  2.0 unx     7112 b- defN 24-Apr-11 19:12 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
+-rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
+-rw-r--r--  2.0 unx     6110 b- defN 24-Apr-11 12:04 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    23164 b- defN 24-Apr-11 12:26 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
+-rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
+-rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+-rw-r--r--  2.0 unx     9028 b- defN 24-Apr-20 15:08 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     7108 b- defN 24-Apr-22 12:03 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
+-rw-r--r--  2.0 unx     6613 b- defN 24-Apr-21 14:26 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
+-rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
+-rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx     9540 b- defN 24-Apr-11 18:19 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     8671 b- defN 24-Apr-16 07:07 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
--rw-r--r--  2.0 unx     6057 b- defN 24-Apr-11 11:29 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     9028 b- defN 24-Apr-20 15:08 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     7108 b- defN 24-Apr-22 12:03 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     7112 b- defN 24-Apr-11 19:12 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     6613 b- defN 24-Apr-21 14:26 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
--rw-r--r--  2.0 unx     6110 b- defN 24-Apr-11 12:04 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
--rw-r--r--  2.0 unx    23164 b- defN 24-Apr-11 12:26 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
 -rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
 -rw-r--r--  2.0 unx     9028 b- defN 24-Apr-20 15:08 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
 -rw-r--r--  2.0 unx     7108 b- defN 24-Apr-22 12:03 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
 -rw-r--r--  2.0 unx     6613 b- defN 24-Apr-21 14:26 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
 -rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 -rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
 -rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
 -rw-r--r--  2.0 unx     9028 b- defN 24-Apr-20 15:08 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
 -rw-r--r--  2.0 unx     7108 b- defN 24-Apr-22 12:03 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
 -rw-r--r--  2.0 unx     6613 b- defN 24-Apr-21 14:26 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
 -rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 -rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    13017 b- defN 24-Apr-24 17:23 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     9028 b- defN 24-Apr-20 15:08 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
--rw-r--r--  2.0 unx     7108 b- defN 24-Apr-22 12:03 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     9630 b- defN 24-Apr-24 17:35 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     7072 b- defN 24-Apr-24 14:39 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     6613 b- defN 24-Apr-21 14:26 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     6613 b- defN 24-Apr-24 14:18 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
--rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
--rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx     6290 b- defN 24-Apr-24 14:18 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    25822 b- defN 24-Apr-24 16:52 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/build/lib/build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx    11332 b- defN 24-Apr-22 13:54 build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    14940 b- defN 24-Apr-25 10:35 build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     9028 b- defN 24-Apr-20 15:08 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
--rw-r--r--  2.0 unx     7108 b- defN 24-Apr-22 12:03 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     9632 b- defN 24-Apr-25 10:25 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     8427 b- defN 24-Apr-24 20:23 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     6613 b- defN 24-Apr-21 14:26 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     8170 b- defN 24-Apr-25 10:23 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
--rw-r--r--  2.0 unx     6290 b- defN 24-Apr-20 15:07 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
--rw-r--r--  2.0 unx    23168 b- defN 24-Apr-18 21:19 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx     6343 b- defN 24-Apr-25 10:24 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    26085 b- defN 24-Apr-25 10:19 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/build/lib/uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx    13017 b- defN 24-Apr-24 17:23 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    15437 b- defN 24-Apr-25 10:59 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     9630 b- defN 24-Apr-24 17:35 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
--rw-r--r--  2.0 unx     7072 b- defN 24-Apr-24 14:39 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     9632 b- defN 24-Apr-25 11:01 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     8427 b- defN 24-Apr-24 20:23 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     6613 b- defN 24-Apr-24 14:18 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     8359 b- defN 24-Apr-25 10:56 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
--rw-r--r--  2.0 unx     6290 b- defN 24-Apr-24 14:18 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
--rw-r--r--  2.0 unx    25822 b- defN 24-Apr-24 16:52 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 build/lib/tests/test_sample.py
+-rw-r--r--  2.0 unx     6343 b- defN 24-Apr-25 10:24 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    26085 b- defN 24-Apr-25 10:19 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 build/lib/tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 build/lib/tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 build/lib/tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 build/lib/uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 build/lib/uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 build/lib/uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 build/lib/uav_collision_avoidance/version.py
 -rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx    14940 b- defN 24-Apr-25 10:35 build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx    15437 b- defN 24-Apr-25 10:59 build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
 -rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     9632 b- defN 24-Apr-25 10:25 build/lib/uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     9632 b- defN 24-Apr-25 11:01 build/lib/uav_collision_avoidance/src/simulation/simulation.py
 -rw-r--r--  2.0 unx     8427 b- defN 24-Apr-24 20:23 build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
 -rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     8170 b- defN 24-Apr-25 10:23 build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     8359 b- defN 24-Apr-25 10:56 build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
 -rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
 -rw-r--r--  2.0 unx     6343 b- defN 24-Apr-25 10:24 build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 -rw-r--r--  2.0 unx    26085 b- defN 24-Apr-25 10:19 build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 tests/test_sample.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-29 09:20 tests/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 10:09 tests/test_headless.py
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-26 09:45 tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 10:59 uav_collision_avoidance/main.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-22 14:13 uav_collision_avoidance/version.py
--rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 uav_collision_avoidance/src/aircraft/aircraft.py
--rw-r--r--  2.0 unx    15437 b- defN 24-Apr-25 10:59 uav_collision_avoidance/src/aircraft/aircraft_fcc.py
--rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
--rw-r--r--  2.0 unx     9632 b- defN 24-Apr-25 11:01 uav_collision_avoidance/src/simulation/simulation.py
--rw-r--r--  2.0 unx     8427 b- defN 24-Apr-24 20:23 uav_collision_avoidance/src/simulation/simulation_adsb.py
--rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 uav_collision_avoidance/src/simulation/simulation_fps.py
--rw-r--r--  2.0 unx     8359 b- defN 24-Apr-25 10:56 uav_collision_avoidance/src/simulation/simulation_physics.py
--rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 uav_collision_avoidance/src/simulation/simulation_render.py
+-rw-r--r--  2.0 unx     2581 b- defN 24-Apr-29 10:36 uav_collision_avoidance/src/aircraft/aircraft.py
+-rw-r--r--  2.0 unx    21654 b- defN 24-Apr-29 10:37 uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx     7090 b- defN 24-Apr-29 10:38 uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+-rw-r--r--  2.0 unx    11968 b- defN 24-Apr-29 10:51 uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx    11341 b- defN 24-Apr-29 10:34 uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-Apr-28 18:07 uav_collision_avoidance/src/simulation/simulation_fps.py
+-rw-r--r--  2.0 unx     9854 b- defN 24-Apr-29 10:27 uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-Apr-28 19:23 uav_collision_avoidance/src/simulation/simulation_render.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 uav_collision_avoidance/src/simulation/simulation_settings.py
--rw-r--r--  2.0 unx     6343 b- defN 24-Apr-25 10:24 uav_collision_avoidance/src/simulation/simulation_state.py
--rw-r--r--  2.0 unx    26085 b- defN 24-Apr-25 10:19 uav_collision_avoidance/src/simulation/simulation_widget.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     7374 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       58 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    17504 b- defN 24-Apr-25 11:08 uav_collision_avoidance-0.6.4.dist-info/RECORD
-126 files, 655134 bytes uncompressed, 146235 bytes compressed:  77.7%
+-rw-r--r--  2.0 unx    16393 b- defN 24-Apr-29 08:53 uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    29872 b- defN 24-Apr-29 07:47 uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-29 11:03 uav_collision_avoidance-0.6.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7677 b- defN 24-Apr-29 11:03 uav_collision_avoidance-0.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 11:03 uav_collision_avoidance-0.6.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 24-Apr-29 11:03 uav_collision_avoidance-0.6.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       58 b- defN 24-Apr-29 11:03 uav_collision_avoidance-0.6.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    25639 b- defN 24-Apr-29 11:03 uav_collision_avoidance-0.6.6.dist-info/RECORD
+176 files, 875960 bytes uncompressed, 191308 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,7 +1,115 @@
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+Comment: 
+
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
@@ -39,14 +147,20 @@
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+Comment: 
+
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
@@ -84,14 +198,20 @@
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+Comment: 
+
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
@@ -129,14 +249,20 @@
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
+Filename: build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/build/lib/tests/test_headless.py
+Comment: 
+
 Filename: build/lib/build/lib/build/lib/build/lib/tests/test_sample.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
@@ -174,14 +300,20 @@
 
 Filename: build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
+Filename: build/lib/build/lib/build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/tests/test_headless.py
+Comment: 
+
 Filename: build/lib/build/lib/build/lib/tests/test_sample.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/uav_collision_avoidance/main.py
@@ -219,14 +351,20 @@
 
 Filename: build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
+Filename: build/lib/build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/tests/test_headless.py
+Comment: 
+
 Filename: build/lib/build/lib/tests/test_sample.py
 Comment: 
 
 Filename: build/lib/build/lib/uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: build/lib/build/lib/uav_collision_avoidance/main.py
@@ -264,14 +402,20 @@
 
 Filename: build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
+Filename: build/lib/tests/__init__.py
+Comment: 
+
+Filename: build/lib/tests/test_headless.py
+Comment: 
+
 Filename: build/lib/tests/test_sample.py
 Comment: 
 
 Filename: build/lib/uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: build/lib/uav_collision_avoidance/main.py
@@ -309,14 +453,20 @@
 
 Filename: build/lib/uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/test_headless.py
+Comment: 
+
 Filename: tests/test_sample.py
 Comment: 
 
 Filename: uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: uav_collision_avoidance/main.py
@@ -354,26 +504,26 @@
 
 Filename: uav_collision_avoidance/src/simulation/simulation_state.py
 Comment: 
 
 Filename: uav_collision_avoidance/src/simulation/simulation_widget.py
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.4.dist-info/LICENSE
+Filename: uav_collision_avoidance-0.6.6.dist-info/LICENSE
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.4.dist-info/METADATA
+Filename: uav_collision_avoidance-0.6.6.dist-info/METADATA
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.4.dist-info/WHEEL
+Filename: uav_collision_avoidance-0.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.4.dist-info/entry_points.txt
+Filename: uav_collision_avoidance-0.6.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.4.dist-info/top_level.txt
+Filename: uav_collision_avoidance-0.6.6.dist-info/top_level.txt
 Comment: 
 
-Filename: uav_collision_avoidance-0.6.4.dist-info/RECORD
+Filename: uav_collision_avoidance-0.6.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py

```diff
@@ -1,20 +1,28 @@
 """Main module for UAV Collision Avoidance application"""
 
 import logging
 import platform
 import datetime
 import signal
 from pathlib import Path
+from screeninfo import get_monitors
 
 from PySide6.QtWidgets import QApplication
 from .version import __version__ as version
 from .src.simulation.simulation import Simulation, SimulationSettings
 
-signal.signal(signal.SIGINT, signal.SIG_DFL)
+def signal_handler(sig, frame):
+    logging.warning("Ctrl+C keyboard interrupt. Exiting...")
+    try:
+        signal.default_int_handler(sig, frame)
+    except KeyboardInterrupt:
+        import sys
+        sys.exit(1)
+signal.signal(signal.SIGINT, signal_handler)
 try:
     start_time = datetime.datetime.now().strftime("%Y-%m-%d")
     Path("logs").mkdir(parents=True, exist_ok=True)
     logging.basicConfig(
         filename=f"logs/simulation-{start_time}.log",
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s")
@@ -27,45 +35,45 @@
 logging.info("-" * 120)
 if platform.system() == "Windows":
     import ctypes
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(
         f"io.github.mldxo.uav-collision-avoidance.{version}")
 logging.info("Detected platform: %s", platform.system())
 
-def main():
+def main(arg = None):
     """Executes main function"""
     import sys
     args = sys.argv[1:]
-    realtime : bool = True
-    run_tests : bool = False
-    if len(args) > 0:
+    app = QApplication(args)
+    app.setApplicationName("UAV Collsion Avoidance")
+    app.setApplicationVersion(version)
+    SimulationSettings.screen_resolution = app.primaryScreen().size()
+    logging.info("%s %s", app.applicationName(), app.applicationVersion())
+    sim : Simulation | None = None
+    if len(args) > 0 or arg is not None:
         if args[0] == "realtime":
-            realtime = True
-        elif args[0] == "prerender":
-            realtime = False
-        elif args[0] == "tests":
-            run_tests = True
+            if len(get_monitors) == 0:
+                logging.warning("Launching GUI Application without monitors detected")
+            sim = Simulation()
+            sys.exit(app.exec())
+        elif args[0] == "headless" or arg == "headless":
+            sim = Simulation(headless = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
+        elif args[0] == "tests" or arg == "tests":
+            sim = Simulation(headless = True, tests = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
         elif len(args) > 1:
+            print(f"Invalid arguments: {args}")
             logging.error("Invalid arguments: %s", args)
             sys.exit(1)
         else:
+            print(f"Invalid argument: {args[0]}")
             logging.error("Invalid argument: %s", args[0])
             sys.exit(1)
-    app = QApplication(args)
-    app.setApplicationName("UAV Collsion Avoidance")
-    app.setApplicationVersion(version)
-    SimulationSettings.screen_resolution = app.primaryScreen().size()
-    logging.info("%s %s", app.applicationName(), app.applicationVersion())
-    sim = Simulation()
-    if run_tests:
-        realtime = False
-        sim.run_tests(20)
-        sys.exit()
-    elif realtime:
-        sim.run_realtime()
-        sys.exit(app.exec())
     else:
-        sim.run_prerender()
-        sys.exit()
+        sim = Simulation()
+    sys.exit(app.exec())
 
 if __name__ == "__main__":
     main()
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -27,14 +27,16 @@
             self.target_yaw_angle : float = self.find_best_yaw_angle(aircraft.position, initial_target)
             self.add_first_destination(initial_target)
 
         self.initial_course : float = copy(self.target_yaw_angle)
         self.target_roll_angle : float = 0.0
         self.target_pitch_angle : float = 0.0
         self.__target_speed : float = self.aircraft.absolute_speed
+        self.__is_turning_right : bool = False
+        self.__is_turning_left : bool = False
 
         self.__evade_maneuver : bool = False
         self.vector_sharing_resolution : QVector3D | None = None
 
         self.destinations_history : List[QVector3D] = []
         self.visited : List[QVector3D] = []
     
@@ -44,37 +46,63 @@
         return self.__target_speed
     
     @target_speed.setter
     def target_speed(self, speed : float) -> None:
         """Sets target speed"""
         if speed > 0:
             self.__target_speed = speed
+    
+    @property
+    def is_turning_right(self) -> bool:
+        """Returns turning right state"""
+        return self.__is_turning_right
+    
+    @is_turning_right.setter
+    def is_turning_right(self, value : bool) -> None:
+        """Sets turning right state"""
+        self.__is_turning_right = value
+
+    @property
+    def is_turning_left(self) -> bool:
+        """Returns turning left state"""
+        return self.__is_turning_left
+    
+    @is_turning_left.setter
+    def is_turning_left(self, value : bool) -> None:
+        """Sets turning left state"""
+        self.__is_turning_left = value
 
     def add_last_destination(self, destination : QVector3D) -> None:
-        """Appends given location to the end of destinations list"""
-        assert isinstance(destination.x(), (int, float))
-        assert isinstance(destination.y(), (int, float))
-        assert isinstance(destination.z(), (int, float))
+        """Appends the given location (QVector3D) to the end of the destinations list."""
+        if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
+            raise TypeError("Destination coordinates must be int or float.")
 
         self.destinations.append(destination)
 
     def add_first_destination(self, destination : QVector3D) -> None:
         """Pushes given location to the top of destinations list"""
-        assert isinstance(destination.x(), (int, float))
-        assert isinstance(destination.y(), (int, float))
-        assert isinstance(destination.z(), (int, float))
+        if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
+            raise TypeError("Destination coordinates must be int or float.")
 
-        if len(self.destinations) > 0 and dist(destination.toTuple(), self.destinations[0].toTuple()) < 1:
+        if len(self.destinations) > 0 and dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
             print("Attempted to stack same destination")
-            logging.warning("Attempted to stack same destination")
+            logging.warning(f"Attempted to stack same destination: {destination}")
             return
 
         self.destinations.appendleft(destination)
         logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
+    @property
+    def destination(self) -> QVector3D | None:
+        """Returns current destination"""
+        if len(self.destinations) > 0:
+            return self.destinations[0]
+        else:
+            return None
+
     def append_visited(self) -> None:
         """Appends current location to visited list"""
         self.visited.append(copy(self.aircraft.position))
 
     def normalize_angle(self, angle : float) -> float:
         """Normalizes -180-180 angle into 360 domain"""
         angle = angle % 360
@@ -121,19 +149,46 @@
     def reset_evade_maneuver(self) -> None:
         """Resets evade maneuver"""
         if self.__evade_maneuver:
             logging.info("Aircraft %s reset evade maneuver", self.aircraft.aircraft_id)
             self.__evade_maneuver = False
             #self.vector_sharing_resolution = None
 
-    def find_best_roll_angle(self, current_yaw_angle : float, target_yaw_angle : float) -> float:
+    def find_best_roll_angle(self, current_yaw_angle: float, target_yaw_angle: float) -> float:
         """Finds best roll angle for the targeted yaw angle"""
         difference = (target_yaw_angle - current_yaw_angle + 180) % 360 - 180
-        return 0.0 if abs(difference) < 0.01 else 30.0 if difference > 0 else -30.0
-
+        if abs(difference) < 0.001:
+            self.is_turning_right = False
+            self.is_turning_left = False
+            return 0.0
+        elif difference > 0:
+            self.is_turning_right = True
+            self.is_turning_left = False
+            if difference > 90:
+                return 30.0
+            elif difference > 45:
+                return 20.0
+            elif difference > 20:
+                return 10.0
+            else:
+                return 5.0
+        elif difference < 0:
+            self.is_turning_left = True
+            self.is_turning_right = False
+            if difference < -90:
+                return -30.0
+            elif difference < -45:
+                return -20.0
+            elif difference < -20:
+                return -10.0
+            else:
+                return -5.0
+        else:
+            return 0.0
+        
     def find_best_yaw_angle(self, position : QVector3D, destination : QVector3D) -> float:
         """Finds best yaw angle for the given destination"""
         target_yaw_angle : float  = degrees(atan2(
             destination.y() - position.y(),
             destination.x() - position.x()))
         target_yaw_angle += 90
         return self.format_angle(target_yaw_angle)
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py

```diff
@@ -23,38 +23,46 @@
 class Simulation(QMainWindow):
     """Main simulation App"""
 
     def __init__(self, aircrafts : List[Aircraft] | None = None, simulation_time : int = 100_000) -> None:
         super().__init__()
         SimulationSettings().__init__()
         if aircrafts is None:
-            self.aircrafts : List[Aircraft] = [
-                Aircraft( # detection test
-                    position = QVector3D(100, 1000, 1000),
-                    speed = QVector3D(50, -50, 0),
-                    initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
-                Aircraft(
-                    position = QVector3D(900, 1300, 1000),
-                    speed = QVector3D(0, -70, 0),
-                    initial_target = QVector3D(900, -1_001_300, 1000)),
-                # Aircraft( # head on
-                #     position = QVector3D(100, 500, 1000),
-                #     speed = QVector3D(70, 0, 0)),
-                # Aircraft(
-                #     position = QVector3D(900, 500, 1000),
-                #     speed = QVector3D(-50, 0, 0)),
-                # Aircraft( # avoidance test
-                #     position = QVector3D(10, -10, 0),
-                #     speed = QVector3D(300, -300, 0),
-                #     initial_target = QVector3D(75000, -75000, 0)), # 75 km, -75 km
-                # Aircraft(
-                #     position = QVector3D(0, -100_000, 0),
-                #     speed = QVector3D(300, 290, 0),
-                #     initial_target = QVector3D(75000, -27500, 0)), # 75 km, -27.5 km
-            ]
+            test_case : int = 0
+            if test_case == 0:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # detection test
+                        position = QVector3D(-800, 4000, 1000),
+                        speed = QVector3D(60, -60, 0),
+                        initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
+                    Aircraft(
+                        position = QVector3D(4000, 6000, 1000),
+                        speed = QVector3D(0, -85, 0),
+                        initial_target = QVector3D(900, -1_001_300, 1000)),
+                ]
+            elif test_case == 1:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # almost head on
+                        position = QVector3D(-3000, 500, 1000),
+                        speed = QVector3D(70, 0.1, 0)),
+                    Aircraft(
+                        position = QVector3D(5000, 500, 1000),
+                        speed = QVector3D(-50, 0, 0)),
+                ]
+            elif test_case == 2:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # avoidance test
+                        position = QVector3D(10, -10, 1000),
+                        speed = QVector3D(300, -300, 0),
+                        initial_target = QVector3D(75000, -75000, 0)), # 75 km, -75 km
+                    Aircraft(
+                        position = QVector3D(0, -100_000, 1000),
+                        speed = QVector3D(300, 290, 0),
+                        initial_target = QVector3D(75000, -27500, 0)), # 75 km, -27.5 km
+                ]
         else:
             self.aircrafts = aircrafts
         self.simulation_time : int = simulation_time
         self.state : SimulationState | None = None
 
     def run_realtime(self) -> None:
         """Executes realtime simulation"""
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py

```diff
@@ -40,14 +40,22 @@
             self.adsb_cycles += 1
             self.simulation_state.update_adsb_settings()
 
             relative_position = aircraft_vehicle_1.position - aircraft_vehicle_2.position
             speed_difference = aircraft_vehicle_1.speed - aircraft_vehicle_2.speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             print("Time to closest approach: " + "{:.2f}".format(time_to_closest_approach) + "s")
+            
+            for aircraft in self.aircraft_vehicles:
+                # path
+                self.aircraft_fccs[aircraft.aircraft_id].append_visited()
+
+                # console output
+                if self.simulation_state.adsb_report and aircraft.aircraft_id == 0:
+                    self.print_adsb_report(aircraft)
 
             if not self.simulation_state.avoid_collisions:
                 return
 
             if time_to_closest_approach > 0:
                 # miss distance at closest approach
                 speed_difference_unit = speed_difference.normalized()
@@ -81,31 +89,43 @@
                 if collision_region > 0:
                     print("Collision detected")
             else:
                 for aircraft in self.aircraft_fccs:
                     if aircraft.evade_maneuver:
                         aircraft.reset_evade_maneuver()
 
-            for aircraft in self.aircraft_vehicles:
-                # path
-                self.aircraft_fccs[aircraft.aircraft_id].append_visited()
-
-                # console output
-                if self.simulation_state.adsb_report and aircraft.aircraft_id == 0:
-                    self.print_adsb_report(aircraft)
-
     def print_adsb_report(self, aircraft : AircraftVehicle) -> None:
         """Prints ADS-B report for the aircraft to the console"""
-        print("Aircraft id: " + str(aircraft.aircraft_id) +
+        fcc = self.aircraft_fccs[aircraft.aircraft_id]
+        turning_direction = "Not turning"
+        if fcc.is_turning_left:
+            turning_direction = "Turning left"
+        elif fcc.is_turning_right:
+            turning_direction = "Turning right"
+        print("- Aircraft id: " + str(aircraft.aircraft_id) +
             "; speed: " + "{:.2f}".format(aircraft.absolute_speed) +
-            "; target speed: " + "{:.2f}".format(self.aircraft_fccs[aircraft.aircraft_id].target_speed) +
+            "; turning: " + turning_direction +
+            "; roll angle: " + "{:.2f}".format(aircraft.roll_angle) +
+            "; target roll angle: " + "{:.2f}".format(fcc.target_roll_angle) +
+            "; yaw angle: " + "{:.2f}".format(aircraft.yaw_angle) +
+            "; target yaw angle: " + "{:.2f}".format(fcc.target_yaw_angle) +
             "; x: " + "{:.2f}".format(aircraft.position.x()) +
             "; y: " + "{:.2f}".format(aircraft.position.y()) +
-            "; yaw angle: " + "{:.2f}".format(aircraft.yaw_angle) +
-            "; target yaw angle: " + "{:.2f}".format(self.aircraft_fccs[aircraft.aircraft_id].target_yaw_angle) +
-            "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
-            "; roll angle: " + "{:.2f}".format(aircraft.roll_angle) +
-            "; target roll angle: " + "{:.2f}".format(self.aircraft_fccs[aircraft.aircraft_id].target_roll_angle) +
-            "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
-            "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
-            "; t: " + str(self.adsb_cycles) +
-            "; phys: " + str(self.simulation_state.physics_cycles))
+            "; z: " + "{:.2f}".format(aircraft.position.z()))
+        if fcc.destination is not None:
+            print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
+                "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
+                "; dest x: " + "{:.2f}".format(fcc.destination.x()) +
+                "; dest y: " + "{:.2f}".format(fcc.destination.y()) +
+                "; dest z: " + "{:.2f}".format(fcc.destination.z()) +
+                "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
+                "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
+                "; t: " + str(self.adsb_cycles) +
+                "; phys: " + str(self.simulation_state.physics_cycles))
+        else:
+            print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
+                "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
+                "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
+                "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
+                "; t: " + str(self.adsb_cycles) +
+                "; phys: " + str(self.simulation_state.physics_cycles) +
+                "; no destination")
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py

```diff
@@ -117,34 +117,24 @@
             # pitch angle
 
             # yaw angle
             roll_angle : float = aircraft.roll_angle
 
             if roll_angle == 0.0:
                 continue
-            elif fcc.target_roll_angle > 0.0 and roll_angle < 0.0:
-                continue
-            elif fcc.target_roll_angle < 0.0 and roll_angle > 0.0:
-                continue
 
             current_yaw_angle : float = aircraft.yaw_angle
             target_yaw_angle : float = fcc.target_yaw_angle
             if abs(current_yaw_angle - target_yaw_angle) < 0.001:
                 continue
             current_horizontal_speed : float = aircraft.horizontal_speed
-            max_delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
-            max_delta_yaw_angle = abs(max_delta_yaw_angle)
-            if roll_angle < 0.0:
-                max_delta_yaw_angle = -max_delta_yaw_angle
+            delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
 
             new_yaw_angle : float = 0.0
-            if abs(current_yaw_angle - target_yaw_angle) < abs(max_delta_yaw_angle):
-                new_yaw_angle = target_yaw_angle
-            else:
-                new_yaw_angle = current_yaw_angle + max_delta_yaw_angle
+            new_yaw_angle = current_yaw_angle + delta_yaw_angle
 
             aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
             aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
 
     def count_cycles(self) -> None:
         """Increments physics cycle counter"""
         self.cycles += 1
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py

```diff
@@ -23,28 +23,32 @@
         self.minimum_separation : float = 9260.0 # 5nmi
         self.physics_cycles : int = 0
         self.is_paused : bool = False
         self.is_running : bool = True
         self.__reset_demanded : bool = False
         self.pause_start_timestamp : QTime | None = None
         self.time_paused : int = 0 # ms
-        self.__adsb_report : bool = False
+        self.__adsb_report : bool = True
         self.__collision : bool = False
         self.__first_cause_collision : bool = False
         self.__second_cause_collision : bool = False
 
         if is_realtime:
             # render state
-            self.__gui_scale : float = 1.0 # define gui scaling
-            if SimulationSettings.screen_resolution.height() < 1440:
-                self.gui_scale = 0.75
-            elif SimulationSettings.screen_resolution.height() < 1080:
-                self.gui_scale = 0.5
-            elif SimulationSettings.screen_resolution.height() < 480:
-                self.gui_scale = 0.25
+            override_gui_scale : bool = True
+            if not override_gui_scale:
+                self.__gui_scale : float = 0.5 # define gui scaling
+                if SimulationSettings.screen_resolution.height() < 1440:
+                    self.gui_scale = 0.375
+                elif SimulationSettings.screen_resolution.height() < 1080:
+                    self.gui_scale = 0.25
+                elif SimulationSettings.screen_resolution.height() < 480:
+                    self.gui_scale = 0.125
+            else:
+                self.__gui_scale : float = 0.75
             self.fps : float = 0.0
             self.draw_fps : bool = True
             self.draw_aircraft : bool = True
             self.draw_grid : bool = False
             self.draw_path : bool = True
             self.draw_speed_vectors : bool = True
             self.draw_collision_detection : bool = True
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py

```diff
@@ -396,17 +396,17 @@
                 return super().keyPressEvent(event)
             self.simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_R:
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
             self.simulation_state.reset()
         elif event.key() == Qt.Key.Key_Plus:
-            self.zoom(0.25)
+            self.zoom(0.0625)
         elif event.key() == Qt.Key.Key_Minus:
-            self.zoom(-0.25)
+            self.zoom(-0.0625)
         elif event.key() == Qt.Key.Key_F1:
             self.simulation_state.toggle_adsb_report()
         elif event.key() == Qt.Key.Key_F2:
             self.aircraft_fccs[0].target_speed -= 10.0
         elif event.key() == Qt.Key.Key_F3:
             self.aircraft_fccs[0].target_speed += 10.0
         elif event.key() == Qt.Key.Key_O:
```

## build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py

```diff
@@ -1,20 +1,28 @@
 """Main module for UAV Collision Avoidance application"""
 
 import logging
 import platform
 import datetime
 import signal
 from pathlib import Path
+from screeninfo import get_monitors
 
 from PySide6.QtWidgets import QApplication
 from .version import __version__ as version
 from .src.simulation.simulation import Simulation, SimulationSettings
 
-signal.signal(signal.SIGINT, signal.SIG_DFL)
+def signal_handler(sig, frame):
+    logging.warning("Ctrl+C keyboard interrupt. Exiting...")
+    try:
+        signal.default_int_handler(sig, frame)
+    except KeyboardInterrupt:
+        import sys
+        sys.exit(1)
+signal.signal(signal.SIGINT, signal_handler)
 try:
     start_time = datetime.datetime.now().strftime("%Y-%m-%d")
     Path("logs").mkdir(parents=True, exist_ok=True)
     logging.basicConfig(
         filename=f"logs/simulation-{start_time}.log",
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s")
@@ -27,45 +35,45 @@
 logging.info("-" * 120)
 if platform.system() == "Windows":
     import ctypes
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(
         f"io.github.mldxo.uav-collision-avoidance.{version}")
 logging.info("Detected platform: %s", platform.system())
 
-def main():
+def main(arg = None):
     """Executes main function"""
     import sys
     args = sys.argv[1:]
-    realtime : bool = True
-    run_tests : bool = False
-    if len(args) > 0:
+    app = QApplication(args)
+    app.setApplicationName("UAV Collsion Avoidance")
+    app.setApplicationVersion(version)
+    SimulationSettings.screen_resolution = app.primaryScreen().size()
+    logging.info("%s %s", app.applicationName(), app.applicationVersion())
+    sim : Simulation | None = None
+    if len(args) > 0 or arg is not None:
         if args[0] == "realtime":
-            realtime = True
-        elif args[0] == "prerender":
-            realtime = False
-        elif args[0] == "tests":
-            run_tests = True
+            if len(get_monitors) == 0:
+                logging.warning("Launching GUI Application without monitors detected")
+            sim = Simulation()
+            sys.exit(app.exec())
+        elif args[0] == "headless" or arg == "headless":
+            sim = Simulation(headless = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
+        elif args[0] == "tests" or arg == "tests":
+            sim = Simulation(headless = True, tests = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
         elif len(args) > 1:
+            print(f"Invalid arguments: {args}")
             logging.error("Invalid arguments: %s", args)
             sys.exit(1)
         else:
+            print(f"Invalid argument: {args[0]}")
             logging.error("Invalid argument: %s", args[0])
             sys.exit(1)
-    app = QApplication(args)
-    app.setApplicationName("UAV Collsion Avoidance")
-    app.setApplicationVersion(version)
-    SimulationSettings.screen_resolution = app.primaryScreen().size()
-    logging.info("%s %s", app.applicationName(), app.applicationVersion())
-    sim = Simulation()
-    if run_tests:
-        realtime = False
-        sim.run_tests(20)
-        sys.exit()
-    elif realtime:
-        sim.run_realtime()
-        sys.exit(app.exec())
     else:
-        sim.run_prerender()
-        sys.exit()
+        sim = Simulation()
+    sys.exit(app.exec())
 
 if __name__ == "__main__":
     main()
```

## build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py

```diff
@@ -1,20 +1,28 @@
 """Main module for UAV Collision Avoidance application"""
 
 import logging
 import platform
 import datetime
 import signal
 from pathlib import Path
+from screeninfo import get_monitors
 
 from PySide6.QtWidgets import QApplication
 from .version import __version__ as version
 from .src.simulation.simulation import Simulation, SimulationSettings
 
-signal.signal(signal.SIGINT, signal.SIG_DFL)
+def signal_handler(sig, frame):
+    logging.warning("Ctrl+C keyboard interrupt. Exiting...")
+    try:
+        signal.default_int_handler(sig, frame)
+    except KeyboardInterrupt:
+        import sys
+        sys.exit(1)
+signal.signal(signal.SIGINT, signal_handler)
 try:
     start_time = datetime.datetime.now().strftime("%Y-%m-%d")
     Path("logs").mkdir(parents=True, exist_ok=True)
     logging.basicConfig(
         filename=f"logs/simulation-{start_time}.log",
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s")
@@ -27,45 +35,45 @@
 logging.info("-" * 120)
 if platform.system() == "Windows":
     import ctypes
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(
         f"io.github.mldxo.uav-collision-avoidance.{version}")
 logging.info("Detected platform: %s", platform.system())
 
-def main():
+def main(arg = None):
     """Executes main function"""
     import sys
     args = sys.argv[1:]
-    realtime : bool = True
-    run_tests : bool = False
-    if len(args) > 0:
+    app = QApplication(args)
+    app.setApplicationName("UAV Collsion Avoidance")
+    app.setApplicationVersion(version)
+    SimulationSettings.screen_resolution = app.primaryScreen().size()
+    logging.info("%s %s", app.applicationName(), app.applicationVersion())
+    sim : Simulation | None = None
+    if len(args) > 0 or arg is not None:
         if args[0] == "realtime":
-            realtime = True
-        elif args[0] == "prerender":
-            realtime = False
-        elif args[0] == "tests":
-            run_tests = True
+            if len(get_monitors) == 0:
+                logging.warning("Launching GUI Application without monitors detected")
+            sim = Simulation()
+            sys.exit(app.exec())
+        elif args[0] == "headless" or arg == "headless":
+            sim = Simulation(headless = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
+        elif args[0] == "tests" or arg == "tests":
+            sim = Simulation(headless = True, tests = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
         elif len(args) > 1:
+            print(f"Invalid arguments: {args}")
             logging.error("Invalid arguments: %s", args)
             sys.exit(1)
         else:
+            print(f"Invalid argument: {args[0]}")
             logging.error("Invalid argument: %s", args[0])
             sys.exit(1)
-    app = QApplication(args)
-    app.setApplicationName("UAV Collsion Avoidance")
-    app.setApplicationVersion(version)
-    SimulationSettings.screen_resolution = app.primaryScreen().size()
-    logging.info("%s %s", app.applicationName(), app.applicationVersion())
-    sim = Simulation()
-    if run_tests:
-        realtime = False
-        sim.run_tests(20)
-        sys.exit()
-    elif realtime:
-        sim.run_realtime()
-        sys.exit(app.exec())
     else:
-        sim.run_prerender()
-        sys.exit()
+        sim = Simulation()
+    sys.exit(app.exec())
 
 if __name__ == "__main__":
     main()
```

## build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py

```diff
@@ -1,20 +1,28 @@
 """Main module for UAV Collision Avoidance application"""
 
 import logging
 import platform
 import datetime
 import signal
 from pathlib import Path
+from screeninfo import get_monitors
 
 from PySide6.QtWidgets import QApplication
 from .version import __version__ as version
 from .src.simulation.simulation import Simulation, SimulationSettings
 
-signal.signal(signal.SIGINT, signal.SIG_DFL)
+def signal_handler(sig, frame):
+    logging.warning("Ctrl+C keyboard interrupt. Exiting...")
+    try:
+        signal.default_int_handler(sig, frame)
+    except KeyboardInterrupt:
+        import sys
+        sys.exit(1)
+signal.signal(signal.SIGINT, signal_handler)
 try:
     start_time = datetime.datetime.now().strftime("%Y-%m-%d")
     Path("logs").mkdir(parents=True, exist_ok=True)
     logging.basicConfig(
         filename=f"logs/simulation-{start_time}.log",
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s")
@@ -27,45 +35,45 @@
 logging.info("-" * 120)
 if platform.system() == "Windows":
     import ctypes
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(
         f"io.github.mldxo.uav-collision-avoidance.{version}")
 logging.info("Detected platform: %s", platform.system())
 
-def main():
+def main(arg = None):
     """Executes main function"""
     import sys
     args = sys.argv[1:]
-    realtime : bool = True
-    run_tests : bool = False
-    if len(args) > 0:
+    app = QApplication(args)
+    app.setApplicationName("UAV Collsion Avoidance")
+    app.setApplicationVersion(version)
+    SimulationSettings.screen_resolution = app.primaryScreen().size()
+    logging.info("%s %s", app.applicationName(), app.applicationVersion())
+    sim : Simulation | None = None
+    if len(args) > 0 or arg is not None:
         if args[0] == "realtime":
-            realtime = True
-        elif args[0] == "prerender":
-            realtime = False
-        elif args[0] == "tests":
-            run_tests = True
+            if len(get_monitors) == 0:
+                logging.warning("Launching GUI Application without monitors detected")
+            sim = Simulation()
+            sys.exit(app.exec())
+        elif args[0] == "headless" or arg == "headless":
+            sim = Simulation(headless = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
+        elif args[0] == "tests" or arg == "tests":
+            sim = Simulation(headless = True, tests = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
         elif len(args) > 1:
+            print(f"Invalid arguments: {args}")
             logging.error("Invalid arguments: %s", args)
             sys.exit(1)
         else:
+            print(f"Invalid argument: {args[0]}")
             logging.error("Invalid argument: %s", args[0])
             sys.exit(1)
-    app = QApplication(args)
-    app.setApplicationName("UAV Collsion Avoidance")
-    app.setApplicationVersion(version)
-    SimulationSettings.screen_resolution = app.primaryScreen().size()
-    logging.info("%s %s", app.applicationName(), app.applicationVersion())
-    sim = Simulation()
-    if run_tests:
-        realtime = False
-        sim.run_tests(20)
-        sys.exit()
-    elif realtime:
-        sim.run_realtime()
-        sys.exit(app.exec())
     else:
-        sim.run_prerender()
-        sys.exit()
+        sim = Simulation()
+    sys.exit(app.exec())
 
 if __name__ == "__main__":
     main()
```

## build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -29,14 +29,15 @@
 
         self.initial_course : float = copy(self.target_yaw_angle)
         self.target_roll_angle : float = 0.0
         self.target_pitch_angle : float = 0.0
         self.__target_speed : float = self.aircraft.absolute_speed
         self.__is_turning_right : bool = False
         self.__is_turning_left : bool = False
+        self.ignore_destinations : bool = False
 
         self.__evade_maneuver : bool = False
         self.vector_sharing_resolution : QVector3D | None = None
 
         self.destinations_history : List[QVector3D] = []
         self.visited : List[QVector3D] = []
     
@@ -120,34 +121,49 @@
 
     def apply_evade_maneuver(self, opponent_speed : QVector3D, miss_distance_vector : QVector3D, unresolved_region : float, time_to_closest_approach : float) -> None:
         """Applies evade maneuver"""
         print(str(self.aircraft.aircraft_id) + ": opponent speed: " + "{:.2f}".format(opponent_speed.x()) + " " + "{:.2f}".format(opponent_speed.y()) + " " + "{:.2f}".format(opponent_speed.z()))
         print(str(self.aircraft.aircraft_id) + ": miss distance vector: " + "{:.2f}".format(miss_distance_vector.x()) + " " + "{:.2f}".format(miss_distance_vector.y()) + " " + "{:.2f}".format(miss_distance_vector.z()))
         print(str(self.aircraft.aircraft_id) + ": unresolved region: " + "{:.2f}".format(unresolved_region))
         print(str(self.aircraft.aircraft_id) + ": time to closest approach: " + "{:.2f}".format(time_to_closest_approach))
-        
-        if (miss_distance_vector.x() == 0 and miss_distance_vector.y() == 0 and miss_distance_vector.z() == 0):
-            return
 
         if self.__evade_maneuver:
             logging.warning("Another evade maneuver in progress")
         else:
             print(f"Aircraft {self.aircraft.aircraft_id} applying evade maneuver")
             logging.info("Aircraft %s applying evade maneuver", self.aircraft.aircraft_id)
             self.__evade_maneuver = True
-            self.vector_sharing_resolution : QVector3D | None = None
-            if self.aircraft_id == 0:
-                self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * -(miss_distance_vector)) / ((self.aircraft.speed.length() + opponent_speed.length()) * miss_distance_vector.length())
+
+            # this is temporal solution of the problem below
+            if miss_distance_vector.length() == 0:
+                miss_distance_vector = QVector3D(0.01, 0.01, 0.0)
+
+            target_avoiding : QVector3D = QVector3D()
+            if miss_distance_vector.length() == 0:
+                # todo: fix or just change height
+                # modified_speed_vector : QVector3D = self.aircraft.speed + 0.01 * (self.aircraft.speed.normalized().z() * self.aircraft.speed)
+                # modified_speed_vector : QVector3D = self.aircraft.speed + 0.01 * QVector3D.crossProduct(self.aircraft.speed.normalized(), self.aircraft.speed)
+                # modified_speed_vector : QVector3D = self.aircraft.speed + (QVector3D.crossProduct(QVector3D(0, 0, self.aircraft.speed.normalized().z()), self.aircraft.speed))
+                # print("Modified speed vector: " + "{:.2f}".format(modified_speed_vector.x()) + " " + "{:.2f}".format(modified_speed_vector.y()) + " " + "{:.2f}".format(modified_speed_vector.z()))
+                # unit_vector : QVector3D = modified_speed_vector.normalized()
+                # print("Unit vector: " + "{:.2f}".format(unit_vector.x()) + " " + "{:.2f}".format(unit_vector.y()) + " " + "{:.2f}".format(unit_vector.z()))
+                # target_avoiding = self.aircraft.position + (unit_vector * modified_speed_vector.length())
+                pass
             else:
-                self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * miss_distance_vector) / ((opponent_speed.length() + self.aircraft.speed.length()) * miss_distance_vector.length())
-            print("Vector sharing resolution: " + "{:.2f}".format(self.vector_sharing_resolution.x()) + " " + "{:.2f}".format(self.vector_sharing_resolution.y()) + " " + "{:.2f}".format(self.vector_sharing_resolution.z()))
+                self.vector_sharing_resolution : QVector3D | None = None
+                if self.aircraft_id == 0:
+                    self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * -(miss_distance_vector)) / ((self.aircraft.speed.length() + opponent_speed.length()) * miss_distance_vector.length())
+                elif self.aircraft_id == 1:
+                    self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * miss_distance_vector) / ((opponent_speed.length() + self.aircraft.speed.length()) * miss_distance_vector.length())
+                print("Vector sharing resolution: " + "{:.2f}".format(self.vector_sharing_resolution.x()) + " " + "{:.2f}".format(self.vector_sharing_resolution.y()) + " " + "{:.2f}".format(self.vector_sharing_resolution.z()))
+                modified_speed_vector : QVector3D = (self.aircraft.speed * time_to_closest_approach + self.vector_sharing_resolution)
+                unit_vector : QVector3D = modified_speed_vector.normalized()
+                target_avoiding = self.aircraft.position + (unit_vector * modified_speed_vector.length())
             
-            # self.vector_sharing_resolution *= 2
-
-            target_avoiding : QVector3D = self.aircraft.position + (self.aircraft.speed * time_to_closest_approach + self.vector_sharing_resolution)
+            print("Set target avoiding collision: " + "{:.2f}".format(target_avoiding.x()) + " " + "{:.2f}".format(target_avoiding.y()) + " " + "{:.2f}".format(target_avoiding.z()))
             self.add_first_destination(target_avoiding)
 
     def reset_evade_maneuver(self) -> None:
         """Resets evade maneuver"""
         if self.__evade_maneuver:
             logging.info("Aircraft %s reset evade maneuver", self.aircraft.aircraft_id)
             self.__evade_maneuver = False
@@ -191,15 +207,15 @@
             destination.y() - position.y(),
             destination.x() - position.x()))
         target_yaw_angle += 90
         return self.format_angle(target_yaw_angle)
 
     def update_target_yaw_angle(self) -> None:
         """Updates current yaw angle"""
-        if self.destinations:
+        if self.destinations and not self.ignore_destinations:
             destination = self.destinations[0]
             distance = dist(self.aircraft.position.toTuple(), destination.toTuple())
             if distance < self.aircraft.size / 2:
                 self.destinations_history.append(self.destinations.popleft())
                 if self.destinations:
                     destination = self.destinations[0]
                     logging.info("Aircraft %s visited destination and took next one", self.aircraft.aircraft_id)
```

## build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py

```diff
@@ -23,15 +23,15 @@
 class Simulation(QMainWindow):
     """Main simulation App"""
 
     def __init__(self, aircrafts : List[Aircraft] | None = None, simulation_time : int = 100_000) -> None:
         super().__init__()
         SimulationSettings().__init__()
         if aircrafts is None:
-            test_case : int = 0
+            test_case : int = 3
             if test_case == 0:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # detection test
                         position = QVector3D(-800, 4000, 1000),
                         speed = QVector3D(60, -60, 0),
                         initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
                     Aircraft(
@@ -47,21 +47,32 @@
                     Aircraft(
                         position = QVector3D(5000, 500, 1000),
                         speed = QVector3D(-50, 0, 0)),
                 ]
             elif test_case == 2:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # avoidance test
-                        position = QVector3D(10, -10, 1000),
+                        position = QVector3D(0, 0, 1000),
+                        speed = QVector3D(30, -30, 0),
+                        initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
+                    Aircraft(
+                        position = QVector3D(0, -100_000, 1000),
+                        speed = QVector3D(30, 29, 0),
+                        initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
+                ]
+            elif test_case == 3:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # avoidance test fast
+                        position = QVector3D(0, 0, 1000),
                         speed = QVector3D(300, -300, 0),
-                        initial_target = QVector3D(75000, -75000, 0)), # 75 km, -75 km
+                        initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
                     Aircraft(
                         position = QVector3D(0, -100_000, 1000),
                         speed = QVector3D(300, 290, 0),
-                        initial_target = QVector3D(75000, -27500, 0)), # 75 km, -27.5 km
+                        initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
                 ]
         else:
             self.aircrafts = aircrafts
         self.simulation_time : int = simulation_time
         self.state : SimulationState | None = None
 
     def run_realtime(self) -> None:
```

## build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py

```diff
@@ -62,16 +62,15 @@
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
                     speed_difference_unit,
                     QVector3D.crossProduct(relative_position, speed_difference_unit))
                 print("Miss distance at closest approach: " + "{:.2f}".format(miss_distance_vector.length()) + "m")
 
                 if miss_distance_vector.length() == 0:
                     print("Head-on collision detected")
-                    # todo: height change maneuver
-                    # else other evade maneuver
+                    logging.info("Head-on collision detected")
 
                 # resolve confict condition
                 unresolved_region : float = self.simulation_state.minimum_separation - abs(miss_distance_vector.length())
                 if unresolved_region > 0.0:
                     print("Conflict condition detected")
                     for aircraft in self.aircraft_fccs:
                         if not aircraft.evade_maneuver:
```

## build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py

```diff
@@ -38,24 +38,42 @@
             SimulationSettings.screen_resolution.height() / 2 - self.window_height / 2 - 30,
             self.window_width,
             self.window_height)
         self.setStyleSheet("background-color: white;")
         self.setWindowTitle(QApplication.applicationName() + " " + QApplication.applicationVersion())
 
         self.icon = QIcon()
-        self.icon.addPixmap(self.simulation_state.aircraft_pixmap, QIcon.Mode.Normal, QIcon.State.Off)
+        self.icon.addPixmap(self.generate_icon(), QIcon.Mode.Normal, QIcon.State.Off)
         self.setWindowIcon(self.icon)
 
-        self.__moving_view_up = False
-        self.__moving_view_down = False
-        self.__moving_view_left = False
-        self.__moving_view_right = False
+        self.__moving_view_up : bool = False
+        self.__moving_view_down : bool = False
+        self.__moving_view_left : bool = False
+        self.__moving_view_right : bool = False
+        self.__steering_left : bool = False
+        self.__steering_right : bool = False
+        self.__steering_up : bool = False
+        self.__steering_down : bool = False
 
         self.center_offsets()
 
+    def generate_icon(self) -> QPixmap:
+        """Returns icon for the main window"""
+        pixmap = QPixmap(self.simulation_state.aircraft_pixmap)
+        painter = QPainter(pixmap)
+        painter.setBrush(QColor("white"))
+        painter.drawEllipse(self.simulation_state.aircraft_pixmap.rect())
+        painter.drawPixmap(
+            self.simulation_state.aircraft_pixmap.width() * 0.125,
+            self.simulation_state.aircraft_pixmap.height() * 0.125,
+            self.simulation_state.aircraft_pixmap.scaled(self.simulation_state.aircraft_pixmap.width() * 0.75,
+            self.simulation_state.aircraft_pixmap.height() * 0.75))
+        painter.end()
+        return pixmap
+
     def draw_aircraft(self, aircraft : AircraftVehicle, scale : float) -> None:
         """Draws given aircraft vehicle"""
         yaw_angle : float = aircraft.yaw_angle
         size : float = aircraft.size * scale
         pixmap : QPixmap
         if not self.simulation_state.aircraft_pixmap.isNull():
             pixmap = self.simulation_state.aircraft_pixmap.scaled(
@@ -272,14 +290,40 @@
         if self.__moving_view_down:
             self.screen_offset_y -= 10.0 / scale
         if self.__moving_view_left:
             self.screen_offset_x += 10.0 / scale
         if self.__moving_view_right:
             self.screen_offset_x -= 10.0 / scale
 
+    def update_steering(self) -> None:
+        """Updates aircraft steering based on current input"""
+        if self.aircrafts[0] and (self.__steering_up or self.__steering_down or self.__steering_left or self.__steering_right):
+            if sum([self.__steering_up, self.__steering_down, self.__steering_left, self.__steering_right]) >= 3:
+                return
+            self.aircraft_fccs[0].ignore_destinations = True
+            target_yaw_angle : float | None = None
+            if self.__steering_up and self.__steering_left:
+                target_yaw_angle = -45.0
+            elif self.__steering_up and self.__steering_right:
+                target_yaw_angle = 45.0
+            elif self.__steering_down and self.__steering_left:
+                target_yaw_angle = -135.0
+            elif self.__steering_down and self.__steering_right:
+                target_yaw_angle = 135.0
+            elif self.__steering_up:
+                target_yaw_angle = 0.0
+            elif self.__steering_down:
+                target_yaw_angle = 180.0
+            elif self.__steering_left:
+                target_yaw_angle = -90.0
+            elif self.__steering_right:
+                target_yaw_angle = 90.0
+            if target_yaw_angle is not None:
+                self.aircraft_fccs[0].target_yaw_angle = target_yaw_angle
+
     def center_offsets(self) -> None:
         """Updates screen offsets centering on selected aircraft"""
         scale : float = self.simulation_state.gui_scale
         id = self.simulation_state.focus_aircraft_id
         self.screen_offset_x = - self.aircraft_vehicles[id].position.x() + self.window_width / 2 / scale
         self.screen_offset_y = - self.aircraft_vehicles[id].position.y() + self.window_height / 2 / scale
 
@@ -291,21 +335,22 @@
     def zoom(self, factor : float) -> None:
         """Zooms in/out the simulation render"""
         if self.simulation_state.gui_scale + factor <= 0:
             return
         old_scale : float = self.simulation_state.gui_scale
         self.simulation_state.gui_scale += factor
         scale : float = self.simulation_state.gui_scale
-        self.screen_offset_x = self.screen_offset_x * old_scale / scale
-        self.screen_offset_y = self.screen_offset_y * old_scale / scale
+        self.screen_offset_x = self.screen_offset_x * (old_scale / scale)
+        self.screen_offset_y = self.screen_offset_y * (old_scale / scale)
 
     def paintEvent(self, event : QPaintEvent) -> None:
         """Qt method painting the aircrafts"""
         self.simulation_fps.count_frame()
         scale : float = self.simulation_state.gui_scale
+        self.update_steering()
         if not self.simulation_state.follow_aircraft:
             self.update_moving_offsets()
         else:
             self.center_offsets()
 
         if self.simulation_state.draw_fps:
             self.draw_text(QVector3D(10, 10, 0), 0, "FPS: " + "{:.2f}".format(self.simulation_state.fps))
@@ -395,14 +440,15 @@
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
             self.simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_R:
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
             self.simulation_state.reset()
+            self.center_offsets()
         elif event.key() == Qt.Key.Key_Plus:
             self.zoom(0.0625)
         elif event.key() == Qt.Key.Key_Minus:
             self.zoom(-0.0625)
         elif event.key() == Qt.Key.Key_F1:
             self.simulation_state.toggle_adsb_report()
         elif event.key() == Qt.Key.Key_F2:
@@ -425,35 +471,45 @@
             self.__moving_view_right = True
         elif event.key() == Qt.Key.Key_Up:
             self.__moving_view_up = True
         elif event.key() == Qt.Key.Key_Down:
             self.__moving_view_down = True
         if self.aircrafts[0]:
             if event.key() == Qt.Key.Key_A:
-                self.aircraft_fccs[0].target_yaw_angle = -90.0
+                self.__steering_left = True
             elif event.key() == Qt.Key.Key_D:
-                self.aircraft_fccs[0].target_yaw_angle = 90.0
+                self.__steering_right = True
             elif event.key() == Qt.Key.Key_W:
-                self.aircraft_fccs[0].target_yaw_angle = 0.0
+                self.__steering_up = True
             elif event.key() == Qt.Key.Key_S:
-                self.aircraft_fccs[0].target_yaw_angle = 180.0
+                self.__steering_down = True
         return super().keyPressEvent(event)
     
     def keyReleaseEvent(self, event: QKeyEvent) -> None:
         """Qt method controlling keyboard input"""
         if event.key() == Qt.Key.Key_Slash and event.isAutoRepeat() and self.simulation_state.is_paused:
             self.simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_Left:
             self.__moving_view_left = False
         elif event.key() == Qt.Key.Key_Right:
             self.__moving_view_right = False
         elif event.key() == Qt.Key.Key_Up:
             self.__moving_view_up = False
         elif event.key() == Qt.Key.Key_Down:
             self.__moving_view_down = False
+        if self.aircrafts[0]:
+            self.aircraft_fccs[0].ignore_destinations = False
+            if event.key() == Qt.Key.Key_A:
+                self.__steering_left = False
+            elif event.key() == Qt.Key.Key_D:
+                self.__steering_right = False
+            elif event.key() == Qt.Key.Key_W:
+                self.__steering_up = False
+            elif event.key() == Qt.Key.Key_S:
+                self.__steering_down = False
         return super().keyReleaseEvent(event)
     
     def resizeEvent(self, event: QPaintEvent) -> None:
         """Qt method controlling window resize event"""
         self.update_resolutions()
         return super().resizeEvent(event)
```

## build/lib/build/lib/build/lib/uav_collision_avoidance/main.py

```diff
@@ -1,20 +1,28 @@
 """Main module for UAV Collision Avoidance application"""
 
 import logging
 import platform
 import datetime
 import signal
 from pathlib import Path
+from screeninfo import get_monitors
 
 from PySide6.QtWidgets import QApplication
 from .version import __version__ as version
 from .src.simulation.simulation import Simulation, SimulationSettings
 
-signal.signal(signal.SIGINT, signal.SIG_DFL)
+def signal_handler(sig, frame):
+    logging.warning("Ctrl+C keyboard interrupt. Exiting...")
+    try:
+        signal.default_int_handler(sig, frame)
+    except KeyboardInterrupt:
+        import sys
+        sys.exit(1)
+signal.signal(signal.SIGINT, signal_handler)
 try:
     start_time = datetime.datetime.now().strftime("%Y-%m-%d")
     Path("logs").mkdir(parents=True, exist_ok=True)
     logging.basicConfig(
         filename=f"logs/simulation-{start_time}.log",
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s")
@@ -27,45 +35,45 @@
 logging.info("-" * 120)
 if platform.system() == "Windows":
     import ctypes
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(
         f"io.github.mldxo.uav-collision-avoidance.{version}")
 logging.info("Detected platform: %s", platform.system())
 
-def main():
+def main(arg = None):
     """Executes main function"""
     import sys
     args = sys.argv[1:]
-    realtime : bool = True
-    run_tests : bool = False
-    if len(args) > 0:
+    app = QApplication(args)
+    app.setApplicationName("UAV Collsion Avoidance")
+    app.setApplicationVersion(version)
+    SimulationSettings.screen_resolution = app.primaryScreen().size()
+    logging.info("%s %s", app.applicationName(), app.applicationVersion())
+    sim : Simulation | None = None
+    if len(args) > 0 or arg is not None:
         if args[0] == "realtime":
-            realtime = True
-        elif args[0] == "prerender":
-            realtime = False
-        elif args[0] == "tests":
-            run_tests = True
+            if len(get_monitors) == 0:
+                logging.warning("Launching GUI Application without monitors detected")
+            sim = Simulation()
+            sys.exit(app.exec())
+        elif args[0] == "headless" or arg == "headless":
+            sim = Simulation(headless = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
+        elif args[0] == "tests" or arg == "tests":
+            sim = Simulation(headless = True, tests = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
         elif len(args) > 1:
+            print(f"Invalid arguments: {args}")
             logging.error("Invalid arguments: %s", args)
             sys.exit(1)
         else:
+            print(f"Invalid argument: {args[0]}")
             logging.error("Invalid argument: %s", args[0])
             sys.exit(1)
-    app = QApplication(args)
-    app.setApplicationName("UAV Collsion Avoidance")
-    app.setApplicationVersion(version)
-    SimulationSettings.screen_resolution = app.primaryScreen().size()
-    logging.info("%s %s", app.applicationName(), app.applicationVersion())
-    sim = Simulation()
-    if run_tests:
-        realtime = False
-        sim.run_tests(20)
-        sys.exit()
-    elif realtime:
-        sim.run_realtime()
-        sys.exit(app.exec())
     else:
-        sim.run_prerender()
-        sys.exit()
+        sim = Simulation()
+    sys.exit(app.exec())
 
 if __name__ == "__main__":
     main()
```

## build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -29,15 +29,17 @@
 
         self.initial_course : float = copy(self.target_yaw_angle)
         self.target_roll_angle : float = 0.0
         self.target_pitch_angle : float = 0.0
         self.__target_speed : float = self.aircraft.absolute_speed
         self.__is_turning_right : bool = False
         self.__is_turning_left : bool = False
+        self.ignore_destinations : bool = False
 
+        self.__safe_zone_occupied : bool = False
         self.__evade_maneuver : bool = False
         self.vector_sharing_resolution : QVector3D | None = None
 
         self.destinations_history : List[QVector3D] = []
         self.visited : List[QVector3D] = []
     
     @property
@@ -67,33 +69,43 @@
         return self.__is_turning_left
     
     @is_turning_left.setter
     def is_turning_left(self, value : bool) -> None:
         """Sets turning left state"""
         self.__is_turning_left = value
 
-    def add_last_destination(self, destination : QVector3D) -> None:
-        """Appends the given location (QVector3D) to the end of the destinations list."""
+    def check_new_destination(self, destination : QVector3D, first : bool) -> QVector3D | None:
+        """Checks if the given destination is already in the destinations list"""
         if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
             raise TypeError("Destination coordinates must be int or float.")
+        if len(self.destinations) > 0 and first:
+            if dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
+                print("Attempted to stack same destination")
+                logging.warning(f"Attempted to stack same destination: {destination}")
+                return None
+        elif len(self.destinations) > 0 and not first:
+            if dist(destination.toTuple(), self.destinations[len(self.destinations) - 1].toTuple()) < 1.0:
+                print("Attempted to stack same destination")
+                logging.warning(f"Attempted to stack same destination: {destination}")
+                return None
+        return destination
 
-        self.destinations.append(destination)
+    def add_last_destination(self, destination : QVector3D) -> None:
+        """Appends the given location (QVector3D) to the end of the destinations list."""
+        destination = self.check_new_destination(destination, False)
+        if destination is not None:
+            self.destinations.append(destination)
+            logging.info("Aircraft %s added new last destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     def add_first_destination(self, destination : QVector3D) -> None:
         """Pushes given location to the top of destinations list"""
-        if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
-            raise TypeError("Destination coordinates must be int or float.")
-
-        if len(self.destinations) > 0 and dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
-            print("Attempted to stack same destination")
-            logging.warning(f"Attempted to stack same destination: {destination}")
-            return
-
-        self.destinations.appendleft(destination)
-        logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
+        destination = self.check_new_destination(destination, True)
+        if destination is not None:
+            self.destinations.appendleft(destination)
+            logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     @property
     def destination(self) -> QVector3D | None:
         """Returns current destination"""
         if len(self.destinations) > 0:
             return self.destinations[0]
         else:
@@ -104,50 +116,81 @@
         self.visited.append(copy(self.aircraft.position))
 
     def normalize_angle(self, angle : float) -> float:
         """Normalizes -180-180 angle into 360 domain"""
         angle = angle % 360
         return angle if angle >= 0 else angle + 360
 
-    def format_angle(self, angle : float) -> float:
+    def format_yaw_angle(self, angle : float) -> float:
         """Formats angle into -180-180 domain"""
         angle = self.normalize_angle(angle)
         return angle if angle <= 180 else -180 + (angle - 180)
     
     @property
+    def safe_zone_occupied(self) -> bool:
+        """Returns safe zone occupied state"""
+        return self.__safe_zone_occupied
+    
+    @safe_zone_occupied.setter
+    def safe_zone_occupied(self, value : bool) -> None:
+        """Sets safe zone occupied state"""
+        if self.__safe_zone_occupied and value:
+            print("Safe zone already occupied")
+            logging.warning("Safe zone already occupied")
+        if not self.__safe_zone_occupied and not value:
+            print("Safe zone already free")
+            logging.warning("Safe zone already free")
+        self.__safe_zone_occupied = value
+    
+    @property
     def evade_maneuver(self) -> bool:
         """Returns evade maneuver state"""
         return self.__evade_maneuver
 
     def apply_evade_maneuver(self, opponent_speed : QVector3D, miss_distance_vector : QVector3D, unresolved_region : float, time_to_closest_approach : float) -> None:
         """Applies evade maneuver"""
         print(str(self.aircraft.aircraft_id) + ": opponent speed: " + "{:.2f}".format(opponent_speed.x()) + " " + "{:.2f}".format(opponent_speed.y()) + " " + "{:.2f}".format(opponent_speed.z()))
         print(str(self.aircraft.aircraft_id) + ": miss distance vector: " + "{:.2f}".format(miss_distance_vector.x()) + " " + "{:.2f}".format(miss_distance_vector.y()) + " " + "{:.2f}".format(miss_distance_vector.z()))
         print(str(self.aircraft.aircraft_id) + ": unresolved region: " + "{:.2f}".format(unresolved_region))
         print(str(self.aircraft.aircraft_id) + ": time to closest approach: " + "{:.2f}".format(time_to_closest_approach))
-        
-        if (miss_distance_vector.x() == 0 and miss_distance_vector.y() == 0 and miss_distance_vector.z() == 0):
-            return
 
         if self.__evade_maneuver:
             logging.warning("Another evade maneuver in progress")
         else:
             print(f"Aircraft {self.aircraft.aircraft_id} applying evade maneuver")
             logging.info("Aircraft %s applying evade maneuver", self.aircraft.aircraft_id)
             self.__evade_maneuver = True
-            self.vector_sharing_resolution : QVector3D | None = None
-            if self.aircraft_id == 0:
-                self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * -(miss_distance_vector)) / ((self.aircraft.speed.length() + opponent_speed.length()) * miss_distance_vector.length())
+
+            # this is temporal solution of the problem below
+            if miss_distance_vector.length() == 0:
+                miss_distance_vector = QVector3D(0.01, 0.01, 0.0)
+
+            target_avoiding : QVector3D = QVector3D()
+            if miss_distance_vector.length() == 0:
+                # todo: fix or just change height
+                # modified_speed_vector : QVector3D = self.aircraft.speed + 0.01 * (self.aircraft.speed.normalized().z() * self.aircraft.speed)
+                # modified_speed_vector : QVector3D = self.aircraft.speed + 0.01 * QVector3D.crossProduct(self.aircraft.speed.normalized(), self.aircraft.speed)
+                # modified_speed_vector : QVector3D = self.aircraft.speed + (QVector3D.crossProduct(QVector3D(0, 0, self.aircraft.speed.normalized().z()), self.aircraft.speed))
+                # print("Modified speed vector: " + "{:.2f}".format(modified_speed_vector.x()) + " " + "{:.2f}".format(modified_speed_vector.y()) + " " + "{:.2f}".format(modified_speed_vector.z()))
+                # unit_vector : QVector3D = modified_speed_vector.normalized()
+                # print("Unit vector: " + "{:.2f}".format(unit_vector.x()) + " " + "{:.2f}".format(unit_vector.y()) + " " + "{:.2f}".format(unit_vector.z()))
+                # target_avoiding = self.aircraft.position + (unit_vector * modified_speed_vector.length())
+                pass
             else:
-                self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * miss_distance_vector) / ((opponent_speed.length() + self.aircraft.speed.length()) * miss_distance_vector.length())
-            print("Vector sharing resolution: " + "{:.2f}".format(self.vector_sharing_resolution.x()) + " " + "{:.2f}".format(self.vector_sharing_resolution.y()) + " " + "{:.2f}".format(self.vector_sharing_resolution.z()))
+                self.vector_sharing_resolution : QVector3D | None = None
+                if self.aircraft_id == 0:
+                    self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * -(miss_distance_vector)) / ((self.aircraft.speed.length() + opponent_speed.length()) * miss_distance_vector.length())
+                elif self.aircraft_id == 1:
+                    self.vector_sharing_resolution = (opponent_speed.length() * unresolved_region * miss_distance_vector) / ((opponent_speed.length() + self.aircraft.speed.length()) * miss_distance_vector.length())
+                print("Vector sharing resolution: " + "{:.2f}".format(self.vector_sharing_resolution.x()) + " " + "{:.2f}".format(self.vector_sharing_resolution.y()) + " " + "{:.2f}".format(self.vector_sharing_resolution.z()))
+                modified_speed_vector : QVector3D = (self.aircraft.speed * time_to_closest_approach + self.vector_sharing_resolution)
+                unit_vector : QVector3D = modified_speed_vector.normalized()
+                target_avoiding = self.aircraft.position + (unit_vector * modified_speed_vector.length())
             
-            # self.vector_sharing_resolution *= 2
-
-            target_avoiding : QVector3D = self.aircraft.position + (self.aircraft.speed * time_to_closest_approach + self.vector_sharing_resolution)
+            print("Set target avoiding collision: " + "{:.2f}".format(target_avoiding.x()) + " " + "{:.2f}".format(target_avoiding.y()) + " " + "{:.2f}".format(target_avoiding.z()))
             self.add_first_destination(target_avoiding)
 
     def reset_evade_maneuver(self) -> None:
         """Resets evade maneuver"""
         if self.__evade_maneuver:
             logging.info("Aircraft %s reset evade maneuver", self.aircraft.aircraft_id)
             self.__evade_maneuver = False
@@ -187,19 +230,26 @@
         
     def find_best_yaw_angle(self, position : QVector3D, destination : QVector3D) -> float:
         """Finds best yaw angle for the given destination"""
         target_yaw_angle : float  = degrees(atan2(
             destination.y() - position.y(),
             destination.x() - position.x()))
         target_yaw_angle += 90
-        return self.format_angle(target_yaw_angle)
+        return self.format_yaw_angle(target_yaw_angle)
+    
+    def find_best_pitch_angle(self, position : QVector3D, destination : QVector3D) -> float:
+        """Finds best pitch angle for the given destination"""
+        target_pitch_angle : float = degrees(atan2(
+            destination.z() - position.z(),
+            dist(position.toTuple(), destination.toTuple())))
+        return target_pitch_angle
 
-    def update_target_yaw_angle(self) -> None:
+    def update_target_yaw_pitch_angles(self) -> None:
         """Updates current yaw angle"""
-        if self.destinations:
+        if self.destinations and not self.ignore_destinations:
             destination = self.destinations[0]
             distance = dist(self.aircraft.position.toTuple(), destination.toTuple())
             if distance < self.aircraft.size / 2:
                 self.destinations_history.append(self.destinations.popleft())
                 if self.destinations:
                     destination = self.destinations[0]
                     logging.info("Aircraft %s visited destination and took next one", self.aircraft.aircraft_id)
@@ -207,14 +257,17 @@
                 else:
                     logging.info("Aircraft %s visited destination and is free now", self.aircraft.aircraft_id)
                     print(f"Aircraft {self.aircraft.aircraft_id} visited destination and is free now")
                     return
             self.target_yaw_angle = self.find_best_yaw_angle(
                 self.aircraft.position,
                 destination)
+            self.target_pitch_angle = self.find_best_pitch_angle(
+                self.aircraft.position,
+                destination)
             
     def update_target_roll_angle(self) -> None:
         """Updates target roll angle"""
         current_yaw_angle = self.normalize_angle(self.aircraft.yaw_angle)
         target_yaw_angle = self.normalize_angle(self.target_yaw_angle)
         self.target_roll_angle = self.find_best_roll_angle(current_yaw_angle, target_yaw_angle)
 
@@ -224,21 +277,21 @@
                 next_position = self.destinations[0]
                 next_destination = self.destinations[1]
                 next_target_yaw_angle : float = self.find_best_yaw_angle(next_position, next_destination)
                 self.target_roll_angle = self.find_best_roll_angle(current_yaw_angle, next_target_yaw_angle)
 
     def update(self) -> None:
         """Updates current targeted movement angles"""
-        self.update_target_yaw_angle()
+        self.update_target_yaw_pitch_angles()
         self.update_target_roll_angle()
 
     def update_target(self, target : QVector3D) -> None:
         """Updates target position"""
         self.target_yaw_angle = self.find_best_yaw_angle(self.aircraft.position, target)
-        self.update_target_roll_angle()    
+        self.update_target_roll_angle()      
 
     def reset(self) -> None:
         """Resets aircraft flight control computer"""
         self.destinations.clear()
         self.destinations_history.clear()
         self.visited.clear()
         self.target_yaw_angle = self.initial_course
```

## build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py

```diff
@@ -29,39 +29,50 @@
         if aircrafts is None:
             test_case : int = 0
             if test_case == 0:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # detection test
                         position = QVector3D(-800, 4000, 1000),
                         speed = QVector3D(60, -60, 0),
-                        initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
+                        initial_target = QVector3D(1_000_100, -1_001_000, 10000)),
                     Aircraft(
                         position = QVector3D(4000, 6000, 1000),
                         speed = QVector3D(0, -85, 0),
-                        initial_target = QVector3D(900, -1_001_300, 1000)),
+                        initial_target = QVector3D(900, -1_001_300, 10000)),
                 ]
             elif test_case == 1:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # almost head on
                         position = QVector3D(-3000, 500, 1000),
                         speed = QVector3D(70, 0.1, 0)),
                     Aircraft(
                         position = QVector3D(5000, 500, 1000),
                         speed = QVector3D(-50, 0, 0)),
                 ]
             elif test_case == 2:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # avoidance test
-                        position = QVector3D(10, -10, 1000),
+                        position = QVector3D(0, 0, 1000),
+                        speed = QVector3D(30, -30, 0),
+                        initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
+                    Aircraft(
+                        position = QVector3D(0, -100_000, 1000),
+                        speed = QVector3D(30, 29, 0),
+                        initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
+                ]
+            elif test_case == 3:
+                self.aircrafts : List[Aircraft] = [
+                    Aircraft( # avoidance test fast
+                        position = QVector3D(0, 0, 1000),
                         speed = QVector3D(300, -300, 0),
-                        initial_target = QVector3D(75000, -75000, 0)), # 75 km, -75 km
+                        initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
                     Aircraft(
                         position = QVector3D(0, -100_000, 1000),
                         speed = QVector3D(300, 290, 0),
-                        initial_target = QVector3D(75000, -27500, 0)), # 75 km, -27.5 km
+                        initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
                 ]
         else:
             self.aircrafts = aircrafts
         self.simulation_time : int = simulation_time
         self.state : SimulationState | None = None
 
     def run_realtime(self) -> None:
```

## build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py

```diff
@@ -42,36 +42,56 @@
 
             relative_position = aircraft_vehicle_1.position - aircraft_vehicle_2.position
             speed_difference = aircraft_vehicle_1.speed - aircraft_vehicle_2.speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             print("Time to closest approach: " + "{:.2f}".format(time_to_closest_approach) + "s")
             
             for aircraft in self.aircraft_vehicles:
+                fcc : AircraftFCC = self.aircraft_fccs[aircraft.aircraft_id]
+
                 # path
-                self.aircraft_fccs[aircraft.aircraft_id].append_visited()
+                fcc.append_visited()
+
+                # console destination reach time
+                if fcc.destination and self.simulation_state.adsb_report:
+                    time_to_reaching_destination : float = (QVector3D.dotProduct(fcc.destination - aircraft.position, aircraft.speed) / QVector3D.dotProduct(aircraft.speed, aircraft.speed))
+                    print(f"Aircraft {aircraft.aircraft_id} will reach its destination in " + "{:.2f}".format(time_to_reaching_destination) + " (" + "{:.1f}".format(time_to_reaching_destination / 60) + " minutes or " + "{:.1f}".format(time_to_reaching_destination / 3600) + " hours)")
 
-                # console output
+                # console report output
                 if self.simulation_state.adsb_report and aircraft.aircraft_id == 0:
                     self.print_adsb_report(aircraft)
 
+                # safe zone occupancy check
+                if relative_position.length() < self.simulation_state.minimum_separation:
+                    if not fcc.safe_zone_occupied:
+                        fcc.safe_zone_occupied = True
+                        if not self.simulation_state.override_avoid_collisions:
+                            self.simulation_state.avoid_collisions = True
+                    print("Safe zone occupied")
+                else:
+                    if fcc.safe_zone_occupied:
+                        fcc.safe_zone_occupied = False
+                        self.simulation_state.avoid_collisions = False
+                    print("Safe zone free")
+                    return
+
             if not self.simulation_state.avoid_collisions:
                 return
 
             if time_to_closest_approach > 0:
                 # miss distance at closest approach
                 speed_difference_unit = speed_difference.normalized()
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
                     speed_difference_unit,
                     QVector3D.crossProduct(relative_position, speed_difference_unit))
                 print("Miss distance at closest approach: " + "{:.2f}".format(miss_distance_vector.length()) + "m")
 
                 if miss_distance_vector.length() == 0:
                     print("Head-on collision detected")
-                    # todo: height change maneuver
-                    # else other evade maneuver
+                    logging.info("Head-on collision detected")
 
                 # resolve confict condition
                 unresolved_region : float = self.simulation_state.minimum_separation - abs(miss_distance_vector.length())
                 if unresolved_region > 0.0:
                     print("Conflict condition detected")
                     for aircraft in self.aircraft_fccs:
                         if not aircraft.evade_maneuver:
```

## build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py

```diff
@@ -1,12 +1,12 @@
 """Simulation physics thread module"""
 
 import logging
 from copy import copy
-from math import sin, cos, dist, tan, radians
+from math import sin, cos, dist, tan, radians, sqrt
 from typing import List
 
 from PySide6.QtCore import QThread, QTime
 from PySide6.QtGui import QVector3D
 from PySide6.QtWidgets import QApplication, QMainWindow
 
 from ..aircraft.aircraft import Aircraft
@@ -50,15 +50,15 @@
         if self.simulation_state.reset_demanded:
             self.reset_aircrafts()
         if not self.simulation_state.is_paused:
             self.count_cycles()
             self.simulation_state.update_simulation_settings()
             self.update_aircrafts_speed_angles(elapsed_time)
             if self.update_aircrafts_position(elapsed_time):
-                logging.warn("Aircrafts collided at coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
+                logging.warn("Collision Occured. Aircrafts coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
                 QApplication.beep()
                 self.simulation_state.register_collision()
                 if self.isRunning():
                     self.requestInterruption()
 
     def reset_aircrafts(self) -> None:
         """Resets aircrafts to initial state"""
@@ -67,17 +67,20 @@
         self.aircraft_fccs[0].reset()
         self.aircraft_fccs[1].reset()
         self.simulation_state.apply_reset()
 
     def update_aircrafts_position(self, elapsed_time : float) -> bool:
         """Updates aircrafts position, returns true on collision"""
         for aircraft in self.aircraft_vehicles:
+            if aircraft.position.z() <= 0.0:
+                print("Collision with ground")
+                return True
             relative_distance : float = dist(aircraft.position.toTuple(), self.aircraft_vehicles[1 - aircraft.aircraft_id].position.toTuple())
             if relative_distance <= aircraft.size:
-                print("Collision")
+                print("Collision with another aircraft")
                 return True
             old_pos : QVector3D = copy(aircraft.position)
             aircraft.move(
                 aircraft.speed.x() * elapsed_time / 1000.0,
                 aircraft.speed.y() * elapsed_time / 1000.0,
                 aircraft.speed.z() * elapsed_time / 1000.0)
             aircraft.distance_covered = dist(old_pos.toTuple(), aircraft.position.toTuple())
@@ -93,15 +96,15 @@
             cause_collision = self.simulation_state.first_cause_collision if id == 0 else self.simulation_state.second_cause_collision
             fcc.update() if not cause_collision else fcc.update_target(self.aircraft_vehicles[1 - id].position + self.aircraft_vehicles[1 - id].speed)
             
             # speed
             current_speed = aircraft.absolute_speed
             target_speed = fcc.target_speed
             speed_difference = abs(current_speed - target_speed)
-            if speed_difference > 0.001 and target_speed > 20.0:
+            if speed_difference > 0.001 and current_speed > 20.0 and current_speed < 340: # make drone subsonic
                 max_speed_delta = aircraft.max_acceleration / elapsed_time
                 if speed_difference < max_speed_delta:
                     pass # become target
                 elif current_speed < target_speed:
                     target_speed = current_speed + max_speed_delta
                 else:
                     target_speed = current_speed - max_speed_delta
@@ -111,31 +114,48 @@
                     aircraft.speed.y() * speed_scale_factor,
                     aircraft.speed.z() * speed_scale_factor)
 
             # roll angle
             aircraft.roll_angle = (1.0 / (aircraft.roll_dynamic_delay / elapsed_time)) * (fcc.target_roll_angle - aircraft.roll_angle)
 
             # pitch angle
+            current_pitch_angle : float = aircraft.pitch_angle
+            target_pitch_angle : float = copy(fcc.target_pitch_angle)
+            if not abs(current_pitch_angle - target_pitch_angle) < 0.001 and current_pitch_angle < 90.0 and current_pitch_angle > -90.0:
+                delta_pitch_angle : float = (1.0 / (aircraft.pitch_dynamic_delay / elapsed_time)) * (target_pitch_angle - aircraft.pitch_angle)
+                new_pitch_angle : float = current_pitch_angle
+                if target_pitch_angle > 0:
+                    if target_pitch_angle > current_pitch_angle:
+                        new_pitch_angle = current_pitch_angle + delta_pitch_angle
+                    else:
+                        new_pitch_angle = current_pitch_angle - delta_pitch_angle
+                else: # target_pitch_angle < 0
+                    if target_pitch_angle < current_pitch_angle:
+                        new_pitch_angle = current_pitch_angle + delta_pitch_angle
+                    else:
+                        new_pitch_angle = current_pitch_angle - delta_pitch_angle
 
+                current_speed : float = aircraft.absolute_speed
+                new_speed_z = current_speed * sin(radians(new_pitch_angle))
+                aircraft.speed = QVector3D(
+                    aircraft.speed.x(),
+                    aircraft.speed.y(),
+                    new_speed_z)
+                
             # yaw angle
             roll_angle : float = aircraft.roll_angle
-
-            if roll_angle == 0.0:
-                continue
-
             current_yaw_angle : float = aircraft.yaw_angle
             target_yaw_angle : float = fcc.target_yaw_angle
-            if abs(current_yaw_angle - target_yaw_angle) < 0.001:
-                continue
-            current_horizontal_speed : float = aircraft.horizontal_speed
-            delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
+            if not (roll_angle == 0.0 or abs(current_yaw_angle - target_yaw_angle) < 0.001):
+                current_horizontal_speed : float = aircraft.horizontal_speed
+                delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
 
-            new_yaw_angle : float = 0.0
-            new_yaw_angle = current_yaw_angle + delta_yaw_angle
+                new_yaw_angle : float = 0.0
+                new_yaw_angle = current_yaw_angle + delta_yaw_angle
 
-            aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
-            aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
+                aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
+                aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
 
     def count_cycles(self) -> None:
         """Increments physics cycle counter"""
         self.cycles += 1
         self.simulation_state.physics_cycles = self.cycles
```

## build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py

```diff
@@ -16,14 +16,15 @@
         self.__mutex : QMutex = QMutex()
 
         # simulation state
         self.simulation_settings = simulation_settings
         self.update_settings()
         self.is_realtime : bool = is_realtime
         self.avoid_collisions : bool = avoid_collisions
+        self.override_avoid_collisions : bool = True
         self.minimum_separation : float = 9260.0 # 5nmi
         self.physics_cycles : int = 0
         self.is_paused : bool = False
         self.is_running : bool = True
         self.__reset_demanded : bool = False
         self.pause_start_timestamp : QTime | None = None
         self.time_paused : int = 0 # ms
```

## build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py

```diff
@@ -38,24 +38,42 @@
             SimulationSettings.screen_resolution.height() / 2 - self.window_height / 2 - 30,
             self.window_width,
             self.window_height)
         self.setStyleSheet("background-color: white;")
         self.setWindowTitle(QApplication.applicationName() + " " + QApplication.applicationVersion())
 
         self.icon = QIcon()
-        self.icon.addPixmap(self.simulation_state.aircraft_pixmap, QIcon.Mode.Normal, QIcon.State.Off)
+        self.icon.addPixmap(self.generate_icon(), QIcon.Mode.Normal, QIcon.State.Off)
         self.setWindowIcon(self.icon)
 
-        self.__moving_view_up = False
-        self.__moving_view_down = False
-        self.__moving_view_left = False
-        self.__moving_view_right = False
+        self.__moving_view_up : bool = False
+        self.__moving_view_down : bool = False
+        self.__moving_view_left : bool = False
+        self.__moving_view_right : bool = False
+        self.__steering_left : bool = False
+        self.__steering_right : bool = False
+        self.__steering_up : bool = False
+        self.__steering_down : bool = False
 
         self.center_offsets()
 
+    def generate_icon(self) -> QPixmap:
+        """Returns icon for the main window"""
+        pixmap = QPixmap(self.simulation_state.aircraft_pixmap)
+        painter = QPainter(pixmap)
+        painter.setBrush(QColor("white"))
+        painter.drawEllipse(self.simulation_state.aircraft_pixmap.rect())
+        painter.drawPixmap(
+            self.simulation_state.aircraft_pixmap.width() * 0.125,
+            self.simulation_state.aircraft_pixmap.height() * 0.125,
+            self.simulation_state.aircraft_pixmap.scaled(self.simulation_state.aircraft_pixmap.width() * 0.75,
+            self.simulation_state.aircraft_pixmap.height() * 0.75))
+        painter.end()
+        return pixmap
+
     def draw_aircraft(self, aircraft : AircraftVehicle, scale : float) -> None:
         """Draws given aircraft vehicle"""
         yaw_angle : float = aircraft.yaw_angle
         size : float = aircraft.size * scale
         pixmap : QPixmap
         if not self.simulation_state.aircraft_pixmap.isNull():
             pixmap = self.simulation_state.aircraft_pixmap.scaled(
@@ -199,15 +217,15 @@
         predicted_collision : bool = False
         time_to_closest_approach : float = 0.0
         if self.simulation_state.collision:
             self.draw_text(QVector3D(self.window_width - 70, 10, 0), 0, "COLLISION", QColor(255, 0, 0))
             return
         for aircraft in self.aircraft_vehicles:
             relative_position = aircraft.position - self.aircraft_vehicles[1 - aircraft.aircraft_id].position
-            speed_difference = aircraft.speed - self.aircraft_vehicles[1 - aircraft.aircraft_id].speed
+            speed_difference : QVector3D = aircraft.speed - self.aircraft_vehicles[1 - aircraft.aircraft_id].speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             if time_to_closest_approach > 0:
                 speed_difference_unit = speed_difference.normalized()
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
                     speed_difference_unit,
                     QVector3D.crossProduct(relative_position, speed_difference_unit))
                 collision_distance = aircraft.size / 2 + self.aircraft_vehicles[1 - aircraft.aircraft_id].size / 2
@@ -272,40 +290,72 @@
         if self.__moving_view_down:
             self.screen_offset_y -= 10.0 / scale
         if self.__moving_view_left:
             self.screen_offset_x += 10.0 / scale
         if self.__moving_view_right:
             self.screen_offset_x -= 10.0 / scale
 
+    def update_steering(self) -> None:
+        """Updates aircraft steering based on current input"""
+        if self.aircrafts[0] and (self.__steering_up or self.__steering_down or self.__steering_left or self.__steering_right):
+            if sum([self.__steering_up, self.__steering_down, self.__steering_left, self.__steering_right]) >= 3:
+                return
+            self.aircraft_fccs[0].ignore_destinations = True
+            target_yaw_angle : float | None = None
+            if self.__steering_up and self.__steering_left:
+                target_yaw_angle = -45.0
+            elif self.__steering_up and self.__steering_right:
+                target_yaw_angle = 45.0
+            elif self.__steering_down and self.__steering_left:
+                target_yaw_angle = -135.0
+            elif self.__steering_down and self.__steering_right:
+                target_yaw_angle = 135.0
+            elif self.__steering_up:
+                target_yaw_angle = 0.0
+            elif self.__steering_down:
+                target_yaw_angle = 180.0
+            elif self.__steering_left:
+                target_yaw_angle = -90.0
+            elif self.__steering_right:
+                target_yaw_angle = 90.0
+            if target_yaw_angle is not None:
+                self.aircraft_fccs[0].target_yaw_angle = target_yaw_angle
+
     def center_offsets(self) -> None:
         """Updates screen offsets centering on selected aircraft"""
         scale : float = self.simulation_state.gui_scale
         id = self.simulation_state.focus_aircraft_id
-        self.screen_offset_x = - self.aircraft_vehicles[id].position.x() + self.window_width / 2 / scale
-        self.screen_offset_y = - self.aircraft_vehicles[id].position.y() + self.window_height / 2 / scale
+        self.screen_offset_x = (self.window_width / 2.0) / scale - self.aircraft_vehicles[id].position.x()
+        self.screen_offset_y = (self.window_height / 2.0) / scale - self.aircraft_vehicles[id].position.y()
 
     def update_resolutions(self) -> None:
         """Updates bounding box resolution"""
         self.window_width = self.width()
         self.window_height = self.height()
 
     def zoom(self, factor : float) -> None:
         """Zooms in/out the simulation render"""
-        if self.simulation_state.gui_scale + factor <= 0:
+        if self.simulation_state.gui_scale + factor >= 2:
+            self.simulation_state.gui_scale = 2
             return
+        while factor > 0 and factor > 2 * self.simulation_state.gui_scale:
+            factor /= 2
+        while factor < 0 and self.simulation_state.gui_scale + factor <= 0:
+            factor /= 2
         old_scale : float = self.simulation_state.gui_scale
         self.simulation_state.gui_scale += factor
         scale : float = self.simulation_state.gui_scale
-        self.screen_offset_x = self.screen_offset_x * old_scale / scale
-        self.screen_offset_y = self.screen_offset_y * old_scale / scale
+        self.screen_offset_x = self.screen_offset_x * (old_scale / scale)
+        self.screen_offset_y = self.screen_offset_y * (old_scale / scale)
 
     def paintEvent(self, event : QPaintEvent) -> None:
         """Qt method painting the aircrafts"""
         self.simulation_fps.count_frame()
         scale : float = self.simulation_state.gui_scale
+        self.update_steering()
         if not self.simulation_state.follow_aircraft:
             self.update_moving_offsets()
         else:
             self.center_offsets()
 
         if self.simulation_state.draw_fps:
             self.draw_text(QVector3D(10, 10, 0), 0, "FPS: " + "{:.2f}".format(self.simulation_state.fps))
@@ -395,14 +445,15 @@
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
             self.simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_R:
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
             self.simulation_state.reset()
+            self.center_offsets()
         elif event.key() == Qt.Key.Key_Plus:
             self.zoom(0.0625)
         elif event.key() == Qt.Key.Key_Minus:
             self.zoom(-0.0625)
         elif event.key() == Qt.Key.Key_F1:
             self.simulation_state.toggle_adsb_report()
         elif event.key() == Qt.Key.Key_F2:
@@ -425,35 +476,45 @@
             self.__moving_view_right = True
         elif event.key() == Qt.Key.Key_Up:
             self.__moving_view_up = True
         elif event.key() == Qt.Key.Key_Down:
             self.__moving_view_down = True
         if self.aircrafts[0]:
             if event.key() == Qt.Key.Key_A:
-                self.aircraft_fccs[0].target_yaw_angle = -90.0
+                self.__steering_left = True
             elif event.key() == Qt.Key.Key_D:
-                self.aircraft_fccs[0].target_yaw_angle = 90.0
+                self.__steering_right = True
             elif event.key() == Qt.Key.Key_W:
-                self.aircraft_fccs[0].target_yaw_angle = 0.0
+                self.__steering_up = True
             elif event.key() == Qt.Key.Key_S:
-                self.aircraft_fccs[0].target_yaw_angle = 180.0
+                self.__steering_down = True
         return super().keyPressEvent(event)
     
     def keyReleaseEvent(self, event: QKeyEvent) -> None:
         """Qt method controlling keyboard input"""
         if event.key() == Qt.Key.Key_Slash and event.isAutoRepeat() and self.simulation_state.is_paused:
             self.simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_Left:
             self.__moving_view_left = False
         elif event.key() == Qt.Key.Key_Right:
             self.__moving_view_right = False
         elif event.key() == Qt.Key.Key_Up:
             self.__moving_view_up = False
         elif event.key() == Qt.Key.Key_Down:
             self.__moving_view_down = False
+        if self.aircrafts[0]:
+            self.aircraft_fccs[0].ignore_destinations = False
+            if event.key() == Qt.Key.Key_A:
+                self.__steering_left = False
+            elif event.key() == Qt.Key.Key_D:
+                self.__steering_right = False
+            elif event.key() == Qt.Key.Key_W:
+                self.__steering_up = False
+            elif event.key() == Qt.Key.Key_S:
+                self.__steering_down = False
         return super().keyReleaseEvent(event)
     
     def resizeEvent(self, event: QPaintEvent) -> None:
         """Qt method controlling window resize event"""
         self.update_resolutions()
         return super().resizeEvent(event)
```

## build/lib/build/lib/uav_collision_avoidance/main.py

```diff
@@ -1,20 +1,28 @@
 """Main module for UAV Collision Avoidance application"""
 
 import logging
 import platform
 import datetime
 import signal
 from pathlib import Path
+from screeninfo import get_monitors
 
 from PySide6.QtWidgets import QApplication
 from .version import __version__ as version
 from .src.simulation.simulation import Simulation, SimulationSettings
 
-signal.signal(signal.SIGINT, signal.SIG_DFL)
+def signal_handler(sig, frame):
+    logging.warning("Ctrl+C keyboard interrupt. Exiting...")
+    try:
+        signal.default_int_handler(sig, frame)
+    except KeyboardInterrupt:
+        import sys
+        sys.exit(1)
+signal.signal(signal.SIGINT, signal_handler)
 try:
     start_time = datetime.datetime.now().strftime("%Y-%m-%d")
     Path("logs").mkdir(parents=True, exist_ok=True)
     logging.basicConfig(
         filename=f"logs/simulation-{start_time}.log",
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s")
@@ -27,45 +35,45 @@
 logging.info("-" * 120)
 if platform.system() == "Windows":
     import ctypes
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(
         f"io.github.mldxo.uav-collision-avoidance.{version}")
 logging.info("Detected platform: %s", platform.system())
 
-def main():
+def main(arg = None):
     """Executes main function"""
     import sys
     args = sys.argv[1:]
-    realtime : bool = True
-    run_tests : bool = False
-    if len(args) > 0:
+    app = QApplication(args)
+    app.setApplicationName("UAV Collsion Avoidance")
+    app.setApplicationVersion(version)
+    SimulationSettings.screen_resolution = app.primaryScreen().size()
+    logging.info("%s %s", app.applicationName(), app.applicationVersion())
+    sim : Simulation | None = None
+    if len(args) > 0 or arg is not None:
         if args[0] == "realtime":
-            realtime = True
-        elif args[0] == "prerender":
-            realtime = False
-        elif args[0] == "tests":
-            run_tests = True
+            if len(get_monitors) == 0:
+                logging.warning("Launching GUI Application without monitors detected")
+            sim = Simulation()
+            sys.exit(app.exec())
+        elif args[0] == "headless" or arg == "headless":
+            sim = Simulation(headless = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
+        elif args[0] == "tests" or arg == "tests":
+            sim = Simulation(headless = True, tests = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
         elif len(args) > 1:
+            print(f"Invalid arguments: {args}")
             logging.error("Invalid arguments: %s", args)
             sys.exit(1)
         else:
+            print(f"Invalid argument: {args[0]}")
             logging.error("Invalid argument: %s", args[0])
             sys.exit(1)
-    app = QApplication(args)
-    app.setApplicationName("UAV Collsion Avoidance")
-    app.setApplicationVersion(version)
-    SimulationSettings.screen_resolution = app.primaryScreen().size()
-    logging.info("%s %s", app.applicationName(), app.applicationVersion())
-    sim = Simulation()
-    if run_tests:
-        realtime = False
-        sim.run_tests(20)
-        sys.exit()
-    elif realtime:
-        sim.run_realtime()
-        sys.exit(app.exec())
     else:
-        sim.run_prerender()
-        sys.exit()
+        sim = Simulation()
+    sys.exit(app.exec())
 
 if __name__ == "__main__":
     main()
```

## build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -31,14 +31,15 @@
         self.target_roll_angle : float = 0.0
         self.target_pitch_angle : float = 0.0
         self.__target_speed : float = self.aircraft.absolute_speed
         self.__is_turning_right : bool = False
         self.__is_turning_left : bool = False
         self.ignore_destinations : bool = False
 
+        self.__safe_zone_occupied : bool = False
         self.__evade_maneuver : bool = False
         self.vector_sharing_resolution : QVector3D | None = None
 
         self.destinations_history : List[QVector3D] = []
         self.visited : List[QVector3D] = []
     
     @property
@@ -68,33 +69,51 @@
         return self.__is_turning_left
     
     @is_turning_left.setter
     def is_turning_left(self, value : bool) -> None:
         """Sets turning left state"""
         self.__is_turning_left = value
 
-    def add_last_destination(self, destination : QVector3D) -> None:
-        """Appends the given location (QVector3D) to the end of the destinations list."""
+    def check_new_destination(self, destination : QVector3D, first : bool) -> QVector3D | None:
+        """Checks if the given destination is already in the destinations list"""
         if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
             raise TypeError("Destination coordinates must be int or float.")
+        if len(self.destinations) > 0 and first:
+            if dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
+                print("Attempted to stack same destination")
+                logging.warning(f"Attempted to stack same destination: {destination}")
+                return None
+        elif len(self.destinations) > 0 and not first:
+            if dist(destination.toTuple(), self.destinations[len(self.destinations) - 1].toTuple()) < 1.0:
+                print("Attempted to stack same destination")
+                logging.warning(f"Attempted to stack same destination: {destination}")
+                return None
+        if destination.z() < 500:
+            if destination.z() < 0:
+                print("Attempted to set destination below ground")
+                logging.warning(f"Attempted to set destination below ground: {destination}")
+            else:
+                print("Attempted to set destination too low")
+                logging.warning(f"Attempted to set destination too low: {destination}")
+            destination = QVector3D(destination.x(), destination.y(), 500)
+        return destination
 
-        self.destinations.append(destination)
+    def add_last_destination(self, destination : QVector3D) -> None:
+        """Appends the given location (QVector3D) to the end of the destinations list."""
+        destination : QVector3D = self.check_new_destination(destination, False)
+        if destination is not None:
+            self.destinations.append(destination)
+            logging.info("Aircraft %s added new last destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     def add_first_destination(self, destination : QVector3D) -> None:
         """Pushes given location to the top of destinations list"""
-        if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
-            raise TypeError("Destination coordinates must be int or float.")
-
-        if len(self.destinations) > 0 and dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
-            print("Attempted to stack same destination")
-            logging.warning(f"Attempted to stack same destination: {destination}")
-            return
-
-        self.destinations.appendleft(destination)
-        logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
+        destination : QVector3D = self.check_new_destination(destination, True)
+        if destination is not None:
+            self.destinations.appendleft(destination)
+            logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     @property
     def destination(self) -> QVector3D | None:
         """Returns current destination"""
         if len(self.destinations) > 0:
             return self.destinations[0]
         else:
@@ -105,20 +124,36 @@
         self.visited.append(copy(self.aircraft.position))
 
     def normalize_angle(self, angle : float) -> float:
         """Normalizes -180-180 angle into 360 domain"""
         angle = angle % 360
         return angle if angle >= 0 else angle + 360
 
-    def format_angle(self, angle : float) -> float:
+    def format_yaw_angle(self, angle : float) -> float:
         """Formats angle into -180-180 domain"""
         angle = self.normalize_angle(angle)
         return angle if angle <= 180 else -180 + (angle - 180)
     
     @property
+    def safe_zone_occupied(self) -> bool:
+        """Returns safe zone occupied state"""
+        return self.__safe_zone_occupied
+    
+    @safe_zone_occupied.setter
+    def safe_zone_occupied(self, value : bool) -> None:
+        """Sets safe zone occupied state"""
+        if self.__safe_zone_occupied and value:
+            print("Safe zone already occupied")
+            logging.warning("Safe zone already occupied")
+        if not self.__safe_zone_occupied and not value:
+            print("Safe zone already free")
+            logging.warning("Safe zone already free")
+        self.__safe_zone_occupied = value
+    
+    @property
     def evade_maneuver(self) -> bool:
         """Returns evade maneuver state"""
         return self.__evade_maneuver
 
     def apply_evade_maneuver(self, opponent_speed : QVector3D, miss_distance_vector : QVector3D, unresolved_region : float, time_to_closest_approach : float) -> None:
         """Applies evade maneuver"""
         print(str(self.aircraft.aircraft_id) + ": opponent speed: " + "{:.2f}".format(opponent_speed.x()) + " " + "{:.2f}".format(opponent_speed.y()) + " " + "{:.2f}".format(opponent_speed.z()))
@@ -203,17 +238,24 @@
         
     def find_best_yaw_angle(self, position : QVector3D, destination : QVector3D) -> float:
         """Finds best yaw angle for the given destination"""
         target_yaw_angle : float  = degrees(atan2(
             destination.y() - position.y(),
             destination.x() - position.x()))
         target_yaw_angle += 90
-        return self.format_angle(target_yaw_angle)
+        return self.format_yaw_angle(target_yaw_angle)
+    
+    def find_best_pitch_angle(self, position : QVector3D, destination : QVector3D) -> float:
+        """Finds best pitch angle for the given destination"""
+        target_pitch_angle : float = degrees(atan2(
+            destination.z() - position.z(),
+            dist(position.toTuple(), destination.toTuple())))
+        return target_pitch_angle
 
-    def update_target_yaw_angle(self) -> None:
+    def update_target_yaw_pitch_angles(self) -> None:
         """Updates current yaw angle"""
         if self.destinations and not self.ignore_destinations:
             destination = self.destinations[0]
             distance = dist(self.aircraft.position.toTuple(), destination.toTuple())
             if distance < self.aircraft.size / 2:
                 self.destinations_history.append(self.destinations.popleft())
                 if self.destinations:
@@ -223,14 +265,17 @@
                 else:
                     logging.info("Aircraft %s visited destination and is free now", self.aircraft.aircraft_id)
                     print(f"Aircraft {self.aircraft.aircraft_id} visited destination and is free now")
                     return
             self.target_yaw_angle = self.find_best_yaw_angle(
                 self.aircraft.position,
                 destination)
+            self.target_pitch_angle = self.find_best_pitch_angle(
+                self.aircraft.position,
+                destination)
             
     def update_target_roll_angle(self) -> None:
         """Updates target roll angle"""
         current_yaw_angle = self.normalize_angle(self.aircraft.yaw_angle)
         target_yaw_angle = self.normalize_angle(self.target_yaw_angle)
         self.target_roll_angle = self.find_best_roll_angle(current_yaw_angle, target_yaw_angle)
 
@@ -240,21 +285,21 @@
                 next_position = self.destinations[0]
                 next_destination = self.destinations[1]
                 next_target_yaw_angle : float = self.find_best_yaw_angle(next_position, next_destination)
                 self.target_roll_angle = self.find_best_roll_angle(current_yaw_angle, next_target_yaw_angle)
 
     def update(self) -> None:
         """Updates current targeted movement angles"""
-        self.update_target_yaw_angle()
+        self.update_target_yaw_pitch_angles()
         self.update_target_roll_angle()
 
     def update_target(self, target : QVector3D) -> None:
         """Updates target position"""
         self.target_yaw_angle = self.find_best_yaw_angle(self.aircraft.position, target)
-        self.update_target_roll_angle()    
+        self.update_target_roll_angle()      
 
     def reset(self) -> None:
         """Resets aircraft flight control computer"""
         self.destinations.clear()
         self.destinations_history.clear()
         self.visited.clear()
         self.target_yaw_angle = self.initial_course
```

## build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py

```diff
@@ -23,25 +23,25 @@
 class Simulation(QMainWindow):
     """Main simulation App"""
 
     def __init__(self, aircrafts : List[Aircraft] | None = None, simulation_time : int = 100_000) -> None:
         super().__init__()
         SimulationSettings().__init__()
         if aircrafts is None:
-            test_case : int = 3
+            test_case : int = 0
             if test_case == 0:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # detection test
                         position = QVector3D(-800, 4000, 1000),
                         speed = QVector3D(60, -60, 0),
-                        initial_target = QVector3D(1_000_100, -1_001_000, 1000)),
+                        initial_target = QVector3D(1_000_100, -1_001_000, 10000)),
                     Aircraft(
                         position = QVector3D(4000, 6000, 1000),
                         speed = QVector3D(0, -85, 0),
-                        initial_target = QVector3D(900, -1_001_300, 1000)),
+                        initial_target = QVector3D(900, -1_001_300, 10000)),
                 ]
             elif test_case == 1:
                 self.aircrafts : List[Aircraft] = [
                     Aircraft( # almost head on
                         position = QVector3D(-3000, 500, 1000),
                         speed = QVector3D(70, 0.1, 0)),
                     Aircraft(
```

## build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py

```diff
@@ -42,21 +42,42 @@
 
             relative_position = aircraft_vehicle_1.position - aircraft_vehicle_2.position
             speed_difference = aircraft_vehicle_1.speed - aircraft_vehicle_2.speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             print("Time to closest approach: " + "{:.2f}".format(time_to_closest_approach) + "s")
             
             for aircraft in self.aircraft_vehicles:
+                fcc : AircraftFCC = self.aircraft_fccs[aircraft.aircraft_id]
+
                 # path
-                self.aircraft_fccs[aircraft.aircraft_id].append_visited()
+                fcc.append_visited()
+
+                # console destination reach time
+                if fcc.destination and self.simulation_state.adsb_report:
+                    time_to_reaching_destination : float = (QVector3D.dotProduct(fcc.destination - aircraft.position, aircraft.speed) / QVector3D.dotProduct(aircraft.speed, aircraft.speed))
+                    print(f"Aircraft {aircraft.aircraft_id} will reach its destination in " + "{:.2f}".format(time_to_reaching_destination) + " (" + "{:.1f}".format(time_to_reaching_destination / 60) + " minutes or " + "{:.1f}".format(time_to_reaching_destination / 3600) + " hours)")
 
-                # console output
+                # console report output
                 if self.simulation_state.adsb_report and aircraft.aircraft_id == 0:
                     self.print_adsb_report(aircraft)
 
+                # safe zone occupancy check
+                if relative_position.length() < self.simulation_state.minimum_separation:
+                    if not fcc.safe_zone_occupied:
+                        fcc.safe_zone_occupied = True
+                        if not self.simulation_state.override_avoid_collisions:
+                            self.simulation_state.avoid_collisions = True
+                    print("Safe zone occupied")
+                else:
+                    if fcc.safe_zone_occupied:
+                        fcc.safe_zone_occupied = False
+                        self.simulation_state.avoid_collisions = False
+                    print("Safe zone free")
+                    return
+
             if not self.simulation_state.avoid_collisions:
                 return
 
             if time_to_closest_approach > 0:
                 # miss distance at closest approach
                 speed_difference_unit = speed_difference.normalized()
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
```

## build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py

```diff
@@ -1,12 +1,12 @@
 """Simulation physics thread module"""
 
 import logging
 from copy import copy
-from math import sin, cos, dist, tan, radians
+from math import sin, cos, dist, tan, radians, sqrt
 from typing import List
 
 from PySide6.QtCore import QThread, QTime
 from PySide6.QtGui import QVector3D
 from PySide6.QtWidgets import QApplication, QMainWindow
 
 from ..aircraft.aircraft import Aircraft
@@ -50,15 +50,14 @@
         if self.simulation_state.reset_demanded:
             self.reset_aircrafts()
         if not self.simulation_state.is_paused:
             self.count_cycles()
             self.simulation_state.update_simulation_settings()
             self.update_aircrafts_speed_angles(elapsed_time)
             if self.update_aircrafts_position(elapsed_time):
-                logging.warn("Aircrafts collided at coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
                 QApplication.beep()
                 self.simulation_state.register_collision()
                 if self.isRunning():
                     self.requestInterruption()
 
     def reset_aircrafts(self) -> None:
         """Resets aircrafts to initial state"""
@@ -67,17 +66,22 @@
         self.aircraft_fccs[0].reset()
         self.aircraft_fccs[1].reset()
         self.simulation_state.apply_reset()
 
     def update_aircrafts_position(self, elapsed_time : float) -> bool:
         """Updates aircrafts position, returns true on collision"""
         for aircraft in self.aircraft_vehicles:
+            if aircraft.position.z() <= 0.0:
+                logging.warn("Aircraft's " + str(aircraft.aircraft_id) + "collision with the ground. Coordinates: " + str(self.aircraft_vehicles[aircraft.aircraft_id].position.toTuple()))
+                print("Collision with ground")
+                return True
             relative_distance : float = dist(aircraft.position.toTuple(), self.aircraft_vehicles[1 - aircraft.aircraft_id].position.toTuple())
             if relative_distance <= aircraft.size:
-                print("Collision")
+                logging.warn("Aircrafts' 0 and 1 collision. Coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
+                print("Collision with another aircraft")
                 return True
             old_pos : QVector3D = copy(aircraft.position)
             aircraft.move(
                 aircraft.speed.x() * elapsed_time / 1000.0,
                 aircraft.speed.y() * elapsed_time / 1000.0,
                 aircraft.speed.z() * elapsed_time / 1000.0)
             aircraft.distance_covered = dist(old_pos.toTuple(), aircraft.position.toTuple())
@@ -93,15 +97,15 @@
             cause_collision = self.simulation_state.first_cause_collision if id == 0 else self.simulation_state.second_cause_collision
             fcc.update() if not cause_collision else fcc.update_target(self.aircraft_vehicles[1 - id].position + self.aircraft_vehicles[1 - id].speed)
             
             # speed
             current_speed = aircraft.absolute_speed
             target_speed = fcc.target_speed
             speed_difference = abs(current_speed - target_speed)
-            if speed_difference > 0.001 and target_speed > 20.0:
+            if speed_difference > 0.001 and current_speed > 20.0 and current_speed < 340: # make drone subsonic
                 max_speed_delta = aircraft.max_acceleration / elapsed_time
                 if speed_difference < max_speed_delta:
                     pass # become target
                 elif current_speed < target_speed:
                     target_speed = current_speed + max_speed_delta
                 else:
                     target_speed = current_speed - max_speed_delta
@@ -111,31 +115,48 @@
                     aircraft.speed.y() * speed_scale_factor,
                     aircraft.speed.z() * speed_scale_factor)
 
             # roll angle
             aircraft.roll_angle = (1.0 / (aircraft.roll_dynamic_delay / elapsed_time)) * (fcc.target_roll_angle - aircraft.roll_angle)
 
             # pitch angle
+            current_pitch_angle : float = aircraft.pitch_angle
+            target_pitch_angle : float = copy(fcc.target_pitch_angle)
+            if not abs(current_pitch_angle - target_pitch_angle) < 0.001 and current_pitch_angle < 90.0 and current_pitch_angle > -90.0:
+                delta_pitch_angle : float = (1.0 / (aircraft.pitch_dynamic_delay / elapsed_time)) * (target_pitch_angle - aircraft.pitch_angle)
+                new_pitch_angle : float = current_pitch_angle
+                if target_pitch_angle > 0:
+                    if target_pitch_angle > current_pitch_angle:
+                        new_pitch_angle = current_pitch_angle + delta_pitch_angle
+                    else:
+                        new_pitch_angle = current_pitch_angle - delta_pitch_angle
+                else: # target_pitch_angle < 0
+                    if target_pitch_angle < current_pitch_angle:
+                        new_pitch_angle = current_pitch_angle + delta_pitch_angle
+                    else:
+                        new_pitch_angle = current_pitch_angle - delta_pitch_angle
 
+                current_speed : float = aircraft.absolute_speed
+                new_speed_z = current_speed * sin(radians(new_pitch_angle))
+                aircraft.speed = QVector3D(
+                    aircraft.speed.x(),
+                    aircraft.speed.y(),
+                    new_speed_z)
+                
             # yaw angle
             roll_angle : float = aircraft.roll_angle
-
-            if roll_angle == 0.0:
-                continue
-
             current_yaw_angle : float = aircraft.yaw_angle
             target_yaw_angle : float = fcc.target_yaw_angle
-            if abs(current_yaw_angle - target_yaw_angle) < 0.001:
-                continue
-            current_horizontal_speed : float = aircraft.horizontal_speed
-            delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
+            if not (roll_angle == 0.0 or abs(current_yaw_angle - target_yaw_angle) < 0.001):
+                current_horizontal_speed : float = aircraft.horizontal_speed
+                delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
 
-            new_yaw_angle : float = 0.0
-            new_yaw_angle = current_yaw_angle + delta_yaw_angle
+                new_yaw_angle : float = 0.0
+                new_yaw_angle = current_yaw_angle + delta_yaw_angle
 
-            aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
-            aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
+                aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
+                aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
 
     def count_cycles(self) -> None:
         """Increments physics cycle counter"""
         self.cycles += 1
         self.simulation_state.physics_cycles = self.cycles
```

## build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py

```diff
@@ -16,14 +16,15 @@
         self.__mutex : QMutex = QMutex()
 
         # simulation state
         self.simulation_settings = simulation_settings
         self.update_settings()
         self.is_realtime : bool = is_realtime
         self.avoid_collisions : bool = avoid_collisions
+        self.override_avoid_collisions : bool = True
         self.minimum_separation : float = 9260.0 # 5nmi
         self.physics_cycles : int = 0
         self.is_paused : bool = False
         self.is_running : bool = True
         self.__reset_demanded : bool = False
         self.pause_start_timestamp : QTime | None = None
         self.time_paused : int = 0 # ms
```

## build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py

```diff
@@ -217,15 +217,15 @@
         predicted_collision : bool = False
         time_to_closest_approach : float = 0.0
         if self.simulation_state.collision:
             self.draw_text(QVector3D(self.window_width - 70, 10, 0), 0, "COLLISION", QColor(255, 0, 0))
             return
         for aircraft in self.aircraft_vehicles:
             relative_position = aircraft.position - self.aircraft_vehicles[1 - aircraft.aircraft_id].position
-            speed_difference = aircraft.speed - self.aircraft_vehicles[1 - aircraft.aircraft_id].speed
+            speed_difference : QVector3D = aircraft.speed - self.aircraft_vehicles[1 - aircraft.aircraft_id].speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             if time_to_closest_approach > 0:
                 speed_difference_unit = speed_difference.normalized()
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
                     speed_difference_unit,
                     QVector3D.crossProduct(relative_position, speed_difference_unit))
                 collision_distance = aircraft.size / 2 + self.aircraft_vehicles[1 - aircraft.aircraft_id].size / 2
@@ -320,26 +320,31 @@
             if target_yaw_angle is not None:
                 self.aircraft_fccs[0].target_yaw_angle = target_yaw_angle
 
     def center_offsets(self) -> None:
         """Updates screen offsets centering on selected aircraft"""
         scale : float = self.simulation_state.gui_scale
         id = self.simulation_state.focus_aircraft_id
-        self.screen_offset_x = - self.aircraft_vehicles[id].position.x() + self.window_width / 2 / scale
-        self.screen_offset_y = - self.aircraft_vehicles[id].position.y() + self.window_height / 2 / scale
+        self.screen_offset_x = (self.window_width / 2.0) / scale - self.aircraft_vehicles[id].position.x()
+        self.screen_offset_y = (self.window_height / 2.0) / scale - self.aircraft_vehicles[id].position.y()
 
     def update_resolutions(self) -> None:
         """Updates bounding box resolution"""
         self.window_width = self.width()
         self.window_height = self.height()
 
     def zoom(self, factor : float) -> None:
         """Zooms in/out the simulation render"""
-        if self.simulation_state.gui_scale + factor <= 0:
+        if self.simulation_state.gui_scale + factor >= 2:
+            self.simulation_state.gui_scale = 2
             return
+        while factor > 0 and factor > 2 * self.simulation_state.gui_scale:
+            factor /= 2
+        while factor < 0 and self.simulation_state.gui_scale + factor <= 0:
+            factor /= 2
         old_scale : float = self.simulation_state.gui_scale
         self.simulation_state.gui_scale += factor
         scale : float = self.simulation_state.gui_scale
         self.screen_offset_x = self.screen_offset_x * (old_scale / scale)
         self.screen_offset_y = self.screen_offset_y * (old_scale / scale)
 
     def paintEvent(self, event : QPaintEvent) -> None:
```

## build/lib/uav_collision_avoidance/main.py

```diff
@@ -1,20 +1,28 @@
 """Main module for UAV Collision Avoidance application"""
 
 import logging
 import platform
 import datetime
 import signal
 from pathlib import Path
+from screeninfo import get_monitors
 
 from PySide6.QtWidgets import QApplication
 from .version import __version__ as version
 from .src.simulation.simulation import Simulation, SimulationSettings
 
-signal.signal(signal.SIGINT, signal.SIG_DFL)
+def signal_handler(sig, frame):
+    logging.warning("Ctrl+C keyboard interrupt. Exiting...")
+    try:
+        signal.default_int_handler(sig, frame)
+    except KeyboardInterrupt:
+        import sys
+        sys.exit(1)
+signal.signal(signal.SIGINT, signal_handler)
 try:
     start_time = datetime.datetime.now().strftime("%Y-%m-%d")
     Path("logs").mkdir(parents=True, exist_ok=True)
     logging.basicConfig(
         filename=f"logs/simulation-{start_time}.log",
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s")
@@ -27,45 +35,45 @@
 logging.info("-" * 120)
 if platform.system() == "Windows":
     import ctypes
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(
         f"io.github.mldxo.uav-collision-avoidance.{version}")
 logging.info("Detected platform: %s", platform.system())
 
-def main():
+def main(arg = None):
     """Executes main function"""
     import sys
     args = sys.argv[1:]
-    realtime : bool = True
-    run_tests : bool = False
-    if len(args) > 0:
+    app = QApplication(args)
+    app.setApplicationName("UAV Collsion Avoidance")
+    app.setApplicationVersion(version)
+    SimulationSettings.screen_resolution = app.primaryScreen().size()
+    logging.info("%s %s", app.applicationName(), app.applicationVersion())
+    sim : Simulation | None = None
+    if len(args) > 0 or arg is not None:
         if args[0] == "realtime":
-            realtime = True
-        elif args[0] == "prerender":
-            realtime = False
-        elif args[0] == "tests":
-            run_tests = True
+            if len(get_monitors) == 0:
+                logging.warning("Launching GUI Application without monitors detected")
+            sim = Simulation()
+            sys.exit(app.exec())
+        elif args[0] == "headless" or arg == "headless":
+            sim = Simulation(headless = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
+        elif args[0] == "tests" or arg == "tests":
+            sim = Simulation(headless = True, tests = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
         elif len(args) > 1:
+            print(f"Invalid arguments: {args}")
             logging.error("Invalid arguments: %s", args)
             sys.exit(1)
         else:
+            print(f"Invalid argument: {args[0]}")
             logging.error("Invalid argument: %s", args[0])
             sys.exit(1)
-    app = QApplication(args)
-    app.setApplicationName("UAV Collsion Avoidance")
-    app.setApplicationVersion(version)
-    SimulationSettings.screen_resolution = app.primaryScreen().size()
-    logging.info("%s %s", app.applicationName(), app.applicationVersion())
-    sim = Simulation()
-    if run_tests:
-        realtime = False
-        sim.run_tests(20)
-        sys.exit()
-    elif realtime:
-        sim.run_realtime()
-        sys.exit(app.exec())
     else:
-        sim.run_prerender()
-        sys.exit()
+        sim = Simulation()
+    sys.exit(app.exec())
 
 if __name__ == "__main__":
     main()
```

## build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -83,26 +83,34 @@
                 logging.warning(f"Attempted to stack same destination: {destination}")
                 return None
         elif len(self.destinations) > 0 and not first:
             if dist(destination.toTuple(), self.destinations[len(self.destinations) - 1].toTuple()) < 1.0:
                 print("Attempted to stack same destination")
                 logging.warning(f"Attempted to stack same destination: {destination}")
                 return None
+        if destination.z() < 500:
+            if destination.z() < 0:
+                print("Attempted to set destination below ground")
+                logging.warning(f"Attempted to set destination below ground: {destination}")
+            else:
+                print("Attempted to set destination too low")
+                logging.warning(f"Attempted to set destination too low: {destination}")
+            destination = QVector3D(destination.x(), destination.y(), 500)
         return destination
 
     def add_last_destination(self, destination : QVector3D) -> None:
         """Appends the given location (QVector3D) to the end of the destinations list."""
-        destination = self.check_new_destination(destination, False)
+        destination : QVector3D = self.check_new_destination(destination, False)
         if destination is not None:
             self.destinations.append(destination)
             logging.info("Aircraft %s added new last destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     def add_first_destination(self, destination : QVector3D) -> None:
         """Pushes given location to the top of destinations list"""
-        destination = self.check_new_destination(destination, True)
+        destination : QVector3D = self.check_new_destination(destination, True)
         if destination is not None:
             self.destinations.appendleft(destination)
             logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
 
     @property
     def destination(self) -> QVector3D | None:
         """Returns current destination"""
```

## build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py

```diff
@@ -50,15 +50,14 @@
         if self.simulation_state.reset_demanded:
             self.reset_aircrafts()
         if not self.simulation_state.is_paused:
             self.count_cycles()
             self.simulation_state.update_simulation_settings()
             self.update_aircrafts_speed_angles(elapsed_time)
             if self.update_aircrafts_position(elapsed_time):
-                logging.warn("Collision Occured. Aircrafts coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
                 QApplication.beep()
                 self.simulation_state.register_collision()
                 if self.isRunning():
                     self.requestInterruption()
 
     def reset_aircrafts(self) -> None:
         """Resets aircrafts to initial state"""
@@ -68,18 +67,20 @@
         self.aircraft_fccs[1].reset()
         self.simulation_state.apply_reset()
 
     def update_aircrafts_position(self, elapsed_time : float) -> bool:
         """Updates aircrafts position, returns true on collision"""
         for aircraft in self.aircraft_vehicles:
             if aircraft.position.z() <= 0.0:
+                logging.warn("Aircraft's " + str(aircraft.aircraft_id) + "collision with the ground. Coordinates: " + str(self.aircraft_vehicles[aircraft.aircraft_id].position.toTuple()))
                 print("Collision with ground")
                 return True
             relative_distance : float = dist(aircraft.position.toTuple(), self.aircraft_vehicles[1 - aircraft.aircraft_id].position.toTuple())
             if relative_distance <= aircraft.size:
+                logging.warn("Aircrafts' 0 and 1 collision. Coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
                 print("Collision with another aircraft")
                 return True
             old_pos : QVector3D = copy(aircraft.position)
             aircraft.move(
                 aircraft.speed.x() * elapsed_time / 1000.0,
                 aircraft.speed.y() * elapsed_time / 1000.0,
                 aircraft.speed.z() * elapsed_time / 1000.0)
```

## uav_collision_avoidance/main.py

```diff
@@ -1,20 +1,28 @@
 """Main module for UAV Collision Avoidance application"""
 
 import logging
 import platform
 import datetime
 import signal
 from pathlib import Path
+from screeninfo import get_monitors
 
 from PySide6.QtWidgets import QApplication
 from .version import __version__ as version
 from .src.simulation.simulation import Simulation, SimulationSettings
 
-signal.signal(signal.SIGINT, signal.SIG_DFL)
+def signal_handler(sig, frame):
+    logging.warning("Ctrl+C keyboard interrupt. Exiting...")
+    try:
+        signal.default_int_handler(sig, frame)
+    except KeyboardInterrupt:
+        import sys
+        sys.exit(1)
+signal.signal(signal.SIGINT, signal_handler)
 try:
     start_time = datetime.datetime.now().strftime("%Y-%m-%d")
     Path("logs").mkdir(parents=True, exist_ok=True)
     logging.basicConfig(
         filename=f"logs/simulation-{start_time}.log",
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(filename)s - %(message)s")
@@ -27,45 +35,45 @@
 logging.info("-" * 120)
 if platform.system() == "Windows":
     import ctypes
     ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(
         f"io.github.mldxo.uav-collision-avoidance.{version}")
 logging.info("Detected platform: %s", platform.system())
 
-def main():
+def main(arg = None):
     """Executes main function"""
     import sys
     args = sys.argv[1:]
-    realtime : bool = True
-    run_tests : bool = False
-    if len(args) > 0:
+    app = QApplication(args)
+    app.setApplicationName("UAV Collsion Avoidance")
+    app.setApplicationVersion(version)
+    SimulationSettings.screen_resolution = app.primaryScreen().size()
+    logging.info("%s %s", app.applicationName(), app.applicationVersion())
+    sim : Simulation | None = None
+    if len(args) > 0 or arg is not None:
         if args[0] == "realtime":
-            realtime = True
-        elif args[0] == "prerender":
-            realtime = False
-        elif args[0] == "tests":
-            run_tests = True
+            if len(get_monitors) == 0:
+                logging.warning("Launching GUI Application without monitors detected")
+            sim = Simulation()
+            sys.exit(app.exec())
+        elif args[0] == "headless" or arg == "headless":
+            sim = Simulation(headless = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
+        elif args[0] == "tests" or arg == "tests":
+            sim = Simulation(headless = True, tests = True)
+            QApplication.shutdown(app)
+            sys.exit(0)
         elif len(args) > 1:
+            print(f"Invalid arguments: {args}")
             logging.error("Invalid arguments: %s", args)
             sys.exit(1)
         else:
+            print(f"Invalid argument: {args[0]}")
             logging.error("Invalid argument: %s", args[0])
             sys.exit(1)
-    app = QApplication(args)
-    app.setApplicationName("UAV Collsion Avoidance")
-    app.setApplicationVersion(version)
-    SimulationSettings.screen_resolution = app.primaryScreen().size()
-    logging.info("%s %s", app.applicationName(), app.applicationVersion())
-    sim = Simulation()
-    if run_tests:
-        realtime = False
-        sim.run_tests(20)
-        sys.exit()
-    elif realtime:
-        sim.run_realtime()
-        sys.exit(app.exec())
     else:
-        sim.run_prerender()
-        sys.exit()
+        sim = Simulation()
+    sys.exit(app.exec())
 
 if __name__ == "__main__":
     main()
```

## uav_collision_avoidance/src/aircraft/aircraft.py

```diff
@@ -1,53 +1,74 @@
 """Aircraft class module"""
 
 from copy import copy
 
-from PySide6.QtCore import QObject
+from PySide6.QtCore import QObject, QMutex, QMutexLocker
 from PySide6.QtGui import QVector3D
 
 from .aircraft_vehicle import AircraftVehicle
 from .aircraft_fcc import AircraftFCC
 
 class Aircraft(QObject):
     """Main aircraft class"""
     
     __current_id : int = 0
 
-    def __init__(self, position : QVector3D, speed : QVector3D, initial_target : QVector3D | None = None) -> None:
+    def __init__(self, position : QVector3D, speed : QVector3D, initial_target : QVector3D | None = None, initial_roll_angle : float = 0.0) -> None:
         super().__init__()
+        self.__mutex : QMutex = QMutex()
         self.__aircraft_id = self.__obtain_id()
-        self.__vehicle = AircraftVehicle(self.__aircraft_id, position=position, speed=speed)
+        self.__vehicle = AircraftVehicle(self.__aircraft_id, position=position, speed=speed, initial_roll_angle=initial_roll_angle)
         self.__fcc = AircraftFCC(self.__aircraft_id, initial_target, self.__vehicle)
         self.__initial_position = copy(position)
         self.__initial_speed = copy(speed)
+        self.__initial_roll_angle = initial_roll_angle
     
     @property
     def vehicle(self) -> AircraftVehicle:
         """Returns aircraft vehicle"""
-        return self.__vehicle
+        with QMutexLocker(self.__mutex):
+            return self.__vehicle
     
     @property
     def fcc(self) -> AircraftFCC:
         """Returns aircraft fcc"""
-        return self.__fcc
+        with QMutexLocker(self.__mutex):
+            return self.__fcc
     
     @property
     def initial_position(self) -> QVector3D:
         """Returns initial position"""
-        return self.__initial_position
+        with QMutexLocker(self.__mutex):
+            return self.__initial_position
     
     @property
     def initial_speed(self) -> QVector3D:
         """Returns initial speed"""
-        return self.__initial_speed
+        with QMutexLocker(self.__mutex):
+            return self.__initial_speed
+        
+    @property
+    def initial_roll_angle(self) -> float:
+        """Returns initial roll angle"""
+        with QMutexLocker(self.__mutex):
+            return self.__initial_roll_angle
 
     def __obtain_id(self) -> int:
         """Gets unique id for the aircraft"""
-        aircraft_id = Aircraft.__current_id
-        Aircraft.__current_id += 1
-        return aircraft_id
-    
+        with QMutexLocker(self.__mutex):
+            aircraft_id = Aircraft.__current_id
+            Aircraft.__current_id += 1
+            return aircraft_id
+    
+    def __reset_current_id(self) -> None:
+        """Resets current id"""
+        with QMutexLocker(self.__mutex):
+            Aircraft.__current_id = 0
+
     def reset(self) -> None:
         """Resets aircraft to initial state"""
+        self.__reset_current_id()
         self.__vehicle.speed = copy(self.initial_speed)
         self.__vehicle.position = copy(self.initial_position)
+        self.__vehicle.roll_angle = copy(self.initial_roll_angle)
+        self.__vehicle.reset_distance_covered()
```

## uav_collision_avoidance/src/aircraft/aircraft_fcc.py

```diff
@@ -2,80 +2,187 @@
 
 import logging
 from copy import copy
 from typing import List
 from collections import deque
 from math import dist, atan2, degrees
 
-from PySide6.QtCore import QObject
+from PySide6.QtCore import QObject, QMutex, QMutexLocker
 from PySide6.QtGui import QVector3D
 
 from .aircraft_vehicle import AircraftVehicle
 
 class AircraftFCC(QObject):
     """Aircraft Flight Control Computer"""
-
+    
     def __init__(self, aircraft_id : int, initial_target : QVector3D | None, aircraft : AircraftVehicle) -> None:
         super().__init__()
-        self.aircraft_id = aircraft_id
-        self.aircraft = aircraft
-
-        self.destinations : deque[QVector3D] = deque()
-
+        self.__mutex : QMutex = QMutex()
+        self.__aircraft_id = aircraft_id
+        self.__aircraft = aircraft
+        self.__destinations : deque[QVector3D] = deque()
+        self.__destinations_history : List[QVector3D] = []
+        self.__visited : List[QVector3D] = []
+        self.__autopilot : bool = True
+        self.__ignore_destinations : bool = False
+        self.__initial_target : QVector3D | None = initial_target
+        self.__target_yaw_angle : float = 0.0
         if initial_target is None:
-            self.target_yaw_angle : float = aircraft.yaw_angle
+            self.__target_yaw_angle = aircraft.yaw_angle
+            self.__autopilot = False
         else:
-            self.target_yaw_angle : float = self.find_best_yaw_angle(aircraft.position, initial_target)
+            self.__target_yaw_angle = self.find_best_yaw_angle(aircraft.position, initial_target)
             self.add_first_destination(initial_target)
-
-        self.initial_course : float = copy(self.target_yaw_angle)
-        self.target_roll_angle : float = 0.0
-        self.target_pitch_angle : float = 0.0
+        self.__target_roll_angle : float = 0.0
+        self.__target_pitch_angle : float = 0.0
         self.__target_speed : float = self.aircraft.absolute_speed
         self.__is_turning_right : bool = False
         self.__is_turning_left : bool = False
-        self.ignore_destinations : bool = False
-
         self.__safe_zone_occupied : bool = False
         self.__evade_maneuver : bool = False
-        self.vector_sharing_resolution : QVector3D | None = None
+        self.__vector_sharing_resolution : QVector3D | None = None
+
+    @property
+    def aircraft_id(self) -> int:
+        """Returns aircraft id"""
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_id
+    
+    @property
+    def aircraft(self) -> AircraftVehicle:
+        """Returns aircraft vehicle"""
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft
+    
+    @property
+    def destinations(self) -> deque[QVector3D]:
+        """Returns destinations list"""
+        with QMutexLocker(self.__mutex):
+            return self.__destinations
+    
+    @property
+    def destinations_history(self) -> List[QVector3D]:
+        """Returns destinations history list"""
+        with QMutexLocker(self.__mutex):
+            return self.__destinations_history
+    
+    @property
+    def visited(self) -> List[QVector3D]:
+        """Returns visited list"""
+        with QMutexLocker(self.__mutex):
+            return self.__visited
+    
+    @property
+    def autopilot(self) -> bool:
+        """Returns autopilot state"""
+        with QMutexLocker(self.__mutex):
+            return self.__autopilot
+    
+    def toggle_autopilot(self) -> None:
+        """Toggles autopilot state"""
+        with QMutexLocker(self.__mutex):
+            self.__autopilot = not self.__autopilot
 
-        self.destinations_history : List[QVector3D] = []
-        self.visited : List[QVector3D] = []
+    @property
+    def ignore_destinations(self) -> bool:
+        """Returns ignore destinations state"""
+        with QMutexLocker(self.__mutex):
+            return self.__ignore_destinations
+    
+    @ignore_destinations.setter
+    def ignore_destinations(self, value : bool) -> None:
+        """Sets ignore destinations state"""
+        with QMutexLocker(self.__mutex):
+            self.__ignore_destinations = value
+
+    @property
+    def initial_target(self) -> QVector3D | None:
+        """Returns initial target"""
+        with QMutexLocker(self.__mutex):
+            return self.__initial_target
+
+    @property
+    def target_yaw_angle(self) -> float:
+        """Returns target yaw angle"""
+        with QMutexLocker(self.__mutex):
+            return self.__target_yaw_angle
+    
+    @target_yaw_angle.setter
+    def target_yaw_angle(self, angle : float) -> None:
+        """Sets target yaw angle"""
+        with QMutexLocker(self.__mutex):
+            self.__target_yaw_angle = angle
+
+    @property
+    def target_roll_angle(self) -> float:
+        """Returns target roll angle"""
+        with QMutexLocker(self.__mutex):
+            return self.__target_roll_angle
+    
+    @target_roll_angle.setter
+    def target_roll_angle(self, angle : float) -> None:
+        """Sets target roll angle"""
+        with QMutexLocker(self.__mutex):
+            self.__target_roll_angle = angle
+
+    @property
+    def target_pitch_angle(self) -> float:
+        """Returns target pitch angle"""
+        with QMutexLocker(self.__mutex):
+            return self.__target_pitch_angle
+    
+    @target_pitch_angle.setter
+    def target_pitch_angle(self, angle : float) -> None:
+        """Sets target pitch angle"""
+        with QMutexLocker(self.__mutex):
+            self.__target_pitch_angle = angle
     
     @property
     def target_speed(self) -> float:
         """Returns target speed"""
-        return self.__target_speed
+        with QMutexLocker(self.__mutex):
+            return self.__target_speed
     
     @target_speed.setter
     def target_speed(self, speed : float) -> None:
         """Sets target speed"""
         if speed > 0:
-            self.__target_speed = speed
+            with QMutexLocker(self.__mutex):
+                self.__target_speed = speed
+
+    def accelerate(self, acceleration : float) -> None:
+        """Accelerates aircraft's targeted speed"""
+        with QMutexLocker(self.__mutex):
+            if self.__target_speed + acceleration <= 0:
+                return
+            self.__target_speed += acceleration
     
     @property
     def is_turning_right(self) -> bool:
         """Returns turning right state"""
-        return self.__is_turning_right
+        with QMutexLocker(self.__mutex):
+            return self.__is_turning_right
     
     @is_turning_right.setter
     def is_turning_right(self, value : bool) -> None:
         """Sets turning right state"""
-        self.__is_turning_right = value
+        with QMutexLocker(self.__mutex):
+            self.__is_turning_right = value
 
     @property
     def is_turning_left(self) -> bool:
         """Returns turning left state"""
-        return self.__is_turning_left
+        with QMutexLocker(self.__mutex):
+            return self.__is_turning_left
     
     @is_turning_left.setter
     def is_turning_left(self, value : bool) -> None:
         """Sets turning left state"""
-        self.__is_turning_left = value
+        with QMutexLocker(self.__mutex):
+            self.__is_turning_left = value
 
     def check_new_destination(self, destination : QVector3D, first : bool) -> QVector3D | None:
         """Checks if the given destination is already in the destinations list"""
         if not all(isinstance(coord, (int, float)) for coord in (destination.x(), destination.y(), destination.z())):
             raise TypeError("Destination coordinates must be int or float.")
         if len(self.destinations) > 0 and first:
             if dist(destination.toTuple(), self.destinations[0].toTuple()) < 1.0:
@@ -91,37 +198,44 @@
             if destination.z() < 0:
                 print("Attempted to set destination below ground")
                 logging.warning(f"Attempted to set destination below ground: {destination}")
             else:
                 print("Attempted to set destination too low")
                 logging.warning(f"Attempted to set destination too low: {destination}")
             destination = QVector3D(destination.x(), destination.y(), 500)
+        elif destination.z() > 10000:
+            print("Attempted to set destination too high")
+            logging.warning(f"Attempted to set destination too high: {destination}")
+            destination = QVector3D(destination.x(), destination.y(), 10000)
         return destination
 
     def add_last_destination(self, destination : QVector3D) -> None:
         """Appends the given location (QVector3D) to the end of the destinations list."""
         destination : QVector3D = self.check_new_destination(destination, False)
         if destination is not None:
-            self.destinations.append(destination)
-            logging.info("Aircraft %s added new last destination: %s", self.aircraft.aircraft_id, destination.toTuple())
+            with QMutexLocker(self.__mutex):
+                self.__destinations.append(destination)
+                logging.info("Aircraft %s added new last destination: %s", self.__aircraft.aircraft_id, destination.toTuple())
 
     def add_first_destination(self, destination : QVector3D) -> None:
         """Pushes given location to the top of destinations list"""
         destination : QVector3D = self.check_new_destination(destination, True)
         if destination is not None:
-            self.destinations.appendleft(destination)
-            logging.info("Aircraft %s added new first destination: %s", self.aircraft.aircraft_id, destination.toTuple())
+            with QMutexLocker(self.__mutex):
+                self.__destinations.appendleft(destination)
+                logging.info("Aircraft %s added new first destination: %s", self.__aircraft.aircraft_id, destination.toTuple())
 
     @property
     def destination(self) -> QVector3D | None:
         """Returns current destination"""
-        if len(self.destinations) > 0:
-            return self.destinations[0]
-        else:
-            return None
+        with QMutexLocker(self.__mutex):
+            if len(self.__destinations) > 0:
+                return self.__destinations[0]
+            else:
+                return None
 
     def append_visited(self) -> None:
         """Appends current location to visited list"""
         self.visited.append(copy(self.aircraft.position))
 
     def normalize_angle(self, angle : float) -> float:
         """Normalizes -180-180 angle into 360 domain"""
@@ -130,33 +244,48 @@
 
     def format_yaw_angle(self, angle : float) -> float:
         """Formats angle into -180-180 domain"""
         angle = self.normalize_angle(angle)
         return angle if angle <= 180 else -180 + (angle - 180)
     
     @property
+    def vector_sharing_resolution(self) -> QVector3D | None:
+        """Returns vector sharing resolution"""
+        with QMutexLocker(self.__mutex):
+            return self.__vector_sharing_resolution
+    
+    @vector_sharing_resolution.setter
+    def vector_sharing_resolution(self, value : QVector3D | None) -> None:
+        """Sets vector sharing resolution"""
+        with QMutexLocker(self.__mutex):
+            self.__vector_sharing_resolution = value
+
+    @property
     def safe_zone_occupied(self) -> bool:
         """Returns safe zone occupied state"""
-        return self.__safe_zone_occupied
+        with QMutexLocker(self.__mutex):
+            return self.__safe_zone_occupied
     
     @safe_zone_occupied.setter
     def safe_zone_occupied(self, value : bool) -> None:
         """Sets safe zone occupied state"""
-        if self.__safe_zone_occupied and value:
-            print("Safe zone already occupied")
-            logging.warning("Safe zone already occupied")
-        if not self.__safe_zone_occupied and not value:
-            print("Safe zone already free")
-            logging.warning("Safe zone already free")
-        self.__safe_zone_occupied = value
+        with QMutexLocker(self.__mutex):
+            if self.__safe_zone_occupied and value:
+                print("Safe zone already occupied")
+                logging.warning("Safe zone already occupied")
+            if not self.__safe_zone_occupied and not value:
+                print("Safe zone already free")
+                logging.warning("Safe zone already free")
+            self.__safe_zone_occupied = value
     
     @property
     def evade_maneuver(self) -> bool:
         """Returns evade maneuver state"""
-        return self.__evade_maneuver
+        with QMutexLocker(self.__mutex):
+            return self.__evade_maneuver
 
     def apply_evade_maneuver(self, opponent_speed : QVector3D, miss_distance_vector : QVector3D, unresolved_region : float, time_to_closest_approach : float) -> None:
         """Applies evade maneuver"""
         print(str(self.aircraft.aircraft_id) + ": opponent speed: " + "{:.2f}".format(opponent_speed.x()) + " " + "{:.2f}".format(opponent_speed.y()) + " " + "{:.2f}".format(opponent_speed.z()))
         print(str(self.aircraft.aircraft_id) + ": miss distance vector: " + "{:.2f}".format(miss_distance_vector.x()) + " " + "{:.2f}".format(miss_distance_vector.y()) + " " + "{:.2f}".format(miss_distance_vector.z()))
         print(str(self.aircraft.aircraft_id) + ": unresolved region: " + "{:.2f}".format(unresolved_region))
         print(str(self.aircraft.aircraft_id) + ": time to closest approach: " + "{:.2f}".format(time_to_closest_approach))
@@ -195,18 +324,19 @@
                 target_avoiding = self.aircraft.position + (unit_vector * modified_speed_vector.length())
             
             print("Set target avoiding collision: " + "{:.2f}".format(target_avoiding.x()) + " " + "{:.2f}".format(target_avoiding.y()) + " " + "{:.2f}".format(target_avoiding.z()))
             self.add_first_destination(target_avoiding)
 
     def reset_evade_maneuver(self) -> None:
         """Resets evade maneuver"""
-        if self.__evade_maneuver:
-            logging.info("Aircraft %s reset evade maneuver", self.aircraft.aircraft_id)
-            self.__evade_maneuver = False
-            #self.vector_sharing_resolution = None
+        with QMutexLocker(self.__mutex):
+            if self.__evade_maneuver:
+                logging.info("Aircraft %s reset evade maneuver", self.aircraft.aircraft_id)
+                self.__evade_maneuver = False
+                #self.vector_sharing_resolution = None
 
     def find_best_roll_angle(self, current_yaw_angle: float, target_yaw_angle: float) -> float:
         """Finds best roll angle for the targeted yaw angle"""
         difference = (target_yaw_angle - current_yaw_angle + 180) % 360 - 180
         if abs(difference) < 0.001:
             self.is_turning_right = False
             self.is_turning_left = False
@@ -249,15 +379,15 @@
         target_pitch_angle : float = degrees(atan2(
             destination.z() - position.z(),
             dist(position.toTuple(), destination.toTuple())))
         return target_pitch_angle
 
     def update_target_yaw_pitch_angles(self) -> None:
         """Updates current yaw angle"""
-        if self.destinations and not self.ignore_destinations:
+        if self.destinations and self.autopilot and not self.ignore_destinations:
             destination = self.destinations[0]
             distance = dist(self.aircraft.position.toTuple(), destination.toTuple())
             if distance < self.aircraft.size / 2:
                 self.destinations_history.append(self.destinations.popleft())
                 if self.destinations:
                     destination = self.destinations[0]
                     logging.info("Aircraft %s visited destination and took next one", self.aircraft.aircraft_id)
@@ -298,11 +428,47 @@
         self.update_target_roll_angle()      
 
     def reset(self) -> None:
         """Resets aircraft flight control computer"""
         self.destinations.clear()
         self.destinations_history.clear()
         self.visited.clear()
-        self.target_yaw_angle = self.initial_course
-        self.target_roll_angle = 0.0
-        self.target_pitch_angle = 0.0
+        if self.initial_target is not None:
+            self.add_first_destination(self.initial_target)
+        self.__target_yaw_angle = 0.0
+        self.__target_roll_angle = 0.0
+        self.__target_pitch_angle = 0.0
         self.__evade_maneuver = False
+        self.__vector_sharing_resolution = None
+        self.__safe_zone_occupied = False
+        self.__autopilot = True
+        self.__ignore_destinations = False
+        self.__is_turning_right = False
+        self.__is_turning_left = False
+
+    def __str__(self) -> str:
+        return f"AircraftFCC: {self.aircraft_id}"
+    
+    def __repr__(self) -> str:
+        return f"AircraftFCC: {self.aircraft_id}"
+    
+    def __del__(self) -> None:
+        with QMutexLocker(self.__mutex):
+            del self.__aircraft_id
+            del self.__aircraft
+            del self.__destinations
+            del self.__destinations_history
+            del self.__visited
+            del self.__autopilot
+            del self.__ignore_destinations
+            del self.__initial_target
+            del self.__target_yaw_angle
+            del self.__target_roll_angle
+            del self.__target_pitch_angle
+            del self.__target_speed
+            del self.__is_turning_right
+            del self.__is_turning_left
+            del self.__safe_zone_occupied
+            del self.__evade_maneuver
+            del self.__vector_sharing_resolution
+            del self.__mutex
+            del self
```

## uav_collision_avoidance/src/aircraft/aircraft_vehicle.py

```diff
@@ -8,79 +8,100 @@
 class AircraftVehicle(QObject):
     """Aircraft physical UAV"""
 
     roll_dynamic_delay : float = 1000 # ms
     pitch_dynamic_delay : float = 2000 # ms
     max_acceleration : float = 2.0 # m/s^2
 
-    def __init__(self, aircraft_id : int, position : QVector3D, speed : QVector3D) -> None:
+    def __init__(self, aircraft_id : int, position : QVector3D, speed : QVector3D, initial_roll_angle : float) -> None:
         super().__init__()
         self.__mutex : QMutex = QMutex()
         
         self.__aircraft_id = aircraft_id
         self.__position = position
         if self.__position.z() < 0:
             self.__position.setZ(0)
         self.__speed = speed
 
         self.__size : float = 20.0
-        self.__roll_angle = 0.0 # bank angle
-        self.initial_roll_angle = self.__roll_angle
+        self.__roll_angle = initial_roll_angle
+        self.__initial_roll_angle = self.__roll_angle
         self.__distance_covered : float = 0.0
 
     @property
     def aircraft_id(self) -> int:
         """Returns aircraft id"""
-        return self.__aircraft_id
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_id
     
     @property
     def position(self) -> QVector3D:
         """Returns position"""
-        return self.__position
+        with QMutexLocker(self.__mutex):
+            return self.__position
     
     @position.setter
     def position(self, position : QVector3D) -> None:
         """Sets position"""
         del self.__position
-        self.__position = position
+        with QMutexLocker(self.__mutex):
+            self.__position = position
     
     @property
     def speed(self) -> QVector3D:
         """Returns speed"""
-        return self.__speed
+        with QMutexLocker(self.__mutex):
+            return self.__speed
     
     @speed.setter
     def speed(self, speed : QVector3D) -> None:
         """Sets speed"""
-        self.__speed = speed
+        with QMutexLocker(self.__mutex):
+            self.__speed = speed
     
     @property
     def size(self) -> float:
         """Returns size"""
-        return self.__size
+        with QMutexLocker(self.__mutex):
+            return self.__size
     
     @property
     def roll_angle(self) -> float:
         """Returns roll angle"""
-        return self.__roll_angle
+        with QMutexLocker(self.__mutex):
+            return self.__roll_angle
 
     @roll_angle.setter
     def roll_angle(self, roll_angle_delta : float) -> None:
         """Adds roll angle delta"""
-        self.__roll_angle += roll_angle_delta
+        with QMutexLocker(self.__mutex):
+            self.__roll_angle += roll_angle_delta
+
+    @property
+    def initial_roll_angle(self) -> float:
+        """Returns initial roll angle"""
+        with QMutexLocker(self.__mutex):
+            return self.__initial_roll_angle
     
     @property
     def distance_covered(self) -> float:
         """Returns covered distance"""
-        return self.__distance_covered
+        with QMutexLocker(self.__mutex):
+            return self.__distance_covered
 
     @distance_covered.setter
     def distance_covered(self, distance_covered_delta : float) -> None:
         """Appends delta to distance covered"""
-        self.__distance_covered += distance_covered_delta
+        with QMutexLocker(self.__mutex):
+            self.__distance_covered += distance_covered_delta
+
+    def reset_distance_covered(self) -> None:
+        """Resets distance covered"""
+        with QMutexLocker(self.__mutex):
+            self.__distance_covered = 0.0
     
     def move(self, dx : float, dy : float, dz : float = 0.0) -> None:
         """Applies position deltas for the vehicle"""
         with QMutexLocker(self.__mutex):
             self.__position.setX(self.__position.x() + dx)
             self.__position.setY(self.__position.y() + dy)
             self.__position.setZ(self.__position.z() + dz)
@@ -124,7 +145,59 @@
             return degrees(atan2(speed.x(), -speed.y()))
 
     @property
     def pitch_angle(self) -> float:
         """Returns pitch angle"""
         with QMutexLocker(self.__mutex):
             return degrees(atan2(self.__speed.z(), sqrt(self.__speed.x() ** 2 + self.__speed.y() ** 2)))
+
+    def __str__(self) -> str:
+        with QMutexLocker(self.__mutex):
+            return f"Vehicle {self.__aircraft_id} at {self.__position} with speed {self.__speed} and roll angle {self.__roll_angle} degrees"
+        
+    def __repr__(self) -> str:
+        with QMutexLocker(self.__mutex):
+            return f"Vehicle {self.__aircraft_id} at {self.__position} with speed {self.__speed} and roll angle {self.__roll_angle} degrees"
+        
+    def __eq__(self, other) -> bool:
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_id == other.__aircraft_id
+        
+    def __ne__(self, other) -> bool:
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_id != other.__aircraft_id
+        
+    def __lt__(self, other) -> bool:
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_id < other.__aircraft_id
+        
+    def __le__(self, other) -> bool:
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_id <= other.__aircraft_id
+        
+    def __gt__(self, other) -> bool:
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_id > other.__aircraft_id
+        
+    def __ge__(self, other) -> bool:
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_id >= other.__aircraft_id
+        
+    def __copy__(self):
+        with QMutexLocker(self.__mutex):
+            return AircraftVehicle(self.__aircraft_id, self.__position, self.__speed, self.__initial_roll_angle)
+
+    def __deepcopy__(self, memo):
+        with QMutexLocker(self.__mutex):
+            return AircraftVehicle(self.__aircraft_id, self.__position, self.__speed, self.__initial_roll_angle)
+        
+    def __del__(self):
+        with QMutexLocker(self.__mutex):
+            del self.__position
+            del self.__speed
+            del self.__roll_angle
+            del self.__initial_roll_angle
+            del self.__distance_covered
+            del self.__size
+            del self.__aircraft_id
+            del self.__mutex
+            del self
```

## uav_collision_avoidance/src/simulation/simulation.py

```diff
@@ -19,148 +19,150 @@
 from ..simulation.simulation_widget import SimulationWidget
 from ..simulation.simulation_adsb import SimulationADSB
 from ..simulation.simulation_fps import SimulationFPS
 
 class Simulation(QMainWindow):
     """Main simulation App"""
 
-    def __init__(self, aircrafts : List[Aircraft] | None = None, simulation_time : int = 100_000) -> None:
+    def __init__(self, headless : bool = False, tests : bool = False, simulation_time : int = 10_000_000) -> None: # 10_000_000 ms = 10_000 s = 2h 46m 40s
         super().__init__()
         SimulationSettings().__init__()
-        if aircrafts is None:
-            test_case : int = 0
-            if test_case == 0:
-                self.aircrafts : List[Aircraft] = [
-                    Aircraft( # detection test
-                        position = QVector3D(-800, 4000, 1000),
-                        speed = QVector3D(60, -60, 0),
-                        initial_target = QVector3D(1_000_100, -1_001_000, 10000)),
-                    Aircraft(
-                        position = QVector3D(4000, 6000, 1000),
-                        speed = QVector3D(0, -85, 0),
-                        initial_target = QVector3D(900, -1_001_300, 10000)),
-                ]
-            elif test_case == 1:
-                self.aircrafts : List[Aircraft] = [
-                    Aircraft( # almost head on
-                        position = QVector3D(-3000, 500, 1000),
-                        speed = QVector3D(70, 0.1, 0)),
-                    Aircraft(
-                        position = QVector3D(5000, 500, 1000),
-                        speed = QVector3D(-50, 0, 0)),
-                ]
-            elif test_case == 2:
-                self.aircrafts : List[Aircraft] = [
-                    Aircraft( # avoidance test
-                        position = QVector3D(0, 0, 1000),
-                        speed = QVector3D(30, -30, 0),
-                        initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
-                    Aircraft(
-                        position = QVector3D(0, -100_000, 1000),
-                        speed = QVector3D(30, 29, 0),
-                        initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
-                ]
-            elif test_case == 3:
-                self.aircrafts : List[Aircraft] = [
-                    Aircraft( # avoidance test fast
-                        position = QVector3D(0, 0, 1000),
-                        speed = QVector3D(300, -300, 0),
-                        initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
-                    Aircraft(
-                        position = QVector3D(0, -100_000, 1000),
-                        speed = QVector3D(300, 290, 0),
-                        initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
-                ]
-        else:
-            self.aircrafts = aircrafts
-        self.simulation_time : int = simulation_time
-        self.state : SimulationState | None = None
-
-    def run_realtime(self) -> None:
-        """Executes realtime simulation"""
+        self.__headless : bool = headless
+        self.__tests : bool = tests
+        self.__simulation_time : int = simulation_time
+        self.__aircrafts : List[Aircraft] | None = None
+        self.__state : SimulationState | None = None
+        self.run()
+
+    @property
+    def headless(self) -> bool:
+        """Returns headless flag"""
+        return self.__headless
+    
+    @property
+    def tests(self) -> bool:
+        """Returns tests flag"""
+        return self.__tests
+    
+    @property
+    def simulation_time(self) -> int:
+        """Returns simulation time"""
+        return self.__simulation_time
+    
+    @property
+    def aircrafts(self) -> List[Aircraft]:
+        """Returns aircrafts list"""
+        return self.__aircrafts
+    
+    @property
+    def state(self) -> SimulationState:
+        """Returns simulation state"""
+        return self.__state
+    
+    @state.setter
+    def state(self, state : SimulationState) -> None:
+        """Sets simulation state"""
+        self.__state = state
+    
+    def run(self) -> None:
+        """Executes simulation"""
         if self.state is not None:
             print("Another instance already running")
             return
+        if self.headless:
+            if self.tests:
+                self.run_tests()
+            else:
+                self.run_headless()
+        else:
+            self.run_gui()
+
+    def run_gui(self) -> None:
+        """Executes realtime simulation"""
+        if self.aircrafts is None or self.aircrafts == []:
+            self.setup_debug_aircrafts()
         logging.info("Starting realtime simulation")
         self.state = SimulationState(SimulationSettings(), is_realtime = True)
-
         self.simulation_physics = SimulationPhysics(self, self.aircrafts, self.state)
-        self.simulation_physics.start(priority = QThread.Priority.TimeCriticalPriority)
-
         self.simulation_adsb = SimulationADSB(self, self.aircrafts, self.state)
-        self.simulation_adsb.start(priority = QThread.Priority.NormalPriority)
-
         self.simulation_fps = SimulationFPS(self, self.state)
-        self.simulation_fps.start(priority = QThread.Priority.NormalPriority)
-
         self.simulation_widget = SimulationWidget(self.aircrafts, self.simulation_fps, self.state)
-        self.simulation_widget.show()
-
         self.simulation_render = SimulationRender(self, self.simulation_widget, self.state)
+        self.simulation_physics.start(priority = QThread.Priority.TimeCriticalPriority)
+        self.simulation_adsb.start(priority = QThread.Priority.NormalPriority)
+        self.simulation_fps.start(priority = QThread.Priority.NormalPriority)
+        self.simulation_widget.show()
         self.simulation_render.start(priority = QThread.Priority.NormalPriority)
-
-        self.simulation_widget.stop_signal.connect(self.stop_simulation)
+        self.simulation_widget.stop_signal.connect(self.stop)
     
-    def run_prerender(self) -> None:
-        """Executes prerender simulation"""
-        if self.state is not None:
-            print("Another instance already running")
-            return
-        logging.info("Starting prerendered simulation")
-        self.state = SimulationState(SimulationSettings(), is_realtime = False)
+    def run_headless(self, aircrafts : List[Aircraft] | None = None, avoid_collisions : bool = False) -> None:
+        """Executes simulation without GUI"""
+        logging.info("Starting headless simulation")
+        if aircrafts is None or aircrafts == []:
+            self.setup_debug_aircrafts()
+        else:
+            self.setup_aircrafts(aircrafts)
+        self.state = SimulationState(SimulationSettings(), is_realtime = False, avoid_collisions = avoid_collisions)
         self.simulation_physics = SimulationPhysics(self, self.aircrafts, self.state)
         self.simulation_adsb = SimulationADSB(self, self.aircrafts, self.state)
         time_step : int = int(self.state.simulation_threshold)
         adsb_step : int = int(self.state.adsb_threshold)
         partial_time_counter : int = adsb_step
-        for time in range(0, self.simulation_time, time_step):
+        for time in range(0, int(self.simulation_time / self.state.simulation_threshold), time_step):
             print(time)
             self.simulation_physics.cycle(time_step)
             if partial_time_counter >= adsb_step:
                 self.simulation_adsb.cycle()
                 partial_time_counter = 0
             partial_time_counter += time_step
             if self.state.collision:
                 break
-        self.stop_simulation()
+        self.stop()
     
     def run_tests(self, test_number : int = 10) -> None:
         """Runs simulation tests"""
         if test_number < 1:
             test_number = 10
         logging.info("Running simulation tests")
         start_timestamp = QTime.currentTime()
+        #list_of_aircrafts : List[List[Aircraft]] = self.generate_test_aircrafts(test_number) # todo
         for i in range(0, test_number, 1):
-            logging.info("Test %d", i)
-            self.run_prerender()
+            logging.info("Test %d - no collision avoidance", i)
+            # self.run_headless(aircrafts = list_of_aircrafts[i], avoid_collisions = False)
+            self.run_headless()
+            # self.export_results()
+            self.state = None
+
+            logging.info("Test %d - collision avoidance", i)
+            # self.run_headless(aircrafts = list_of_aircrafts[i], avoid_collisions = True)
+            self.run_headless()
+            # self.export_results()
             self.state = None
         real_time : float = start_timestamp.msecsTo(QTime.currentTime()) / 1000
         print("Total time elapsed: " + "{:.2f}".format(real_time) + "s")
         logging.info("Total time elapsed: %ss", "{:.2f}".format(real_time))
     
-    def stop_simulation(self) -> None:
+    def stop(self) -> None:
         """Stops simulation"""
-        if self.state.is_realtime:
-            self.stop_realtime_simulation()
+        if self.headless:
+            self.stop_headless_simulation()
         else:
-            self.stop_prerender_simulation()
+            self.stop_realtime_simulation()
         self.state.reset()
         self.state.is_running = False
 
     def stop_realtime_simulation(self) -> None:
         """Finishes all active realtime simulation threads"""
         if not self.state.is_running:
             return
         logging.info("Stopping realtime simulation")
-
         self.simulation_physics.requestInterruption()
         self.simulation_adsb.requestInterruption()
         self.simulation_render.requestInterruption()
         self.simulation_fps.requestInterruption()
-
         self.simulation_physics.quit()
         self.simulation_physics.wait()
 
         if self.state.is_paused:
             self.state.append_paused_time()
         simulated_time : float = self.state.physics_cycles / (1000 / self.state.simulation_threshold)
         real_time_pauses : float = self.simulation_physics.global_start_timestamp.msecsTo(self.simulation_physics.global_stop_timestamp) / 1000
@@ -171,30 +173,92 @@
         else:
             print("Time elapsed: " + "{:.2f}".format(real_time) + "s (" + "{:.2f}".format(real_time_pauses) + "s with pauses)")
         if real_time != 0:
             print("Time efficiency: " + "{:.2f}".format(simulated_time / real_time * 100) + "%")
             logging.info("Calculated time efficiency: " + "{:.2f}".format(simulated_time / real_time * 100) + "%")
 
         self.export_visited_locations()
-
         self.simulation_adsb.quit()
         self.simulation_adsb.wait()
         self.simulation_render.quit()
         self.simulation_render.wait()
         self.simulation_fps.quit()
         self.simulation_fps.wait()
     
-    def stop_prerender_simulation(self) -> None:
-        """Finishes all active prerender simulation threads"""
+    def stop_headless_simulation(self) -> None:
+        """Finishes headless simulation"""
         if not self.state.is_running:
+            print("No simulation running")
             return
-        logging.info("Stopping prerendered simulation")
+        logging.info("Stopping headless simulation")
         self.simulation_physics.reset_aircrafts()
         self.state.reset()
-    
+
+    def add_aircraft(self, aircraft : Aircraft) -> None:
+        """Adds aircraft to simulation"""
+        if self.aircrafts is None:
+            self.__aircrafts = []
+        self.aircrafts.append(aircraft)
+
+    def remove_aircraft(self, aircraft : Aircraft) -> None:
+        """Removes aircraft from simulation"""
+        if self.aircrafts is not None:
+            self.aircrafts.remove(aircraft)
+
+    def setup_aircrafts(self, aircrafts : List[Aircraft]) -> None:
+        """Sets up aircrafts list"""
+        self.__aircrafts = aircrafts
+
+    def setup_debug_aircrafts(self) -> None:
+        """Sets up debug aircrafts list"""
+        test_case : int = 3
+        if test_case == 0:
+            aircrafts : List[Aircraft] = [
+                Aircraft( # detection test
+                    position = QVector3D(-800, 4000, 1000),
+                    speed = QVector3D(60, -60, 0),
+                    initial_target = QVector3D(51_900, -50_000, 10000)),
+                Aircraft(
+                    position = QVector3D(4000, 6000, 1000),
+                    speed = QVector3D(0, -85, 0),
+                    initial_target = QVector3D(900, -1_001_300, 1000)),
+            ]
+        elif test_case == 1:
+            aircrafts : List[Aircraft] = [
+                Aircraft( # almost head on
+                    position = QVector3D(-3000, 500, 1000),
+                    speed = QVector3D(70, 0.1, 0)),
+                Aircraft(
+                    position = QVector3D(5000, 500, 1000),
+                    speed = QVector3D(-50, 0, 0)),
+            ]
+        elif test_case == 2:
+            aircrafts : List[Aircraft] = [
+                Aircraft( # avoidance test
+                    position = QVector3D(0, 0, 1000),
+                    speed = QVector3D(30, -30, 0),
+                    initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
+                Aircraft(
+                    position = QVector3D(0, -100_000, 1000),
+                    speed = QVector3D(30, 29, 0),
+                    initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
+            ]
+        elif test_case == 3:
+            aircrafts : List[Aircraft] = [
+                Aircraft( # avoidance test fast
+                    position = QVector3D(0, 0, 1000),
+                    speed = QVector3D(300, -300, 0),
+                    initial_target = QVector3D(75000, -75000, 1000)), # 75 km, -75 km
+                Aircraft(
+                    position = QVector3D(0, -100_000, 1000),
+                    speed = QVector3D(300, 290, 0),
+                    initial_target = QVector3D(75000, -27500, 1000)), # 75 km, -27.5 km
+            ]
+        self.setup_aircrafts(aircrafts)
+
     def export_visited_locations(self) -> None:
         """Exports aircrafts visited location lists"""
         export_time = datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
         aircraft_fccs : List[AircraftFCC] = [aircraft.fcc for aircraft in self.aircrafts]
         for aircraft in aircraft_fccs:
             try:
                 Path("logs/visited").mkdir(parents=True, exist_ok=True)
@@ -204,10 +268,10 @@
             writer = csv.writer(file)
             writer.writerow(["x","y","z"])
             for position in aircraft.visited:
                 writer.writerow([("{:.2f}".format(position.x())),("{:.2f}".format(position.y())),("{:.2f}".format(position.z()))])
     
     def closeEvent(self, event: QCloseEvent) -> None:
         """Qt method performed on the main window close event"""
-        self.stop_simulation()
+        self.stop()
         event.accept()
         return super().closeEvent(event)
```

## uav_collision_avoidance/src/simulation/simulation_adsb.py

```diff
@@ -1,11 +1,12 @@
 """Simulation ADS-B system simulation thread module"""
 
 import logging
 from typing import List
+from math import sqrt
 
 from PySide6.QtCore import QThread, QTime
 from PySide6.QtGui import QVector3D
 from PySide6.QtWidgets import QMainWindow
 
 from ..aircraft.aircraft import Aircraft
 from ..aircraft.aircraft_vehicle import AircraftVehicle
@@ -13,35 +14,67 @@
 from .simulation_state import SimulationState
 
 class SimulationADSB(QThread):
     """Thread running ADS-B system for collision detection and avoidance"""
 
     def __init__(self, parent : QMainWindow, aircrafts : List[Aircraft], simulation_state : SimulationState) -> None:
         super(SimulationADSB, self).__init__(parent)
-        self.aircrafts = aircrafts
-        self.aircraft_vehicles : List[AircraftVehicle] = [aircraft.vehicle for aircraft in self.aircrafts]
-        self.aircraft_fccs : List[AircraftFCC] = [aircraft.fcc for aircraft in self.aircrafts]
-        self.simulation_state = simulation_state
-        self.adsb_cycles : int = 0
+        self.__aircrafts = aircrafts
+        self.__aircraft_vehicles : List[AircraftVehicle] = [aircraft.vehicle for aircraft in self.aircrafts]
+        self.__aircraft_fccs : List[AircraftFCC] = [aircraft.fcc for aircraft in self.aircrafts]
+        self.__simulation_state = simulation_state
+        self.__adsb_cycles : int = 0
         
+    @property
+    def aircrafts(self) -> List[Aircraft]:
+        """Returns aircrafts"""
+        return self.__aircrafts
+    
+    @property
+    def aircraft_vehicles(self) -> List[AircraftVehicle]:
+        """Returns aircraft vehicles"""
+        self.__aircraft_vehicles = [aircraft.vehicle for aircraft in self.aircrafts]
+        return self.__aircraft_vehicles
+    
+    @property
+    def aircraft_fccs(self) -> List[AircraftFCC]:
+        """Returns aircraft flight control computers"""
+        self.__aircraft_fccs = [aircraft.fcc for aircraft in self.aircrafts]
+        return self.__aircraft_fccs
+    
+    @property
+    def simulation_state(self) -> SimulationState:
+        """Returns simulation state"""
+        return self.__simulation_state
+    
+    @property
+    def adsb_cycles(self) -> int:
+        """Returns ADS-B cycles count"""
+        return self.__adsb_cycles
+    
+    def count_adsb_cycles(self) -> None:
+        """Increments ADS-B cycle counter"""
+        self.__adsb_cycles += 1
+        self.simulation_state.adsb_cycles = self.adsb_cycles
+
     def run(self) -> None:
         """Runs ADS-B simulation thread with precise timeout"""
         while not self.isInterruptionRequested():
             start_timestamp = QTime.currentTime()
             self.cycle()
             self.msleep(max(0, self.simulation_state.adsb_threshold - start_timestamp.msecsTo(QTime.currentTime())))
         return super().run()
     
     def cycle(self) -> None:
         """Executes ADS-B simulation cycle"""
         aircraft_vehicle_1 : AircraftVehicle = self.aircraft_vehicles[0]
         aircraft_vehicle_2 : AircraftVehicle = self.aircraft_vehicles[1]
 
         if not self.simulation_state.is_paused:
-            self.adsb_cycles += 1
+            self.count_adsb_cycles()
             self.simulation_state.update_adsb_settings()
 
             relative_position = aircraft_vehicle_1.position - aircraft_vehicle_2.position
             speed_difference = aircraft_vehicle_1.speed - aircraft_vehicle_2.speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             print("Time to closest approach: " + "{:.2f}".format(time_to_closest_approach) + "s")
             
@@ -53,15 +86,15 @@
 
                 # console destination reach time
                 if fcc.destination and self.simulation_state.adsb_report:
                     time_to_reaching_destination : float = (QVector3D.dotProduct(fcc.destination - aircraft.position, aircraft.speed) / QVector3D.dotProduct(aircraft.speed, aircraft.speed))
                     print(f"Aircraft {aircraft.aircraft_id} will reach its destination in " + "{:.2f}".format(time_to_reaching_destination) + " (" + "{:.1f}".format(time_to_reaching_destination / 60) + " minutes or " + "{:.1f}".format(time_to_reaching_destination / 3600) + " hours)")
 
                 # console report output
-                if self.simulation_state.adsb_report and aircraft.aircraft_id == 0:
+                if self.simulation_state.adsb_report and aircraft.aircraft_id == 0 and self.simulation_state.is_realtime:
                     self.print_adsb_report(aircraft)
 
                 # safe zone occupancy check
                 if relative_position.length() < self.simulation_state.minimum_separation:
                     if not fcc.safe_zone_occupied:
                         fcc.safe_zone_occupied = True
                         if not self.simulation_state.override_avoid_collisions:
@@ -70,41 +103,38 @@
                 else:
                     if fcc.safe_zone_occupied:
                         fcc.safe_zone_occupied = False
                         self.simulation_state.avoid_collisions = False
                     print("Safe zone free")
                     return
 
-            if not self.simulation_state.avoid_collisions:
-                return
-
             if time_to_closest_approach > 0:
                 # miss distance at closest approach
                 speed_difference_unit = speed_difference.normalized()
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
                     speed_difference_unit,
                     QVector3D.crossProduct(relative_position, speed_difference_unit))
-                print("Miss distance at closest approach: " + "{:.2f}".format(miss_distance_vector.length()) + "m")
+                print("Miss distance at closest approach: " + "{:.2f}".format(miss_distance_vector.length()) + "m (" + "{:.2f}".format(self.aircraft_vehicles[0].size / 2 + self.aircraft_vehicles[1].size / 2) + "m is collision distance)")
 
                 if miss_distance_vector.length() == 0:
                     print("Head-on collision detected")
                     logging.info("Head-on collision detected")
 
                 # resolve confict condition
                 unresolved_region : float = self.simulation_state.minimum_separation - abs(miss_distance_vector.length())
                 if unresolved_region > 0.0:
                     print("Conflict condition detected")
-                    for aircraft in self.aircraft_fccs:
-                        if not aircraft.evade_maneuver:
-                            aircraft.apply_evade_maneuver(
-                                opponent_speed = self.aircraft_vehicles[1 - aircraft.aircraft_id].speed,
-                                miss_distance_vector = miss_distance_vector,
-                                unresolved_region = unresolved_region,
-                                time_to_closest_approach = time_to_closest_approach)
-                    # print("Sum of vector sharing resolutions: ", self.aircraft_fccs[0].vector_sharing_resolution.length() + self.aircraft_fccs[1].vector_sharing_resolution.length() + miss_distance_vector.length())
+                    if self.simulation_state.avoid_collisions:
+                        for aircraft in self.aircraft_fccs:
+                            if not aircraft.evade_maneuver:
+                                aircraft.apply_evade_maneuver(
+                                    opponent_speed = self.aircraft_vehicles[1 - aircraft.aircraft_id].speed,
+                                    miss_distance_vector = miss_distance_vector,
+                                    unresolved_region = unresolved_region,
+                                    time_to_closest_approach = time_to_closest_approach)
                     print("Relative distance: "+ "{:.2f}".format(relative_position.length()) + "m")
 
                 # probable collision
                 collision_distance = aircraft_vehicle_1.size / 2 + aircraft_vehicle_2.size / 2
                 collision_region = collision_distance - miss_distance_vector.length()
                 if collision_region > 0:
                     print("Collision detected")
@@ -128,24 +158,51 @@
             "; target roll angle: " + "{:.2f}".format(fcc.target_roll_angle) +
             "; yaw angle: " + "{:.2f}".format(aircraft.yaw_angle) +
             "; target yaw angle: " + "{:.2f}".format(fcc.target_yaw_angle) +
             "; x: " + "{:.2f}".format(aircraft.position.x()) +
             "; y: " + "{:.2f}".format(aircraft.position.y()) +
             "; z: " + "{:.2f}".format(aircraft.position.z()))
         if fcc.destination is not None:
-            print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
-                "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
-                "; dest x: " + "{:.2f}".format(fcc.destination.x()) +
-                "; dest y: " + "{:.2f}".format(fcc.destination.y()) +
-                "; dest z: " + "{:.2f}".format(fcc.destination.z()) +
-                "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
-                "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
-                "; t: " + str(self.adsb_cycles) +
-                "; phys: " + str(self.simulation_state.physics_cycles))
+            if self.simulation_state.is_realtime:
+                print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
+                    "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
+                    "; dest x: " + "{:.2f}".format(fcc.destination.x()) +
+                    "; dest y: " + "{:.2f}".format(fcc.destination.y()) +
+                    "; dest z: " + "{:.2f}".format(fcc.destination.z()) +
+                    "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
+                    "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
+                    "; t: " + str(self.adsb_cycles) +
+                    "; phys: " + str(self.simulation_state.physics_cycles))
+            else:
+                print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
+                    "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
+                    "; dest x: " + "{:.2f}".format(fcc.destination.x()) +
+                    "; dest y: " + "{:.2f}".format(fcc.destination.y()) +
+                    "; dest z: " + "{:.2f}".format(fcc.destination.z()) +
+                    "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
+                    "; t: " + str(self.adsb_cycles) +
+                    "; phys: " + str(self.simulation_state.physics_cycles))
         else:
-            print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
-                "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
-                "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
-                "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
-                "; t: " + str(self.adsb_cycles) +
-                "; phys: " + str(self.simulation_state.physics_cycles) +
-                "; no destination")
+            if self.simulation_state.is_realtime:
+                print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
+                    "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
+                    "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
+                    "; fps: " + "{:.2f}".format(self.simulation_state.fps) +
+                    "; t: " + str(self.adsb_cycles) +
+                    "; phys: " + str(self.simulation_state.physics_cycles) +
+                    "; no destination")
+            else:
+                print("target pitch angle: " + "{:.2f}".format(fcc.target_pitch_angle) +
+                    "; pitch angle: " + "{:.2f}".format(aircraft.pitch_angle) +
+                    "; distance covered: " + "{:.2f}".format(aircraft.distance_covered) +
+                    "; t: " + str(self.adsb_cycles) +
+                    "; phys: " + str(self.simulation_state.physics_cycles) +
+                    "; no destination")
+        # speed check
+        absolute_speed = sqrt(aircraft.speed.x() ** 2 + aircraft.speed.y() ** 2 + aircraft.speed.z() ** 2)
+        horizontal_speed = sqrt(aircraft.speed.x() ** 2 + aircraft.speed.y() ** 2)
+        vertical_speed = abs(aircraft.speed.z())
+        geometrical_speed = sqrt(horizontal_speed ** 2 + vertical_speed ** 2)
+        print("absolute speed: " + "{:.2f}".format(absolute_speed) +
+            "; horizontal speed: " + "{:.2f}".format(horizontal_speed) +
+            "; vertical speed: " + "{:.2f}".format(vertical_speed) +
+            "; geometrical speed: " + "{:.2f}".format(geometrical_speed))
```

## uav_collision_avoidance/src/simulation/simulation_fps.py

```diff
@@ -8,18 +8,17 @@
 
 class SimulationFPS(QThread):
     """Thread running frames per second counter"""
 
     def __init__(self, parent : QMainWindow, simulation_state : SimulationState) -> None:
         super(SimulationFPS, self).__init__(parent)
         self.__mutex : QMutex = QMutex()
+        self.__simulation_state = simulation_state
         self.__counted_frames : int = 0
-
-        self.simulation_state = simulation_state
-        self.previous_timestamp = QTime.currentTime()
+        self.__previous_timestamp = QTime.currentTime()
         
     def run(self) -> None:
         """Runs rendered simulation frames counter thread with precise 500ms timeout"""
         while not self.isInterruptionRequested():
             start_timestamp = QTime.currentTime()
             elapsed_time : float = self.previous_timestamp.msecsTo(start_timestamp)
             if self.counted_frames() > 0:
@@ -29,24 +28,42 @@
                 self.simulation_state.fps = 0.0
             self.previous_timestamp = QTime.currentTime()
             self.msleep(max(0, 500 - start_timestamp.msecsTo(QTime.currentTime())))
         return super().run()
 
     def count_frame(self) -> None:
         """Increments fps count"""
-        QMutexLocker(self.__mutex)
-        self.__counted_frames += 1
+        with QMutexLocker(self.__mutex):
+            self.__counted_frames += 1
 
     def reset_frames(self) -> None:
         """Resets fps count"""
-        QMutexLocker(self.__mutex)
-        self.__counted_frames = 0
+        with QMutexLocker(self.__mutex):
+            self.__counted_frames = 0
 
     def counted_frames(self) -> int:
         """Returns counted frames"""
-        QMutexLocker(self.__mutex)
-        return self.__counted_frames
+        with QMutexLocker(self.__mutex):
+            return self.__counted_frames
+        
+    @property
+    def simulation_state(self) -> SimulationState:
+        """Returns simulation state"""
+        with QMutexLocker(self.__mutex):
+            return self.__simulation_state
+    
+    @property
+    def previous_timestamp(self) -> QTime:
+        """Returns previous timestamp"""
+        with QMutexLocker(self.__mutex):
+            return self.__previous_timestamp
+    
+    @previous_timestamp.setter
+    def previous_timestamp(self, previous_timestamp : QTime) -> None:
+        """Sets previous timestamp"""
+        with QMutexLocker(self.__mutex):
+            self.__previous_timestamp = previous_timestamp
 
     def closeEvent(self, event: QCloseEvent) -> None:
         """Qt method performed on the main window close event"""
         event.accept()
         return super().closeEvent(event)
```

## uav_collision_avoidance/src/simulation/simulation_physics.py

```diff
@@ -15,39 +15,81 @@
 from .simulation_state import SimulationState
 
 class SimulationPhysics(QThread):
     """Thread running simulation's physics"""
 
     def __init__(self, parent : QMainWindow, aircrafts : List[Aircraft], simulation_state : SimulationState) -> None:
         super(SimulationPhysics, self).__init__(parent)
-        self.aircrafts = aircrafts
-        self.aircraft_vehicles : List[AircraftVehicle] = [aircraft.vehicle for aircraft in self.aircrafts]
-        self.aircraft_fccs : List[AircraftFCC] = [aircraft.fcc for aircraft in self.aircrafts]
-        self.simulation_state = simulation_state
-        self.cycles : int = 0
-        self.global_start_timestamp : QTime | None = None
-        self.global_stop_timestamp : QTime | None = None
+        self.__aircrafts = aircrafts
+        self.__aircraft_vehicles : List[AircraftVehicle] = [aircraft.vehicle for aircraft in self.aircrafts]
+        self.__aircraft_fccs : List[AircraftFCC] = [aircraft.fcc for aircraft in self.aircrafts]
+        self.__simulation_state = simulation_state
+        self.__cycles : int = 0
+        self.__global_start_timestamp : QTime | None = None
+        self.__global_stop_timestamp : QTime | None = None
+
+    @property
+    def aircrafts(self) -> List[Aircraft]:
+        """Returns aircrafts"""
+        return self.__aircrafts
+    
+    @property
+    def aircraft_vehicles(self) -> List[AircraftVehicle]:
+        """Returns aircraft vehicles"""
+        self.__aircraft_vehicles = [aircraft.vehicle for aircraft in self.aircrafts]
+        return self.__aircraft_vehicles
+    
+    @property
+    def aircraft_fccs(self) -> List[AircraftFCC]:
+        """Returns aircraft flight control computers"""
+        self.__aircraft_fccs = [aircraft.fcc for aircraft in self.aircrafts]
+        return self.__aircraft_fccs
+    
+    @property
+    def simulation_state(self) -> SimulationState:
+        """Returns simulation state"""
+        return self.__simulation_state
+    
+    @property
+    def cycles(self) -> int:
+        """Returns physics cycles count"""
+        return self.__cycles
+    
+    def count_cycles(self) -> None:
+        """Increments physics cycle counter"""
+        self.__cycles += 1
+        self.simulation_state.physics_cycles = self.cycles
+    
+    @property
+    def global_start_timestamp(self) -> QTime | None:
+        """Returns global start timestamp"""
+        return self.__global_start_timestamp
+    
+    @property
+    def global_stop_timestamp(self) -> QTime | None:
+        """Returns global stop timestamp"""
+        return self.__global_stop_timestamp
 
     def run(self) -> None:
         """Runs physics simulation thread"""
         self.mark_start_time()
         while not self.isInterruptionRequested():
             start_timestamp = QTime.currentTime()
             self.cycle(self.simulation_state.simulation_threshold)
             self.msleep(max(0, (self.simulation_state.simulation_threshold) - start_timestamp.msecsTo(QTime.currentTime())))
         self.mark_stop_time()
         return super().run()
     
     def mark_start_time(self) -> None:
         """Marks start time of the simulation"""
-        self.global_start_timestamp = QTime.currentTime()
+        self.__global_start_timestamp = QTime.currentTime()
 
     def mark_stop_time(self) -> None:
         """Marks stop time of the simulation"""
-        self.global_stop_timestamp = QTime.currentTime()
+        self.__global_stop_timestamp = QTime.currentTime()
     
     def cycle(self, elapsed_time : float) -> None:
         """Executes physics simulation cycle"""
         if self.simulation_state.reset_demanded:
             self.reset_aircrafts()
         if not self.simulation_state.is_paused:
             self.count_cycles()
@@ -67,20 +109,20 @@
         self.aircraft_fccs[1].reset()
         self.simulation_state.apply_reset()
 
     def update_aircrafts_position(self, elapsed_time : float) -> bool:
         """Updates aircrafts position, returns true on collision"""
         for aircraft in self.aircraft_vehicles:
             if aircraft.position.z() <= 0.0:
-                logging.warn("Aircraft's " + str(aircraft.aircraft_id) + "collision with the ground. Coordinates: " + str(self.aircraft_vehicles[aircraft.aircraft_id].position.toTuple()))
+                logging.warning("Aircraft's " + str(aircraft.aircraft_id) + "collision with the ground. Coordinates: " + str(self.aircraft_vehicles[aircraft.aircraft_id].position.toTuple()))
                 print("Collision with ground")
                 return True
             relative_distance : float = dist(aircraft.position.toTuple(), self.aircraft_vehicles[1 - aircraft.aircraft_id].position.toTuple())
             if relative_distance <= aircraft.size:
-                logging.warn("Aircrafts' 0 and 1 collision. Coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
+                logging.warning("Aircrafts' 0 and 1 collision. Coordinates: " + str(self.aircraft_vehicles[0].position.toTuple()) + " and " + str(self.aircraft_vehicles[1].position.toTuple()))
                 print("Collision with another aircraft")
                 return True
             old_pos : QVector3D = copy(aircraft.position)
             aircraft.move(
                 aircraft.speed.x() * elapsed_time / 1000.0,
                 aircraft.speed.y() * elapsed_time / 1000.0,
                 aircraft.speed.z() * elapsed_time / 1000.0)
@@ -88,25 +130,30 @@
         return False
     
     def update_aircrafts_speed_angles(self, elapsed_time : float) -> None:
         """Updates aircrafts movement speed and angles"""
         assert elapsed_time > 0.0
         for aircraft in self.aircraft_vehicles:
             # flight control computer
-            id : int = aircraft.aircraft_id
-            fcc : AircraftFCC = self.aircraft_fccs[id]
-            cause_collision = self.simulation_state.first_cause_collision if id == 0 else self.simulation_state.second_cause_collision
-            fcc.update() if not cause_collision else fcc.update_target(self.aircraft_vehicles[1 - id].position + self.aircraft_vehicles[1 - id].speed)
+            aircraft_id : int = aircraft.aircraft_id
+            try:
+                fcc : AircraftFCC = self.aircraft_fccs[aircraft_id]
+            except IndexError:
+                logging.error("Aircraft's " + str(aircraft_id) + " flight control computer not found")
+                return
+            cause_collision = self.simulation_state.first_cause_collision if aircraft_id == 0 else self.simulation_state.second_cause_collision
+            fcc.update() if not cause_collision else fcc.update_target(self.aircraft_vehicles[1 - aircraft_id].position + self.aircraft_vehicles[1 - aircraft_id].speed)
             
             # speed
             current_speed = aircraft.absolute_speed
             target_speed = fcc.target_speed
             speed_difference = abs(current_speed - target_speed)
-            if speed_difference > 0.001 and current_speed > 20.0 and current_speed < 340: # make drone subsonic
-                max_speed_delta = aircraft.max_acceleration / elapsed_time
+            max_speed_delta = aircraft.max_acceleration / elapsed_time
+            if speed_difference > 0.001 and current_speed - max_speed_delta > 20.0 and current_speed + max_speed_delta < 340: # make drone subsonic
+                
                 if speed_difference < max_speed_delta:
                     pass # become target
                 elif current_speed < target_speed:
                     target_speed = current_speed + max_speed_delta
                 else:
                     target_speed = current_speed - max_speed_delta
                 speed_scale_factor : float = target_speed / current_speed
@@ -151,12 +198,7 @@
                 delta_yaw_angle : float = self.simulation_state.g_acceleration * tan(radians(roll_angle)) / (current_horizontal_speed / elapsed_time)
 
                 new_yaw_angle : float = 0.0
                 new_yaw_angle = current_yaw_angle + delta_yaw_angle
 
                 aircraft.speed.setX(sin(radians(new_yaw_angle)) * current_horizontal_speed)
                 aircraft.speed.setY(-cos(radians(new_yaw_angle)) * current_horizontal_speed)
-
-    def count_cycles(self) -> None:
-        """Increments physics cycle counter"""
-        self.cycles += 1
-        self.simulation_state.physics_cycles = self.cycles
```

## uav_collision_avoidance/src/simulation/simulation_render.py

```diff
@@ -7,17 +7,27 @@
 from .simulation_state import SimulationState
 
 class SimulationRender(QThread):
     """Thread running simulation rendering"""
 
     def __init__(self, parent : QMainWindow, simulation_widget : SimulationWidget, simulation_state : SimulationState) -> None:
         super(SimulationRender, self).__init__(parent)
-        self.simulation_widget = simulation_widget
-        self.simulation_state = simulation_state
+        self.__simulation_widget = simulation_widget
+        self.__simulation_state = simulation_state
         
+    @property
+    def simulation_widget(self) -> SimulationWidget:
+        """Returns simulation widget"""
+        return self.__simulation_widget
+    
+    @property
+    def simulation_state(self) -> SimulationState:
+        """Returns simulation state"""
+        return self.__simulation_state
+
     def run(self) -> None:
         """Runs simulation widget update with precise timeout"""
         while not self.isInterruptionRequested():
             start_timestamp = QTime.currentTime()
             self.simulation_state.update_render_settings()
             self.simulation_widget.update()
             self.msleep(max(0, self.simulation_state.gui_render_threshold - start_timestamp.msecsTo(QTime.currentTime())))
```

## uav_collision_avoidance/src/simulation/simulation_state.py

```diff
@@ -12,157 +12,448 @@
     """Class defining simulation's traits"""
 
     def __init__(self, simulation_settings : SimulationSettings, is_realtime : bool = True, avoid_collisions : bool = False) -> None:
         super(SimulationState, self).__init__()
         self.__mutex : QMutex = QMutex()
 
         # simulation state
-        self.simulation_settings = simulation_settings
-        self.update_settings()
-        self.is_realtime : bool = is_realtime
-        self.avoid_collisions : bool = avoid_collisions
-        self.override_avoid_collisions : bool = True
-        self.minimum_separation : float = 9260.0 # 5nmi
-        self.physics_cycles : int = 0
-        self.is_paused : bool = False
-        self.is_running : bool = True
+        self.__simulation_settings = simulation_settings
+        self.__is_realtime : bool = is_realtime
+        self.__avoid_collisions : bool = avoid_collisions
+        self.__override_avoid_collisions : bool = True
+        self.__minimum_separation : float = 9260.0 # 5nmi
+        self.__physics_cycles : int = 0
+        self.__is_paused : bool = False
+        self.__is_running : bool = True
         self.__reset_demanded : bool = False
-        self.pause_start_timestamp : QTime | None = None
-        self.time_paused : int = 0 # ms
+        self.__pause_start_timestamp : QTime | None = None
+        self.__time_paused : int = 0 # ms
         self.__adsb_report : bool = True
         self.__collision : bool = False
         self.__first_cause_collision : bool = False
         self.__second_cause_collision : bool = False
+        self.update_settings()
 
+        # render state
+        self.__fps : float = 0.0
         if is_realtime:
-            # render state
             override_gui_scale : bool = True
             if not override_gui_scale:
                 self.__gui_scale : float = 0.5 # define gui scaling
                 if SimulationSettings.screen_resolution.height() < 1440:
-                    self.gui_scale = 0.375
+                    self.__gui_scale = 0.375
                 elif SimulationSettings.screen_resolution.height() < 1080:
-                    self.gui_scale = 0.25
+                    self.__gui_scale = 0.25
                 elif SimulationSettings.screen_resolution.height() < 480:
-                    self.gui_scale = 0.125
+                    self.__gui_scale = 0.125
             else:
                 self.__gui_scale : float = 0.75
-            self.fps : float = 0.0
-            self.draw_fps : bool = True
-            self.draw_aircraft : bool = True
-            self.draw_grid : bool = False
-            self.draw_path : bool = True
-            self.draw_speed_vectors : bool = True
-            self.draw_collision_detection : bool = True
-            self.optimize_drawing : bool = False
-            self.follow_aircraft : bool = False
-            self.focus_aircraft_id : int = 0
+            self.__draw_fps : bool = True
+            self.__draw_aircraft : bool = True
+            self.__draw_grid : bool = False
+            self.__draw_path : bool = True
+            self.__draw_speed_vectors : bool = True
+            self.__draw_safezones : bool = True
+            self.__draw_collision_detection : bool = True
+            self.__optimize_drawing : bool = False
+            self.__follow_aircraft : bool = False
+            self.__focus_aircraft_id : int = 0
 
             # assets
-            self.aircraft_pixmap : QPixmap = QPixmap()
-            if not self.aircraft_pixmap.load("assets/aircraft.png"):
+            self.__aircraft_pixmap : QPixmap = QPixmap()
+            if not self.__aircraft_pixmap.load("assets/aircraft.png"):
                 try:
                     Path("assets").mkdir(parents=True, exist_ok=True)
                     urlretrieve(
                         "https://raw.githubusercontent.com/mldxo/uav-collision-avoidance/main/assets/aircraft.png",
                         "assets/aircraft.png")
-                    self.aircraft_pixmap.load("assets/aircraft.png")
+                    self.__aircraft_pixmap.load("assets/aircraft.png")
                 except:
                     pass
+
+    @property
+    def simulation_settings(self) -> SimulationSettings:
+        """Returns simulation settings"""
+        with QMutexLocker(self.__mutex):
+            return self.__simulation_settings
     
     @property
-    def adsb_report(self) -> None:
-        """Returns ADS-B commandline info reporting flag"""
-        return self.__adsb_report
+    def is_realtime(self) -> bool:
+        """Returns simulation type"""
+        with QMutexLocker(self.__mutex):
+            return self.__is_realtime
+    
+    @property
+    def avoid_collisions(self) -> bool:
+        """Returns collision avoidance flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__avoid_collisions
+    
+    @avoid_collisions.setter
+    def avoid_collisions(self, avoid_collisions : bool) -> None:
+        """Sets collision avoidance flag"""
+        with QMutexLocker(self.__mutex):
+            self.__avoid_collisions = avoid_collisions
 
-    def update_settings(self) -> None:
-        """Updates all state settings"""
-        self.update_render_settings()
-        self.update_simulation_settings()
-        self.update_adsb_settings()
+    def toggle_avoid_collisions(self) -> None:
+        """Toggles collision avoidance"""
+        with QMutexLocker(self.__mutex):
+            self.__avoid_collisions = not self.__avoid_collisions
 
-    def toggle_adsb_report(self) -> None:
-        """Toggles ADS-B commandline info report"""
-        self.__adsb_report = not self.__adsb_report
+    @property
+    def override_avoid_collisions(self) -> bool:
+        """Returns collision avoidance override flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__override_avoid_collisions
     
-    def update_render_settings(self) -> None:
-        """Updates simulation render state settings"""
-        self.gui_render_threshold = self.simulation_settings.gui_render_threshold
+    @override_avoid_collisions.setter
+    def override_avoid_collisions(self, override_avoid_collisions : bool) -> None:
+        """Sets collision avoidance override flag"""
+        with QMutexLocker(self.__mutex):
+            self.__override_avoid_collisions = override_avoid_collisions
+
+    @property
+    def minimum_separation(self) -> float:
+        """Returns minimum separation distance"""
+        with QMutexLocker(self.__mutex):
+            return self.__minimum_separation
     
-    def update_simulation_settings(self) -> None:
-        """Updates simulation physics state settings"""
-        self.simulation_threshold = self.simulation_settings.simulation_threshold
-        self.g_acceleration = self.simulation_settings.g_acceleration
+    @property
+    def physics_cycles(self) -> int:
+        """Returns physics cycles count"""
+        with QMutexLocker(self.__mutex):
+            return self.__physics_cycles
+        
+    @physics_cycles.setter
+    def physics_cycles(self, physics_cycles : int) -> None:
+        """Sets physics cycles count"""
+        with QMutexLocker(self.__mutex):
+            self.__physics_cycles = physics_cycles
     
-    def update_adsb_settings(self) -> None:
-        """Updates simulation ADS-B state settings"""
-        self.adsb_threshold = self.simulation_settings.adsb_threshold
-
-    def append_paused_time(self) -> None:
-        """Appends time elapsed during recent pause"""
-        if self.pause_start_timestamp is not None:
-            self.time_paused += self.pause_start_timestamp.msecsTo(QTime.currentTime())
-
+    @property
+    def is_paused(self) -> bool:
+        """Returns pause state"""
+        with QMutexLocker(self.__mutex):
+            return self.__is_paused
+        
+    @is_paused.setter
+    def is_paused(self, is_paused : bool) -> None:
+        """Sets pause state"""
+        with QMutexLocker(self.__mutex):
+            self.__is_paused = is_paused
+        
     def toggle_pause(self) -> None:
         """Pauses the simulation"""
         if self.is_paused:
             self.append_paused_time()
             self.is_paused = False
         else:
             if not self.is_running:
                 return
             self.pause_start_timestamp = QTime.currentTime()
             self.is_paused = True
     
     @property
+    def is_running(self) -> bool:
+        """Returns running state"""
+        with QMutexLocker(self.__mutex):
+            return self.__is_running
+        
+    @is_running.setter
+    def is_running(self, is_running : bool) -> None:
+        """Sets running state"""
+        with QMutexLocker(self.__mutex):
+            self.__is_running = is_running
+    
+    @property
+    def reset_demanded(self) -> bool:
+        """Returns simulation reset state"""
+        with QMutexLocker(self.__mutex):
+            return self.__reset_demanded
+        
+    def reset(self) -> None:
+        """Resets simulation to its start state"""
+        with QMutexLocker(self.__mutex):
+            self.__reset_demanded = True
+
+    def apply_reset(self) -> None:
+        """Sets back simulation reset state"""
+        with QMutexLocker(self.__mutex):
+            self.__reset_demanded = False
+    
+    @property
+    def pause_start_timestamp(self) -> QTime | None:
+        """Returns pause start timestamp"""
+        with QMutexLocker(self.__mutex):
+            return self.__pause_start_timestamp
+        
+    @pause_start_timestamp.setter
+    def pause_start_timestamp(self, pause_start_timestamp : QTime | None) -> None:
+        """Sets pause start timestamp"""
+        with QMutexLocker(self.__mutex):
+            self.__pause_start_timestamp = pause_start_timestamp
+        
+    def append_paused_time(self) -> None:
+        """Appends time elapsed during recent pause"""
+        with QMutexLocker(self.__mutex):
+            if self.__pause_start_timestamp is not None:
+                self.__time_paused += self.__pause_start_timestamp.msecsTo(QTime.currentTime())
+    
+    @property
+    def time_paused(self) -> int:
+        """Returns time paused"""
+        with QMutexLocker(self.__mutex):
+            return self.__time_paused
+        
+    @time_paused.setter
+    def time_paused(self, time_paused : int) -> None:
+        """Sets time paused"""
+        with QMutexLocker(self.__mutex):
+            self.__time_paused = time_paused
+    
+    @property
+    def adsb_report(self) -> None:
+        """Returns ADS-B commandline info reporting flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__adsb_report
+
+    def toggle_adsb_report(self) -> None:
+        """Toggles ADS-B commandline info report"""
+        with QMutexLocker(self.__mutex):
+            self.__adsb_report = not self.__adsb_report
+
+    @property
     def collision(self) -> bool:
         """Returns collision state"""
-        return self.__collision
+        with QMutexLocker(self.__mutex):
+            return self.__collision
 
     def register_collision(self) -> None:
         """Registers collision"""
-        self.__collision = True
+        with QMutexLocker(self.__mutex):
+            self.__collision = True
     
     @property
     def first_cause_collision(self) -> bool:
         """Returns causing collision state"""
-        return self.__first_cause_collision
+        with QMutexLocker(self.__mutex):
+            return self.__first_cause_collision
     
     def toggle_first_causing_collision(self) -> None:
         """Toggles causing collision state"""
-        self.__first_cause_collision = not self.__first_cause_collision
+        with QMutexLocker(self.__mutex):
+            self.__first_cause_collision = not self.__first_cause_collision
     
     @property
     def second_cause_collision(self) -> bool:
         """Returns causing collision state"""
-        return self.__second_cause_collision
+        with QMutexLocker(self.__mutex):
+            return self.__second_cause_collision
     
     def toggle_second_causing_collision(self) -> None:
         """Toggles causing collision state"""
-        self.__second_cause_collision = not self.__second_cause_collision
+        with QMutexLocker(self.__mutex):
+            self.__second_cause_collision = not self.__second_cause_collision
+
+    @property
+    def gui_scale(self) -> float:
+        """Returns GUI scaling factor"""
+        with QMutexLocker(self.__mutex):
+            return self.__gui_scale
     
+    @gui_scale.setter
+    def gui_scale(self, gui_scale : float) -> None:
+        """Sets GUI scaling factor"""
+        with QMutexLocker(self.__mutex):
+            self.__gui_scale = gui_scale
+
     @property
-    def reset_demanded(self) -> bool:
-        """Returns simulation reset state"""
+    def fps(self) -> float:
+        """Returns FPS"""
         with QMutexLocker(self.__mutex):
-            return self.__reset_demanded
+            return self.__fps
+    
+    @fps.setter
+    def fps(self, fps : float) -> None:
+        """Sets FPS"""
+        with QMutexLocker(self.__mutex):
+            self.__fps = fps
 
-    def reset(self) -> None:
-        """Resets simulation to its start state"""
+    @property
+    def draw_fps(self) -> bool:
+        """Returns FPS display flag"""
         with QMutexLocker(self.__mutex):
-            self.__reset_demanded = True
+            return self.__draw_fps
 
-    def apply_reset(self) -> None:
-        """Sets back simulation reset state"""
+    def toggle_draw_fps(self) -> None:
+        """Toggles FPS display"""
         with QMutexLocker(self.__mutex):
-            self.__reset_demanded = False
+            self.__draw_fps = not self.__draw_fps
 
     @property
-    def gui_scale(self) -> float:
-        """Returns GUI scaling factor"""
-        return self.__gui_scale
+    def draw_aircraft(self) -> bool:
+        """Returns aircraft display flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__draw_aircraft
+        
+    def toggle_draw_aircraft(self) -> None:
+        """Toggles aircraft display"""
+        with QMutexLocker(self.__mutex):
+            self.__draw_aircraft = not self.__draw_aircraft
+
+    @property
+    def draw_grid(self) -> bool:
+        """Returns grid display flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__draw_grid
+        
+    def toggle_draw_grid(self) -> None:
+        """Toggles grid display"""
+        with QMutexLocker(self.__mutex):
+            self.__draw_grid = not self.__draw_grid
+
+    @property
+    def draw_path(self) -> bool:
+        """Returns path display flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__draw_path
+        
+    def toggle_draw_path(self) -> None:
+        """Toggles path display"""
+        with QMutexLocker(self.__mutex):
+            self.__draw_path = not self.__draw_path
+
+    @property
+    def draw_speed_vectors(self) -> bool:
+        """Returns speed vector display flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__draw_speed_vectors
+        
+    def toggle_draw_speed_vectors(self) -> None:
+        """Toggles speed vector display"""
+        with QMutexLocker(self.__mutex):
+            self.__draw_speed_vectors = not self.__draw_speed_vectors
+
+    @property
+    def draw_safezones(self) -> bool:
+        """Returns safezone display flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__draw_safezones
+        
+    def toggle_draw_safezones(self) -> None:
+        """Toggles safezone display"""
+        with QMutexLocker(self.__mutex):
+            self.__draw_safezones = not self.__draw_safezones
+
+    @property
+    def draw_collision_detection(self) -> bool:
+        """Returns collision detection display flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__draw_collision_detection
+        
+    def toggle_draw_collision_detection(self) -> None:
+        """Toggles collision detection display"""
+        with QMutexLocker(self.__mutex):
+            self.__draw_collision_detection = not self.__draw_collision_detection
+
+    @property
+    def optimize_drawing(self) -> bool:
+        """Returns drawing optimization flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__optimize_drawing
+        
+    def toggle_optimize_drawing(self) -> None:
+        """Toggles drawing optimization"""
+        with QMutexLocker(self.__mutex):
+            self.__optimize_drawing = not self.__optimize_drawing
+
+    @property
+    def follow_aircraft(self) -> bool:
+        """Returns aircraft following flag"""
+        with QMutexLocker(self.__mutex):
+            return self.__follow_aircraft
+        
+    def toggle_follow_aircraft(self) -> None:
+        """Toggles aircraft following"""
+        with QMutexLocker(self.__mutex):
+            self.__follow_aircraft = not self.__follow_aircraft
+
+    @property
+    def focus_aircraft_id(self) -> int:
+        """Returns aircraft id to focus on"""
+        with QMutexLocker(self.__mutex):
+            return self.__focus_aircraft_id
+        
+    def toggle_focus_aircraft(self) -> None:
+        """Toggles aircraft focus"""
+        with QMutexLocker(self.__mutex):
+            self.__focus_aircraft_id = int(not self.__focus_aircraft_id)
+
+    @property
+    def gui_render_threshold(self) -> int:
+        """Returns GUI render threshold"""
+        with QMutexLocker(self.__mutex):
+            return self.__gui_render_threshold
+        
+    @gui_render_threshold.setter
+    def gui_render_threshold(self, gui_render_threshold : int) -> None:
+        """Sets GUI render threshold"""
+        with QMutexLocker(self.__mutex):
+            self.__gui_render_threshold = gui_render_threshold
+
+    @property
+    def aircraft_pixmap(self) -> QPixmap:
+        """Returns aircraft pixmap"""
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_pixmap
+        
+    @aircraft_pixmap.setter
+    def aircraft_pixmap(self, aircraft_pixmap : QPixmap) -> None:
+        """Sets aircraft pixmap"""
+        with QMutexLocker(self.__mutex):
+            self.__aircraft_pixmap = aircraft_pixmap
+
+    @property
+    def adsb_threshold(self) -> int:
+        """Returns ADS-B threshold"""
+        with QMutexLocker(self.__mutex):
+            return self.__adsb_threshold
+        
+    @adsb_threshold.setter
+    def adsb_threshold(self, adsb_threshold : int) -> None:
+        """Sets ADS-B threshold"""
+        with QMutexLocker(self.__mutex):
+            self.__adsb_threshold = adsb_threshold
+
+    @property
+    def simulation_threshold(self) -> float:
+        """Returns simulation threshold"""
+        with QMutexLocker(self.__mutex):
+            return self.__simulation_threshold
+        
+    @property
+    def g_acceleration(self) -> float:
+        """Returns acceleration due to gravity"""
+        with QMutexLocker(self.__mutex):
+            return self.__g_acceleration
+
+    def update_settings(self) -> None:
+        """Updates all state settings"""
+        self.update_render_settings()
+        self.update_simulation_settings()
+        self.update_adsb_settings()
+
+    def update_render_settings(self) -> None:
+        """Updates simulation render state settings"""
+        self.__gui_render_threshold = self.simulation_settings.gui_render_threshold
     
-    @gui_scale.setter
-    def gui_scale(self, value : float) -> None:
-        """Sets GUI scaling factor"""
-        if value > 0.0:
-            self.__gui_scale = value
+    def update_simulation_settings(self) -> None:
+        """Updates simulation physics state settings"""
+        self.__simulation_threshold = self.simulation_settings.simulation_threshold
+        self.__g_acceleration = self.simulation_settings.g_acceleration
+    
+    def update_adsb_settings(self) -> None:
+        """Updates simulation ADS-B state settings"""
+        self.__adsb_threshold = self.simulation_settings.adsb_threshold
+
+    def __del__(self) -> None:
+        self.__mutex.unlock()
```

## uav_collision_avoidance/src/simulation/simulation_widget.py

```diff
@@ -1,14 +1,14 @@
 """Simulation widget for the main window of the simulation app"""
 
 from copy import copy
 from math import cos, radians, sqrt, degrees, atan2, dist
 from typing import List
 
-from PySide6.QtCore import Qt, QPointF, Signal
+from PySide6.QtCore import Qt, QPointF, Signal, QMutex, QMutexLocker
 from PySide6.QtGui import QPaintEvent, QPainter, QKeyEvent, \
     QMouseEvent, QIcon, QPixmap, QCloseEvent, QVector3D, QPolygonF, QWheelEvent, QColor
 from PySide6.QtWidgets import QWidget, QApplication
 
 from ..aircraft.aircraft import Aircraft
 from ..aircraft.aircraft_fcc import AircraftFCC
 from ..aircraft.aircraft_vehicle import AircraftVehicle
@@ -17,83 +17,190 @@
 
 class SimulationWidget(QWidget):
     """Main widget representing the simulation"""
     stop_signal = Signal(str)
     def __init__(self, aircrafts : List[Aircraft],
                  simulation_fps : SimulationFPS, simulation_state : SimulationSettings) -> None:
         super().__init__()
-        self.aircrafts = aircrafts
-        self.aircraft_vehicles : List[AircraftVehicle] = [
-            aircraft.vehicle for aircraft in self.aircrafts]
-        self.aircraft_fccs : List[AircraftFCC] = [
-            aircraft.fcc for aircraft in self.aircrafts]
-        self.simulation_fps = simulation_fps
-        self.simulation_state = simulation_state
-
-        self.window_width : float = SimulationSettings.resolution[0]
-        self.window_height : float = SimulationSettings.resolution[1]
-        self.screen_offset_x : float = 0.0
-        self.screen_offset_y : float = 0.0
+        self.__mutex : QMutex = QMutex()
+        self.__aircrafts = aircrafts
+        self.__aircraft_vehicles : List[AircraftVehicle] = [aircraft.vehicle for aircraft in self.aircrafts]
+        self.__aircraft_fccs : List[AircraftFCC] = [aircraft.fcc for aircraft in self.aircrafts]
+        self.__simulation_fps = simulation_fps
+        self.__simulation_state = simulation_state
+
+        self.__window_width : float = SimulationSettings.resolution[0]
+        self.__window_height : float = SimulationSettings.resolution[1]
+        self.__screen_offset_x : float = 0.0
+        self.__screen_offset_y : float = 0.0
         self.setGeometry(
-            SimulationSettings.screen_resolution.width() / 2 - self.window_width / 2,
-            SimulationSettings.screen_resolution.height() / 2 - self.window_height / 2 - 30,
-            self.window_width,
-            self.window_height)
+            SimulationSettings.screen_resolution.width() / 2 - self.__window_width / 2,
+            SimulationSettings.screen_resolution.height() / 2 - self.__window_height / 2 - 30,
+            self.__window_width,
+            self.__window_height)
         self.setStyleSheet("background-color: white;")
         self.setWindowTitle(QApplication.applicationName() + " " + QApplication.applicationVersion())
 
-        self.icon = QIcon()
-        self.icon.addPixmap(self.generate_icon(), QIcon.Mode.Normal, QIcon.State.Off)
-        self.setWindowIcon(self.icon)
+        self.__icon = QIcon()
+        self.__icon.addPixmap(self.generate_icon(), QIcon.Mode.Normal, QIcon.State.Off)
+        self.setWindowIcon(self.__icon)
 
         self.__moving_view_up : bool = False
         self.__moving_view_down : bool = False
         self.__moving_view_left : bool = False
         self.__moving_view_right : bool = False
         self.__steering_left : bool = False
         self.__steering_right : bool = False
         self.__steering_up : bool = False
         self.__steering_down : bool = False
 
         self.center_offsets()
 
+    @property
+    def aircrafts(self) -> List[Aircraft]:
+        """Returns aircrafts"""
+        with QMutexLocker(self.__mutex):
+            return self.__aircrafts
+        
+    @property
+    def aircraft_vehicles(self) -> List[AircraftVehicle]:
+        """Returns aircraft vehicles"""
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_vehicles
+        
+    @property
+    def aircraft_fccs(self) -> List[AircraftFCC]:
+        """Returns aircraft fccs"""
+        with QMutexLocker(self.__mutex):
+            return self.__aircraft_fccs
+        
+    @property
+    def simulation_fps(self) -> SimulationFPS:
+        """Returns simulation fps"""
+        with QMutexLocker(self.__mutex):
+            return self.__simulation_fps
+        
+    @property
+    def simulation_state(self) -> SimulationSettings:
+        """Returns simulation state"""
+        with QMutexLocker(self.__mutex):
+            return self.__simulation_state
+        
+    @property
+    def window_width(self) -> float:
+        """Returns window width"""
+        with QMutexLocker(self.__mutex):
+            return self.__window_width
+        
+    @property
+    def window_height(self) -> float:
+        """Returns window height"""
+        with QMutexLocker(self.__mutex):
+            return self.__window_height
+        
+    @property
+    def screen_offset_x(self) -> float:
+        """Returns screen offset x"""
+        with QMutexLocker(self.__mutex):
+            return self.__screen_offset_x
+        
+    @property
+    def screen_offset_y(self) -> float:
+        """Returns screen offset y"""
+        with QMutexLocker(self.__mutex):
+            return self.__screen_offset_y
+        
+    @property
+    def icon(self) -> QIcon:
+        """Returns icon"""
+        with QMutexLocker(self.__mutex):
+            return self.__icon
+        
+    @property
+    def moving_view_up(self) -> bool:
+        """Returns moving view up"""
+        with QMutexLocker(self.__mutex):
+            return self.__moving_view_up
+        
+    @property
+    def moving_view_down(self) -> bool:
+        """Returns moving view down"""
+        with QMutexLocker(self.__mutex):
+            return self.__moving_view_down
+        
+    @property
+    def moving_view_left(self) -> bool:
+        """Returns moving view left"""
+        with QMutexLocker(self.__mutex):
+            return self.__moving_view_left
+        
+    @property
+    def moving_view_right(self) -> bool:
+        """Returns moving view right"""
+        with QMutexLocker(self.__mutex):
+            return self.__moving_view_right
+        
+    @property
+    def steering_left(self) -> bool:
+        """Returns steering left"""
+        with QMutexLocker(self.__mutex):
+            return self.__steering_left
+        
+    @property
+    def steering_right(self) -> bool:
+        """Returns steering right"""
+        with QMutexLocker(self.__mutex):
+            return self.__steering_right
+
+    @property
+    def steering_up(self) -> bool:
+        """Returns steering up"""
+        with QMutexLocker(self.__mutex):
+            return self.__steering_up
+        
+    @property
+    def steering_down(self) -> bool:
+        """Returns steering down"""
+        with QMutexLocker(self.__mutex):
+            return self.__steering_down
+
     def generate_icon(self) -> QPixmap:
         """Returns icon for the main window"""
-        pixmap = QPixmap(self.simulation_state.aircraft_pixmap)
-        painter = QPainter(pixmap)
+        pixmap : QPixmap = QPixmap(self.__simulation_state.aircraft_pixmap)
+        painter : QPainter = QPainter(pixmap)
         painter.setBrush(QColor("white"))
-        painter.drawEllipse(self.simulation_state.aircraft_pixmap.rect())
+        painter.drawEllipse(self.__simulation_state.aircraft_pixmap.rect())
         painter.drawPixmap(
-            self.simulation_state.aircraft_pixmap.width() * 0.125,
-            self.simulation_state.aircraft_pixmap.height() * 0.125,
-            self.simulation_state.aircraft_pixmap.scaled(self.simulation_state.aircraft_pixmap.width() * 0.75,
-            self.simulation_state.aircraft_pixmap.height() * 0.75))
+            self.__simulation_state.aircraft_pixmap.width() * 0.125,
+            self.__simulation_state.aircraft_pixmap.height() * 0.125,
+            self.__simulation_state.aircraft_pixmap.scaled(self.__simulation_state.aircraft_pixmap.width() * 0.75,
+            self.__simulation_state.aircraft_pixmap.height() * 0.75))
         painter.end()
         return pixmap
 
     def draw_aircraft(self, aircraft : AircraftVehicle, scale : float) -> None:
         """Draws given aircraft vehicle"""
         yaw_angle : float = aircraft.yaw_angle
         size : float = aircraft.size * scale
         pixmap : QPixmap
-        if not self.simulation_state.aircraft_pixmap.isNull():
-            pixmap = self.simulation_state.aircraft_pixmap.scaled(
+        if not self.__simulation_state.aircraft_pixmap.isNull():
+            pixmap = self.__simulation_state.aircraft_pixmap.scaled(
                 size * abs(cos(radians(aircraft.roll_angle))),
                 size * abs(cos(radians(aircraft.pitch_angle)))
             )
         else:
             pixmap = QPixmap(
                 size * abs(cos(radians(aircraft.roll_angle))),
                 size * abs(cos(radians(aircraft.pitch_angle))))
             pixmap.fill(Qt.GlobalColor.black)
         painter = QPainter(self)
         painter.setRenderHint(QPainter.RenderHint.Antialiasing, True)
         painter.setRenderHint(QPainter.RenderHint.SmoothPixmapTransform, True)
-        x_offset = self.screen_offset_x * scale
-        y_offset = self.screen_offset_y * scale
+        x_offset = self.__screen_offset_x * scale
+        y_offset = self.__screen_offset_y * scale
         painter.translate(QPointF(
             (aircraft.position.x() * scale) + x_offset,
             (aircraft.position.y() * scale) + y_offset))
         painter.rotate(yaw_angle)
         painter.translate(QPointF(
             (- size / 2) - x_offset,
             (- size / 2) - y_offset))
@@ -103,25 +210,25 @@
             size * abs(cos(radians(aircraft.pitch_angle))))
         painter.rotate(-yaw_angle)
         painter.end()
         self.draw_text(aircraft.position, scale, f"Aircraft {aircraft.aircraft_id}")
 
     def draw_destinations(self, aircraft : AircraftVehicle, scale : float) -> None:
         """Draws destinations of given aircraft vehicle"""
-        for idx, destination in enumerate(self.aircraft_fccs[aircraft.aircraft_id].destinations):
+        for idx, destination in enumerate(self.__aircraft_fccs[aircraft.aircraft_id].destinations):
             self.draw_disk(destination, 2.5 / scale, scale)
             self.draw_text(destination, scale, f"Destination {idx} of Aircraft {aircraft.aircraft_id}")
 
     def draw_text(self, point : QVector3D, scale : float, text : str, color : QColor = QColor(0, 0, 0)) -> None:
         """Draws text at given coordinates"""
         painter = QPainter(self)
         painter.setBrush(Qt.BrushStyle.SolidPattern)
         painter.setPen(color)
-        x_offset = self.screen_offset_x * scale
-        y_offset = self.screen_offset_y * scale
+        x_offset = self.__screen_offset_x * scale
+        y_offset = self.__screen_offset_y * scale
         if scale != 0:
             painter.drawText(
                 QPointF(
                     ((point.x() + 10) * scale) + x_offset,
                     ((point.y() + 10) * scale) + y_offset),
                 text)
         else:
@@ -132,61 +239,61 @@
                 text)
         painter.end()
 
     def draw_circle(self, point : QVector3D, size : float, scale : float, color : QColor = QColor(0, 0, 0)) -> None:
         """Draws circle at given coordinates (empty)"""
         painter = QPainter(self)
         painter.setPen(color)
-        x_offset = self.screen_offset_x * scale
-        y_offset = self.screen_offset_y * scale
+        x_offset = self.__screen_offset_x * scale
+        y_offset = self.__screen_offset_y * scale
         painter.drawEllipse(
             QPointF(
-                point.x() * scale - (size * scale / 2) + x_offset,
-                point.y() * scale - (size * scale / 2) + y_offset),
+                point.x() * scale + x_offset,
+                point.y() * scale + y_offset),
             float(size * scale),
             float(size * scale))
         painter.end()
     
     def draw_disk(self, point : QVector3D, size : float, scale : float, color : QColor = QColor(0, 0, 0)) -> None:
         """Draws disk at given coordinates (full)"""
         painter = QPainter(self)
         painter.setBrush(Qt.BrushStyle.SolidPattern)
         painter.setPen(color)
-        x_offset = self.screen_offset_x * scale
-        y_offset = self.screen_offset_y * scale
+        x_offset = self.__screen_offset_x * scale
+        y_offset = self.__screen_offset_y * scale
         painter.drawEllipse(
             QPointF(
-                point.x() * scale - (size * scale / 2) + x_offset,
-                point.y() * scale - (size * scale / 2) + y_offset),
+                point.x() * scale + x_offset,
+                point.y() * scale + y_offset),
             float(size * scale),
             float(size * scale))
         painter.end()
 
     def draw_line(self, point1 : QVector3D, point2 : QVector3D, scale : float, color : QColor = QColor(0, 0, 0)) -> None:
         """Draws line connecting given points"""
         painter = QPainter(self)
         painter.setBrush(Qt.BrushStyle.SolidPattern)
         painter.setPen(color)
-        x_offset = self.screen_offset_x * scale
-        y_offset = self.screen_offset_y * scale
+        x_offset = self.__screen_offset_x * scale
+        y_offset = self.__screen_offset_y * scale
         painter.drawLine(
             int((point1.x() * scale) + x_offset),
             int((point1.y() * scale) + y_offset),
             int((point2.x() * scale) + x_offset),
             int((point2.y() * scale) + y_offset))
         painter.end()
 
     def draw_vector(self, point1 : QVector3D, point2 : QVector3D, scale : float, color : QColor = QColor(0, 0, 0)) -> None:
         """Draws vector pointing from first to second point"""
         self.draw_line(point1, point2, scale, color)
         painter = QPainter(self)
         painter.setBrush(Qt.BrushStyle.SolidPattern)
         painter.setPen(color)
-        x_offset = self.screen_offset_x * scale
-        y_offset = self.screen_offset_y * scale
+        x_offset = self.__screen_offset_x * scale
+        y_offset = self.__screen_offset_y * scale
         angle = degrees(atan2(point1.x() - point2.x(), point1.y() - point2.y()))
         arrowhead_size = SimulationSettings.screen_resolution.width() / 400 * scale
         arrowhead_height = arrowhead_size * sqrt(3) / 2
         polygon = QPolygonF()
         polygon.append(
             QPointF(
                 (point2.x() * scale - arrowhead_size / 2) + x_offset,
@@ -212,98 +319,98 @@
         painter.end()
     
     def draw_collision_detection(self, scale : float) -> None:
         """Draws collision detection elements for the aircrafts"""
         detected_conflict : bool = False
         predicted_collision : bool = False
         time_to_closest_approach : float = 0.0
-        if self.simulation_state.collision:
-            self.draw_text(QVector3D(self.window_width - 70, 10, 0), 0, "COLLISION", QColor(255, 0, 0))
+        if self.__simulation_state.collision:
+            self.draw_text(QVector3D(self.__window_width - 70, 10, 0), 0, "COLLISION", QColor(255, 0, 0))
             return
-        for aircraft in self.aircraft_vehicles:
-            relative_position = aircraft.position - self.aircraft_vehicles[1 - aircraft.aircraft_id].position
-            speed_difference : QVector3D = aircraft.speed - self.aircraft_vehicles[1 - aircraft.aircraft_id].speed
+        for aircraft in self.__aircraft_vehicles:
+            relative_position = aircraft.position - self.__aircraft_vehicles[1 - aircraft.aircraft_id].position
+            speed_difference : QVector3D = aircraft.speed - self.__aircraft_vehicles[1 - aircraft.aircraft_id].speed
             time_to_closest_approach = -(QVector3D.dotProduct(relative_position, speed_difference) / QVector3D.dotProduct(speed_difference, speed_difference))
             if time_to_closest_approach > 0:
                 speed_difference_unit = speed_difference.normalized()
                 miss_distance_vector : QVector3D = QVector3D.crossProduct(
                     speed_difference_unit,
                     QVector3D.crossProduct(relative_position, speed_difference_unit))
-                collision_distance = aircraft.size / 2 + self.aircraft_vehicles[1 - aircraft.aircraft_id].size / 2
-                unresolved_region = self.simulation_state.minimum_separation - miss_distance_vector.length()
+                collision_distance = aircraft.size / 2 + self.__aircraft_vehicles[1 - aircraft.aircraft_id].size / 2
+                unresolved_region = self.__simulation_state.minimum_separation - miss_distance_vector.length()
                 collision_region = collision_distance - miss_distance_vector.length()
                 if miss_distance_vector.length() == 0:
-                    self.draw_text(QVector3D(self.window_width - 200, 10, 0), 0, "DETECTED HEAD-ON COLLISION", QColor(255, 0, 255))
+                    self.draw_text(QVector3D(self.__window_width - 200, 10, 0), 0, "DETECTED HEAD-ON COLLISION", QColor(255, 0, 255))
                     predicted_collision = True
                     detected_conflict = True
                 elif collision_region > 0:
-                    self.draw_text(QVector3D(self.window_width - 140, 10, 0), 0, "DETECTED COLLISION", QColor(255, 0, 0))
+                    self.draw_text(QVector3D(self.__window_width - 140, 10, 0), 0, "DETECTED COLLISION", QColor(255, 0, 0))
                     self.draw_vector(
-                        self.aircraft_vehicles[1 - aircraft.aircraft_id].position,
-                        self.aircraft_vehicles[1 - aircraft.aircraft_id].position + miss_distance_vector,
+                        self.__aircraft_vehicles[1 - aircraft.aircraft_id].position,
+                        self.__aircraft_vehicles[1 - aircraft.aircraft_id].position + miss_distance_vector,
                         scale,
                         QColor(0, 0, 255))
                     predicted_collision = True
                     detected_conflict = True
                 elif unresolved_region > 0:
-                    self.draw_text(QVector3D(self.window_width - 140, 10, 0), 0, "DETECTED CONFLICT")
+                    self.draw_text(QVector3D(self.__window_width - 140, 10, 0), 0, "DETECTED CONFLICT")
                     self.draw_vector(
-                        self.aircraft_vehicles[1 - aircraft.aircraft_id].position,
-                        self.aircraft_vehicles[1 - aircraft.aircraft_id].position + miss_distance_vector,
+                        self.__aircraft_vehicles[1 - aircraft.aircraft_id].position,
+                        self.__aircraft_vehicles[1 - aircraft.aircraft_id].position + miss_distance_vector,
                         scale,
                         QColor(0, 0, 255))
                     detected_conflict = True
-                if self.aircraft_fccs[aircraft.aircraft_id].vector_sharing_resolution is not None:
+                if self.__aircraft_fccs[aircraft.aircraft_id].vector_sharing_resolution is not None:
                     self.draw_vector(aircraft.position, aircraft.position + aircraft.speed * time_to_closest_approach, scale)
-                    self.draw_vector(aircraft.position, aircraft.position + aircraft.speed * time_to_closest_approach + self.aircraft_fccs[aircraft.aircraft_id].vector_sharing_resolution, scale, QColor(30, 255, 30))
+                    self.draw_vector(aircraft.position, aircraft.position + aircraft.speed * time_to_closest_approach + self.__aircraft_fccs[aircraft.aircraft_id].vector_sharing_resolution, scale, QColor(30, 255, 30))
         if predicted_collision:
-            aircraft = self.aircraft_vehicles[0]
+            aircraft = self.__aircraft_vehicles[0]
             collision_location = aircraft.position + aircraft.speed * time_to_closest_approach
             self.draw_circle(collision_location, 2.5 / scale, scale, QColor(255, 0, 0))
-        relative_distance = dist(self.aircraft_vehicles[0].position.toTuple(), self.aircraft_vehicles[1].position.toTuple())
-        if relative_distance < self.simulation_state.minimum_separation:
+        relative_distance = dist(self.__aircraft_vehicles[0].position.toTuple(), self.__aircraft_vehicles[1].position.toTuple())
+        if relative_distance < self.__simulation_state.minimum_separation:
             if detected_conflict:
-                self.draw_text(QVector3D(self.window_width - 260, 30, 0), 0, f"MINIMUM SEPARATION EXCEEDED BY {int(self.simulation_state.minimum_separation - relative_distance)}", QColor(255, 0, 0))
+                self.draw_text(QVector3D(self.__window_width - 260, 30, 0), 0, f"MINIMUM SEPARATION EXCEEDED BY {int(self.__simulation_state.minimum_separation - relative_distance)}", QColor(255, 0, 0))
             else:
-                self.draw_text(QVector3D(self.window_width - 260, 10, 0), 0, f"MINIMUM SEPARATION EXCEEDED BY {int(self.simulation_state.minimum_separation - relative_distance)}", QColor(255, 0, 0))
+                self.draw_text(QVector3D(self.__window_width - 260, 10, 0), 0, f"MINIMUM SEPARATION EXCEEDED BY {int(self.__simulation_state.minimum_separation - relative_distance)}", QColor(255, 0, 0))
     
     def draw_grid(self, x_offset : float, y_offset : float, scale : float) -> None:
         """Draws grid on the screen"""
         # todo: use offsets
-        for x in range(0, int(self.window_width / scale - x_offset / 100), 100): # vertical lines
+        for x in range(0, int(self.__window_width / scale - x_offset / 100), 100): # vertical lines
             self.draw_line(
                 QVector3D(x - x_offset / 100, 0 - y_offset, 0),
-                QVector3D(x - x_offset / 100, self.window_height / scale - y_offset, 0),
+                QVector3D(x - x_offset / 100, self.__window_height / scale - y_offset, 0),
                 scale,
                 QColor(40, 40, 40))
-        for y in range(0, int(self.window_height / scale), 100): # horizontal lines
+        for y in range(0, int(self.__window_height / scale), 100): # horizontal lines
             self.draw_line(
                 QVector3D(- x_offset, y - y_offset / 100, 0),
-                QVector3D(self.window_width / scale - x_offset, y - y_offset / 100, 0),
+                QVector3D(self.__window_width / scale - x_offset, y - y_offset / 100, 0),
                 scale,
                 QColor(40, 40, 40))
 
     def update_moving_offsets(self) -> None:
         """Updates screen offsets based on current input"""
-        scale : float = self.simulation_state.gui_scale
+        scale : float = self.__simulation_state.gui_scale
         if self.__moving_view_up:
-            self.screen_offset_y += 10.0 / scale
+            self.__screen_offset_y += 10.0 / scale
         if self.__moving_view_down:
-            self.screen_offset_y -= 10.0 / scale
+            self.__screen_offset_y -= 10.0 / scale
         if self.__moving_view_left:
-            self.screen_offset_x += 10.0 / scale
+            self.__screen_offset_x += 10.0 / scale
         if self.__moving_view_right:
-            self.screen_offset_x -= 10.0 / scale
+            self.__screen_offset_x -= 10.0 / scale
 
     def update_steering(self) -> None:
         """Updates aircraft steering based on current input"""
         if self.aircrafts[0] and (self.__steering_up or self.__steering_down or self.__steering_left or self.__steering_right):
             if sum([self.__steering_up, self.__steering_down, self.__steering_left, self.__steering_right]) >= 3:
                 return
-            self.aircraft_fccs[0].ignore_destinations = True
+            self.__aircraft_fccs[0].ignore_destinations = True
             target_yaw_angle : float | None = None
             if self.__steering_up and self.__steering_left:
                 target_yaw_angle = -45.0
             elif self.__steering_up and self.__steering_right:
                 target_yaw_angle = 45.0
             elif self.__steering_down and self.__steering_left:
                 target_yaw_angle = -135.0
@@ -314,111 +421,113 @@
             elif self.__steering_down:
                 target_yaw_angle = 180.0
             elif self.__steering_left:
                 target_yaw_angle = -90.0
             elif self.__steering_right:
                 target_yaw_angle = 90.0
             if target_yaw_angle is not None:
-                self.aircraft_fccs[0].target_yaw_angle = target_yaw_angle
+                self.__aircraft_fccs[0].target_yaw_angle = target_yaw_angle
 
     def center_offsets(self) -> None:
         """Updates screen offsets centering on selected aircraft"""
-        scale : float = self.simulation_state.gui_scale
-        id = self.simulation_state.focus_aircraft_id
-        self.screen_offset_x = (self.window_width / 2.0) / scale - self.aircraft_vehicles[id].position.x()
-        self.screen_offset_y = (self.window_height / 2.0) / scale - self.aircraft_vehicles[id].position.y()
+        scale : float = self.__simulation_state.gui_scale
+        id = self.__simulation_state.focus_aircraft_id
+        self.__screen_offset_x = (self.__window_width / 2.0) / scale - self.__aircraft_vehicles[id].position.x()
+        self.__screen_offset_y = (self.__window_height / 2.0) / scale - self.__aircraft_vehicles[id].position.y()
 
     def update_resolutions(self) -> None:
         """Updates bounding box resolution"""
-        self.window_width = self.width()
-        self.window_height = self.height()
+        self.__window_width = self.width()
+        self.__window_height = self.height()
 
     def zoom(self, factor : float) -> None:
         """Zooms in/out the simulation render"""
-        if self.simulation_state.gui_scale + factor >= 2:
-            self.simulation_state.gui_scale = 2
+        if self.__simulation_state.gui_scale + factor >= 3:
+            self.__simulation_state.gui_scale = 3
             return
-        while factor > 0 and factor > 2 * self.simulation_state.gui_scale:
+        while factor > 0 and factor > 2 * self.__simulation_state.gui_scale:
             factor /= 2
-        while factor < 0 and self.simulation_state.gui_scale + factor <= 0:
+        while factor < 0 and self.__simulation_state.gui_scale + factor <= 0:
             factor /= 2
-        old_scale : float = self.simulation_state.gui_scale
-        self.simulation_state.gui_scale += factor
-        scale : float = self.simulation_state.gui_scale
-        self.screen_offset_x = self.screen_offset_x * (old_scale / scale)
-        self.screen_offset_y = self.screen_offset_y * (old_scale / scale)
+        old_scale : float = self.__simulation_state.gui_scale
+        self.__simulation_state.gui_scale += factor
+        scale : float = self.__simulation_state.gui_scale
+        self.__screen_offset_x = self.__screen_offset_x * (old_scale / scale)
+        self.__screen_offset_y = self.__screen_offset_y * (old_scale / scale)
 
     def paintEvent(self, event : QPaintEvent) -> None:
         """Qt method painting the aircrafts"""
-        self.simulation_fps.count_frame()
-        scale : float = self.simulation_state.gui_scale
+        self.__simulation_fps.count_frame()
+        scale : float = self.__simulation_state.gui_scale
         self.update_steering()
-        if not self.simulation_state.follow_aircraft:
+        if not self.__simulation_state.follow_aircraft:
             self.update_moving_offsets()
         else:
             self.center_offsets()
 
-        if self.simulation_state.draw_fps:
-            self.draw_text(QVector3D(10, 10, 0), 0, "FPS: " + "{:.2f}".format(self.simulation_state.fps))
-        if self.simulation_state.draw_grid:
-            self.draw_grid(self.screen_offset_x, self.screen_offset_y, scale)
+        if self.__simulation_state.draw_fps:
+            self.draw_text(QVector3D(10, 10, 0), 0, "FPS: " + "{:.2f}".format(self.__simulation_state.fps))
+        if self.__simulation_state.draw_grid:
+            self.draw_grid(self.__screen_offset_x, self.__screen_offset_y, scale)
 
-        if self.simulation_state.optimize_drawing:
+        if self.__simulation_state.optimize_drawing:
             anything_to_draw : bool = False
-            geometric_center : QVector3D = self.aircraft_vehicles[0].position + self.aircraft_vehicles[1].position / 2
-            if (geometric_center.x() * scale + 300) + self.screen_offset_x * scale >= 0 and \
-                (geometric_center.y() * scale + 200) + self.screen_offset_y * scale >= 0 and \
-                (geometric_center.x() * scale - 300) + self.screen_offset_x * scale <= self.window_width and \
-                (geometric_center.y() * scale - 200) + self.screen_offset_y * scale <= self.window_height:
+            geometric_center : QVector3D = self.__aircraft_vehicles[0].position + self.__aircraft_vehicles[1].position / 2
+            if (geometric_center.x() * scale + 300) + self.__screen_offset_x * scale >= 0 and \
+                (geometric_center.y() * scale + 200) + self.__screen_offset_y * scale >= 0 and \
+                (geometric_center.x() * scale - 300) + self.__screen_offset_x * scale <= self.__window_width and \
+                (geometric_center.y() * scale - 200) + self.__screen_offset_y * scale <= self.__window_height:
                 anything_to_draw = True
             if not anything_to_draw:
-                for aircraft in self.aircraft_vehicles:
-                    if (aircraft.position.x() * scale) + self.screen_offset_x * scale >= 0 and \
-                        (aircraft.position.y() * scale) + self.screen_offset_y * scale >= 0 and \
-                        (aircraft.position.x() * scale) + self.screen_offset_x * scale <= self.window_width and \
-                        (aircraft.position.y() * scale) + self.screen_offset_y * scale <= self.window_height:
+                for aircraft in self.__aircraft_vehicles:
+                    if (aircraft.position.x() * scale) + self.__screen_offset_x * scale >= 0 and \
+                        (aircraft.position.y() * scale) + self.__screen_offset_y * scale >= 0 and \
+                        (aircraft.position.x() * scale) + self.__screen_offset_x * scale <= self.__window_width and \
+                        (aircraft.position.y() * scale) + self.__screen_offset_y * scale <= self.__window_height:
                         anything_to_draw = True
                         break
             if not anything_to_draw:
                 return super().paintEvent(event)
 
-        if self.simulation_state.draw_collision_detection:
+        if self.__simulation_state.draw_collision_detection:
             self.draw_collision_detection(scale)
-        for aircraft in self.aircraft_vehicles:
-            if self.simulation_state.draw_aircraft:
+        for aircraft in self.__aircraft_vehicles:
+            if self.__simulation_state.draw_aircraft:
                 self.draw_aircraft(aircraft, scale)
                 self.draw_destinations(aircraft, scale)
-            if self.simulation_state.draw_speed_vectors:
+            if self.__simulation_state.draw_speed_vectors:
                 self.draw_vector(aircraft.position, aircraft.position + aircraft.speed, scale)
+            if self.__simulation_state.draw_safezones:
+                self.draw_circle(aircraft.position, self.__simulation_state.minimum_separation, scale)
         return super().paintEvent(event)
 
     def mousePressEvent(self, event: QMouseEvent) -> None:
         """Qt method controlling single click mouse input"""
-        scale : float = self.simulation_state.gui_scale
+        scale : float = self.__simulation_state.gui_scale
         click_x : int = event.pos().x()
         click_y : int = event.pos().y()
-        real_x : float = click_x / scale - self.screen_offset_x
-        real_y : float = click_y / scale - self.screen_offset_y
+        real_x : float = click_x / scale - self.__screen_offset_x
+        real_y : float = click_y / scale - self.__screen_offset_y
         print(
             "click: physical coords: x: " + "{:.2f}".format(real_x) +
             "; y: " + "{:.2f}".format(real_y) +
             " | window coords: x: " + "{:.2f}".format(click_x) +
             "; y: " + "{:.2f}".format(click_y))
         if event.button() == Qt.MouseButton.LeftButton:
-            self.aircraft_fccs[0].add_first_destination(QVector3D(
+            self.__aircraft_fccs[0].add_first_destination(QVector3D(
                 real_x,
                 real_y,
                 1000.0))
         elif event.button() == Qt.MouseButton.RightButton:
-            self.aircraft_fccs[0].add_last_destination(QVector3D(
+            self.__aircraft_fccs[0].add_last_destination(QVector3D(
                 real_x,
                 real_y,
                 1000.0))
         elif event.button() == Qt.MouseButton.MiddleButton:
-            self.aircraft_vehicles[0].position = QVector3D(
+            self.__aircraft_vehicles[0].position = QVector3D(
                 real_x,
                 real_y,
                 1000.0)
         return super().mousePressEvent(event)
     
     def mouseReleaseEvent(self, event: QMouseEvent) -> None:
         """Qt method controlling mouse release input"""
@@ -440,40 +549,45 @@
     def keyPressEvent(self, event: QKeyEvent) -> None:
         """Qt method controlling keyboard input"""
         if event.key() == Qt.Key.Key_Escape:
             self.close()
         elif event.key() == Qt.Key.Key_Slash:
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
-            self.simulation_state.toggle_pause()
+            self.__simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_R:
             if event.isAutoRepeat():
                 return super().keyPressEvent(event)
-            self.simulation_state.reset()
+            print("Resetting simulation...")
+            self.__simulation_state.reset()
             self.center_offsets()
+        elif event.key() == Qt.Key.Key_F:
+            self.__simulation_state.toggle_fps()
         elif event.key() == Qt.Key.Key_Plus:
             self.zoom(0.0625)
         elif event.key() == Qt.Key.Key_Minus:
             self.zoom(-0.0625)
         elif event.key() == Qt.Key.Key_F1:
-            self.simulation_state.toggle_adsb_report()
+            self.__simulation_state.toggle_adsb_report()
         elif event.key() == Qt.Key.Key_F2:
-            self.aircraft_fccs[0].target_speed -= 10.0
+            self.__aircraft_fccs[0].accelerate(-10.0)
         elif event.key() == Qt.Key.Key_F3:
-            self.aircraft_fccs[0].target_speed += 10.0
+            self.__aircraft_fccs[0].accelerate(10.0)
         elif event.key() == Qt.Key.Key_O:
-            self.simulation_state.toggle_first_causing_collision()
+            self.__simulation_state.toggle_first_cause_collision()
         elif event.key() == Qt.Key.Key_P:
-            self.simulation_state.toggle_second_causing_collision()
+            self.__simulation_state.toggle_second_cause_collision()
         elif event.key() == Qt.Key.Key_T:
-            self.simulation_state.avoid_collisions = not self.simulation_state.avoid_collisions
+            self.__simulation_state.toggle_avoid_collisions()
         elif event.key() == Qt.Key.Key_N:
-            self.simulation_state.follow_aircraft = not self.simulation_state.follow_aircraft
+            self.__simulation_state.toggle_follow_aircraft()
         elif event.key() == Qt.Key.Key_M:
-            self.simulation_state.focus_aircraft_id = int(not self.simulation_state.focus_aircraft_id)
+            self.__simulation_state.toggle_focus_aircraft()
+        elif event.key() == Qt.Key.Key_Z:
+            self.__simulation_state.toggle_draw_safezones()
         elif event.key() == Qt.Key.Key_Left:
             self.__moving_view_left = True
         elif event.key() == Qt.Key.Key_Right:
             self.__moving_view_right = True
         elif event.key() == Qt.Key.Key_Up:
             self.__moving_view_up = True
         elif event.key() == Qt.Key.Key_Down:
@@ -487,26 +601,26 @@
                 self.__steering_up = True
             elif event.key() == Qt.Key.Key_S:
                 self.__steering_down = True
         return super().keyPressEvent(event)
     
     def keyReleaseEvent(self, event: QKeyEvent) -> None:
         """Qt method controlling keyboard input"""
-        if event.key() == Qt.Key.Key_Slash and event.isAutoRepeat() and self.simulation_state.is_paused:
-            self.simulation_state.toggle_pause()
+        if event.key() == Qt.Key.Key_Slash and event.isAutoRepeat() and self.__simulation_state.is_paused:
+            self.__simulation_state.toggle_pause()
         elif event.key() == Qt.Key.Key_Left:
             self.__moving_view_left = False
         elif event.key() == Qt.Key.Key_Right:
             self.__moving_view_right = False
         elif event.key() == Qt.Key.Key_Up:
             self.__moving_view_up = False
         elif event.key() == Qt.Key.Key_Down:
             self.__moving_view_down = False
         if self.aircrafts[0]:
-            self.aircraft_fccs[0].ignore_destinations = False
+            self.__aircraft_fccs[0].ignore_destinations = False
             if event.key() == Qt.Key.Key_A:
                 self.__steering_left = False
             elif event.key() == Qt.Key.Key_D:
                 self.__steering_right = False
             elif event.key() == Qt.Key.Key_W:
                 self.__steering_up = False
             elif event.key() == Qt.Key.Key_S:
```

## Comparing `uav_collision_avoidance-0.6.4.dist-info/LICENSE` & `uav_collision_avoidance-0.6.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uav_collision_avoidance-0.6.4.dist-info/METADATA` & `uav_collision_avoidance-0.6.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uav-collision-avoidance
-Version: 0.6.4
+Version: 0.6.6
 Summary: UAV collision avoidance simulation
 Author-email: mldxo <miloszmaculewicz@gmail.com>
 Project-URL: Homepage, https://github.com/mldxo/uav-collision-avoidance
 Project-URL: Issues, https://github.com/mldxo/uav-collision-avoidance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,19 +46,17 @@
 ### Structures
 
 Application is built based on two main object types, simulation and aircraft. Simulation is created up to initial settings, allowing for concurrent realtime variant and linear prerendering. Aircraft consists of two elements, physical representation of the UAV and Flight Control Computer, which is controlled by the physics thread. Research among the UAV systems was possible thanks to second paper[^5].
 
 ### App arguments
 
 There are three possible arguments at the moment:
-- realtime - runs GUI application with realtime simulation
-- prerender - runs physical simulation
-- tests - runs full tests with comparison of using and not using collision avoidance algorithm
-
-App defaults to realtime simulation.
+- default (no arguments) - runs GUI simulation
+- headless - runs physical simulation with ADS-B and collision avoidance algorithm
+- tests - runs full tests comparing effectiveness of collision avoidance algorithm
 
 ### Key shortcuts
 
 > [!NOTE]
 > Aircraft 0 is the first one, Aircraft 1 is the second one.
 
 There are several key shortcuts for realtime version of the app that allow full-scale testing.
@@ -79,19 +77,49 @@
 - WSAD keys - sets course for Aircraft 0 - 0, 180, 270, 90 degrees respectively
 - R - resets simulation to start state
 - Slash key (/) - pauses physics simulation
 - Escape key (Esc) - closes and ends simulation
 
 ### Install
 
-Use `pip install uav-collision-avoidance` to install the app and run one of the following:
-- uav-collision-avoidance
-- uav-collision-avoidance realtime
-- uav-collision-avoidance prerender
-- uav-collision-avoidance tests
+Install the app by running the following command:
+
+```bash
+pip install uav-collision-avoidance
+```
+
+#### Debian 12 Dependencies
+
+For Debian 12, you need to install the following dependencies:
+
+```bash
+sudo apt-get install libgl1 libxcb-xinerama0
+```
+
+To run the app headlessly, you need to run the following export:
+
+```bash
+export QT_QPA_PLATFORM=offscreen
+```
+
+### Usage
+
+Use any of the following to run the app:
+
+```bash
+uav-collision-avoidance
+```
+
+```bash
+uav-collision-avoidance headless
+```
+
+```bash
+uav-collision-avoidance tests
+```
 
 ### Build
 
 Build it by cloning the repo and running the following commands:
 
 <p align="left">
     <img width="30px" alt="Bash" style="padding-right:10px;" src="https://skillicons.dev/icons?i=bash" />
@@ -120,18 +148,18 @@
 
 3-dimensional (3D) world is projected on 2D screen by flattening height (z coordinate). On the program start, the view is centered on the first aircraft. The view can be moved with arrow keys.
 
 One coding convention is not preserved in the scope of the project. Qt's methods are CamelCase formatted and the rest is default Python naming convention including snake_case for variable and member names.
 
 ## Current Work / TODOs
 
-- [ ] Reimplement safe zone
+- [x] Reimplement safe zone
 - [x] Head-on collision avoidance
 - [x] Symmetrical bank (roll) during turn, no angle approaximation
-- [ ] Altitude change with symmetrical command
+- [x] Altitude change with symmetrical command
 - [ ] Generating test cases and batch loading
 - [ ] Test cases comparison
 - [x] Aircraft 0 manual control override
 - [ ] Flight control computer angle optimization
 - [ ] Centered view optimization
 - [ ] Documentation
```

## Comparing `uav_collision_avoidance-0.6.4.dist-info/RECORD` & `uav_collision_avoidance-0.6.6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,126 +1,176 @@
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=7y-WaszHOstlbNzr3cAqYNZK4F94-lZqwtFX2M3pRQ8,9540
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=GakasXPXcBn-VBRsF2DxUGB_bQF4ngxRAa2KOdsj7kY,8671
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=xF-IM-ljjJyc2GWSuiwVVcGzlzirrPhEAv3y8qAWobU,6057
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=6yf0nb_AfOsEmyaea5ywDy2q0N1tgfY_fimis4HG3YY,7112
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=lFwovBDK4mmX3Y6B34v--dv-2975e1va6aAtFQ70Ie4,6110
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=XaPV0vLLQ0PrP1_r9dmJ8BlEkfaQ9dHJROGTjqv4t2Q,23164
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=E0SjNZiSmjte8UHPu9yebCFPjzg2-mF3Z7U45cd9KU8,9028
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Av5-ayC8GFdNFXplPsBr3CBhfc_7yoiz3AICrMVdShQ,7108
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=7y-WaszHOstlbNzr3cAqYNZK4F94-lZqwtFX2M3pRQ8,9540
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=GakasXPXcBn-VBRsF2DxUGB_bQF4ngxRAa2KOdsj7kY,8671
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=xF-IM-ljjJyc2GWSuiwVVcGzlzirrPhEAv3y8qAWobU,6057
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=E0SjNZiSmjte8UHPu9yebCFPjzg2-mF3Z7U45cd9KU8,9028
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Av5-ayC8GFdNFXplPsBr3CBhfc_7yoiz3AICrMVdShQ,7108
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=6yf0nb_AfOsEmyaea5ywDy2q0N1tgfY_fimis4HG3YY,7112
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=lFwovBDK4mmX3Y6B34v--dv-2975e1va6aAtFQ70Ie4,6110
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=XaPV0vLLQ0PrP1_r9dmJ8BlEkfaQ9dHJROGTjqv4t2Q,23164
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
-build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=E0SjNZiSmjte8UHPu9yebCFPjzg2-mF3Z7U45cd9KU8,9028
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Av5-ayC8GFdNFXplPsBr3CBhfc_7yoiz3AICrMVdShQ,7108
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
 build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
+build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
 build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
-build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=E0SjNZiSmjte8UHPu9yebCFPjzg2-mF3Z7U45cd9KU8,9028
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Av5-ayC8GFdNFXplPsBr3CBhfc_7yoiz3AICrMVdShQ,7108
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
 build/lib/build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
+build/lib/build/lib/build/lib/build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/build/lib/build/lib/build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
 build/lib/build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
-build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
+build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=tTvb9t_vO-ZwMivy5p1M66zx70oEigyd0sVsZQlgeu8,13017
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
-build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=E0SjNZiSmjte8UHPu9yebCFPjzg2-mF3Z7U45cd9KU8,9028
-build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Av5-ayC8GFdNFXplPsBr3CBhfc_7yoiz3AICrMVdShQ,7108
+build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=PWU65G5kARp5A3saSLI01ieAe2JWgnY0ObmHTrfcF-Y,9630
+build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=xsWQk4Z8GJWhvFC9LIoTznzYBHR88MwsJH50l96mbyE,7072
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
 build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
-build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
+build/lib/build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=EkTPWUgSrPVfz19RQJAaT09kqYyrkES8P15xLEayVwQ,25822
+build/lib/build/lib/build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/build/lib/build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
 build/lib/build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
-build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+build/lib/build/lib/build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
 build/lib/build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=XQOQjmXNAaX5aNeD0SPGLSSqU2dBksXdhOR1acALwgY,11332
+build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=2SYsOuJQZRFbtfLe5-tIQUVcQahHFozmIfUAtK3atPY,14940
 build/lib/build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
-build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=E0SjNZiSmjte8UHPu9yebCFPjzg2-mF3Z7U45cd9KU8,9028
-build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Av5-ayC8GFdNFXplPsBr3CBhfc_7yoiz3AICrMVdShQ,7108
+build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=z1PxcQhD6echdvaDRu9O_gLhCvu7bb2ixqBbesHGrkA,9632
+build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=t_5cGYVMpNkdY4751jeggRKQ_E5yqoRl8y_IBcz2BEw,8427
 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
-build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
+build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=9sfCvqk7_KZPSC7VIzeDEURiHJDA2b9dUefJRTx5rkU,8170
 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
-build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
-build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=f_Pa-mno9bDVRga2LhTAcoQ3jtVRLjuJlMVEFW5cnq4,23168
+build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=TI-8V3DznKtmewZWuHKGYIzzZmAolaj89bPGdO1VyIg,6343
+build/lib/build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=BcH_2wSJsC_6ind9wDG7OGbciKPiQirR4WxPVdSUWsk,26085
+build/lib/build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
 build/lib/build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
-build/lib/build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+build/lib/build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
 build/lib/build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=tTvb9t_vO-ZwMivy5p1M66zx70oEigyd0sVsZQlgeu8,13017
+build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=Fkt_i2AGZcmsiitGbLyRqwLhbID-5eR8BdaOC6GgEVQ,15437
 build/lib/build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
-build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=PWU65G5kARp5A3saSLI01ieAe2JWgnY0ObmHTrfcF-Y,9630
-build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=xsWQk4Z8GJWhvFC9LIoTznzYBHR88MwsJH50l96mbyE,7072
+build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=z1PxcQhD6echdvaDRu9O_gLhCvu7bb2ixqBbesHGrkA,9632
+build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=t_5cGYVMpNkdY4751jeggRKQ_E5yqoRl8y_IBcz2BEw,8427
 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
-build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=0HVuLQl4q7-HkJWGd1dJkss-Dg3WXYVJZl3CkEAGvJI,6613
+build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=I88UTBnPqwmrZ8aZ-uUftF-28_7P14Dff8IjoiepR_A,8359
 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
-build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=OANRlZ5PlGypf36dXPaXbQTwQ7PLQ1BgnFXyWs0RpXg,6290
-build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=EkTPWUgSrPVfz19RQJAaT09kqYyrkES8P15xLEayVwQ,25822
+build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=TI-8V3DznKtmewZWuHKGYIzzZmAolaj89bPGdO1VyIg,6343
+build/lib/build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=BcH_2wSJsC_6ind9wDG7OGbciKPiQirR4WxPVdSUWsk,26085
+build/lib/tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+build/lib/tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
 build/lib/tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 build/lib/uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
-build/lib/uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+build/lib/uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
 build/lib/uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
 build/lib/uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=2SYsOuJQZRFbtfLe5-tIQUVcQahHFozmIfUAtK3atPY,14940
+build/lib/uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=Fkt_i2AGZcmsiitGbLyRqwLhbID-5eR8BdaOC6GgEVQ,15437
 build/lib/uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
 build/lib/uav_collision_avoidance/src/simulation/simulation.py,sha256=z1PxcQhD6echdvaDRu9O_gLhCvu7bb2ixqBbesHGrkA,9632
 build/lib/uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=t_5cGYVMpNkdY4751jeggRKQ_E5yqoRl8y_IBcz2BEw,8427
 build/lib/uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
-build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=9sfCvqk7_KZPSC7VIzeDEURiHJDA2b9dUefJRTx5rkU,8170
+build/lib/uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=I88UTBnPqwmrZ8aZ-uUftF-28_7P14Dff8IjoiepR_A,8359
 build/lib/uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
 build/lib/uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
 build/lib/uav_collision_avoidance/src/simulation/simulation_state.py,sha256=TI-8V3DznKtmewZWuHKGYIzzZmAolaj89bPGdO1VyIg,6343
 build/lib/uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=BcH_2wSJsC_6ind9wDG7OGbciKPiQirR4WxPVdSUWsk,26085
+tests/__init__.py,sha256=CjtH_91mhcVIs0X4o6y5BwuOR-i-ftzaddfNfwpjFlw,76
+tests/test_headless.py,sha256=djVoykXQaJAnlLCH6oqDIl9W3Q2pbLU_lCjRR0VdkUE,150
 tests/test_sample.py,sha256=iSdvIjN0pJhhnnrvTowieDMMnjU1HcZycfH0PK5lhEo,107
 uav_collision_avoidance/__init__.py,sha256=fE4gQOSVcsNLjTsO_Efa39pHqkC6Fjj6nCMGp0twYDw,121
-uav_collision_avoidance/main.py,sha256=kXX-REh00037lwvz5n2EAci-9f2nYYAAAkypW1lDpJU,2203
+uav_collision_avoidance/main.py,sha256=vULBW9vRae2Jdm70S2SDobcDSEBTZSeLi2W_Qf_Lre8,2756
 uav_collision_avoidance/version.py,sha256=I6WvYCjHdTuOXOG8owwghajl8vOW_aevumGXnBl_sPk,238
-uav_collision_avoidance/src/aircraft/aircraft.py,sha256=HbmkQi8lHpJHZL8KBCa3DTzw2q3ybdg7OTHz0eCXJAY,1662
-uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=Fkt_i2AGZcmsiitGbLyRqwLhbID-5eR8BdaOC6GgEVQ,15437
-uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=Hdc1sQujBzdVMM5q5TsVDyJCyIxm7xi8S5FXD9WHJ8g,4195
-uav_collision_avoidance/src/simulation/simulation.py,sha256=z1PxcQhD6echdvaDRu9O_gLhCvu7bb2ixqBbesHGrkA,9632
-uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=t_5cGYVMpNkdY4751jeggRKQ_E5yqoRl8y_IBcz2BEw,8427
-uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=fBVukWmBt1md9Klep9J7_WqpzRIDWYHpdo4o8UZyvk0,1979
-uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=I88UTBnPqwmrZ8aZ-uUftF-28_7P14Dff8IjoiepR_A,8359
-uav_collision_avoidance/src/simulation/simulation_render.py,sha256=_Mb1k6Y1mRHtejgWByU-MmAIx4cSmwVBtaBqao0nrLk,1041
+uav_collision_avoidance/src/aircraft/aircraft.py,sha256=23SeHrgKtbezoqGvhVIE_AZbbjrIVj4vHnZOHwshkLc,2581
+uav_collision_avoidance/src/aircraft/aircraft_fcc.py,sha256=-6-156IixgXQuNUVwRlw24lW-XtVZ8fsVpaUff2gZhQ,21654
+uav_collision_avoidance/src/aircraft/aircraft_vehicle.py,sha256=C_VfEV9bem5Sc5WBkzbOKE5KhCdg_iK-UDZLQEevTb4,7090
+uav_collision_avoidance/src/simulation/simulation.py,sha256=y6wPXiJ0E5Tc4iSDNdK9Kx3hl_M1doVSeg_xcy1UI4M,11968
+uav_collision_avoidance/src/simulation/simulation_adsb.py,sha256=Mmb1oUnLIIuEW-7VlQtxBp7jk_fn_G4eY_3ExSXoUbE,11341
+uav_collision_avoidance/src/simulation/simulation_fps.py,sha256=GjCbtaO8b_EgyeXDTq-HYkEzkUk43C3B98FXlGyF2IM,2642
+uav_collision_avoidance/src/simulation/simulation_physics.py,sha256=sPUa2yy65WO4d77DRqdhbkXJLELF0V9hrKIa707d4C0,9854
+uav_collision_avoidance/src/simulation/simulation_render.py,sha256=kuetZego3MlHWVbPuZ_QeiKYqhYvj_-trccDYjkUbM0,1341
 uav_collision_avoidance/src/simulation/simulation_settings.py,sha256=gL0BI6DecE8MYBNex8-KMgNVqpUWuFoOo65chOypXi0,682
-uav_collision_avoidance/src/simulation/simulation_state.py,sha256=TI-8V3DznKtmewZWuHKGYIzzZmAolaj89bPGdO1VyIg,6343
-uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=BcH_2wSJsC_6ind9wDG7OGbciKPiQirR4WxPVdSUWsk,26085
-uav_collision_avoidance-0.6.4.dist-info/LICENSE,sha256=VCiagDkTdM8_xItFjcyMl-mMsGbzL1CQEXpynU0QLxY,1075
-uav_collision_avoidance-0.6.4.dist-info/METADATA,sha256=rXTCMrVyaaUh05zJSDcw0LYyHz0GCJ0-ZNR5t3HMf5s,7374
-uav_collision_avoidance-0.6.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-uav_collision_avoidance-0.6.4.dist-info/entry_points.txt,sha256=fcy0NnMoUjf7wZty5G169lvrCzHpWtJXyQuYsEGyg3k,73
-uav_collision_avoidance-0.6.4.dist-info/top_level.txt,sha256=miPZH4d_mAR-Tj76v8c0YFs_CNl1TTT4Yf7zwcPSuwY,58
-uav_collision_avoidance-0.6.4.dist-info/RECORD,,
+uav_collision_avoidance/src/simulation/simulation_state.py,sha256=TBbtPf_11O24uy3X4ESEqNh2AwGWPjF9bVMuYFxfUKg,16393
+uav_collision_avoidance/src/simulation/simulation_widget.py,sha256=mupJrVx0_6OFlPLFOIhTg46sJIuKOY7cnUj1JYQkrGQ,29872
+uav_collision_avoidance-0.6.6.dist-info/LICENSE,sha256=VCiagDkTdM8_xItFjcyMl-mMsGbzL1CQEXpynU0QLxY,1075
+uav_collision_avoidance-0.6.6.dist-info/METADATA,sha256=UiwzXbcv3fjCF8Id6ElPiKwbVjSSXO5IxCxwIOcdrx4,7677
+uav_collision_avoidance-0.6.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+uav_collision_avoidance-0.6.6.dist-info/entry_points.txt,sha256=fcy0NnMoUjf7wZty5G169lvrCzHpWtJXyQuYsEGyg3k,73
+uav_collision_avoidance-0.6.6.dist-info/top_level.txt,sha256=miPZH4d_mAR-Tj76v8c0YFs_CNl1TTT4Yf7zwcPSuwY,58
+uav_collision_avoidance-0.6.6.dist-info/RECORD,,
```

