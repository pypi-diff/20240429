# Comparing `tmp/pydfuutil-0.0.2b0.tar.gz` & `tmp/pydfuutil-0.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydfuutil-0.0.2b0.tar", last modified: Tue Mar 26 12:40:30 2024, max compression
+gzip compressed data, was "pydfuutil-0.0.2b1.tar", last modified: Mon Apr 29 19:08:06 2024, max compression
```

## Comparing `pydfuutil-0.0.2b0.tar` & `pydfuutil-0.0.2b1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:40:30.905809 pydfuutil-0.0.2b0/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-03-26 12:40:30.905809 pydfuutil-0.0.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:40:30.905809 pydfuutil-0.0.2b0/pydfuutil/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    19172 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/portable.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/quirks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pydfuutil/usb_dfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:40:30.905809 pydfuutil-0.0.2b0/pydfuutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-03-26 12:40:30.000000 pydfuutil-0.0.2b0/pydfuutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-26 12:40:30.000000 pydfuutil-0.0.2b0/pydfuutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 12:40:30.000000 pydfuutil-0.0.2b0/pydfuutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 12:40:30.000000 pydfuutil-0.0.2b0/pydfuutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-26 12:40:30.000000 pydfuutil-0.0.2b0/pydfuutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 12:40:30.000000 pydfuutil-0.0.2b0/pydfuutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 12:40:30.905809 pydfuutil-0.0.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:40:30.905809 pydfuutil-0.0.2b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/tests/test_dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-26 12:40:15.000000 pydfuutil-0.0.2b0/tests/test_dfu_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:08:06.334406 pydfuutil-0.0.2b1/pydfuutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19172 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/portable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/quirks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pydfuutil/usb_dfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/pydfuutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 19:08:06.000000 pydfuutil-0.0.2b1/pydfuutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:08:06.338406 pydfuutil-0.0.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/tests/test_dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-29 19:07:57.000000 pydfuutil-0.0.2b1/tests/test_dfu_load.py
```

### Comparing `pydfuutil-0.0.2b0/LICENSE` & `pydfuutil-0.0.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b0/PKG-INFO` & `pydfuutil-0.0.2b1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.2b0
+Version: 0.0.2b1
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -236,20 +236,117 @@
 
     # the latest official release
     python -m pip install pydfuutil
 
     # install a specific version (e.g. 0.0.1b1)
     python -m pip install pydfuutil==0.0.1b1
 
