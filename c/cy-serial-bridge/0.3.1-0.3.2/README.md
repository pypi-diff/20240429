# Comparing `tmp/cy_serial_bridge-0.3.1.tar.gz` & `tmp/cy_serial_bridge-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy_serial_bridge-0.3.1.tar", max compression
+gzip compressed data, was "cy_serial_bridge-0.3.2.tar", max compression
```

## Comparing `cy_serial_bridge-0.3.1.tar` & `cy_serial_bridge-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3150 2024-03-19 17:29:53.132315 cy_serial_bridge-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     7652 2024-03-19 17:29:53.132315 cy_serial_bridge-0.3.1/LICENSE
--rw-r--r--   0        0        0    30882 2024-03-19 17:29:53.132315 cy_serial_bridge-0.3.1/README.md
--rw-r--r--   0        0        0       83 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/py.typed
--rw-r--r--   0        0        0     5925 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      770 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/src/cy_serial_bridge/__init__.py
--rw-r--r--   0        0        0    19985 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/src/cy_serial_bridge/cli.py
--rw-r--r--   0        0        0    12820 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/src/cy_serial_bridge/configuration_block.py
--rw-r--r--   0        0        0    16724 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/src/cy_serial_bridge/cy_scb_context.py
--rw-r--r--   0        0        0    51581 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/src/cy_serial_bridge/driver.py
--rw-r--r--   0        0        0        0 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/src/cy_serial_bridge/py.typed
--rw-r--r--   0        0        0     8179 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/src/cy_serial_bridge/usb_constants.py
--rw-r--r--   0        0        0     2270 2024-03-19 17:29:53.160315 cy_serial_bridge-0.3.1/src/cy_serial_bridge/utils.py
--rw-r--r--   0        0        0    31756 1970-01-01 00:00:00.000000 cy_serial_bridge-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3615 2024-04-28 23:50:47.457144 cy_serial_bridge-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     7652 2024-04-28 23:50:47.457144 cy_serial_bridge-0.3.2/LICENSE
+-rw-r--r--   0        0        0    30882 2024-04-28 23:50:47.457144 cy_serial_bridge-0.3.2/README.md
+-rw-r--r--   0        0        0       83 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/py.typed
+-rw-r--r--   0        0        0     5925 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      770 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/src/cy_serial_bridge/__init__.py
+-rw-r--r--   0        0        0    20019 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/src/cy_serial_bridge/cli.py
+-rw-r--r--   0        0        0    13062 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/src/cy_serial_bridge/configuration_block.py
+-rw-r--r--   0        0        0    17402 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/src/cy_serial_bridge/cy_scb_context.py
+-rw-r--r--   0        0        0    51581 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/src/cy_serial_bridge/driver.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/src/cy_serial_bridge/py.typed
+-rw-r--r--   0        0        0     8179 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/src/cy_serial_bridge/usb_constants.py
+-rw-r--r--   0        0        0     2270 2024-04-28 23:50:47.485144 cy_serial_bridge-0.3.2/src/cy_serial_bridge/utils.py
+-rw-r--r--   0        0        0    31756 1970-01-01 00:00:00.000000 cy_serial_bridge-0.3.2/PKG-INFO
```

### Comparing `cy_serial_bridge-0.3.1/CHANGELOG.md` & `cy_serial_bridge-0.3.2/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -44,14 +44,26 @@
 
 - Updated localisation files
 
 -->
 
 _______________________________________________________________________________
 
