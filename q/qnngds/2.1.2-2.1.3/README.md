# Comparing `tmp/qnngds-2.1.2.tar.gz` & `tmp/qnngds-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-2.1.2.tar", last modified: Mon Apr 29 12:50:07 2024, max compression
+gzip compressed data, was "qnngds-2.1.3.tar", last modified: Mon Apr 29 12:54:28 2024, max compression
```

## Comparing `qnngds-2.1.2.tar` & `qnngds-2.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2024-04-29 12:49:56.717745 qnngds-2.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-04-29 12:49:56.717745 qnngds-2.1.2/README.md
--rw-r--r--   0        0        0     1161 2024-04-29 12:50:07.601842 qnngds-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      508 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/__init__.py
--rw-r--r--   0        0        0      291 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/_default_param.py
--rw-r--r--   0        0        0    23463 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/cells.py
--rw-r--r--   0        0        0    10495 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/circuits.py
--rw-r--r--   0        0        0    28386 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/design.py
--rw-r--r--   0        0        0      160 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/devices/__init__.py
--rw-r--r--   0        0        0      231 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/devices/htron.py
--rw-r--r--   0        0        0     1214 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/devices/nanowire.py
--rw-r--r--   0        0        0     4526 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/devices/ntron.py
--rw-r--r--   0        0        0     5935 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/devices/resistor.py
--rw-r--r--   0        0        0     2443 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/devices/snspd.py
--rw-r--r--   0        0        0     1237 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/geometries.py
--rw-r--r--   0        0        0     7907 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/tests.py
--rw-r--r--   0        0        0    21104 2024-04-29 12:49:56.733745 qnngds-2.1.2/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-29 12:54:25.484662 qnngds-2.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-04-29 12:54:25.484662 qnngds-2.1.3/README.md
+-rw-r--r--   0        0        0     1161 2024-04-29 12:54:28.448674 qnngds-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/_default_param.py
+-rw-r--r--   0        0        0    23463 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/cells.py
+-rw-r--r--   0        0        0    10495 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    28385 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/design.py
+-rw-r--r--   0        0        0      158 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/htron.py
+-rw-r--r--   0        0        0     1214 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/nanowire.py
+-rw-r--r--   0        0        0     4526 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/ntron.py
+-rw-r--r--   0        0        0     5935 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/resistor.py
+-rw-r--r--   0        0        0     2443 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/snspd.py
+-rw-r--r--   0        0        0     1237 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/geometries.py
+-rw-r--r--   0        0        0     7925 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/tests.py
+-rw-r--r--   0        0        0    21046 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.1.3/PKG-INFO
```

### Comparing `qnngds-2.1.2/LICENSE.txt` & `qnngds-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/README.md` & `qnngds-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/pyproject.toml` & `qnngds-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "2.1.2"
+version = "2.1.3"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-2.1.2/src/qnngds/cells.py` & `qnngds-2.1.3/src/qnngds/cells.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/src/qnngds/circuits.py` & `qnngds-2.1.3/src/qnngds/circuits.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/src/qnngds/design.py` & `qnngds-2.1.3/src/qnngds/design.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,14 @@
 
     if devices_to_place:
         print(
             "Some devices are still to be placed, " + "no place remaining on the chip."
         )
 
 
-
 class Design:
     """A class for a design on a single layer of superconducting material, and
     additional contact pads.
 
     It is though for a process like:
 
     - exposing the superconductiong material using e-beam lithography. Two
```

### Comparing `qnngds-2.1.2/src/qnngds/devices/nanowire.py` & `qnngds-2.1.3/src/qnngds/devices/nanowire.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/src/qnngds/devices/ntron.py` & `qnngds-2.1.3/src/qnngds/devices/ntron.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/src/qnngds/devices/resistor.py` & `qnngds-2.1.3/src/qnngds/devices/resistor.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/src/qnngds/devices/snspd.py` & `qnngds-2.1.3/src/qnngds/devices/snspd.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/src/qnngds/geometries.py` & `qnngds-2.1.3/src/qnngds/geometries.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.2/src/qnngds/tests.py` & `qnngds-2.1.3/src/qnngds/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-""" Tests contains common test structures for following/characterizing a
-fabrication process and its effect on the materials. """
+"""Tests contains common test structures for following/characterizing a
+fabrication process and its effect on the materials."""
 
 from phidl import Device
 import phidl.geometry as pg
 from typing import List, Union
 import math
 
+
 def alignment_mark(layers: List[int] = [1, 2, 3, 4]) -> Device:
     """Creates an alignment mark for each photolithography.
 
     Args:
         layers (List[int]): An array of layers.
 
     Returns:
@@ -216,34 +217,32 @@
     RES_TEST = pg.union(RES_TEST, layer=layer)
     RES_TEST.move(RES_TEST.center, (0, 0))
     RES_TEST.name = res_test_name
     return RES_TEST
 
 
 def vdp(l: float = 400, w: float = 40, layer: int = 1) -> Device:
-    """
-    Creates a Van der Pauw (VDP) device with specified dimensions.
+    """Creates a Van der Pauw (VDP) device with specified dimensions.
 
     Args:
         l (float): Length of the VDP device, overall maximum dimension, in µm.
         w (float): Width of the contact points (width of the ports), in µm.
         layer (int): Layer to put the device on.
 
     Returns:
         Device: VDP device object.
-
     """
     VDP = pg.Device("VAN DER PAUW")
-    
-    xpts = [-w/2, w/2, l/2, l/2, w/2, -w/2, -l/2, -l/2]
-    ypts = [l/2, l/2, w/2, -w/2, -l/2, -l/2, -w/2, w/2]
+
+    xpts = [-w / 2, w / 2, l / 2, l / 2, w / 2, -w / 2, -l / 2, -l / 2]
+    ypts = [l / 2, l / 2, w / 2, -w / 2, -l / 2, -l / 2, -w / 2, w / 2]
 
     polygon = pg.polygon_ports(xpts=xpts, ypts=ypts, layer=layer)
     VDP << polygon
     VDP.flatten()
 
-    VDP.add_port(port= polygon.ports['1'], name='N1')
-    VDP.add_port(port= polygon.ports['3'], name='E1')
-    VDP.add_port(port= polygon.ports['5'], name='S1')
-    VDP.add_port(port= polygon.ports['7'], name='W1')
+    VDP.add_port(port=polygon.ports["1"], name="N1")
+    VDP.add_port(port=polygon.ports["3"], name="E1")
+    VDP.add_port(port=polygon.ports["5"], name="S1")
+    VDP.add_port(port=polygon.ports["7"], name="W1")
 
-    return VDP
+    return VDP
```

### Comparing `qnngds-2.1.2/src/qnngds/utilities.py` & `qnngds-2.1.3/src/qnngds/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,16 +213,16 @@
     HT.flatten(single_layer=layer)
     return HT, device_ports
 
 
 def route_to_dev(
     ext_ports: List[Port], dev_ports: Set[Port], layer: int = dflt.layers["device"]
 ) -> Device:
-    """Creates smooth routes from external ports to the device's ports.
-    If route_smooth is not working, routes quad.
+    """Creates smooth routes from external ports to the device's ports. If
+    route_smooth is not working, routes quad.
 
     Parameters:
         ext_ports (list of Port): The external ports, e.g., of the die or hyper tapers (use .get_ports()).
         dev_ports (set of Port): The device's ports, should be named as the external ports (use .ports).
         layer (int or array-like[2]): The layer to put the routes on.
 
     Returns:
@@ -250,18 +250,15 @@
                     dev_port,
                     radius,
                     path_type="Z",
                     length1=length1,
                     length2=length2,
                 )
             except ValueError:
-                ROUTES << pr.route_quad(
-                    port,
-                    dev_port
-                )
+                ROUTES << pr.route_quad(port, dev_port)
     ROUTES.flatten(single_layer=layer)
     return ROUTES
 
 
 # from previous qnngds: to be tested...
 
 # def outline(elements, distance = 1, precision = 1e-4, num_divisions = [1, 1],
```

### Comparing `qnngds-2.1.2/PKG-INFO` & `qnngds-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 2.1.2
+Version: 2.1.3
 Summary: The QNN library for creating gds files
 Keywords: phidl,nanowire_electronics,nanofabrication,gds
 Author-Email: "A. Jacquillat" <audrey01@mit.edu>, "A. Jacquillat" <audrey.jacquillat@gmail.com>, "R. Foster" <reedf@mit.edu>
 Maintainer-Email: "A. Jacquillat" <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