+## Usage
+
+### dfu-util
+```Bash
+pydfuutil -h 
+# or
+python -m pydfuutil -h
+
+####### usage:
+usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d VID:PID] [-p BUS-PORT] [-c CONFIG_NR] [-i INTF_NR] [-a ALT] [-t SIZE] [-U FILE] [-D FILE] [-R] [-s ADDRESS]
+
+Python implementation of DFU-Util tools
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         Print the version number
+  -v, --verbose         Print verbose debug statements
+  -l, --list            List the currently attached DFU capable USB devices
+  -e, --detach          Detach the currently attached DFU capable USB devices
+  -d VID:PID, --device VID:PID
+                        Specify Vendor/Product ID of DFU device
+  -p BUS-PORT, --path BUS-PORT
+                        Specify path to DFU device
+  -c CONFIG_NR, --cfg CONFIG_NR
+                        Specify the Configuration of DFU device
+  -i INTF_NR, --intf INTF_NR
+                        Specify the DFU Interface number
+  -a ALT, --alt ALT     Specify the Altsetting of the DFU Interface
+  -t SIZE, --transfer-size SIZE
+                        Specify the number of bytes per USB Transfer
+  -U FILE, --upload FILE
+                        Read firmware from device into <file>
+  -D FILE, --download FILE
+                        Write firmware from <file> into device
+  -R, --reset           Issue USB Reset signalling once we`re finished
+  -s ADDRESS, --dfuse-address ADDRESS
+                        ST DfuSe mode, specify target address for raw file download or upload. Not applicable for DfuSe file (.dfu) downloads
+```
+
+### dfu-suffix
+```Bash
+pydfuutil-suffix -h
+# or 
+python -m pydfuutil.suffix -h
+
+
+usage: dfu-suffix [-h] [-V] (-c | -a | -D) [-p <productID>] [-v <vendorID>] [-d <deviceID>] [-s <address>] [-T] <file>
+
+positional arguments:
+  <file>                Target filename
+
+options:
+  -h, --help            Print this help message
+  -V, --version         Print the version number
+  -c, --check           Check DFU suffix of <file>
+  -a, --add             Add DFU suffix to <file>
+  -D, --delete          Delete DFU suffix from <file>
+  -p <productID>, --pid <productID>
+                        Add product ID into DFU suffix in <file>
+  -v <vendorID>, --vid <vendorID>
+                        Add vendor ID into DFU suffix in <file>
+  -d <deviceID>, --did <deviceID>
+                        Add device ID into DFU suffix in <file>
+  -s <address>, --stellaris-address <address>
+                        Specify lmdfu address for LMDFU_ADD
+  -T, --stellaris       Set lmdfu mode to LMDFU_CHECK
+
+```
+
 
 ## Todos
 
 #### Modules to implement:
 
 - [ ] main
+  - [x] atoi()
+  - [ ] usb_path2devnum()
+  - [x] find_dfu_if()
+  - [x] _get_first_cb()
+  - [x] _get_first_dfu_if()
+  - [x] _check_match_cb()
+  - [x] get_matching_dfu_if()
+  - [x] _count_match_cb()
+  - [x] count_matching_dfu_if()
+  - [x] get_alt_name()
+  - [x] print_dfu_if()
+  - [x] list_dfu_interfaces()
+  - [x] alt_by_name()
+  - [x] _count_cb()
+  - [x] count_dfu_interfaces()
+  - [x] iterate_dfu_devices()
+  - [x] found_dfu_device()
+  - [x] get_first_dfu_device()
+  - [x] count_one_dfu_device()
+  - [x] count_dfu_devices()
+  - [x] parse_vendprod()
+  - [ ] resolve_device_path()
+  - [x] find_descriptor()
+  - [ ] usb_get_any_descriptor()
+  - [x] get_cached_extra_descriptor()
+  - [x] help_()
+  - [x] print_version()
+  - [ ] main()
 - [ ] dfu_load.PROGRESS_BAR -> rich.Progress
 
 
 #### Done:
 - [x] dfu
 - [x] dfu_file
 - [x] dfu_load
```

### Comparing `pydfuutil-0.0.2b0/pydfuutil/dfu.py` & `pydfuutil-0.0.2b1/pydfuutil/dfu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 low-level DFU message sending routines (part of dfu-programmer).
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
 
 import inspect
-from dataclasses import dataclass
-from enum import IntEnum
+from dataclasses import dataclass, field
+from enum import IntEnum, IntFlag
 
 import usb.util
 from construct import Byte, Struct, BytesInteger, Container
 
 from pydfuutil.logger import get_logger
 
 logger = get_logger(__name__)
@@ -96,15 +96,15 @@
     GETSTATUS = 3
     CLRSTATUS = 4
     GETSTATE = 5
     ABORT = 6
 
 
 # /* DFU interface */
-class Mode(IntEnum):
+class Mode(IntFlag):
     """Dfu modes"""
     IFF_DFU = 0x0001  # /* DFU Mode, (not Runtime) */
     IFF_VENDOR = 0x0100
     IFF_PRODUCT = 0x0200
     IFF_CONFIG = 0x0400
     IFF_IFACE = 0x0800
     IFF_ALT = 0x1000
@@ -121,44 +121,67 @@
 
 
 @dataclass
 class DfuIf:  # pylint: disable=too-many-instance-attributes
 
     """DfuIf structure implementation"""
 