+## [0.3.2] - 2024-04-28
+
+### Fixed
+
+- Added udev rule for CY7C65211A default PID
+- Fixed scanning/reconfiguring devices in UART_CDC mode with no serial number (warning is printed instead of crashing)
+- Fixed `default_frequency` missing from ConfigurationBlock string conversion
+- Config block version 2 (observed on CY7C65211A) is now permitted for the driver, and seems to work OK
+
+
+_______________________________________________________________________________
+
 ## [0.3.1] - 2024-03-19
 
 ### Fixed
 
 - Work around [tiangolo/typer#463](https://github.com/tiangolo/typer/pull/463) by explicitly declaring a dependency on Click >=8.0
 - Fix minimum Python version dependency
```

### Comparing `cy_serial_bridge-0.3.1/LICENSE` & `cy_serial_bridge-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cy_serial_bridge-0.3.1/README.md` & `cy_serial_bridge-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cy_serial_bridge-0.3.1/pyproject.toml` & `cy_serial_bridge-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "cy_serial_bridge"
 # this is used by Ruff to disable "upgrade to feature x" inspections where x was added
 # after the given version
 requires-python = ">=3.10"
-version = "0.3.1"
+version = "0.3.2"
 description = "Pure Python driver for using and reconfiguring the CY7C652xx family of USB to SPI/I2C/UART bridge ICs."
 authors = [
   {name = "Jamie Smith", email = "smit109@usc.edu"},
 ]
 readme = "README.md"
 license = {text = "LGPL"}
 classifiers = [
@@ -29,15 +29,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry]
 name = "cy_serial_bridge"
-version = "0.3.1"
+version = "0.3.2"
 description = "Pure Python driver for using and reconfiguring the CY7C652xx family of USB to SPI/I2C/UART bridge ICs."
 authors = ["Jamie Smith <smit109@usc.edu>"]
 readme = "README.md"
 include = ['CHANGELOG.md', 'LICENSE', 'py.typed',]
 packages = [
     { include = 'cy_serial_bridge', from = 'src' },
 ]
```

### Comparing `cy_serial_bridge-0.3.1/src/cy_serial_bridge/__init__.py` & `cy_serial_bridge-0.3.2/src/cy_serial_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `cy_serial_bridge-0.3.1/src/cy_serial_bridge/cli.py` & `cy_serial_bridge-0.3.2/src/cy_serial_bridge/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,20 +182,22 @@
 # ---------------------------------------------------------------------------------------------
 
 RandomizeSernoOption = typer.Option("--randomize-serno", help="Set the serial number of the device to a random value.")
 SetSernoOption = typer.Option("--set-serno", help="Set the serial number of the device.")
 SetVIDOption = typer.Option(
     "--set-vid",
     help="Set the USB Vendor ID to a given value.  Needs a 0x prefix for hex values!",
-    callback=parse_vid_pid,
+    metavar="VID",
+    parser=parse_vid_pid,
 )
 SetPIDOption = typer.Option(
     "--set-pid",
     help="Set the USB Product ID to a given value.  Needs a 0x prefix for hex values!",
-    callback=parse_vid_pid,
+    metavar="PID",
+    parser=parse_vid_pid,
 )
 
 
 @app.command(help="Change configuration of the connected device via the CLI")
 def reconfigure(
     randomize_serno: Annotated[bool, RandomizeSernoOption] = False,
     set_serno: Annotated[Optional[str], SetSernoOption] = None,
```

### Comparing `cy_serial_bridge-0.3.1/src/cy_serial_bridge/configuration_block.py` & `cy_serial_bridge-0.3.2/src/cy_serial_bridge/configuration_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 from cy_serial_bridge.usb_constants import CY_CONFIG_STRING_MAX_LEN_BYTES, CY_DEVICE_CONFIG_SIZE, CyType
 
 if TYPE_CHECKING:
     from cy_serial_bridge.utils import ByteSequence
 
 CONFIG_BLOCK_EXPECTED_MAGIC = b"CYUS"
-CONFIG_BLOCK_EXPECTED_MAJOR_VERSION = 1
+
+# Version 1.0.3 observed on CY7C65211.
+# Version 2.0.3 observed on CY7C65211A.
+# So far no differences have been determined between the two versions.
+CONFIG_BLOCK_EXPECTED_MAJOR_VERSIONS = {1, 2}
 
 
 class ConfigurationBlock:
     """
     Module which implements basic reading/writing of CY7C652xx memory configuration blocks.
 
     These blocks are written to the chip using the reverse engineered API in order to configure the interface
@@ -49,16 +53,16 @@
         # Some dumps contain extra bytes so trim to 512 bytes.
         self._cfg_bytes = self._cfg_bytes[: CY_DEVICE_CONFIG_SIZE + 1]
 
         # Check magic, format, and checksum
         if self._cfg_bytes[0:4] != CONFIG_BLOCK_EXPECTED_MAGIC:
             message = "Incorrect magic at start of configuration block"
             raise ValueError(message)
-        if self.config_format_version[0] != CONFIG_BLOCK_EXPECTED_MAJOR_VERSION:
-            message = f"Only know how to work with config block major version {CONFIG_BLOCK_EXPECTED_MAJOR_VERSION} this is 0x{self.config_format_version[0]}"
+        if self.config_format_version[0] not in CONFIG_BLOCK_EXPECTED_MAJOR_VERSIONS:
+            message = f"Only know how to work with config block major versions {', '.join(str(ver) for ver in CONFIG_BLOCK_EXPECTED_MAJOR_VERSIONS)} this is 0x{self.config_format_version[0]}"
             raise ValueError(message)
         if self._get_checksum() != self._calculate_checksum():
             message = f"Checksum failed for configuration block.  Expected 0x{self._calculate_checksum():x} but read 0x{self._get_checksum():x} from header"
             raise ValueError(message)
 
     def _decode_string_field(self, flag_addr: int, data_start_addr: int) -> str | None:
         """
@@ -285,8 +289,9 @@
     device_type=CY_TYPE.{self.device_type.name},
     vid=0x{self.vid:04x},
     pid=0x{self.pid:04x},
     mfgr_string=\"{self.mfgr_string}\",
     product_string=\"{self.product_string}\",
     serial_number=\"{self.serial_number}\",
     capsense_on={self.capsense_on},
+    default_frequency={self.default_frequency}
 )"""
```

### Comparing `cy_serial_bridge-0.3.1/src/cy_serial_bridge/cy_scb_context.py` & `cy_serial_bridge-0.3.2/src/cy_serial_bridge/cy_scb_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,22 @@
                 list_entry.serial_number = opened_device.getSerialNumber()
             except usb1.USBError:
                 list_entry.open_failed = True
 
             # Iff this is a CDC serial device, find its associated COM port.
             # Luckily, pyserial does the hard work of talking to the OS for us here.
             if curr_cytype == CyType.UART_CDC and not list_entry.open_failed:
-                list_entry.serial_port_name = self._find_serial_port_name_for_serno(cast(str, list_entry.serial_number))
+                if list_entry.serial_number is None:
+                    log.warning(
+                        "Discovered CY7C652xx device in UART mode with no serial number configured.  Will "
+                        "not be able to open a terminal to this device until it is configured with a "
+                        "serial number."
+                    )
+                else:
+                    list_entry.serial_port_name = self._find_serial_port_name_for_serno(list_entry.serial_number)
 
             device_list.append(list_entry)
 
         return device_list
 
     # Time we allow for the device to change its type and be enumerated on the USB bus:
     # It can take quite some time for the OS to re-enumerate the serial port
@@ -363,10 +370,16 @@
                     message = "The CyType of the device did not change to the correct value within the timeout!"
                     raise CySerialBridgeError(message)
 
             log.info(f"Changed type of device in {time.time() - change_type_start_time:.04f} sec")
 
         # Step 3: Instantiate the driver!
         if open_mode == OpenMode.UART_CDC:
+            if device_to_open.serial_port_name is None:
+                message = (
+                    "Cannot open this device as cy_serial_bridge could not determine the COM port/"
+                    "TTY that it's connected to."
+                )
+                raise CySerialBridgeError(message)
             return serial.Serial(port=device_to_open.serial_port_name)
         else:
             return typing.cast(AnyDriverClass, driver_class(self, device_to_open))  # type: ignore[call-arg]
```

### Comparing `cy_serial_bridge-0.3.1/src/cy_serial_bridge/driver.py` & `cy_serial_bridge-0.3.2/src/cy_serial_bridge/driver.py`

 * *Files identical despite different names*

### Comparing `cy_serial_bridge-0.3.1/src/cy_serial_bridge/usb_constants.py` & `cy_serial_bridge-0.3.2/src/cy_serial_bridge/usb_constants.py`

 * *Files identical despite different names*

### Comparing `cy_serial_bridge-0.3.1/src/cy_serial_bridge/utils.py` & `cy_serial_bridge-0.3.2/src/cy_serial_bridge/utils.py`

 * *Files identical despite different names*

### Comparing `cy_serial_bridge-0.3.1/PKG-INFO` & `cy_serial_bridge-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cy_serial_bridge
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pure Python driver for using and reconfiguring the CY7C652xx family of USB to SPI/I2C/UART bridge ICs.
 Home-page: https://github.com/mbed-ce/cy_serial_bridge/
 Author: Jamie Smith
 Author-email: smit109@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

