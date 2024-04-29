# Comparing `tmp/qnngds-2.1.3.tar.gz` & `tmp/qnngds-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-2.1.3.tar", last modified: Mon Apr 29 12:54:28 2024, max compression
+gzip compressed data, was "qnngds-2.2.0.tar", last modified: Mon Apr 29 14:33:23 2024, max compression
```

## Comparing `qnngds-2.1.3.tar` & `qnngds-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2024-04-29 12:54:25.484662 qnngds-2.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-04-29 12:54:25.484662 qnngds-2.1.3/README.md
--rw-r--r--   0        0        0     1161 2024-04-29 12:54:28.448674 qnngds-2.1.3/pyproject.toml
--rw-r--r--   0        0        0      536 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/__init__.py
--rw-r--r--   0        0        0      290 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/_default_param.py
--rw-r--r--   0        0        0    23463 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/cells.py
--rw-r--r--   0        0        0    10495 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/circuits.py
--rw-r--r--   0        0        0    28385 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/design.py
--rw-r--r--   0        0        0      158 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/__init__.py
--rw-r--r--   0        0        0      231 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/htron.py
--rw-r--r--   0        0        0     1214 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/nanowire.py
--rw-r--r--   0        0        0     4526 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/ntron.py
--rw-r--r--   0        0        0     5935 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/resistor.py
--rw-r--r--   0        0        0     2443 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/devices/snspd.py
--rw-r--r--   0        0        0     1237 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/geometries.py
--rw-r--r--   0        0        0     7925 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/tests.py
--rw-r--r--   0        0        0    21046 2024-04-29 12:54:25.500662 qnngds-2.1.3/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-29 14:33:20.279993 qnngds-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-04-29 14:33:20.279993 qnngds-2.2.0/README.md
+-rw-r--r--   0        0        0     1161 2024-04-29 14:33:23.131995 qnngds-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-29 14:33:20.299993 qnngds-2.2.0/src/qnngds/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-29 14:33:20.299993 qnngds-2.2.0/src/qnngds/_default_param.py
+-rw-r--r--   0        0        0    27606 2024-04-29 14:33:20.299993 qnngds-2.2.0/src/qnngds/cells.py
+-rw-r--r--   0        0        0    10495 2024-04-29 14:33:20.299993 qnngds-2.2.0/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    29823 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/design.py
+-rw-r--r--   0        0        0      158 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/devices/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/devices/htron.py
+-rw-r--r--   0        0        0     1214 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/devices/nanowire.py
+-rw-r--r--   0        0        0     4526 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/devices/ntron.py
+-rw-r--r--   0        0        0     5935 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/devices/resistor.py
+-rw-r--r--   0        0        0     2548 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/devices/snspd.py
+-rw-r--r--   0        0        0     1237 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/geometries.py
+-rw-r--r--   0        0        0     7925 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/tests.py
+-rw-r--r--   0        0        0    28047 2024-04-29 14:33:20.303993 qnngds-2.2.0/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.2.0/PKG-INFO
```

### Comparing `qnngds-2.1.3/LICENSE.txt` & `qnngds-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/README.md` & `qnngds-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/pyproject.toml` & `qnngds-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "2.1.3"
+version = "2.2.0"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-2.1.3/src/qnngds/__init__.py` & `qnngds-2.2.0/src/qnngds/__init__.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/src/qnngds/cells.py` & `qnngds-2.2.0/src/qnngds/cells.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Library of pre-built cells containing text, border marks, and an experiment,
 connected to pads for wirebonding."""
 
 from phidl import Device
 import phidl.geometry as pg
 import phidl.routing as pr
-from typing import Tuple, List, Union
+from typing import Tuple, List, Union, Optional
 import math
 
 import qnngds.tests as test
 import qnngds.devices as device
 import qnngds.circuits as circuit
 import qnngds.utilities as utility
 import qnngds._default_param as dflt
@@ -219,15 +219,15 @@
     n = math.ceil((TEST.xsize + 2 * dflt.die_cell_border) / die_w)
     m = math.ceil((TEST.ysize + 2 * dflt.die_cell_border) / die_w)
     BORDER = utility.die_cell(
         die_size=(n * die_w, m * die_w),
         ports={},
         ports_gnd={},
         text=f"ETCH TEST {text}",
-        isolation=10,
+        isolation=outline_die,
         layer=die_layer,
         invert=True,
     )
 
     BORDER.move(TEST.center)
     DIE_ETCH_TEST << BORDER.flatten()
     DIE_ETCH_TEST << TEST
@@ -321,19 +321,23 @@
     pad_layer: int = dflt.layers["pad"],
     text: Union[None, str] = dflt.text,
 ) -> Device:
     """Creates a cell that contains several nanowires of given channel and
     source.
 
     Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        channels_sources_w (list of tuple of float): The list of (channel_w, source_w) of the nanowires to create.