-    __slots__ = (
-        'vendor', 'product', 'bcdDevice',
-        'configuration', 'interface',
-        'altsetting', 'alt_name',
-        'bus', 'devnum',
-        'path', 'flags', 'count',
-        'dev',
-    )
-
-    # pylint: disable=too-many-arguments, invalid-name
-    def __init__(self, vendor: int, product: int, bcdDevice: int,
-                 configuration: int, interface: int,
-                 altsetting: int, alt_name: str,
-                 bus: int, devnum: int,
-                 path: [str, int], flags: int, count: int,
-                 dev: usb.core.Device):
-
-        self.vendor = vendor
-        self.product = product
-        self.bcdDevice = bcdDevice
-        self.configuration = configuration
-        self.interface = interface
-        self.altsetting = altsetting
-        self.alt_name = alt_name  # or Bytes() pointer
-        self.bus = bus
-        self.devnum = devnum
-        self.path = path  # or Bytes() pointer
-        self.flags = flags
-        self.count = count
-        self.dev = dev
+    vendor: int = field(default=None, )
+    product: int = field(default=None, )
+    bcdDevice: int = field(default=0, )
+    configuration: int = field(default=0, )
+    interface: int = field(default=0, )
+    altsetting: int = field(default=0, )
+    alt_name: str = field(default="", )
+    bus: int = field(default=0, )
+    devnum: int = field(default=0, )
+    path: [str, int] = field(default="", )
+    flags: [Mode, int] = field(default=0, )
+    count: int = field(default=0, )
+    dev: usb.core.Device = field(default=None)
+
+    @property
+    def device_ids(self) -> dict:
+        id_filter = {}
+        if self.vendor:
+            id_filter["idVendor"] = self.vendor
+        if self.product:
+            id_filter["idProduct"] = self.product
+        return id_filter
+
+    # __slots__ = (
+    #     'vendor', 'product', 'bcdDevice',
+    #     'configuration', 'interface',
+    #     'altsetting', 'alt_name',
+    #     'bus', 'devnum',
+    #     'path', 'flags', 'count',
+    #     'dev',
+    # )
+
+    # # pylint: disable=too-many-arguments, invalid-name
+    # def __init__(self, vendor: int, product: int, bcdDevice: int,
+    #              configuration: int, interface: int,
+    #              altsetting: int, alt_name: str,
+    #              bus: int, devnum: int,
+    #              path: [str, int], flags: int, count: int,
+    #              dev: usb.core.Device):
+    #
+    #     self.vendor = vendor
+    #     self.product = product
+    #     self.bcdDevice = bcdDevice
+    #     self.configuration = configuration
+    #     self.interface = interface
+    #     self.altsetting = altsetting
+    #     self.alt_name = alt_name  # or Bytes() pointer
+    #     self.bus = bus
+    #     self.devnum = devnum
+    #     self.path = path  # or Bytes() pointer
+    #     self.flags = flags
+    #     self.count = count
+    #     self.dev = dev
 
 
 def init(timeout: int) -> None:
     """
     Initiate dfu_util library with specified commands timeout
     :param timeout in milliseconds
     :return: None
```

### Comparing `pydfuutil-0.0.2b0/pydfuutil/dfu_file.py` & `pydfuutil-0.0.2b1/pydfuutil/dfu_file.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b0/pydfuutil/dfu_load.py` & `pydfuutil-0.0.2b1/pydfuutil/dfu_load.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b0/pydfuutil/dfuse.py` & `pydfuutil-0.0.2b1/pydfuutil/dfuse.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b0/pydfuutil/dfuse_mem.py` & `pydfuutil-0.0.2b1/pydfuutil/dfuse_mem.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b0/pydfuutil/lmdfu.py` & `pydfuutil-0.0.2b1/pydfuutil/lmdfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b0/pydfuutil/quirks.py` & `pydfuutil-0.0.2b1/pydfuutil/quirks.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 QUIRK_FORCE_DFU11 = 1 << 1
 
 # Fallback value, works for OpenMoko
 DEFAULT_POLLTIMEOUT = 5
 
 
 # pylint: disable=invalid-name
-def get_quirks(vendor: int, product: int, bcdDevice: int) -> int:
+def set_quirks(vendor: int, product: int, bcdDevice: int) -> int:
     """
 
     :param vendor: VID
     :param product: PID
     :param bcdDevice:
     :return: quirks
     """
```

### Comparing `pydfuutil-0.0.2b0/pydfuutil/suffix.py` & `pydfuutil-0.0.2b1/pydfuutil/suffix.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     CHECK = 0x4
 
 
 def print_version() -> None:
     """
     Prints dfu-suffix version to console
     """
-    print(f'dfu-suffix " {__version__} "\n')
+    print(f'pydfuutil-suffix " {__version__} "\n')
     print(f'{__copyright__[0]}\n'
           'This program is Free Software and has ABSOLUTELY NO WARRANTY\n\n')
 
 
 OPTS = (
     ("help", 0, 0, 'h'),
     ("version", 0, 0, 'V'),
```

### Comparing `pydfuutil-0.0.2b0/pydfuutil/usb_dfu.py` & `pydfuutil-0.0.2b1/pydfuutil/usb_dfu.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,38 @@
 This ought to be compliant to the USB DFU Spec 1.0 as available from
 https://www.usb.org/developers/devclass_docs/usbdfu10.pdf
 """
 
 from enum import IntEnum
 
 import usb.util
