# Comparing `tmp/netsome-0.3.5.tar.gz` & `tmp/netsome-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsome-0.3.5.tar", max compression
+gzip compressed data, was "netsome-0.3.6.tar", max compression
```

## Comparing `netsome-0.3.5.tar` & `netsome-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.5/LICENSE
--rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.5/README.md
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.5/netsome/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.5/netsome/_converters/__init__.py
--rw-r--r--   0        0        0      967 2024-04-27 12:52:19.064834 netsome-0.3.5/netsome/_converters/bgp.py
--rw-r--r--   0        0        0      343 2024-04-20 09:23:59.213195 netsome-0.3.5/netsome/_converters/ipv4.py
--rw-r--r--   0        0        0     1057 2024-04-27 12:48:27.358013 netsome-0.3.5/netsome/constants.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.823365 netsome-0.3.5/netsome/types/__init__.py
--rw-r--r--   0        0        0     2219 2024-04-20 09:23:59.214154 netsome-0.3.5/netsome/types/bgp.py
--rw-r--r--   0        0        0     4992 2024-04-27 12:51:28.993779 netsome-0.3.5/netsome/types/ipv4.py
--rw-r--r--   0        0        0     3629 2024-04-27 12:48:22.756838 netsome-0.3.5/netsome/types/mac.py
--rw-r--r--   0        0        0      906 2024-04-20 09:23:59.215917 netsome-0.3.5/netsome/types/vlans.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.5/netsome/validators/__init__.py
--rw-r--r--   0        0        0     2016 2024-04-27 12:48:27.359049 netsome-0.3.5/netsome/validators/bgp.py
--rw-r--r--   0        0        0     2112 2024-04-20 09:23:59.217488 netsome-0.3.5/netsome/validators/ipv4.py
--rw-r--r--   0        0        0      379 2024-04-27 12:48:27.359608 netsome-0.3.5/netsome/validators/vlans.py
--rw-r--r--   0        0        0     1234 2024-04-27 12:53:16.570621 netsome-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.6/LICENSE
+-rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.6/netsome/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.6/netsome/_converters/__init__.py
+-rw-r--r--   0        0        0      967 2024-04-27 12:52:19.064834 netsome-0.3.6/netsome/_converters/bgp.py
+-rw-r--r--   0        0        0      343 2024-04-20 09:23:59.213195 netsome-0.3.6/netsome/_converters/ipv4.py
+-rw-r--r--   0        0        0     1057 2024-04-27 12:48:27.358013 netsome-0.3.6/netsome/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.823365 netsome-0.3.6/netsome/types/__init__.py
+-rw-r--r--   0        0        0     2219 2024-04-20 09:23:59.214154 netsome-0.3.6/netsome/types/bgp.py
+-rw-r--r--   0        0        0     6086 2024-04-28 22:16:33.096317 netsome-0.3.6/netsome/types/ipv4.py
+-rw-r--r--   0        0        0     3212 2024-04-28 18:56:11.702930 netsome-0.3.6/netsome/types/mac.py
+-rw-r--r--   0        0        0      906 2024-04-20 09:23:59.215917 netsome-0.3.6/netsome/types/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.6/netsome/validators/__init__.py
+-rw-r--r--   0        0        0     2016 2024-04-27 12:48:27.359049 netsome-0.3.6/netsome/validators/bgp.py
+-rw-r--r--   0        0        0     2112 2024-04-20 09:23:59.217488 netsome-0.3.6/netsome/validators/ipv4.py
+-rw-r--r--   0        0        0      512 2024-04-28 18:55:56.209709 netsome-0.3.6/netsome/validators/mac.py
+-rw-r--r--   0        0        0      379 2024-04-27 12:48:27.359608 netsome-0.3.6/netsome/validators/vlans.py
+-rw-r--r--   0        0        0     1234 2024-04-28 22:17:55.367251 netsome-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.6/PKG-INFO
```

### Comparing `netsome-0.3.5/LICENSE` & `netsome-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netsome-0.3.5/netsome/_converters/bgp.py` & `netsome-0.3.6/netsome/_converters/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.5/netsome/constants.py` & `netsome-0.3.6/netsome/constants.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.5/netsome/types/bgp.py` & `netsome-0.3.6/netsome/types/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.5/netsome/types/ipv4.py` & `netsome-0.3.6/netsome/types/ipv4.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 
     def as_tuple(self) -> tuple[int, int]:
         return int(self.netaddress), self._prefixlen
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}("{self.address}")'
 
+    def __hash__(self) -> int:
+        return hash(self.as_tuple())
+
     @property
     def prefixlen(self) -> int:
         return self._prefixlen
 
     @property
     def netaddress(self) -> IPv4Address:
         return self._netaddr