-        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
-                                   (useful for ebeam lithography).
+        die_w (int or float): Width of a unit die/cell in the design (the output
+            device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width,
+            height).
+        channels_sources_w (list of tuple of float): The list of (channel_w,
+            source_w) of the nanowires to create.
+        overlap_w (int or float): Extra length of the routes above the die's
+            ports to assure alignment with the device (useful for ebeam
+            lithography).
         outline_die (int or float): The width of the pads outline.
         outline_dev (int or float): The width of the device's outline.
         device_layer (int or tuple of int): The layer where the device is placed.
         die_layer (int or tuple of int): The layer where the die is placed.
         pad_layer (int or tuple of int): The layer where the pads are placed.
         text (str, optional): If None, the text is "NWIRES".
 
@@ -507,15 +511,15 @@
         device_max_size=(device_max_w, device_max_w),
         pad_size=pad_size,
         contact_w=die_contact_w,
         contact_l=overlap_w,
         ports={"N": 1, "W": 1, "S": 1},
         ports_gnd=["S"],
         text=text,
-        isolation=10,
+        isolation=outline_die,
         layer=die_layer,
         pad_layer=pad_layer,
         invert=True,
     )
 
     # place the ntron
     NTRON.movex(NTRON.ports["N1"].midpoint[0], BORDER.ports["N1"].midpoint[0])
@@ -541,14 +545,123 @@
     DIE_NTRON << BORDER
 
     DIE_NTRON = pg.union(DIE_NTRON, by_layer=True)
     DIE_NTRON.name = f"DIE NTRON {text} "
     return DIE_NTRON
 
 