-from construct import FlagsEnum, Byte, Int8ul, Struct, Int16ul
+from construct import Int8ul, Struct, Int16ul
+# from construct import FlagsEnum, Byte
 
 USB_DT_DFU = 0x21
 
-bmAttributes = FlagsEnum(
-    Byte,
-    USB_DFU_CAN_DOWNLOAD=0x1,  # is support updates
-    USB_DFU_CAN_UPLOAD=0x2,  # is prog warranty ok
-    USB_DFU_MANIFEST_TOL=0x4,
-    USB_DFU_WILL_DETACH=0x8,
-)
+class bmAttributes(IntEnum):
+    USB_DFU_CAN_DOWNLOAD = 0x1
+    USB_DFU_CAN_UPLOAD = 0x2
+    USB_DFU_MANIFEST_TOL = 0x3
+    USB_DFU_WILL_DETACH = 0x4
+
+# bmAttributes = FlagsEnum(
+#     Byte,
+#     USB_DFU_CAN_DOWNLOAD=0x1,  # is support updates
+#     USB_DFU_CAN_UPLOAD=0x2,  # is prog warranty ok
+#     USB_DFU_MANIFEST_TOL=0x4,
+#     USB_DFU_WILL_DETACH=0x8,
+# )
 
 USB_DFU_FUNC_DESCRIPTOR = Struct(
     bLength=Int8ul,
     bDescriptorType=Int8ul,
-    bmAttributes=bmAttributes,
+    # bmAttributes=bmAttributes,
+    bmAttributes=Int8ul,
     wDetachTimeOut=Int16ul,
     wTransferSize=Int16ul,
     bcdDFUVersion=Int16ul,
 )
 
 USB_DT_DFU_SIZE = 9
```

### Comparing `pydfuutil-0.0.2b0/pydfuutil.egg-info/PKG-INFO` & `pydfuutil-0.0.2b1/pydfuutil.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.2b0
+Version: 0.0.2b1
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -236,20 +236,117 @@
 
     # the latest official release
     python -m pip install pydfuutil
 
     # install a specific version (e.g. 0.0.1b1)
     python -m pip install pydfuutil==0.0.1b1
 