@@ -153,7 +156,40 @@
 
     def hosts(self):
         start = int(self._netaddr) + 1
         end = int(self.broadcast)
 
         for addr in range(start, end):
             yield IPv4Address.from_int(addr)
+
+
+class IPv4Interface:
+    def __init__(self, address: str) -> None:
+        addr, prefixlen = address.split(c.DELIMITERS.SLASH, maxsplit=1)
+        self._addr = IPv4Address(addr)
+
+        prefixlen = int(prefixlen)
+        netmask = c.IPV4.ADDRESS_MAX ^ (c.IPV4.ADDRESS_MAX >> prefixlen)
+        netaddr = int(self._addr) & netmask
+        self._network = IPv4Network.from_int(netaddr, prefixlen)
+
+    def __repr__(self) -> str:
+        ip = c.DELIMITERS.SLASH.join_as_str(self._addr.address, self._network.prefixlen)
+        return f'{self.__class__.__name__}("{ip}")'
+
+    def __hash__(self) -> int:
+        return hash((self._addr, self._network))
+
+    def __eq__(self, other: t.Any) -> bool:
+        return (
+            isinstance(other, self.__class__)
+            and self._addr == other._addr
+            and self._network == other._network
+        )
+
+    @property
+    def network(self) -> "IPv4Network":
+        return self._network
+
+    @property
+    def address(self) -> "IPv4Address":
+        return self._addr
```

### Comparing `netsome-0.3.5/netsome/types/mac.py` & `netsome-0.3.6/netsome/types/mac.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,13 @@
 import contextlib
 import functools
-import re
 import typing as t
 
 from netsome import constants as c
-
-
-# TODO: make common
-def validate_hex_string(string: str, size: int) -> None:
-
-    # TODO: make common
-    if not isinstance(string, str):
-        raise TypeError
-
-    if not re.fullmatch(r"^[0-9a-fA-F]{%s}$" % size, string):
-        raise ValueError
-
-
-# TODO: make common
-def validate_int(number: int) -> None:
-    if not isinstance(number, int):
-        raise TypeError()
-
-    if not (c.MAC.ADDRESS_MIN <= number <= c.MAC.ADDRESS_MAX):
-        raise ValueError()
+from netsome.validators import mac as valids
 
 
 class MacAddress:
     # MAC-48/EUI-48
 
     MIN = c.MAC.ADDRESS_MIN
     MAX = c.MAC.ADDRESS_MAX
@@ -36,15 +16,15 @@
     NIC_MAX = c.MAC.NIC_MAX
 
     # can be calculated from const above
     ADDR_STRING_SIZE = 12
     OUI_PART_STRING_SIZE = 6
 
     def __init__(self, addr: str) -> None:
-        validate_hex_string(addr, self.ADDR_STRING_SIZE)
+        valids.validate_hex_string(addr, self.ADDR_STRING_SIZE)
         self._addr = int(addr, base=c.NUMERALSYSTEMS.HEX)
 
     @functools.cached_property
     def address(self):
         addr = hex(self._addr)[2:]  # ignore 0x part
         leading_zeros = "0" * (self.ADDR_STRING_SIZE - len(addr))
         return leading_zeros + addr
@@ -80,15 +60,15 @@
 
     @classmethod
     def from_dotted(cls, string: str) -> "MacAddress":
         return cls(string.replace(c.DELIMITERS.DOT, ""))
 
     @classmethod
     def from_int(cls, number: int) -> "MacAddress":
-        validate_int(number)
+        valids.validate_int(number)
         obj = cls.__new__(cls)
         obj._addr = number
         return obj
 
     @classmethod
     def parse(cls, addr: str | int) -> "MacAddress":
         # TODO: can collect all this from cls attrs?
```

### Comparing `netsome-0.3.5/netsome/types/vlans.py` & `netsome-0.3.6/netsome/types/vlans.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.5/netsome/validators/bgp.py` & `netsome-0.3.6/netsome/validators/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.5/netsome/validators/ipv4.py` & `netsome-0.3.6/netsome/validators/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.5/pyproject.toml` & `netsome-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 description = "The one and only library to make your network code handsome"
 keywords = ["library", "network"]
 license = "X11 License Distribution Modification Variant"
 name = "netsome"
 readme = "README.md"
 repository = "https://github.com/kuderr/netsome"
-version = "0.3.5"
+version = "0.3.6"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.25.0"
 pytest = "^8.1.1"
```

### Comparing `netsome-0.3.5/PKG-INFO` & `netsome-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsome
-Version: 0.3.5
+Version: 0.3.6
 Summary: The one and only library to make your network code handsome
 Home-page: https://github.com/kuderr/netsome
 License: X11-distribute-modifications-variant
 Keywords: library,network
 Author: kuderr
 Author-email: dakudryavcev@gmail.com
 Requires-Python: >=3.10,<4.0
```