+def snspd(
+    die_w: Union[int, float] = dflt.die_w,
+    pad_size: Tuple[float] = dflt.pad_size,
+    snspd_width: float = 0.2,
+    snspd_pitch: float = 0.6,
+    snspd_size: Tuple[Union[int, float], Union[int, float]] = tuple(
+        x / 2 for x in utility.calculate_available_space_for_dev()
+    ),
+    snspd_num_squares: Optional[int] = None,
+    overlap_w: Union[int, float] = dflt.ebeam_overlap,
+    outline_die: Union[int, float] = dflt.die_outline,
+    outline_dev: Union[int, float] = dflt.device_outline,
+    device_layer: int = dflt.layers["device"],
+    die_layer: int = dflt.layers["die"],
+    pad_layer: int = dflt.layers["pad"],
+    text: Union[None, str] = dflt.text,
+) -> Device:
+    """Creates a cell that contains a vertical superconducting nanowire single-
+    photon detector (SNSPD).
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output
+        device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width,
+            height).
+        snspd_width (float): Width of the nanowire.
+        snspd_pitch (float): Pitch of the nanowire.
+        snspd_size (tuple of int or float): Size of the detector in squares (width, height).
+        snspd_num_squares (Optional[int]): Number of squares in the detector.
+        overlap_w (int or float): Extra length of the routes above the die's
+            ports to assure alignment with the device (useful for ebeam
+            lithography).
+        outline_die (int or float): The width of the pads outline.
+        outline_dev (int or float): The width of the device's outline.
+        device_layer (int or array-like[2]): The layer where the device is placed.
+        die_layer (int or array-like[2]): The layer where the die is placed.
+        pad_layer (int or array-like[2]): The layer where the pads are placed.
+        text (string, optional): If None, text = f'SNSPD {w_choke}'.
+
+    Returns:
+        Device: A cell (of size n*m unit die_cells) containing the SNSPD.
+    """
+    if text is None:
+        text = f"{snspd_width}"
+
+    SNSPD_CELL = Device(f"CELL SNSPD {text} ")
+    DEVICE = Device(f"SNSPD {text} ")
+
+    # create SNSPD, make its ports compass, add safe optimal step
+    SNSPD = device.snspd.vertical(
+        wire_width=snspd_width,
+        wire_pitch=snspd_pitch,
+        size=snspd_size,
+        num_squares=snspd_num_squares,
+        layer=device_layer,
+    )
+    SNSPD = utility.rename_ports_to_compass(SNSPD)
+    SNSPD = utility.add_optimalstep_to_dev(SNSPD, ratio=10)
+    DEVICE << SNSPD
+
+    # create die
+    die_contact_w = utility.calculate_contact_w(
+        circuit_ports=SNSPD.get_ports(), overlap_w=overlap_w
+    )
+    device_max_size = tuple(
+        x + 2 * overlap_w for x in SNSPD.size
+    )  # not valide anymore if pads are not aligned with dev ports
+    n, m = utility.find_num_diecells_for_dev(
+        device_max_size, (die_w, die_w), pad_size, overlap_w, outline_die
+    )
+    BORDER = utility.die_cell(
+        die_size=(n * die_w, m * die_w),
+        device_max_size=device_max_size,
+        pad_size=pad_size,
+        contact_w=die_contact_w,
+        contact_l=overlap_w,
+        ports={"N": 1, "S": 1},
+        ports_gnd=["S"],
+        text=f"SNSPD {text}",
+        isolation=outline_die,
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+    )
+
+    # add hyper tapers at die pads
+    dev_contact_w = SNSPD.ports["N1"].width
+    HT, dev_ports = utility.add_hyptap_to_cell(
+        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
+    )
+    DEVICE.ports = dev_ports.ports
+    DEVICE << HT
+
+    # link hyper tapers to the device
+    ROUTES = utility.route_to_dev(
+        HT.get_ports(), SNSPD.ports
+    )  # absolutly no need to route, but will be useful when ports are no longer aligned with pads
+    DEVICE << ROUTES
+
+    DEVICE = pg.outline(
+        DEVICE, outline_dev, open_ports=2 * outline_dev, layer=device_layer
+    )
+    DEVICE.name = f"SNSPD {text} "
+
+    SNSPD_CELL << DEVICE
+    SNSPD_CELL << BORDER
+    return SNSPD_CELL
+
+
 def snspd_ntron(
     die_w: Union[int, float] = dflt.die_w,
     pad_size: Tuple[float, float] = dflt.pad_size,
     w_choke: Union[int, float] = 0.1,
     w_snspd: Union[int, float] = dflt.auto_param,
     overlap_w: Union[int, float] = dflt.ebeam_overlap,
     outline_die: Union[int, float] = dflt.die_outline,
```

### Comparing `qnngds-2.1.3/src/qnngds/circuits.py` & `qnngds-2.2.0/src/qnngds/circuits.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/src/qnngds/design.py` & `qnngds-2.2.0/src/qnngds/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     useful_area = CHIP.add_polygon(
         [(0, 0), (useful_w, 0), (useful_w, useful_w), (0, useful_w)],
         layer=annotations_layer,
     )
     useful_area.move((margin, margin))
 
     if die_w is not None:
-        N_dies = useful_w / die_w
+        N_dies = int(useful_w / die_w)
         return_N_or_w = N_dies
     else:
         die_w = useful_w / N_dies
         return_N_or_w = die_w
     CELL = pg.rectangle([die_w, die_w], layer=annotations_layer)
     array = CHIP.add_array(CELL, columns=N_dies, rows=N_dies, spacing=(die_w, die_w))
     array.move((0, 0), (margin, margin))
@@ -286,16 +286,16 @@
     """
 
     def __init__(
         self,
         name="new_design",
         chip_w=dflt.chip_w,
         chip_margin=dflt.chip_margin,
-        N_dies=dflt.N_dies,
-        die_w=dflt.auto_param,
+        N_dies=dflt.auto_param,
+        die_w=dflt.die_w,
         pad_size=dflt.pad_size,
         device_outline=dflt.device_outline,
         die_outline=dflt.die_outline,
         ebeam_overlap=dflt.ebeam_overlap,
         annotation_layer=dflt.layers["annotation"],
         device_layer=dflt.layers["device"],
         die_layer=dflt.layers["die"],
@@ -678,14 +678,52 @@
             overlap_w=self.ebeam_overlap,
             outline_die=self.die_outline,
             outline_dev=self.device_outline,
             device_layer=self.layers["device"],
             die_layer=self.layers["die"],
             pad_layer=self.layers["pad"],
             text=text,
+        )
+
+    def snspd_cell(
+        self,
+        snspd_width: float = 0.2,
+        snspd_pitch: float = 0.6,
+        snspd_size: Tuple[Union[int, float], Union[int, float]] = (100, 100),
+        snspd_num_squares: Optional[int] = None,
+        text: Union[None, str] = dflt.text,
+    ) -> Device:
+        """Creates a cell that contains a vertical superconducting nanowire
+        single-photon detector (SNSPD).
+
+        Parameters:
+            snspd_width (float): Width of the nanowire.
+            snspd_pitch (float): Pitch of the nanowire.
+            snspd_size (tuple of int or float): Size of the detector in squares (width, height).
+            snspd_num_squares (Optional[int]): Number of squares in the detector.
+            text (string, optional): If None, text = f'SNSPD {w_choke}'.
+
+        Returns:
+            Device: A cell (of size n*m unit die_cells) containing the SNSPD.
+        """
+
+        return cell.snspd(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            snspd_width=snspd_width,
+            snspd_pitch=snspd_pitch,
+            size=snspd_size,
+            num_squares=snspd_num_squares,
+            overlap_w=self.ebeam_overlap,
+            outline_die=self.die_outline,
+            outline_dev=self.device_outline,
+            device_layer=self.layers["device"],
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
         )
 
     def snspd_ntron_cell(
         self,
         w_choke: float,
         w_snspd: Union[float, None] = dflt.auto_param,
         text: Union[str, None] = dflt.text,
```

### Comparing `qnngds-2.1.3/src/qnngds/devices/nanowire.py` & `qnngds-2.2.0/src/qnngds/devices/nanowire.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/src/qnngds/devices/ntron.py` & `qnngds-2.2.0/src/qnngds/devices/ntron.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/src/qnngds/devices/resistor.py` & `qnngds-2.2.0/src/qnngds/devices/resistor.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/src/qnngds/devices/snspd.py` & `qnngds-2.2.0/src/qnngds/devices/snspd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Superconducting nanowire single photon detector geometries."""
 
 from phidl import Device
 
 import phidl.geometry as pg
-from typing import Tuple, Optional
+from typing import Tuple, Optional, Union
 
 
 def vertical(
     wire_width: float = 0.2,
     wire_pitch: float = 0.6,
-    size: Tuple[int, int] = (6, 10),
+    size: Tuple[Union[int, float], Union[int, float]] = (6, 10),
     num_squares: Optional[int] = None,
     terminals_same_side: bool = False,
     extend: Optional[float] = None,
     layer: int = 0,
 ) -> Device:
     """Creates a vertical superconducting nanowire single-photon detector
     (SNSPD).
 
     Args:
         wire_width (float): Width of the nanowire.
         wire_pitch (float): Pitch of the nanowire.
-        size (Tuple[int, int]): Size of the detector in squares (width, height).
+        size (tuple of int or float): Size of the detector in squares (width, height).
         num_squares (Optional[int]): Number of squares in the detector.
         terminals_same_side (bool): Whether the terminals are on the same side of the detector.
         extend (Optional[bool]): Whether or not to extend the ports.
         layer (int): Layer for the device to be created on.
 
     Returns:
         Device: The vertical SNSPD device.
     """
-    D = Device("snspd_vert")
+    D = Device("SNSPD VERTICAL")
+
     S = pg.snspd(
         wire_width=wire_width,
         wire_pitch=wire_pitch,
         size=size,
         num_squares=num_squares,
         terminals_same_side=terminals_same_side,
         layer=layer,
@@ -74,8 +75,10 @@
         D.add_port(name=1, port=e1.ports[2])
         D.add_port(name=2, port=e2.ports[2])
     else:
         D.add_port(name=1, port=t1.ports[2])
         D.add_port(name=2, port=t2.ports[2])
 
     D.info = S.info
+    D.move(D.center, (0, 0))
+    D.name = "SNSPD VERTICAL"
     return D
```

### Comparing `qnngds-2.1.3/src/qnngds/geometries.py` & `qnngds-2.2.0/src/qnngds/geometries.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/src/qnngds/tests.py` & `qnngds-2.2.0/src/qnngds/tests.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.3/src/qnngds/utilities.py` & `qnngds-2.2.0/src/qnngds/utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 import phidl.geometry as pg
 import phidl.routing as pr
 from typing import Tuple, List, Union, Dict, Set
 from phidl.device_layout import (
     Device,
     Port,
 )
-import qnngds.geometries as qg
+import qnngds.geometries as geometry
 import qnngds._default_param as dflt
 
-
-die_cell_border = 80
+die_cell_border = dflt.die_cell_border
 
 
 def die_cell(
-    die_size: Tuple[int, int] = (dflt.die_w, dflt.die_w),
-    device_max_size: Tuple[int, int] = (100, 100),
-    pad_size: Tuple[int, int] = dflt.pad_size,
+    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
+    device_max_size: Tuple[Union[int, float], Union[int, float]] = (
+        round(dflt.die_w / 3),
+        round(dflt.die_w / 3),
+    ),
+    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
     contact_w: Union[int, float] = 50,
     contact_l: Union[int, float] = dflt.ebeam_overlap,
     ports: Dict[str, int] = {"N": 1, "E": 1, "W": 1, "S": 1},
     ports_gnd: List[str] = ["E", "S"],
     isolation: Union[int, float] = dflt.die_outline,
     text: str = "",
     text_size: Union[int, float] = die_cell_border / 2,
@@ -35,17 +37,17 @@
     pad_layer: int = dflt.layers["pad"],
     invert: bool = False,
 ) -> Device:
     """Creates a die cell with dicing marks, text, and pads to connect to a
     device.
 
     Parameters:
-        die_size (tuple of int): Overall size of the cell (width, height).
-        device_max_size (tuple of int): Max dimensions of the device inside the cell (width, height).
-        pad_size (tuple of int): Dimensions of the cell's pads (width, height).
+        die_size (tuple of int or float): Overall size of the cell (width, height).
+        device_max_size (tuple of int or float): Max dimensions of the device inside the cell (width, height).
+        pad_size (tuple of int or float): Dimensions of the cell's pads (width, height).
         contact_w (int or float): Width of the ports and route to be connected to a device.
         contact_l (int or float): Extra length of the routes above the ports to assure alignment with the device
                                    (useful for ebeam lithography).
         ports (dict): The ports of the device, format must be {'N':m, 'E':n, 'W':p, 'S':q}.
         ports_gnd (list of string): The ports connected to ground.
         isolation (int or float): The width of the pads outline.
         text (string): The text to be displayed on the cell.
@@ -162,22 +164,208 @@
 
     DIE.flatten()
     ports = DIE.get_ports()
     DIE = pg.union(DIE, by_layer=True)
     if invert:
         PADS = pg.deepcopy(DIE)
         PADS.remove_layers([layer])
+        PADS.name = "pads"
         DIE = pg.invert(DIE, border=0, layer=layer)
         DIE << PADS
     for port in ports:
         DIE.add_port(port)
     DIE.name = f"DIE {text}"
     return DIE
 
 
+def calculate_available_space_for_dev(
+    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
+    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
+    contact_l: Union[int, float] = dflt.ebeam_overlap,
+    isolation: Union[int, float] = dflt.die_outline,
+) -> Tuple[float, float]:
+    """Calculates the maximum space available for a device in a die_cell.
+
+    Note that the device should be even smaller than this function's output, as
+    it does not account for routing from the device to the die's ports.
+
+    Parameters:
+        die_size (tuple of int or float): Overall size of the cell (width, height).
+        pad_size (tuple of int or float): Dimensions of the cell's pads (width, height).
+        contact_l (int or float): Extra length of the routes above the ports to
+            assure alignment with the device (useful for ebeam lithography).
+        isolation (int or float): The width of the pads outline.
+
+    Returns:
+        Tuple[float, float]: A tuple containing the width and height of space
+        available for a device in a die_cell
+    """
+
+    dev_max_size = [
+        2 * (die_w / 2 - 3 * isolation - pad_size[1] - 2 * contact_l)
+        for die_w in die_size
+    ]
+    return dev_max_size[0], dev_max_size[1]
+
+
+def calculate_contact_w(
+    circuit_ports: List[Port] = [Port(width=50)],
+    overlap_w: Union[int, float] = dflt.ebeam_overlap,
+) -> Union[int, float]:
+    """Calculate the minimal width acceptable for the contact from the die_cell
+    to the circuit/experiment.
+
+    The conditions are that the contact width should be bigger than (1) the
+    biggest port of the circuit, (2) the overlap_w (to avoid a short).
+
+    Parameters:
+        circuit_ports (list of Port): The ports of the circuit to be placed in the
+            cell (use .get_ports()).
+        overlap_w (int or float): The overlap width in µm (accounts for
+            misalignment between 1st and 2nd ebeam exposures).
+
+    Returns:
+        (int or float): the suggested contact_w to input in the die_cell of the
+        given circuit
+    """
+    max_circuit_port_width = max([port.width for port in circuit_ports])
+    return max(max_circuit_port_width, overlap_w)
+
+
+def add_optimalstep_to_dev(
+    DEVICE: Device, ratio: Union[int, float] = 10, layer: int = dflt.layers["device"]
+) -> Device:
+    """Add an optimal step to the device's ports.
+
+    Note that the subports of the input Device are ignored but still conserved
+    in the returned device.
+
+    Parameters:
+        DEVICE (Device): The Phidl Device to add the optimal steps to.
+        ratio (int or float): the ratio between the width at the end of the step
+            and the width of the device's ports.
+        layer (int or array-like[2]): the layer to place the optimal steps into.
+
+    Returns:
+        (Device): The given Device, with additional steps on its ports. The
+        ports of the returned device have the same name than the ports of the
+        input device and correspond to the steps extremities.
+    """
+    DEV_STP = Device(DEVICE.name)
+
+    DEV_STP << DEVICE
+    for port in DEVICE.flatten().get_ports():
+        STP = pg.optimal_step(
+            port.width, port.width * ratio, symmetric=True, layer=layer
+        )
+        STP.name = f"optimal step x{ratio} "
+        stp = DEV_STP << STP
+        stp.connect(port=1, destination=port)
+        DEV_STP.add_port(port=stp.ports[2], name=port.name)
+
+    return DEV_STP
+
+
+def find_num_diecells_for_dev(
+    device_max_size: Tuple[Union[int, float], Union[int, float]] = (
+        dflt.die_w,
+        dflt.die_w,
+    ),
+    die_size: Tuple[Union[int, float], Union[int, float]] = (dflt.die_w, dflt.die_w),
+    pad_size: Tuple[Union[int, float], Union[int, float]] = dflt.pad_size,
+    contact_l: Union[int, float] = dflt.ebeam_overlap,
+    isolation: Union[int, float] = dflt.die_outline,
+) -> Tuple[float, float]:
+    """Finds the number of die cells that can accommodate a device.
+
+    Parameters:
+        device_max_size(tuple of int or float, optional): Max dimensions of the
+            device inside the cell (width, height).
+        die_size(tuple of int or float, optional): Overall size of the cell (width,
+            height).
+        pad_size(tuple of int or float, optional): Dimensions of the cell's pads
+            (width, height).
+        contact_l (Union[int, float], optional): Extra length of the routes
+            above the ports to assure alignment with the device (useful for
+            ebeam lithography).
+        isolation (Union[int, float], optional): The width of the pads outline.
+
+    Returns:
+        Tuple[float, float]: A tuple containing the number of die cells in width
+        and height required to accommodate the device
+    """
+    n = 1
+    dev_x_bigger = True
+
+    while dev_x_bigger:
+        available_space_for_dev = calculate_available_space_for_dev(
+            (n * die_size[0], die_size[1]), pad_size, contact_l, isolation
+        )
+
+        if device_max_size[0] > available_space_for_dev[0]:
+            n += 1
+        else:
+            break
+
+    m = 1
+    dev_y_bigger = True
+
+    while dev_y_bigger:
+        available_space_for_dev = calculate_available_space_for_dev(
+            (n * die_size[0], m * die_size[1]), pad_size, contact_l, isolation
+        )
+
+        if device_max_size[1] > available_space_for_dev[1]:
+            m += 1
+        else:
+            break
+
+    return n, m
+
+
+def rename_ports_to_compass(DEVICE: Device) -> Device:
+    """Rename ports of a Device based on compass directions.
+
+    Parameters:
+        DEVICE (Device): The Phidl Device object whose ports are to be renamed.
+
+    Returns:
+        Device: A new Phidl Device object with ports renamed to compass directions.
+    """
+    # Create a new Device object to store renamed ports
+    DEV_COMPASS = Device(DEVICE.name)
+
+    # Copy ports from the original device to the new device
+    DEV_COMPASS << DEVICE.flatten()
+
+    # Initialize counters for each direction
+    E_count = 1
+    N_count = 1
+    W_count = 1
+    S_count = 1
+
+    # Iterate through each port in the original device
+    for port in DEVICE.get_ports():
+        # Determine the orientation of the port and rename it accordingly
+        if port.orientation % 360 == 0:
+            DEV_COMPASS.add_port(port=port, name=f"E{E_count}")
+            E_count += 1
+        elif port.orientation % 360 == 90:
+            DEV_COMPASS.add_port(port=port, name=f"N{N_count}")
+            N_count += 1
+        elif port.orientation % 360 == 180:
+            DEV_COMPASS.add_port(port=port, name=f"W{W_count}")
+            W_count += 1
+        elif port.orientation % 360 == 270:
+            DEV_COMPASS.add_port(port=port, name=f"S{S_count}")
+            S_count += 1
+
+    return DEV_COMPASS
+
+
 def add_hyptap_to_cell(
     die_ports: List[Port],
     overlap_w: Union[int, float] = dflt.ebeam_overlap,
     contact_w: Union[int, float] = 5,
     layer: int = dflt.layers["device"],
 ) -> Tuple[Device, Device]:
     """Takes the cell and adds hyper taper at its ports.
@@ -201,15 +389,15 @@
     """
 
     HT = Device("HYPER TAPERS ")
     device_ports = Device()
 
     for port in die_ports:
         ht_w = port.width + 2 * overlap_w
-        ht = HT << qg.hyper_taper(overlap_w, ht_w, contact_w)
+        ht = HT << geometry.hyper_taper(overlap_w, ht_w, contact_w)
         ht.connect(ht.ports[2], port)
         HT.add_port(port=ht.ports[1], name=port.name)
         device_ports.add_port(port=ht.ports[2], name=port.name)
 
     HT.flatten(single_layer=layer)
     return HT, device_ports
```

### Comparing `qnngds-2.1.3/PKG-INFO` & `qnngds-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 2.1.3
+Version: 2.2.0
 Summary: The QNN library for creating gds files
 Keywords: phidl,nanowire_electronics,nanofabrication,gds
 Author-Email: "A. Jacquillat" <audrey01@mit.edu>, "A. Jacquillat" <audrey.jacquillat@gmail.com>, "R. Foster" <reedf@mit.edu>
 Maintainer-Email: "A. Jacquillat" <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