+## Usage
+
+### dfu-util
+```Bash
+pydfuutil -h 
+# or
+python -m pydfuutil -h
+
+####### usage:
+usage: pydfuutil [-h] [-V] [-v] [-l] [-e] [-d VID:PID] [-p BUS-PORT] [-c CONFIG_NR] [-i INTF_NR] [-a ALT] [-t SIZE] [-U FILE] [-D FILE] [-R] [-s ADDRESS]
+
+Python implementation of DFU-Util tools
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         Print the version number
+  -v, --verbose         Print verbose debug statements
+  -l, --list            List the currently attached DFU capable USB devices
+  -e, --detach          Detach the currently attached DFU capable USB devices
+  -d VID:PID, --device VID:PID
+                        Specify Vendor/Product ID of DFU device
+  -p BUS-PORT, --path BUS-PORT
+                        Specify path to DFU device
+  -c CONFIG_NR, --cfg CONFIG_NR
+                        Specify the Configuration of DFU device
+  -i INTF_NR, --intf INTF_NR
+                        Specify the DFU Interface number
+  -a ALT, --alt ALT     Specify the Altsetting of the DFU Interface
+  -t SIZE, --transfer-size SIZE
+                        Specify the number of bytes per USB Transfer
+  -U FILE, --upload FILE
+                        Read firmware from device into <file>
+  -D FILE, --download FILE
+                        Write firmware from <file> into device
+  -R, --reset           Issue USB Reset signalling once we`re finished
+  -s ADDRESS, --dfuse-address ADDRESS
+                        ST DfuSe mode, specify target address for raw file download or upload. Not applicable for DfuSe file (.dfu) downloads
+```
+
+### dfu-suffix
+```Bash
+pydfuutil-suffix -h
+# or 
+python -m pydfuutil.suffix -h
+
+
+usage: dfu-suffix [-h] [-V] (-c | -a | -D) [-p <productID>] [-v <vendorID>] [-d <deviceID>] [-s <address>] [-T] <file>
+
+positional arguments:
+  <file>                Target filename
+
+options:
+  -h, --help            Print this help message
+  -V, --version         Print the version number
+  -c, --check           Check DFU suffix of <file>
+  -a, --add             Add DFU suffix to <file>
+  -D, --delete          Delete DFU suffix from <file>
+  -p <productID>, --pid <productID>
+                        Add product ID into DFU suffix in <file>
+  -v <vendorID>, --vid <vendorID>
+                        Add vendor ID into DFU suffix in <file>
+  -d <deviceID>, --did <deviceID>
+                        Add device ID into DFU suffix in <file>
+  -s <address>, --stellaris-address <address>
+                        Specify lmdfu address for LMDFU_ADD
+  -T, --stellaris       Set lmdfu mode to LMDFU_CHECK
+
+```
+
 
 ## Todos
 
 #### Modules to implement:
 
 - [ ] main
+  - [x] atoi()
+  - [ ] usb_path2devnum()
+  - [x] find_dfu_if()
+  - [x] _get_first_cb()
+  - [x] _get_first_dfu_if()
+  - [x] _check_match_cb()
+  - [x] get_matching_dfu_if()
+  - [x] _count_match_cb()
+  - [x] count_matching_dfu_if()
+  - [x] get_alt_name()
+  - [x] print_dfu_if()
+  - [x] list_dfu_interfaces()
+  - [x] alt_by_name()
+  - [x] _count_cb()
+  - [x] count_dfu_interfaces()
+  - [x] iterate_dfu_devices()
+  - [x] found_dfu_device()
+  - [x] get_first_dfu_device()
+  - [x] count_one_dfu_device()
+  - [x] count_dfu_devices()
+  - [x] parse_vendprod()
+  - [ ] resolve_device_path()
+  - [x] find_descriptor()
+  - [ ] usb_get_any_descriptor()
+  - [x] get_cached_extra_descriptor()
+  - [x] help_()
+  - [x] print_version()
+  - [ ] main()
 - [ ] dfu_load.PROGRESS_BAR -> rich.Progress
 
 
 #### Done:
 - [x] dfu
 - [x] dfu_file
 - [x] dfu_load
```

### Comparing `pydfuutil-0.0.2b0/pydfuutil.egg-info/SOURCES.txt` & `pydfuutil-0.0.2b1/pydfuutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b0/pyproject.toml` & `pydfuutil-0.0.2b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,9 @@
 version = {attr = "pydfuutil.__version__"}
 
 
 [project.optional-dependencies]
 dev = ['build']
 
 [project.scripts]
-dfu-suffix = "pydfuutil.suffix:main"
+pydfuutil = "pydfuutil.__main__:main"
+pydfuutil-suffix = "pydfuutil.suffix:main"
```

### Comparing `pydfuutil-0.0.2b0/tests/test_dfu_file.py` & `pydfuutil-0.0.2b1/tests/test_dfu_file.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b0/tests/test_dfu_load.py` & `pydfuutil-0.0.2b1/tests/test_dfu_load.py`

 * *Files identical despite different names*

