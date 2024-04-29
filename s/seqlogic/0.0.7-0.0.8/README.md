# Comparing `tmp/seqlogic-0.0.7.tar.gz` & `tmp/seqlogic-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqlogic-0.0.7.tar", last modified: Mon Mar 11 04:11:41 2024, max compression
+gzip compressed data, was "seqlogic-0.0.8.tar", last modified: Mon Apr 29 04:37:57 2024, max compression
```

## Comparing `seqlogic-0.0.7.tar` & `seqlogic-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 04:11:41.579006 seqlogic-0.0.7/
--rw-rw-rw-   0        0        0      960 2024-03-11 04:11:41.563361 seqlogic-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-12-13 03:22:59.000000 seqlogic-0.0.7/README.md
--rw-rw-rw-   0        0        0      263 2024-03-11 04:09:02.000000 seqlogic-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-11 04:11:41.579684 seqlogic-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-11 04:11:41.499496 seqlogic-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-03-11 04:11:41.524119 seqlogic-0.0.7/src/seqlogic/
--rw-rw-rw-   0        0        0      325 2024-03-11 02:48:00.000000 seqlogic-0.0.7/src/seqlogic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 04:11:41.548524 seqlogic-0.0.7/src/seqlogic/algorithms/
--rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.0.7/src/seqlogic/algorithms/__init__.py
--rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.0.7/src/seqlogic/algorithms/aes.py
--rw-rw-rw-   0        0        0      343 2024-03-10 17:03:07.000000 seqlogic-0.0.7/src/seqlogic/algorithms/gray.py
--rw-rw-rw-   0        0        0    21780 2024-03-11 03:59:27.000000 seqlogic-0.0.7/src/seqlogic/bits.py
--rw-rw-rw-   0        0        0     6189 2024-03-11 03:02:36.000000 seqlogic-0.0.7/src/seqlogic/design.py
--rw-rw-rw-   0        0        0     2338 2024-03-10 18:52:13.000000 seqlogic-0.0.7/src/seqlogic/enum.py
--rw-rw-rw-   0        0        0     3183 2024-03-11 02:48:00.000000 seqlogic-0.0.7/src/seqlogic/hier.py
--rw-rw-rw-   0        0        0    66755 2024-03-11 03:25:36.000000 seqlogic-0.0.7/src/seqlogic/lbool.py
--rw-rw-rw-   0        0        0    14236 2024-03-11 03:02:36.000000 seqlogic-0.0.7/src/seqlogic/sim.py
--rw-rw-rw-   0        0        0     1215 2023-11-27 07:28:50.000000 seqlogic-0.0.7/src/seqlogic/util.py
-drwxrwxrwx   0        0        0        0 2024-03-11 04:11:41.563361 seqlogic-0.0.7/src/seqlogic.egg-info/
--rw-rw-rw-   0        0        0      960 2024-03-11 04:11:41.000000 seqlogic-0.0.7/src/seqlogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2024-03-11 04:11:41.000000 seqlogic-0.0.7/src/seqlogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 04:11:41.000000 seqlogic-0.0.7/src/seqlogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-11 04:11:41.000000 seqlogic-0.0.7/src/seqlogic.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-11 04:11:41.563361 seqlogic-0.0.7/tests/
--rw-rw-rw-   0        0        0     4281 2024-03-09 21:03:27.000000 seqlogic-0.0.7/tests/test_aes.py
--rw-rw-rw-   0        0        0    24141 2024-03-11 04:09:02.000000 seqlogic-0.0.7/tests/test_bits.py
--rw-rw-rw-   0        0        0     1186 2024-03-10 18:44:46.000000 seqlogic-0.0.7/tests/test_enum.py
--rw-rw-rw-   0        0        0     4601 2024-03-11 02:32:11.000000 seqlogic-0.0.7/tests/test_fsm.py
--rw-rw-rw-   0        0        0      665 2024-03-09 21:07:08.000000 seqlogic-0.0.7/tests/test_gray.py
--rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.0.7/tests/test_hier.py
--rw-rw-rw-   0        0        0    19376 2024-03-10 06:27:07.000000 seqlogic-0.0.7/tests/test_lbool.py
--rw-rw-rw-   0        0        0     3399 2024-03-10 16:08:44.000000 seqlogic-0.0.7/tests/test_lfsr.py
--rw-rw-rw-   0        0        0    36321 2024-03-11 02:48:00.000000 seqlogic-0.0.7/tests/test_riscv.py
--rw-rw-rw-   0        0        0     4425 2024-03-11 03:02:36.000000 seqlogic-0.0.7/tests/test_sim.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.900610 seqlogic-0.0.8/
+-rw-rw-rw-   0        0        0      956 2024-04-29 04:37:57.900610 seqlogic-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.0.8/README.md
+-rw-rw-rw-   0        0        0      263 2024-04-29 04:35:17.000000 seqlogic-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:37:57.900610 seqlogic-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.820661 seqlogic-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.850142 seqlogic-0.0.8/src/seqlogic/
+-rw-rw-rw-   0        0        0      399 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.874767 seqlogic-0.0.8/src/seqlogic/algorithms/
+-rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.0.8/src/seqlogic/algorithms/__init__.py
+-rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.0.8/src/seqlogic/algorithms/aes.py
+-rw-rw-rw-   0        0        0      285 2024-04-29 04:32:28.000000 seqlogic-0.0.8/src/seqlogic/algorithms/gray.py
+-rw-rw-rw-   0        0        0    21726 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/bits.py
+-rw-rw-rw-   0        0        0     7331 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/design.py
+-rw-rw-rw-   0        0        0     2981 2024-04-01 05:33:29.000000 seqlogic-0.0.8/src/seqlogic/hier.py
+-rw-rw-rw-   0        0        0    75435 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/lbool.py
+-rw-rw-rw-   0        0        0    14107 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/sim.py
+-rw-rw-rw-   0        0        0     1215 2023-11-27 07:28:50.000000 seqlogic-0.0.8/src/seqlogic/util.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.900610 seqlogic-0.0.8/src/seqlogic.egg-info/
+-rw-rw-rw-   0        0        0      956 2024-04-29 04:37:57.000000 seqlogic-0.0.8/src/seqlogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2024-04-29 04:37:57.000000 seqlogic-0.0.8/src/seqlogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:37:57.000000 seqlogic-0.0.8/src/seqlogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 04:37:57.000000 seqlogic-0.0.8/src/seqlogic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.900610 seqlogic-0.0.8/tests/
+-rw-rw-rw-   0        0        0     4281 2024-03-09 21:03:27.000000 seqlogic-0.0.8/tests/test_aes.py
+-rw-rw-rw-   0        0        0    24106 2024-04-28 01:11:05.000000 seqlogic-0.0.8/tests/test_bits.py
+-rw-rw-rw-   0        0        0     1991 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_enum.py
+-rw-rw-rw-   0        0        0     4713 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_fsm.py
+-rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.0.8/tests/test_gray.py
+-rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.0.8/tests/test_hier.py
+-rw-rw-rw-   0        0        0    22816 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_lbool.py
+-rw-rw-rw-   0        0        0     3514 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_lfsr.py
+-rw-rw-rw-   0        0        0    29052 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_riscv.py
+-rw-rw-rw-   0        0        0     4299 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_sim.py
+-rw-rw-rw-   0        0        0     1865 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_struct.py
```

### Comparing `seqlogic-0.0.7/PKG-INFO` & `seqlogic-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.0.7
+Version: 0.0.8
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
 
 Sequential Logic (`seqlogic`) is a logic simulation library.
 It uses Python's `async` / `await` syntax to model time,
-and provides an N-dimensional `logicvec` data type for combinational logic.
+and provides an N-dimensional `bits` data type for combinational logic.
 
 The API design is a work in progress, and documentation has not started.
 See the `tests` directory for example usage.
 
 # Installing
 
 Sequential Logic is available on [PyPI](https://pypi.org):
```

### Comparing `seqlogic-0.0.7/README.md` & `seqlogic-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Sequential Logic
 
 Sequential Logic (`seqlogic`) is a logic simulation library.
 It uses Python's `async` / `await` syntax to model time,
-and provides an N-dimensional `logicvec` data type for combinational logic.
+and provides an N-dimensional `bits` data type for combinational logic.
 
 The API design is a work in progress, and documentation has not started.
 See the `tests` directory for example usage.
 
 # Installing
 
 Sequential Logic is available on [PyPI](https://pypi.org):
```

### Comparing `seqlogic-0.0.7/src/seqlogic/algorithms/aes.py` & `seqlogic-0.0.8/src/seqlogic/algorithms/aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.7/src/seqlogic/bits.py` & `seqlogic-0.0.8/src/seqlogic/bits.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     @property
     def data(self) -> int:
         """Return bit array data."""
         return self._data
 
     @cached_property
     def _v(self) -> Vec:
-        return Vec(self.size, self._data)
+        return Vec[self.size](self._data)
 
     def reshape(self, shape: tuple[int, ...]) -> Bits:
         """Return an equivalent bit array with modified shape."""
         if math.prod(shape) != self.size:
             s = f"Expected shape with size {self.size}, got {shape}"
             raise ValueError(s)
         return Bits(shape, self._data)
@@ -164,137 +164,137 @@
 
     def lnot(self) -> Bits:
         """Bitwise lifted NOT.
 
         Returns:
             bit array of equal size and inverted data.
         """
-        return Bits(self._shape, self._v.lnot().data)
+        return Bits(self._shape, self._v.not_().data)
 
     def lnor(self, other: Bits) -> Bits:
         """Bitwise lifted NOR.
 
         Args:
             other: bit array of equal size.
 
         Returns:
             bit array of equal size, data contains NOR result.
 
         Raises:
             ValueError: bit array shapes do not match.
         """
         self._check_shape(other)
-        return _v2b(self._v.lnor(other._v))
+        return _v2b(self._v.nor(other._v))
 
     def lor(self, other: Bits) -> Bits:
         """Bitwise lifted OR.
 
         Args:
             other: bit array of equal size.
 
         Returns:
             bit array of equal size, data contains OR result.
 
         Raises:
             ValueError: bit array shapes do not match.
         """
         self._check_shape(other)
-        return _v2b(self._v.lor(other._v))
+        return _v2b(self._v.or_(other._v))
 
     def ulor(self) -> Bits[1]:
         """Unary lifted OR reduction.
 
         Returns:
             One-bit array, data contains OR reduction.
         """
-        return _v2b(self._v.ulor())
+        return _v2b(self._v.uor())
 
     def lnand(self, other: Bits) -> Bits:
         """Bitwise lifted NAND.
 
         Args:
             other: bit array of equal size.
 
         Returns:
             bit array of equal size, data contains NAND result.
 
         Raises:
             ValueError: bit array shapes do not match.
         """
         self._check_shape(other)
-        return _v2b(self._v.lnand(other._v))
+        return _v2b(self._v.nand(other._v))
 
     def land(self, other: Bits) -> Bits:
         """Bitwise lifted AND.
 
         Args:
             other: bit array of equal size.
 
         Returns:
             bit array of equal size, data contains AND result.
 
         Raises:
             ValueError: bit array shapes do not match.
         """
         self._check_shape(other)
-        return _v2b(self._v.land(other._v))
+        return _v2b(self._v.and_(other._v))
 
     def uland(self) -> Bits[1]:
         """Unary lifted AND reduction.
 
         Returns:
             One-bit array, data contains AND reduction.
         """
-        return _v2b(self._v.uland())
+        return _v2b(self._v.uand())
 
     def lxnor(self, other: Bits) -> Bits:
         """Bitwise lifted XNOR.
 
         Args:
             other: bit array of equal size.
 
         Returns:
             bit array of equal size, data contains XNOR result.
 
         Raises:
             ValueError: bit array shapes do not match.
         """
         self._check_shape(other)
-        return _v2b(self._v.lxnor(other._v))
+        return _v2b(self._v.xnor(other._v))
 
     def lxor(self, other: Bits) -> Bits:
         """Bitwise lifted XOR.
 
         Args:
             other: bit array of equal size.
 
         Returns:
             bit array of equal size, data contains XOR result.
 
         Raises:
             ValueError: bit array shapes do not match.
         """
         self._check_shape(other)
-        return _v2b(self._v.lxor(other._v))
+        return _v2b(self._v.xor(other._v))
 
     def ulxnor(self) -> Bits[1]:
         """Unary lifted XNOR reduction.
 
         Returns:
             One-bit array, data contains XOR reduction.
         """
-        return _v2b(self._v.ulxnor())
+        return _v2b(self._v.uxnor())
 
     def ulxor(self) -> Bits[1]:
         """Unary lifted XOR reduction.
 
         Returns:
             One-bit array, data contains XOR reduction.
         """
-        return _v2b(self._v.ulxor())
+        return _v2b(self._v.uxor())
 
     def to_uint(self) -> int:
         """Convert to unsigned integer.
 
         Returns:
             An unsigned int.
 
@@ -365,17 +365,17 @@
         Vectors of higher dimension will be flattened, then shifted.
         """
         v = self.flatten()
         match n:
             case int():
                 pass
             case Bits():
-                if n._v.has_illogical():
+                if n._v.has_x():
                     return illogicals((v.size,)), E
-                elif n._v.has_unknown():
+                elif n._v.has_dc():
                     return xes((v.size,)), E
                 else:
                     n = n.to_uint()
             case _:
                 raise TypeError("Expected n to be int or Bits")
         if ci is None:
             y, co = self._v.lsh(n)
@@ -390,17 +390,17 @@
         Vectors of higher dimension will be flattened, then shifted.
         """
         v = self.flatten()
         match n:
             case int():
                 pass
             case Bits():
-                if n._v.has_illogical():
+                if n._v.has_x():
                     return illogicals((v.size,)), E
-                elif n._v.has_unknown():
+                elif n._v.has_dc():
                     return xes((v.size,)), E
                 else:
                     n = n.to_uint()
             case _:
                 raise TypeError("Expected n to be int or Bits")
         if ci is None:
             y, co = self._v.rsh(n)
@@ -415,17 +415,17 @@
         Vectors of higher dimension will be flattened, then shifted.
         """
         v = self.flatten()
         match n:
             case int():
                 pass
             case Bits():
-                if n._v.has_illogical():
+                if n._v.has_x():
                     return illogicals((v.size,)), E
-                elif n._v.has_unknown():
+                elif n._v.has_dc():
                     return xes((v.size,)), E
                 else:
                     n = n.to_uint()
             case _:
                 raise TypeError("Expected n to be int or Bits")
         y, co = self._v.arsh(n)
         return _v2b(y), _v2b(co)
@@ -721,15 +721,15 @@
 # The empty vector is a singleton
 E = Bits((0,), 0)
 
 
 def illogicals(shape: tuple[int, ...]) -> Bits:
     """Return a new logic_vector of given shape, filled with ILLOGICAL."""
     n = math.prod(shape)
-    v = lbool.illogicals(n)
+    v = lbool.xes(n)
     return Bits(shape, v.data)
 
 
 def zeros(shape: tuple[int, ...]) -> Bits:
     """Return a new logic_vector of given shape, filled with zeros."""
     n = math.prod(shape)
     v = lbool.zeros(n)
@@ -742,15 +742,15 @@
     v = lbool.ones(n)
     return Bits(shape, v.data)
 
 
 def xes(shape: tuple[int, ...]) -> Bits:
     """Return a new logic_vector of given shape, filled with Xes."""
     n = math.prod(shape)
-    v = lbool.xes(n)
+    v = lbool.dcs(n)
     return Bits(shape, v.data)
 
 
 # One bit values
 W = illogicals((1,))
 F = zeros((1,))
 T = ones((1,))
```

### Comparing `seqlogic-0.0.7/src/seqlogic/design.py` & `seqlogic-0.0.8/src/seqlogic/design.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 
 from __future__ import annotations
 
 import inspect
 import re
 from abc import ABC
 from collections import defaultdict
+from collections.abc import Callable
 
 from vcd.writer import VarValue
 from vcd.writer import VCDWriter as VcdWriter
 
-from . import bits, hier, sim
-from .bits import F, T, xes
-from .sim import changed, get_loop
+from .hier import Branch, Leaf
+from .lbool import Vec, ones, xes, zeros
+from .sim import Aggregate, Region, SimAwaitable, Singular, State, changed, get_loop
 
 _item2char = {
     0b00: "x",
     0b01: "0",
     0b10: "1",
     0b11: "x",
 }
 
 
-def _bits2vcd(b: bits.Bits) -> VarValue:
+def _vec2vcd(v: Vec) -> VarValue:
     """Convert bit array to VCD value."""
     # pylint: disable = protected-access
-    return "".join(_item2char[b._v._get_item(i)] for i in range(b._v._n - 1, -1, -1))
+    return "".join(_item2char[v._get_item(i)] for i in range(len(v) - 1, -1, -1))
 
 
 class _TraceIf(ABC):
     """TODO(cjdrake): Write docstring."""
 
     def dump_waves(self, waves: defaultdict, pattern: str):
         """TODO(cjdrake): Write docstring."""
@@ -38,55 +39,67 @@
         """TODO(cjdrake): Write docstring."""
 
 
 class _ProcIf(ABC):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self):
-        self._procs = set()
+        self._procs = []
 
-        def is_proc_region(m):
-            return isinstance(m, tuple) and len(m) == 2 and inspect.iscoroutinefunction(m[0])
+        def is_proc(m) -> bool:
+            match m:
+                case [int(), Callable() as f] if inspect.iscoroutinefunction(f):
+                    return True
+                case _:
+                    return False
 
-        for _, (proc, region) in inspect.getmembers(self, is_proc_region):
-            self._procs.add((proc, region))
+        for _, (region, func) in inspect.getmembers(self, is_proc):
+            self._procs.append((region, func, (), {}))
 
     @property
     def procs(self):
         return self._procs
 
 
-class Module(hier.Branch, _TraceIf, _ProcIf):
+class Module(Branch, _TraceIf, _ProcIf):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, name: str, parent: Module | None = None):
         """TODO(cjdrake): Write docstring."""
-        hier.Branch.__init__(self, name, parent)
+        Branch.__init__(self, name, parent)
         _ProcIf.__init__(self)
 
+    @property
+    def scope(self) -> str:
+        """Return the branch's full name using dot separator syntax."""
+        if self._parent is None:
+            return self.name
+        assert isinstance(self._parent, Module)
+        return f"{self._parent.scope}.{self.name}"
+
     def dump_waves(self, waves: defaultdict, pattern: str):
         """TODO(cjdrake): Write docstring."""
         for child in self._children:
             assert isinstance(child, _TraceIf)
             child.dump_waves(waves, pattern)
 
     def dump_vcd(self, vcdw: VcdWriter, pattern: str):
         """TODO(cjdrake): Write docstring."""
         for child in self._children:
             assert isinstance(child, _TraceIf)
             child.dump_vcd(vcdw, pattern)
 
 
-class _TraceSingular(hier.Leaf, _TraceIf, sim.Singular, _ProcIf):
+class _TraceSingular(Leaf, _TraceIf, Singular, _ProcIf):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, name: str, parent: Module, value):
         """TODO(cjdrake): Write docstring."""
-        hier.Leaf.__init__(self, name, parent)
-        sim.Singular.__init__(self, value)
+        Leaf.__init__(self, name, parent)
+        Singular.__init__(self, value)
         _ProcIf.__init__(self)
         self._waves_change = None
         self._vcd_change = None
 
     def update(self):
         """TODO(cjdrake): Write docstring."""
         if self._waves_change and self.dirty():
@@ -94,112 +107,133 @@
         if self._vcd_change and self.dirty():
             self._vcd_change()
         super().update()
 
     def dump_waves(self, waves: defaultdict, pattern: str):
         """TODO(cjdrake): Write docstring."""
         if re.fullmatch(pattern, self.qualname):
-            t = self._sim.time()
+            t = self._sim.time
             waves[t][self] = self._value
 
             def change():
-                t = self._sim.time()
+                t = self._sim.time
                 waves[t][self] = self._next_value
 
             self._waves_change = change
 
     def dump_vcd(self, vcdw, pattern: str):
         """TODO(cjdrake): Write docstring."""
         assert isinstance(self._parent, Module)
         if re.match(pattern, self.qualname):
             var = vcdw.register_var(
                 scope=self._parent.scope,
                 name=self.name,
                 var_type="reg",
-                size=self._value.size,
-                init=_bits2vcd(self._value),
+                size=len(self._value),
+                init=_vec2vcd(self._value),
             )
 
             def change():
-                t = self._sim.time()
-                vcdw.change(var, t, _bits2vcd(self._next_value))
+                t = self._sim.time
+                vcdw.change(var, t, _vec2vcd(self._next_value))
 
             self._vcd_change = change
 
     def connect(self, src):
         """TODO(cjdrake): Write docstring."""
 
         async def proc():
             while True:
                 await changed(src)
                 self.next = src.next
 
-        self._procs.add((proc, 0))
+        self._procs.append((Region(0), proc, (), {}))
 
 
-class _TraceAggregate(hier.Leaf, _TraceIf, sim.Aggregate, _ProcIf):
+class _TraceAggregate(Leaf, _TraceIf, Aggregate, _ProcIf):
     """TODO(cjdrake): Write docstring."""
 
-    def __init__(self, name: str, parent: Module, shape: tuple[int, ...], value):
+    def __init__(self, name: str, parent: Module, value):
         """TODO(cjdrake): Write docstring."""
-        hier.Leaf.__init__(self, name, parent)
-        sim.Aggregate.__init__(self, shape, value)
+        Leaf.__init__(self, name, parent)
+        Aggregate.__init__(self, value)
         _ProcIf.__init__(self)
 
-    # def update(self):
-    #    """TODO(cjdrake): Write docstring."""
-    #    super().update()
-
 
 class Bits(_TraceSingular):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, name: str, parent: Module, shape: tuple[int, ...]):
         """TODO(cjdrake): Write docstring."""
-        super().__init__(name, parent, value=xes(shape))
+        assert len(shape) == 1
+        n = shape[0]
+        super().__init__(name, parent, value=xes(n))
 
 
 class Bit(Bits):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, name: str, parent: Module):
         """TODO(cjdrake): Write docstring."""
         super().__init__(name, parent, shape=(1,))
 
-    def posedge(self) -> bool:
+    def is_posedge(self) -> bool:
+        """TODO(cjdrake): Write docstring."""
+        return self._value == zeros(1) and self._next_value == ones(1)
+
+    async def posedge(self) -> State:
         """TODO(cjdrake): Write docstring."""
-        return self._value == F and self._next_value == T
+        self._sim.add_event(self, self.is_posedge)
+        state = await SimAwaitable()
+        return state
 
-    def negedge(self) -> bool:
+    def is_negedge(self) -> bool:
         """TODO(cjdrake): Write docstring."""
-        return self._value == T and self._next_value == F
+        return self._value == ones(1) and self._next_value == zeros(1)
+
+    async def negedge(self) -> State:
+        """TODO(cjdrake): Write docstring."""
+        self._sim.add_event(self, self.is_negedge)
+        state = await SimAwaitable()
+        return state
 
 
 class Enum(_TraceSingular):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, name: str, parent: Module, cls):
         """TODO(cjdrake): Write docstring."""
         super().__init__(name, parent, value=cls.X)
 
 
+class Struct(_TraceSingular):
+    """TODO(cjdrake): Write docstring."""
+
+    def __init__(self, name: str, parent: Module, cls):
+        """TODO(cjdrake): Write docstring."""
+        super().__init__(name, parent, value=cls())
+
+
 class Array(_TraceAggregate):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(
         self,
         name: str,
         parent: Module,
         unpacked_shape: tuple[int, ...],
         packed_shape: tuple[int, ...],
     ):
         """TODO(cjdrake): Write docstring."""
-        super().__init__(name, parent, unpacked_shape, value=xes(packed_shape))
+        assert len(unpacked_shape) == 1
+        assert len(packed_shape) == 1
+        n = packed_shape[0]
+        super().__init__(name, parent, value=xes(n))
 
 
 def simify(d: Module | Bits | Enum | Array):
     """TODO(cjdrake): Write docstring."""
     loop = get_loop()
     for node in d.iter_bfs():
         assert isinstance(node, _ProcIf)
-        for proc, region in node.procs:
-            loop.add_proc(proc, region)
+        for region, func, args, kwargs in node.procs:
+            loop.add_proc(region, func, *args, **kwargs)
```

### Comparing `seqlogic-0.0.7/src/seqlogic/hier.py` & `seqlogic-0.0.8/src/seqlogic/hier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,41 @@
-"""Logic Design Hierarchy."""
+"""Logic Design Hierarchy.
+
+Implement the fundamental components of an N-ary tree.
+A tree has branches and leaves.
+Leaves must have a parent.
+A branch may either have a parent, or no parent (the root).
+"""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Generator
 
 
 class Hierarchy(ABC):
     """Any hierarchical design element."""
 
-    def __init__(self, name: str, parent: Hierarchy | None):
-        """TODO(cjdrake): Write docstring."""
+    def __init__(self, name: str, parent: Branch | None):
+        """Initialize.
+
+        Args:
+            name: Name of this tree node.
+            parent: Parent tree node, or None.
+        """
         self._name = name
         self._parent = parent
 
     @property
     def name(self) -> str:
         """Return the design element name."""
         return self._name
 
     @property
-    def parent(self) -> Hierarchy | None:
+    def parent(self) -> Branch | None:
         """Return the parent, or None."""
         return self._parent
 
     @property
     @abstractmethod
     def qualname(self) -> str:
         """Return the design element's fully qualified name."""
@@ -38,67 +49,57 @@
         """Iterate through the design hierarchy in DFS order."""
 
 
 class Branch(Hierarchy):
     """Design hierarchy branch node."""
 
     def __init__(self, name: str, parent: Branch | None = None):
-        """TODO(cjdrake): Write docstring."""
         super().__init__(name, parent)
-        self._children: list[Hierarchy] = []
+        self._children: list[Branch | Leaf] = []
         if parent is not None:
             parent.add_child(self)
 
     @property
     def qualname(self) -> str:
-        """Return the branch's fully qualified name."""
         if self._parent is None:
             return f"/{self._name}"
         else:
             return f"{self._parent.qualname}/{self._name}"
 
     def iter_bfs(self) -> Generator[Hierarchy, None, None]:
-        """TODO(cjdrake): Write docstring."""
         yield self
         for child in self._children:
             yield from child.iter_bfs()
 
     def iter_dfs(self) -> Generator[Hierarchy, None, None]:
-        """TODO(cjdrake): Write docstring."""
         for child in self._children:
             yield from child.iter_dfs()
         yield self
 
-    @property
-    def scope(self) -> str:
-        """Return the branch's full name using dot separator syntax."""
-        if self._parent is None:
-            return self.name
-        assert isinstance(self._parent, Branch)
-        return f"{self._parent.scope}.{self.name}"
-
-    def add_child(self, child: Hierarchy):
+    def add_child(self, child: Branch | Leaf):
         """Add child branch or leaf."""
         self._children.append(child)
 
+    def is_root(self) -> bool:
+        """Return True if this branch is the root of the tree."""
+        return self._parent is None
+
 
 class Leaf(Hierarchy):
     """Design hierarchy leaf node."""
 
     def __init__(self, name: str, parent: Branch):
-        """TODO(cjdrake): Write docstring."""
         super().__init__(name, parent)
         parent.add_child(self)
 
+        # Help type checker verify parent is not None
+        self._parent: Branch
+
     @property
     def qualname(self) -> str:
-        """Return the leaf's fully qualified name."""
-        assert self._parent is not None
         return f"{self._parent.qualname}/{self._name}"
 
-    def iter_bfs(self) -> Generator[Leaf, None, None]:
-        """TODO(cjdrake): Write docstring."""
+    def iter_bfs(self) -> Generator[Hierarchy, None, None]:
         yield self
 
-    def iter_dfs(self) -> Generator[Leaf, None, None]:
-        """TODO(cjdrake): Write docstring."""
+    def iter_dfs(self) -> Generator[Hierarchy, None, None]:
         yield self
```

### Comparing `seqlogic-0.0.7/src/seqlogic/lbool.py` & `seqlogic-0.0.8/src/seqlogic/lbool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,357 +1,357 @@
 """Lifted Boolean scalar and vector data types.
 
 The conventional Boolean type consists of {False, True}, or {0, 1}.
 You can pack Booleans using an int, e.g. hex(0xaa | 0x55) == '0xff'.
 
-The "lifted" Boolean data type expands {0, 1} to {0, 1, Unknown, Illogical}.
+The "lifted" Boolean data type expands {0, 1} to {0, 1, Neither, DontCare}.
 
 Zero and One retain their original meanings.
 
-"Illogical" means neither zero nor one.
+"Neither" means neither zero nor one.
 This is an illogical or metastable value that always dominates other values.
+We will use a shorthand character 'X'.
 
-"Unknown" means either zero or one.
+"DontCare" means either zero or one.
 This is an unknown or uninitialized value that may either dominate or be
 dominated by other values, depending on the operation.
 
 The 'vec' class packs multiple lifted Booleans into a vector,
 which enables efficient, bit-wise operations and arithmetic.
 """
 
+# Simplify access to friend object attributes
 # pylint: disable = protected-access
 
+# PyLint/PyRight are confused by MetaClass behavior
+# pyright: reportAttributeAccessIssue=false
+
+
 from __future__ import annotations
 
 import re
 from collections.abc import Generator, Iterable
-from functools import cached_property
+from functools import cached_property, partial
 
 from .util import clog2
 
 _ITEM_BITS = 2
 _ITEM_MASK = 0b11
 
 # Scalars
-_ILLOGICAL = 0b00
-_ZERO = 0b01
-_ONE = 0b10
-_UNKNOWN = 0b11
+_X = 0b00
+_0 = 0b01
+_1 = 0b10
+_W = 0b11
+
+
+_LNOT = (_X, _1, _0, _W)
 
 
-def lnot(x: int) -> int:
+def not_(x: int) -> int:
     """Lifted NOT function.
 
     f(x) -> y:
-        ? => ? | 00 => 00
+        X => X | 00 => 00
         0 => 1 | 01 => 10
         1 => 0 | 10 => 01
-        X => X | 11 => 11
+        - => - | 11 => 11
     """
-    x_0 = x & 1
-    x_1 = x >> 1
+    return _LNOT[x]
 
-    y_0, y_1 = x_1, x_0
-    y = (y_1 << 1) | y_0
 
-    return y
+_LNOR = (
+    (_X, _X, _X, _X),
+    (_X, _1, _0, _W),
+    (_X, _0, _0, _0),
+    (_X, _W, _0, _W),
+)
 
 
-def lnor(x0: int, x1: int) -> int:
+def nor(x0: int, x1: int) -> int:
     """Lifted NOR function.
 
     f(x0, x1) -> y:
         0 0 => 1
-        1 X => 0
-        ? X => ?
-        X 0 => X
+        1 - => 0
+        X - => X
+        - 0 => -
 
            x1
            00 01 11 10
           +--+--+--+--+
     x0 00 |00|00|00|00|  y1 = x0[0] & x1[0]
           +--+--+--+--+
        01 |00|10|11|01|
           +--+--+--+--+
        11 |00|11|11|01|  y0 = x0[0] & x1[1]
           +--+--+--+--+     | x0[1] & x1[0]
        10 |00|01|01|01|     | x0[1] & x1[1]
           +--+--+--+--+
     """
-    x0_0 = x0 & 1
-    x0_1 = x0 >> 1
-    x1_0 = x1 & 1
-    x1_1 = x1 >> 1
+    return _LNOR[x0][x1]
 
-    y_0 = x0_0 & x1_1 | x0_1 & x1_0 | x0_1 & x1_1
-    y_1 = x0_0 & x1_0
-    y = (y_1 << 1) | y_0
 
-    return y
+_LOR = (
+    (_X, _X, _X, _X),
+    (_X, _0, _1, _W),
+    (_X, _1, _1, _1),
+    (_X, _W, _1, _W),
+)
 
 
-def lor(x0: int, x1: int) -> int:
+def or_(x0: int, x1: int) -> int:
     """Lifted OR function.
 
     f(x0, x1) -> y:
         0 0 => 0
-        1 X => 1
-        ? X => ?
-        X 0 => X
+        1 - => 1
+        X - => X
+        - 0 => -
 
            x1
            00 01 11 10
           +--+--+--+--+
     x0 00 |00|00|00|00|  y1 = x0[0] & x1[1]
           +--+--+--+--+     | x0[1] & x1[0]
        01 |00|01|11|10|     | x0[1] & x1[1]
           +--+--+--+--+
        11 |00|11|11|10|  y0 = x0[0] & x1[0]
           +--+--+--+--+
        10 |00|10|10|10|
           +--+--+--+--+
     """
-    x0_0 = x0 & 1
-    x0_1 = x0 >> 1
-    x1_0 = x1 & 1
-    x1_1 = x1 >> 1
+    return _LOR[x0][x1]
 
-    y_0 = x0_0 & x1_0
-    y_1 = x0_0 & x1_1 | x0_1 & x1_0 | x0_1 & x1_1
-    y = (y_1 << 1) | y_0
 
-    return y
+_LNAND = (
+    (_X, _X, _X, _X),
+    (_X, _1, _1, _1),
+    (_X, _1, _0, _W),
+    (_X, _1, _W, _W),
+)
 
 
-def lnand(x0: int, x1: int) -> int:
+def nand(x0: int, x1: int) -> int:
     """Lifted NAND function.
 
     f(x0, x1) -> y:
         1 1 => 0
-        0 X => 1
-        ? X => ?
-        X 1 => X
+        0 - => 1
+        X - => X
+        - 1 => -
 
            x1
            00 01 11 10
           +--+--+--+--+
     x0 00 |00|00|00|00|  y1 = x0[0] & x1[0]
           +--+--+--+--+     | x0[0] & x1[1]
        01 |00|10|10|10|     | x0[1] & x1[0]
           +--+--+--+--+
        11 |00|10|11|11|  y0 = x0[1] & x1[1]
           +--+--+--+--+
        10 |00|10|11|01|
           +--+--+--+--+
     """
-    x0_0 = x0 & 1
-    x0_1 = x0 >> 1
-    x1_0 = x1 & 1
-    x1_1 = x1 >> 1
+    return _LNAND[x0][x1]
 
-    y_0 = x0_1 & x1_1
-    y_1 = x0_0 & x1_0 | x0_0 & x1_1 | x0_1 & x1_0
-    y = (y_1 << 1) | y_0
 
-    return y
+_LAND = (
+    (_X, _X, _X, _X),
+    (_X, _0, _0, _0),
+    (_X, _0, _1, _W),
+    (_X, _0, _W, _W),
+)
 
 
-def land(x0: int, x1: int) -> int:
+def and_(x0: int, x1: int) -> int:
     """Lifted AND function.
 
     f(x0, x1) -> y:
         1 1 => 1
-        0 X => 0
-        ? X => ?
-        X 1 => X
+        0 - => 0
+        X - => X
+        - 1 => -
 
            x1
            00 01 11 10
           +--+--+--+--+
     x0 00 |00|00|00|00|  y1 = x0[1] & x1[1]
           +--+--+--+--+
        01 |00|01|01|01|
           +--+--+--+--+
        11 |00|01|11|11|  y0 = x0[0] & x1[0]
           +--+--+--+--+     | x0[0] & x1[1]
        10 |00|01|11|10|     | x0[1] & x1[0]
           +--+--+--+--+
     """
-    x0_0 = x0 & 1
-    x0_1 = x0 >> 1
-    x1_0 = x1 & 1
-    x1_1 = x1 >> 1
+    return _LAND[x0][x1]
 
-    y_0 = x0_0 & x1_0 | x0_0 & x1_1 | x0_1 & x1_0
-    y_1 = x0_1 & x1_1
-    y = (y_1 << 1) | y_0
 
-    return y
+_LXNOR = (
+    (_X, _X, _X, _X),
+    (_X, _1, _0, _W),
+    (_X, _0, _1, _W),
+    (_X, _W, _W, _W),
+)
 
 
-def lxnor(x0: int, x1: int) -> int:
+def xnor(x0: int, x1: int) -> int:
     """Lifted XNOR function.
 
     f(x0, x1) -> y:
         0 0 => 1
         0 1 => 0
         1 0 => 0
         1 1 => 1
-        ? X => ?
-        X 0 => X
-        X 1 => X
+        X - => X
+        - 0 => -
+        - 1 => -
 
            x1
            00 01 11 10
           +--+--+--+--+
     x0 00 |00|00|00|00|  y1 = x0[0] & x1[0]
           +--+--+--+--+     | x0[1] & x1[1]
        01 |00|10|11|01|
           +--+--+--+--+
        11 |00|11|11|11|  y0 = x0[0] & x1[1]
           +--+--+--+--+     | x0[1] & x1[0]
        10 |00|01|11|10|
           +--+--+--+--+
     """
-    x0_0 = x0 & 1
-    x0_1 = x0 >> 1
-    x1_0 = x1 & 1
-    x1_1 = x1 >> 1
+    return _LXNOR[x0][x1]
 
-    y_0 = x0_0 & x1_1 | x0_1 & x1_0
-    y_1 = x0_0 & x1_0 | x0_1 & x1_1
-    y = (y_1 << 1) | y_0
 
-    return y
+_LXOR = (
+    (_X, _X, _X, _X),
+    (_X, _0, _1, _W),
+    (_X, _1, _0, _W),
+    (_X, _W, _W, _W),
+)
 
 
-def lxor(x0: int, x1: int) -> int:
+def xor(x0: int, x1: int) -> int:
     """Lifted XOR function.
 
     f(x0, x1) -> y:
         0 0 => 0
         0 1 => 1
         1 0 => 1
         1 1 => 0
-        ? X => ?
-        X 0 => X
-        X 1 => X
+        X - => X
+        - 0 => -
+        - 1 => -
 
            x1
            00 01 11 10
           +--+--+--+--+
     x0 00 |00|00|00|00|  y1 = x0[0] & x1[1]
           +--+--+--+--+     | x0[1] & x1[0]
        01 |00|01|11|10|
           +--+--+--+--+
        11 |00|11|11|11|  y0 = x0[0] & x1[0]
           +--+--+--+--+     | x0[1] & x1[1]
        10 |00|10|11|01|
           +--+--+--+--+
     """
-    x0_0 = x0 & 1
-    x0_1 = x0 >> 1
-    x1_0 = x1 & 1
-    x1_1 = x1 >> 1
+    return _LXOR[x0][x1]
 
-    y_0 = x0_0 & x1_0 | x0_1 & x1_1
-    y_1 = x0_0 & x1_1 | x0_1 & x1_0
-    y = (y_1 << 1) | y_0
 
-    return y
+_LIMPLIES = (
+    (_X, _X, _X, _X),
+    (_X, _1, _1, _1),
+    (_X, _0, _1, _W),
+    (_X, _W, _1, _W),
+)
 
 
-def limplies(p: int, q: int) -> int:
+def implies(p: int, q: int) -> int:
     """Lifted IMPLIES function.
 
     f(p, q) -> y:
         0 0 => 1
         0 1 => 1
         1 0 => 0
         1 1 => 1
-        N X => N
-        0 X => 1
-        1 X => X
-        X 0 => X
-        X 1 => 1
-        X X => X
+        N - => N
+        0 - => 1
+        1 - => -
+        - 0 => -
+        - 1 => 1
+        - - => -
 
            q
            00 01 11 10
           +--+--+--+--+
      p 00 |00|00|00|00|  y1 = p[0] & q[0]
           +--+--+--+--+     | p[0] & q[1]
        01 |00|10|10|10|     | p[1] & q[1]
           +--+--+--+--+
        11 |00|11|11|10|  y0 = p[1] & q[0]
           +--+--+--+--+
        10 |00|01|11|10|
           +--+--+--+--+
     """
-    p_0 = p & 1
-    p_1 = p >> 1
-    q_0 = q & 1
-    q_1 = q >> 1
-
-    y_0 = p_1 & q_0
-    y_1 = p_0 & q_0 | p_0 & q_1 | p_1 & q_1
-    y = (y_1 << 1) | y_0
+    return _LIMPLIES[p][q]
+
 
-    return y
+_VecN = {}
 
 
 class Vec:
     """One dimensional vector of lbool items.
 
     Though it is possible to construct an lbool Vec directly,
     it is easier to use one of the factory functions:
 
     * vec
     * uint2vec
     * int2vec
-    * illogicals
+    * xes
     * zeros
     * ones
-    * xes
+    * dcs
     """
 
-    def __class_getitem__(cls, key: int):
-        pass  # pragma: no cover
+    def __class_getitem__(cls, n: int):
+        if n < 0:
+            raise ValueError(f"Expected n ≥ 0, got {n}")
+
+        if (vec_n := _VecN.get(n)) is None:
+            _VecN[n] = vec_n = type(f"Vec[{n}]", (Vec,), {"_n": n})
+        return vec_n
 
-    def __init__(self, n: int, data: int):
+    def __init__(self, data: int):
         """Initialize.
 
         Args:
-            n: Length
             data: lbool items packed into an int.
 
         Raises:
-            ValueError if n or data is invalid/inconsistent
+            ValueError if data is invalid/inconsistent
         """
-        if n < 0:
-            raise ValueError(f"Expected n ≥ 0, got {n}")
-        self._n = n
-
+        assert hasattr(self, "_n")
         a, b = 0, 1 << self.nbits
         if not a <= data < b:
             raise ValueError(f"Expected data in [{a}, {b}), got {data}")
         self._data = data
 
     def __len__(self) -> int:
         return self._n
 
     def __getitem__(self, key: int | slice) -> Vec:
         match key:
             case int() as i:
                 d = self._get_item(self._norm_index(i))
-                return Vec(1, d)
+                return Vec[1](d)
             case slice() as sl:
                 i, j = self._norm_slice(sl)
                 n, d = self._get_items(i, j)
-                return Vec(n, d)
+                return Vec[n](d)
             case _:
                 raise TypeError("Expected key to be int or slice")
 
     def __iter__(self) -> Generator[Vec[1], None, None]:
         for i in range(self._n):
             yield self.__getitem__(i)
 
@@ -363,16 +363,15 @@
         for i in range(self._n):
             if i % 4 == 0 and i != 0:
                 chars.append("_")
             chars.append(_to_char[self._get_item(i)])
         return prefix + "".join(reversed(chars))
 
     def __repr__(self) -> str:
-        d = f"0b{self._data:0{self.nbits}b}"
-        return f"vec({self._n}, {d})"
+        return f"Vec[{self._n}](0b{self._data:0{self.nbits}b})"
 
     def __bool__(self) -> bool:
         return self.to_uint() != 0
 
     def __int__(self) -> int:
         return self.to_int()
 
@@ -388,33 +387,33 @@
                 return False
 
     def __hash__(self) -> int:
         return hash(self._n) ^ hash(self._data)
 
     # Bitwise Arithmetic
     def __invert__(self) -> Vec:
-        return self.lnot()
+        return self.not_()
 
     def __or__(self, other: Vec) -> Vec:
-        return self.lor(other)
+        return self.or_(other)
 
     def __and__(self, other: Vec) -> Vec:
-        return self.land(other)
+        return self.and_(other)
 
     def __xor__(self, other: Vec) -> Vec:
-        return self.lxor(other)
+        return self.xor(other)
 
     def __lshift__(self, n: int) -> Vec:
         return self.lsh(n)[0]
 
     def __rshift__(self, n: int) -> Vec:
         return self.rsh(n)[0]
 
     def __add__(self, other: Vec) -> Vec:
-        return self.add(other, ci=_F)[0]
+        return self.add(other, ci=_Vec0)[0]
 
     def __sub__(self, other: Vec) -> Vec:
         return self.sub(other)[0]
 
     def __neg__(self) -> Vec:
         return self.neg()[0]
 
@@ -424,32 +423,32 @@
         return self._data
 
     @cached_property
     def nbits(self) -> int:
         """Number of bits of data."""
         return _ITEM_BITS * self._n
 
-    def lnot(self) -> Vec:
+    def not_(self) -> Vec:
         """Bitwise lifted NOT.
 
         Returns:
             vec of equal length and inverted data.
         """
         x_0 = self._bit_mask[0]
         x_01 = x_0 << 1
         x_1 = self._bit_mask[1]
         x_10 = x_1 >> 1
 
         y0 = x_10
         y1 = x_01
         y = y1 | y0
 
-        return Vec(self._n, y)
+        return Vec[self._n](y)
 
-    def lnor(self, other: Vec) -> Vec:
+    def nor(self, other: Vec) -> Vec:
         """Bitwise lifted NOR.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains NOR result.
@@ -469,17 +468,17 @@
         x1_1 = other._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_0 & x1_10 | x0_10 & x1_0 | x0_10 & x1_10
         y1 = x0_01 & x1_01
         y = y1 | y0
 
-        return Vec(self._n, y)
+        return Vec[self._n](y)
 
-    def lor(self, other: Vec) -> Vec:
+    def or_(self, other: Vec) -> Vec:
         """Bitwise lifted OR.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains OR result.
@@ -497,28 +496,28 @@
         x1_01 = x1_0 << 1
         x1_1 = other._bit_mask[1]
 
         y0 = x0_0 & x1_0
         y1 = x0_01 & x1_1 | x0_1 & x1_01 | x0_1 & x1_1
         y = y1 | y0
 
-        return Vec(self._n, y)
+        return Vec[self._n](y)
 
-    def ulor(self) -> Vec[1]:
+    def uor(self) -> Vec[1]:
         """Unary lifted OR reduction.
 
         Returns:
             One-bit vec, data contains OR reduction.
         """
-        data = _ZERO
+        data = _0
         for i in range(self._n):
-            data = lor(data, self._get_item(i))
-        return Vec(1, data)
+            data = or_(data, self._get_item(i))
+        return Vec[1](data)
 
-    def lnand(self, other: Vec) -> Vec:
+    def nand(self, other: Vec) -> Vec:
         """Bitwise lifted NAND.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains NAND result.
@@ -538,17 +537,17 @@
         x1_1 = other._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_10 & x1_10
         y1 = x0_01 & x1_01 | x0_01 & x1_1 | x0_1 & x1_01
         y = y1 | y0
 
-        return Vec(self._n, y)
+        return Vec[self._n](y)
 
-    def land(self, other: Vec) -> Vec:
+    def and_(self, other: Vec) -> Vec:
         """Bitwise lifted AND.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains AND result.
@@ -566,28 +565,28 @@
         x1_1 = other._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_0 & x1_0 | x0_0 & x1_10 | x0_10 & x1_0
         y1 = x0_1 & x1_1
         y = y1 | y0
 
-        return Vec(self._n, y)
+        return Vec[self._n](y)
 
-    def uland(self) -> Vec[1]:
+    def uand(self) -> Vec[1]:
         """Unary lifted AND reduction.
 
         Returns:
             One-bit vec, data contains AND reduction.
         """
-        data = _ONE
+        data = _1
         for i in range(self._n):
-            data = land(data, self._get_item(i))
-        return Vec(1, data)
+            data = and_(data, self._get_item(i))
+        return Vec[1](data)
 
-    def lxnor(self, other: Vec) -> Vec:
+    def xnor(self, other: Vec) -> Vec:
         """Bitwise lifted XNOR.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains XNOR result.
@@ -607,17 +606,17 @@
         x1_1 = other._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_0 & x1_10 | x0_10 & x1_0
         y1 = x0_01 & x1_01 | x0_1 & x1_1
         y = y1 | y0
 
-        return Vec(self._n, y)
+        return Vec[self._n](y)
 
-    def lxor(self, other: Vec) -> Vec:
+    def xor(self, other: Vec) -> Vec:
         """Bitwise lifted XOR.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains XOR result.
@@ -637,65 +636,68 @@
         x1_1 = other._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_0 & x1_0 | x0_10 & x1_10
         y1 = x0_01 & x1_1 | x0_1 & x1_01
         y = y1 | y0
 
-        return Vec(self._n, y)
+        return Vec[self._n](y)
 
-    def ulxnor(self) -> Vec[1]:
+    def uxnor(self) -> Vec[1]:
         """Unary lifted XNOR reduction.
 
         Returns:
             One-bit vec, data contains XNOR reduction.
         """
-        data = _ONE
+        data = _1
         for i in range(self._n):
-            data = lxnor(data, self._get_item(i))
-        return Vec(1, data)
+            data = xnor(data, self._get_item(i))
+        return Vec[1](data)
 
-    def ulxor(self) -> Vec[1]:
+    def uxor(self) -> Vec[1]:
         """Unary lifted XOR reduction.
 
         Returns:
             One-bit vec, data contains XOR reduction.
         """
-        data = _ZERO
+        data = _0
         for i in range(self._n):
-            data = lxor(data, self._get_item(i))
-        return Vec(1, data)
+            data = xor(data, self._get_item(i))
+        return Vec[1](data)
 
     def to_uint(self) -> int:
         """Convert to unsigned integer.
 
         Returns:
             An unsigned int.
 
         Raises:
             ValueError: vec is partially unknown.
         """
-        y = 0
-
-        if self.has_illogical() or self.has_unknown():
+        if self.has_unknown():
             raise ValueError("Cannot convert unknown to uint")
 
-        i, data = 0, self._data
-        while i <= (self._n - 8):
-            y |= _wyde_uint[data & _WYDE_MASK] << i
-            data >>= 16
-            i += 8
-        while i <= (self._n - 4):
-            y |= _byte_uint[data & _BYTE_MASK] << i
-            data >>= 8
-            i += 4
-        while i <= (self._n - 1):
-            y |= _item_uint[data & _ITEM_MASK] << i
-            data >>= 2
-            i += 1
+        y = 0
+        n, data = 0, self._data
+
+        stride = 8
+        while n <= (self._n - stride):
+            y |= _wyde_uint[data & _WYDE_MASK] << n
+            n += stride
+            data >>= _ITEM_BITS * stride
+        stride = 4
+        while n <= (self._n - stride):
+            y |= _byte_uint[data & _BYTE_MASK] << n
+            n += stride
+            data >>= _ITEM_BITS * stride
+        stride = 1
+        while n <= (self._n - stride):
+            y |= _item_uint[data & _ITEM_MASK] << n
+            n += stride
+            data >>= _ITEM_BITS * stride
 
         return y
 
     def to_int(self) -> int:
         """Convert to signed integer.
 
         Returns:
@@ -703,16 +705,16 @@
 
         Raises:
             ValueError: vec is partially unknown.
         """
         if self._n == 0:
             return 0
         sign = self._get_item(self._n - 1)
-        if sign == _ONE:
-            return -(self.lnot().to_uint() + 1)
+        if sign == _1:
+            return -(self.not_().to_uint() + 1)
         return self.to_uint()
 
     def ult(self, other: Vec) -> bool:
         """Unsigned less than.
 
         Args:
             other: vec of equal length.
@@ -753,16 +755,16 @@
         Raises:
             ValueError: If n is negative.
         """
         if n < 0:
             raise ValueError(f"Expected n ≥ 0, got {n}")
         if n == 0:
             return self
-        prefix = _fill(_ZERO, n)
-        return Vec(self._n + n, self._data | (prefix << self.nbits))
+        prefix = _fill(_0, n)
+        return Vec[self._n + n](self._data | (prefix << self.nbits))
 
     def sext(self, n: int) -> Vec:
         """Sign extend by n bits.
 
         Args:
             n: Non-negative number of bits.
 
@@ -774,88 +776,124 @@
         """
         if n < 0:
             raise ValueError(f"Expected n ≥ 0, got {n}")
         if n == 0:
             return self
         sign = self._get_item(self._n - 1)
         prefix = _fill(sign, n)
-        return Vec(self._n + n, self._data | (prefix << self.nbits))
+        return Vec[self._n + n](self._data | (prefix << self.nbits))
 
-    def lsh(self, n: int, ci: Vec[1] | None = None) -> tuple[Vec, Vec]:
+    def lsh(self, n: int | Vec, ci: Vec[1] | None = None) -> tuple[Vec, Vec]:
         """Left shift by n bits.
 
         Args:
             n: Non-negative number of bits.
             ci: Optional "carry in"
 
         Returns:
             vec left-shifted by n bits. If ci is provided, use it for shift
             input. Otherwise use zeros.
 
         Raises:
             ValueError: If n or ci are invalid/inconsistent.
         """
+        match n:
+            case int():
+                pass
+            case Vec():
+                if n.has_x():
+                    return xes(self._n), _VecE
+                elif n.has_dc():
+                    return dcs(self._n), _VecE
+                else:
+                    n = n.to_uint()
+            case _:
+                raise TypeError("Expected n to be int or Vec")
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
-            return self, _E
+            return self, _VecE
         if ci is None:
-            ci = Vec(n, _fill(_ZERO, n))
+            ci = Vec[n](_fill(_0, n))
         elif len(ci) != n:
             raise ValueError(f"Expected ci to have len {n}")
         sh, co = self[:-n], self[-n:]
-        y = Vec(self._n, ci._data | (sh._data << ci.nbits))
+        y = Vec[self._n](ci._data | (sh._data << ci.nbits))
         return y, co
 
-    def rsh(self, n: int, ci: Vec[1] | None = None) -> tuple[Vec, Vec]:
+    def rsh(self, n: int | Vec, ci: Vec[1] | None = None) -> tuple[Vec, Vec]:
         """Right shift by n bits.
 
         Args:
             n: Non-negative number of bits.
             ci: Optional "carry in"
 
         Returns:
             vec right-shifted by n bits. If ci is provided, use it for shift
             input. Otherwise use zeros.
 
         Raises:
             ValueError: If n or ci are invalid/inconsistent.
         """
+        match n:
+            case int():
+                pass
+            case Vec():
+                if n.has_x():
+                    return xes(self._n), _VecE
+                elif n.has_dc():
+                    return dcs(self._n), _VecE
+                else:
+                    n = n.to_uint()
+            case _:
+                raise TypeError("Expected n to be int or Vec")
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
-            return self, _E
+            return self, _VecE
         if ci is None:
-            ci = Vec(n, _fill(_ZERO, n))
+            ci = Vec[n](_fill(_0, n))
         elif len(ci) != n:
             raise ValueError(f"Expected ci to have len {n}")
         co, sh = self[:n], self[n:]
-        y = Vec(self._n, sh._data | (ci._data << sh.nbits))
+        y = Vec[self._n](sh._data | (ci._data << sh.nbits))
         return y, co
 
-    def arsh(self, n: int) -> tuple[Vec, Vec]:
+    def arsh(self, n: int | Vec) -> tuple[Vec, Vec]:
         """Arithmetically right shift by n bits.
 
         Args:
             n: Non-negative number of bits.
 
         Returns:
             vec arithmetically right-shifted by n bits.
 
         Raises:
             ValueError: If n is invalid.
         """
+        match n:
+            case int():
+                pass
+            case Vec():
+                if n.has_x():
+                    return xes(self._n), _VecE
+                elif n.has_dc():
+                    return dcs(self._n), _VecE
+                else:
+                    n = n.to_uint()
+            case _:
+                raise TypeError("Expected n to be int or Vec")
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
-            return self, _E
+            return self, _VecE
         sign = self._get_item(self._n - 1)
         ci_data = _fill(sign, n)
         co, sh = self[:n], self[n:]
-        y = Vec(self._n, sh._data | (ci_data << sh.nbits))
+        y = Vec[self._n](sh._data | (ci_data << sh.nbits))
         return y, co
 
     def add(self, other: Vec, ci: Vec[1]) -> tuple[Vec, Vec[1], Vec[1]]:
         """Twos complement addition.
 
         Args:
             other: vec of equal length.
@@ -867,30 +905,30 @@
             ValueError: vec lengths are invalid/inconsistent.
         """
         self._check_len(other)
 
         # Rename for readability
         n, a, b = self._n, self, other
 
-        if a.has_illogical() or b.has_illogical() or ci.has_illogical():
-            return Vec(n, _fill(_ILLOGICAL, n)), _W, _W
-        if a.has_unknown() or b.has_unknown() or ci.has_unknown():
-            return Vec(n, _fill(_UNKNOWN, n)), _X, _X
+        if a.has_x() or b.has_x() or ci.has_x():
+            return Vec[n](_fill(_X, n)), _VecX, _VecX
+        if a.has_dc() or b.has_dc() or ci.has_dc():
+            return Vec[n](_fill(_W, n)), _VecW, _VecW
 
         s = a.to_uint() + b.to_uint() + ci.to_uint()
 
         data = 0
         for i in range(n):
-            data |= _from_bit[s & 1] << (2 * i)
+            data |= _from_bit[s & 1] << (_ITEM_BITS * i)
             s >>= 1
 
         # Carry out is True if there is leftover sum data
-        co = (_F, _T)[s != 0]
+        co = (_Vec0, _Vec1)[s != 0]
 
-        s = Vec(n, data)
+        s = Vec[n](data)
 
         # Overflow is true if sign A matches sign B, and mismatches sign S
         aa = a[-1]
         bb = b[-1]
         ss = s[-1]
         ovf = ~aa & ~bb & ss | aa & bb & ~ss
 
@@ -904,78 +942,88 @@
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
 
         Raises:
             ValueError: vec lengths are invalid/inconsistent.
         """
-        return self.add(other.lnot(), ci=_T)
+        return self.add(other.not_(), ci=_Vec1)
 
     def neg(self) -> tuple[Vec, Vec[1], Vec[1]]:
         """Twos complement negation.
 
         Computed using 0 - self.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
         """
-        zero = Vec(self._n, _fill(_ZERO, self._n))
+        zero = Vec[self._n](_fill(_0, self._n))
         return zero.sub(self)
 
     def _check_len(self, other: Vec):
         if self._n != other._n:
             s = f"Expected n = {self._n}, got {other._n}"
             raise ValueError(s)
 
     def _count(self, byte_cnt: dict[int, int], item: int) -> int:
         y = 0
-
         n, data = self._n, self._data
-        while n >= 4:
+
+        stride = 4
+        while n >= stride:
             y += byte_cnt[data & _BYTE_MASK]
-            n -= 4
-            data >>= 8
-        while n >= 1:
+            n -= stride
+            data >>= _ITEM_BITS * stride
+        stride = 1
+        while n >= stride:
             y += (data & _ITEM_MASK) == item
-            n -= 1
-            data >>= 2
+            n -= stride
+            data >>= _ITEM_BITS * stride
 
         return y
 
-    def count_illogicals(self) -> int:
-        """Return number of ILLOGICAL items."""
-        return self._count(_byte_cnt_illogicals, _ILLOGICAL)
+    def count_xes(self) -> int:
+        """Return number of X items."""
+        return self._count(_byte_cnt_xes, _X)
 
     def count_zeros(self) -> int:
-        """Return number of ZERO items."""
-        return self._count(_byte_cnt_zeros, _ZERO)
+        """Return number of 0 items."""
+        return self._count(_byte_cnt_zeros, _0)
 
     def count_ones(self) -> int:
-        """Return number of ONE items."""
-        return self._count(_byte_cnt_ones, _ONE)
+        """Return number of 1 items."""
+        return self._count(_byte_cnt_ones, _1)
 
-    def count_unknowns(self) -> int:
-        """Return number of UNKNOWN items."""
-        return self._count(_byte_cnt_unknowns, _UNKNOWN)
+    def count_dcs(self) -> int:
+        """Return number of DC items."""
+        return self._count(_byte_cnt_dcs, _W)
+
+    def count_unknown(self) -> int:
+        """Return number of X/DC items."""
+        return self.count_xes() + self.count_dcs()
 
     def onehot(self) -> bool:
-        """Return True if vec contains exactly one ONE item."""
-        return not self.has_illogical() and not self.has_unknown() and self.count_ones() == 1
+        """Return True if vec contains exactly one 1 item."""
+        return not self.has_unknown() and self.count_ones() == 1
 
     def onehot0(self) -> bool:
-        """Return True if vec contains at most one ONE item."""
-        return not self.has_illogical() and not self.has_unknown() and self.count_ones() <= 1
+        """Return True if vec contains at most one 1 item."""
+        return not self.has_unknown() and self.count_ones() <= 1
 
-    def has_illogical(self) -> bool:
-        """Return True if vec contains at least one ILLOGICAL item."""
-        return self.count_illogicals() != 0
+    def has_x(self) -> bool:
+        """Return True if vec contains at least one X item."""
+        return self.count_xes() != 0
+
+    def has_dc(self) -> bool:
+        """Return True if vec contains at least one DC item."""
+        return self.count_dcs() != 0
 
     def has_unknown(self) -> bool:
-        """Return True if vec contains at least one UNKNOWN item."""
-        return self.count_unknowns() != 0
+        """Return True if vec contains at least one X/DC item."""
+        return self.count_unknown() != 0
 
     def _norm_index(self, index: int) -> int:
         a, b = -self._n, self._n
         if not a <= index < b:
             s = f"Expected index in [{a}, {b}), got {index}"
             raise IndexError(s)
         # Normalize negative start index
@@ -1008,15 +1056,15 @@
         n = j - i
         nbits = _ITEM_BITS * n
         mask = (1 << nbits) - 1
         return n, (self._data >> (_ITEM_BITS * i)) & mask
 
     @cached_property
     def _mask(self) -> tuple[int, int]:
-        zero_mask = _fill(_ZERO, self._n)
+        zero_mask = _fill(_0, self._n)
         one_mask = zero_mask << 1
         return zero_mask, one_mask
 
     @cached_property
     def _bit_mask(self) -> tuple[int, int]:
         return self._data & self._mask[0], self._data & self._mask[1]
 
@@ -1057,15 +1105,15 @@
     req_n = clog2(num + 1)
     if n is None:
         n = req_n
     elif n < req_n:
         s = f"Overflow: num = {num} required n ≥ {req_n}, got {n}"
         raise ValueError(s)
 
-    return Vec(i, data).zext(n - i)
+    return Vec[i](data).zext(n - i)
 
 
 def int2vec(num: int, n: int | None = None) -> Vec:
     """Convert int to vec.
 
     Args:
         num: An integer.
@@ -1095,90 +1143,95 @@
         req_n = clog2(num + 1) + 1
     if n is None:
         n = req_n
     elif n < req_n:
         s = f"Overflow: num = {num} required n ≥ {req_n}, got {n}"
         raise ValueError(s)
 
-    v = Vec(i, data).zext(n - i)
+    v = Vec[i](data).zext(n - i)
     return v.neg()[0] if neg else v
 
 
-_NUM_RE = re.compile(
-    r"((?P<BinSize>[0-9]+)b(?P<BinDigits>[?01X_]+))|"
-    r"((?P<HexSize>[0-9]+)h(?P<HexDigits>[0-9a-fA-F_]+))"
-)
-
-
 def bools2vec(xs: Iterable[int]) -> Vec:
     """Convert an iterable of bools to a vec.
 
     This is a convenience function.
     For data in the form of [0, 1, 0, 1, ...],
     or [False, True, False, True, ...].
     """
     i, data = 0, 0
     for x in xs:
         data |= _from_bit[x] << (_ITEM_BITS * i)
         i += 1
-    return Vec(i, data)
+    return Vec[i](data)
 
 
-def lit2vec(lit: str) -> Vec:
-    """Convert a string literal to a vec.
-
-    A string literal is in the form {width}{base}{characters},
-    where width is the number of bits, base is either 'b' for binary or
-    'h' for hexadecimal, and characters is a string of legal characters.
-    The character string can contains '_' separators for readability.
-
-    For example:
-        4b1010
-        6b11_X10?
-        64hdead_beef_feed_face
+_NUM_RE = re.compile(
+    r"((?P<BinSize>[0-9]+)b(?P<BinDigits>[X01\-_]+))|"
+    r"((?P<HexSize>[0-9]+)h(?P<HexDigits>[0-9a-fA-F_]+))"
+)
 
-    Returns:
-        A Vec instance.
 
-    Raises:
-        ValueError: If input literal has a syntax error.
-    """
+def _lit2vec(lit: str) -> tuple[int, int]:
     if m := _NUM_RE.match(lit):
         # Binary
         if m.group("BinSize"):
             size = int(m.group("BinSize"))
             digits = m.group("BinDigits").replace("_", "")
             ndigits = len(digits)
             if ndigits != size:
                 s = f"Expected {size} digits, got {ndigits}"
                 raise ValueError(s)
             i, data = 0, 0
             for c in reversed(digits):
                 data |= _from_char[c] << (i * _ITEM_BITS)
                 i += 1
-            return Vec(i, data)
+            return i, data
         # Hexadecimal
         elif m.group("HexSize"):
             size = int(m.group("HexSize"))
             digits = m.group("HexDigits").replace("_", "")
             ndigits = len(digits)
             if 4 * ndigits != size:
                 s = f"Expected size to match # digits, got {size} ≠ {4 * ndigits}"
                 raise ValueError(s)
             i, data = 0, 0
             for c in reversed(digits):
                 data |= _from_hexchar[c] << (i * _ITEM_BITS)
                 i += 4
-            return Vec(i, data)
+            return i, data
         else:  # pragma: no cover
             assert False
     else:
         raise ValueError(f"Expected str literal, got {lit}")
 
 
+def lit2vec(lit: str) -> Vec:
+    """Convert a string literal to a vec.
+
+    A string literal is in the form {width}{base}{characters},
+    where width is the number of bits, base is either 'b' for binary or
+    'h' for hexadecimal, and characters is a string of legal characters.
+    The character string can contains '_' separators for readability.
+
+    For example:
+        4b1010
+        6b11_-10X
+        64hdead_beef_feed_face
+
+    Returns:
+        A Vec instance.
+
+    Raises:
+        ValueError: If input literal has a syntax error.
+    """
+    n, data = _lit2vec(lit)
+    return Vec[n](data)
+
+
 def vec(obj=None) -> Vec:
     """Create a Vec using standard input formats.
 
     vec() or vec(None) will return the empty vec
     vec(False | True) will return a length 1 vec
     vec([False | True, ...]) will return a length n vec
     vec(str) will parse a string literal and return an arbitrary vec
@@ -1189,76 +1242,306 @@
     Returns:
         A Vec instance.
 
     Raises:
         TypeError: If input obj is invalid.
     """
     match obj:
-        case None:
-            return Vec(0, 0)
+        case None | []:
+            return _VecE
         case 0 | 1 as x:
-            return bools2vec([x])
+            return (_Vec0, _Vec1)[x]
         case [0 | 1 as x, *rst]:
             return bools2vec([x, *rst])
         case str() as lit:
             return lit2vec(lit)
         case _:
             raise TypeError(f"Invalid input: {obj}")
 
 
+def cat(*objs: int | Vec) -> Vec:
+    """Concatenate a sequence of vectors.
+
+    Args:
+        objs: a sequence of bools.
+
+    Returns:
+        A Vec instance.
+
+    Raises:
+        TypeError: If input obj is invalid.
+    """
+    if len(objs) == 0:
+        return _VecE
+
+    # Convert inputs
+    vs = []
+    for obj in objs:
+        match obj:
+            case 0 | 1 as x:
+                vs.append((_Vec0, _Vec1)[x])
+            case Vec() as v:
+                vs.append(v)
+            case _:
+                raise TypeError(f"Invalid input: {obj}")
+
+    if len(vs) == 1:
+        return vs[0]
+
+    i, data = 0, 0
+    for v in vs:
+        data |= v.data << (_ITEM_BITS * i)
+        i += len(v)
+    return Vec[i](data)
+
+
+def rep(obj: int | Vec, n: int) -> Vec:
+    """Repeat a vector n times."""
+    objs = [obj] * n
+    return cat(*objs)
+
+
 def _consts(x: int, n: int) -> Vec:
     if n < 0:
         raise ValueError(f"Expected n ≥, got {n}")
-    return Vec(n, _fill(x, n))
+    return Vec[n](_fill(x, n))
 
 
-def illogicals(n: int) -> Vec:
-    """Return a vec packed with n ILLOGICAL items."""
-    return _consts(_ILLOGICAL, n)
+def xes(n: int) -> Vec:
+    """Return a vec packed with n X items."""
+    return _consts(_X, n)
 
 
 def zeros(n: int) -> Vec:
-    """Return a vec packed with n ZERO items."""
-    return _consts(_ZERO, n)
+    """Return a vec packed with n 0 items."""
+    return _consts(_0, n)
 
 
 def ones(n: int) -> Vec:
-    """Return a vec packed with n ONE items."""
-    return _consts(_ONE, n)
+    """Return a vec packed with n 1 items."""
+    return _consts(_1, n)
 
 
-def xes(n: int) -> Vec:
-    """Return a vec packed with n UNKNOWN items."""
-    return _consts(_UNKNOWN, n)
+def dcs(n: int) -> Vec:
+    """Return a vec packed with n DC items."""
+    return _consts(_W, n)
 
 
 # Empty
-_E = Vec(0, 0)
+_VecE = Vec[0](0)
 
 # One bit values
-_W = Vec(1, _ILLOGICAL)
-_F = Vec(1, _ZERO)
-_T = Vec(1, _ONE)
-_X = Vec(1, _UNKNOWN)
+_VecX = Vec[1](_X)
+_Vec0 = Vec[1](_0)
+_Vec1 = Vec[1](_1)
+_VecW = Vec[1](_W)
+
+
+class _VecEnumMeta(type):
+    """Enum Metaclass: Create enum base classes."""
+
+    def __new__(mcs, name, bases, attrs):
+        # Base case for API
+        if name == "VecEnum":
+            return super().__new__(mcs, name, bases, attrs)
+
+        base_attrs = {}
+        # ident = literal
+        lit2name: dict[str, str] = {}
+        data2name: dict[int, str] = {}
+        n = None
+        for key, val in attrs.items():
+            if key.startswith("__"):
+                base_attrs[key] = val
+            else:
+                if n is None:
+                    n, data = _lit2vec(val)
+                else:
+                    n_i, data = _lit2vec(val)
+                    if n_i != n:
+                        raise ValueError(f"Expected lit len {n}, got {n_i}")
+                if key == "X":
+                    raise ValueError("Cannot use reserved name = 'X'")
+                if data == 0:
+                    raise ValueError("Cannot use reserved data = 0")
+                lit2name[val] = key
+                data2name[data] = key
+
+        # Empty Enum
+        if n is None:
+            # Create class
+            super_cls = Vec[0]
+            cls = super().__new__(mcs, name, bases + (super_cls,), base_attrs)
+            cls._data2name = data2name
+            # Instantiate member
+            obj = object.__new__(cls)  # pyright: ignore[reportArgumentType]
+            super_cls.__init__(obj, 0)
+            # Define methods
+            cls.__new__ = lambda c: obj
+            cls.__init__ = lambda s: None
+            cls.name = property(fget=lambda self: "")
+
+            return cls
+
+        # Add X member
+        x_lit = f"{n}b" + "X" * n
+        lit2name[x_lit] = "X"
+        data2name[0] = "X"
+
+        def _new(cls, arg: str | int):
+            match arg:
+                case str() as lit:
+                    try:
+                        name = lit2name[lit]
+                    except KeyError as e:
+                        raise ValueError(f"Invalid lit: {lit}") from e
+                case int() as data:
+                    try:
+                        name = data2name[data]
+                    except KeyError as e:
+                        raise ValueError(f"Invalid data: {data}") from e
+                case _:
+                    raise TypeError("Expected arg to be str or int")
+            return getattr(cls, name)
+
+        # Create class
+        super_cls = Vec[n]
+        cls = super().__new__(mcs, name, bases + (super_cls,), base_attrs)
+        cls._data2name = data2name
+
+        # Instantiate members
+        for data, name in data2name.items():
+            obj = object.__new__(cls)  # pyright: ignore[reportArgumentType]
+            super_cls.__init__(obj, data)
+            obj._name = name
+            setattr(cls, name, obj)
+
+        # Define methods
+        cls.__new__ = _new
+        cls.__init__ = lambda s, lit: None
+        cls.name = property(fget=lambda self: self._name)
+
+        return cls
+
+
+class VecEnum(metaclass=_VecEnumMeta):
+    """Enum Base Class: Create enums."""
+
+
+def _vec_struct_init(fields: list[tuple[str, type]]) -> str:
+    """Return code for a Struct __init__ method w/ fields."""
+    lines = []
+    line = "def init(self"
+    for field_name, field_type in fields:
+        line += f", {field_name}: {field_type.__name__} | None = None"
+    line += "):\n"
+    lines.append(line)
+    lines.append("    _n = 0\n")
+    lines.append("    _data = 0\n")
+    for field_name, field_type in fields:
+        offset = f"({_ITEM_BITS} * self._{field_name}_base)"
+        lines.append(f"    self._{field_name}_base = _n\n")
+        lines.append(f"    self._{field_name}_size = {field_type._n}\n")
+        lines.append(f"    _n += self._{field_name}_size\n")
+        lines.append(f"    if {field_name} is not None:\n")
+        lines.append(f"        _data |= {field_name}.data << {offset}\n")
+    lines.append("    self._data = _data\n")
+    return "".join(lines)
+
+
+class _VecStructMeta(type):
+    """Struct Metaclass: Create struct base classes."""
+
+    def __new__(mcs, name, bases, attrs):
+        # Base case for API
+        if name == "VecStruct":
+            return super().__new__(mcs, name, bases, attrs)
+
+        # Scan attributes for field_name: field_type items
+        base_attrs = {}
+        # ident: vec_type
+        fields: list[tuple[str, type]] = []
+        for key, val in attrs.items():
+            if key == "__annotations__":
+                for field_name, field_type in val.items():
+                    fields.append((field_name, field_type))
+            else:
+                base_attrs[key] = val
+
+        # Create Struct class
+        n = sum(field_type._n for _, field_type in fields)
+        cls = super().__new__(mcs, name, bases + (Vec[n],), base_attrs)
+
+        # Create Struct.__init__
+        code = _vec_struct_init(fields)
+        d = {}
+        exec(code, None, d)  # pylint: disable=exec-used
+        cls.__init__ = d["init"]
+
+        # Create Struct.__str__
+        def _str(self):
+            args = []
+            for fn, ft in fields:
+                v = getattr(self, fn)
+                if issubclass(ft, VecEnum):
+                    arg = f"{fn}={ft.__name__}.{ft._data2name[v.data]}"
+                else:
+                    arg = f"{fn}={v!s}"
+                args.append(arg)
+            return f'{name}({", ".join(args)})'
+
+        cls.__str__ = _str
+
+        # Create Struct.__repr__
+        def _repr(self):
+            args = []
+            for fn, ft in fields:
+                v = getattr(self, fn)
+                if issubclass(ft, VecEnum):
+                    arg = f"{fn}={ft.__name__}.{ft._data2name[v.data]}"
+                else:
+                    arg = f"{fn}={v!r}"
+                args.append(arg)
+            return f'{name}({", ".join(args)})'
+
+        cls.__repr__ = _repr
+
+        # Create Struct fields
+        def _fget(name, cls, self):
+            n = getattr(self, f"_{name}_size")
+            nbits = _ITEM_BITS * n
+            mask = (1 << nbits) - 1
+            i = getattr(self, f"_{name}_base")
+            data = (self._data >> (_ITEM_BITS * i)) & mask
+            return cls(data)
+
+        for fn, ft in fields:
+            setattr(cls, fn, property(fget=partial(_fget, fn, ft)))
+
+        return cls
+
+
+class VecStruct(metaclass=_VecStructMeta):
+    """Struct Base Class: Create struct."""
 
 
-_from_bit = (_ZERO, _ONE)
+_from_bit = (_0, _1)
 
 _from_char = {
-    "?": _ILLOGICAL,
-    "0": _ZERO,
-    "1": _ONE,
-    "X": _UNKNOWN,
+    "X": _X,
+    "0": _0,
+    "1": _1,
+    "-": _W,
 }
 
 _to_char = {
-    _ILLOGICAL: "?",
-    _ZERO: "0",
-    _ONE: "1",
-    _UNKNOWN: "X",
+    _X: "X",
+    _0: "0",
+    _1: "1",
+    _W: "-",
 }
 
 _from_hexchar = {
     "0": 0b01_01_01_01,
     "1": 0b01_01_01_10,
     "2": 0b01_01_10_01,
     "3": 0b01_01_10_10,
@@ -1278,15 +1561,15 @@
     "D": 0b10_10_01_10,
     "e": 0b10_10_10_01,
     "E": 0b10_10_10_01,
     "f": 0b10_10_10_10,
     "F": 0b10_10_10_10,
 }
 
-_byte_cnt_illogicals = {
+_byte_cnt_xes = {
     0b00_00_00_00: 4,
     0b00_00_00_01: 3,
     0b00_00_00_10: 3,
     0b00_00_00_11: 3,
     0b00_00_01_00: 3,
     0b00_00_01_01: 2,
     0b00_00_01_10: 2,
@@ -2055,15 +2338,15 @@
     0b11_11_10_11: 1,
     0b11_11_11_00: 0,
     0b11_11_11_01: 0,
     0b11_11_11_10: 1,
     0b11_11_11_11: 0,
 }
 
-_byte_cnt_unknowns = {
+_byte_cnt_dcs = {
     0b00_00_00_00: 0,
     0b00_00_00_01: 0,
     0b00_00_00_10: 0,
     0b00_00_00_11: 1,
     0b00_00_01_00: 0,
     0b00_00_01_01: 0,
     0b00_00_01_10: 0,
```

### Comparing `seqlogic-0.0.7/src/seqlogic/sim.py` & `seqlogic-0.0.8/src/seqlogic/sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from functools import partial
 from typing import NewType, TypeAlias
 
 Region = NewType("Region", int)
 
 
 _INIT_TIME = -1
-_INIT_REGION = Region(-1)
 _START_TIME = 0
 
 
 class State(ABC):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, value):
@@ -42,30 +41,24 @@
         raise NotImplementedError()
 
 
 class Singular(State):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, value):
-        """TODO(cjdrake): Write docstring."""
         super().__init__(value)
-
         self._value = self._init_value
         self._next_value = self._init_value
         self._changed = False
 
     def get_value(self):
         """TODO(cjdrake): Write docstring."""
         return self._value
 
-    def set_value(self, value):
-        """TODO(cjdrake): Write docstring."""
-        self._value = self._next_value = value
-
-    value = property(fget=get_value, fset=set_value)
+    value = property(fget=get_value)
 
     def get_next(self):
         """TODO(cjdrake): Write docstring."""
         return self._next_value
 
     def set_next(self, value):
         """TODO(cjdrake): Write docstring."""
@@ -74,72 +67,79 @@
 
         # Notify the event loop
         _sim.touch(self)
 
     next = property(fget=get_next, fset=set_next)
 
     def changed(self) -> bool:
-        """TODO(cjdrake): Write docstring."""
         return self._changed
 
     def update(self):
-        """TODO(cjdrake): Write docstring."""
         self._value = self._next_value
         self._changed = False
 
     def dirty(self) -> bool:
         """TODO(cjdrake): Write docstring."""
         return self._next_value != self._value
 
 
 class Aggregate(State):
     """TODO(cjdrake): Write docstring."""
 
-    def __init__(self, shape: tuple[int, ...], value):
-        """TODO(cjdrake): Write docstring."""
+    def __init__(self, value):
         super().__init__(value)
-
-        # TODO(cjdrake): Use this for index checking
-        self._shape = shape
         self._values = defaultdict(lambda: self._init_value)
         self._next_values = defaultdict(lambda: self._init_value)
         self._changed = set()
 
-    def get_value(self, index):
+    def get_value(self, index: int):
         """TODO(cjdrake): Write docstring."""
         return self._values[index]
 
-    def set_value(self, index, value):
-        """TODO(cjdrake): Write docstring."""
-        self._values[index] = self._next_values[index] = value
-
-    def get_next(self, index):
+    def get_next(self, index: int):
         """TODO(cjdrake): Write docstring."""
         return self._next_values[index]
 
-    def set_next(self, index, value):
+    def set_next(self, index: int, value):
         """TODO(cjdrake): Write docstring."""
         if value != self._next_values[index]:
             self._changed.add(index)
         self._next_values[index] = value
 
         # Notify the event loop
         _sim.touch(self)
 
+    def __getitem__(self, key: int):
+        return _ItemWrap(self, key)
+
     def changed(self) -> bool:
-        """TODO(cjdrake): Write docstring."""
         return bool(self._changed)
 
     def update(self):
-        """TODO(cjdrake): Write docstring."""
         for index in self._changed:
             self._values[index] = self._next_values[index]
         self._changed.clear()
 
 
+class _ItemWrap:
+    """Wrap Aggregate item getter/setter"""
+
+    def __init__(self, obj: Aggregate, index: int):
+        self._obj = obj
+        self._index = index
+
+    def _get_next(self):
+        return self._obj.get_next(self._index)
+
+    def _set_next(self, value):
+        self._obj.set_next(self._index, value)
+
+    next = property(fget=_get_next, fset=_set_next)
+
+
 _SimQueueItem: TypeAlias = tuple[int, Region, Coroutine, State | None]
 
 
 class _SimQueue:
     """Priority queue for ordering task execution."""
 
     def __init__(self):
@@ -151,15 +151,15 @@
     def __bool__(self) -> bool:
         return bool(self._items)
 
     def clear(self):
         self._items.clear()
         self._index = 0
 
-    def push(self, time: int, region: Region, task: Coroutine, state: State | None):
+    def push(self, time: int, region: Region, task: Coroutine, state: State | None = None):
         heapq.heappush(self._items, (time, region, self._index, task, state))
         self._index += 1
 
     def peek(self) -> _SimQueueItem:
         time, region, _, task, state = self._items[0]
         return (time, region, task, state)
 
@@ -175,15 +175,15 @@
             if t == time and r == region:
                 heapq.heappop(self._items)
                 yield (time, region, task, state)
             else:
                 break
 
 
-class _SimAwaitable(Awaitable):
+class SimAwaitable(Awaitable):
     """Suspend execution of the current task."""
 
     def __await__(self):
         state = yield
         return state
 
 
@@ -191,15 +191,15 @@
     """Simulation event loop."""
 
     def __init__(self):
         """TODO(cjdrake): Write docstring."""
         self._started: bool = False
         # Simulation time
         self._time: int = _INIT_TIME
-        self._region: Region = _INIT_REGION
+        self._region: Region | None = None
         # Task queue
         self._queue = _SimQueue()
         # Currently executing task
         self._task: Coroutine | None = None
         self._task_region: dict[Coroutine, Region] = {}
         # Dynamic event dependencies
         self._waiting: dict[State, set[Coroutine]] = defaultdict(set)
@@ -214,65 +214,66 @@
         """TODO(cjdrake): Write docstring."""
         return self._started
 
     def restart(self):
         """Restart the simulation."""
         self._started = False
         self._time = _INIT_TIME
-        self._region = _INIT_REGION
+        self._region = None
         self._queue.clear()
         self._task = None
         self._waiting.clear()
         self._triggers.clear()
         self._touched.clear()
 
     def reset(self):
         """Reset the simulation state."""
         self.restart()
         self._procs.clear()
         self._task_region.clear()
 
+    @property
     def time(self) -> int:
         """TODO(cjdrake): Write docstring."""
         return self._time
 
-    def region(self) -> Region:
+    @property
+    def region(self) -> Region | None:
         """TODO(cjdrake): Write docstring."""
         return self._region
 
-    def task(self) -> Coroutine:
+    @property
+    def task(self) -> Coroutine | None:
         """TODO(cjdrake): Write docstring."""
-        assert self._task is not None
         return self._task
 
     def call_soon(self, task: Coroutine, state: State | None = None):
         """Schedule the task in the current timeslot."""
         region = self._task_region[task]
         self._queue.push(self._time, region, task, state)
 
     def call_later(self, delay: int, task: Coroutine):
         """Schedule the task after a relative delay."""
         region = self._task_region[task]
-        self._queue.push(self._time + delay, region, task, None)
+        self._queue.push(self._time + delay, region, task)
 
     def call_at(self, when: int, task: Coroutine):
         """Schedule the task for an absolute timeslot."""
         region = self._task_region[task]
-        self._queue.push(when, region, task, None)
+        self._queue.push(when, region, task)
 
-    def add_proc(self, proc, region: Region, *args, **kwargs):
+    def add_proc(self, region: Region, func, *args, **kwargs):
         """Add a process to run at start of simulation."""
-        self._procs.append((proc, region, args, kwargs))
+        self._procs.append((region, func, args, kwargs))
 
-    def add_event(self, event: Callable[[], bool]):
+    def add_event(self, state: State, cond: Callable[[], bool]):
         """Add a conditional state => task dependency."""
         assert self._task is not None
-        state = event.__self__
         self._waiting[state].add(self._task)
-        self._triggers[state][self._task] = event
+        self._triggers[state][self._task] = cond
 
     def touch(self, state: State):
         """Notify dependent tasks about state change."""
         tasks = [task for task in self._waiting[state] if self._triggers[state][task]()]
         for task in tasks:
             self.call_soon(task, state)
             self._waiting[state].remove(task)
@@ -294,16 +295,16 @@
             case int(), None:
                 return max(_START_TIME, self._time) + ticks
             case _:
                 s = "Expected either ticks or until to be int | None"
                 raise TypeError(s)
 
     def _start(self):
-        for proc, region, args, kwargs in self._procs:
-            task = proc(*args, **kwargs)
+        for region, func, args, kwargs in self._procs:
+            task = func(*args, **kwargs)
             self._task_region[task] = region
             self.call_at(_START_TIME, task)
         self._started = True
 
     def run(self, ticks: int | None = None, until: int | None = None):
         """Run the simulation.
 
@@ -327,19 +328,21 @@
             # Next task scheduled: same time slot, different region
             if time == self._time and region != self._region:
                 self._region = region
             # Next task scheduled: future time slot
             elif time > self._time:
                 # Update all simulation state
                 self._update_state()
+
                 # Exit if we hit the run limit
                 if limit is not None and time >= limit:
                     break
                 # Otherwise, advance
                 self._time = time
+                self._region = region
 
             # Resume execution
             for _, _, self._task, state in self._queue.pop_region():
                 try:
                     self._task.send(state)
                 except StopIteration:
                     pass
@@ -370,19 +373,21 @@
             if time == self._time and region != self._region:
                 self._region = region
             # Next task scheduled: future time slot
             elif time > self._time:
                 # Update all simulation state
                 self._update_state()
                 yield self._time
+
                 # Exit if we hit the run limit
                 if limit is not None and time >= limit:
                     return
                 # Otherwise, advance
                 self._time = time
+                self._region = region
 
             # Resume execution
             for _, _, self._task, state in self._queue.pop_region():
                 try:
                     self._task.send(state)
                 except StopIteration:
                     pass
@@ -395,66 +400,67 @@
 
 
 _sim = Sim()
 
 
 async def sleep(delay: int):
     """Suspend the task, and wake up after a delay."""
-    _sim.call_later(delay, _sim.task())
-    await _SimAwaitable()
-
-
-async def notify(*events: Callable[[], bool]) -> State:
-    """Suspend the task, and wake up after an event notification."""
-    for event in events:
-        _sim.add_event(event)
-    var = await _SimAwaitable()
-    return var
+    assert _sim.task is not None
+    _sim.call_later(delay, _sim.task)
+    await SimAwaitable()
 
 
 async def changed(*states: State) -> State:
     """TODO(cjdrake): Write docstring."""
     for state in states:
-        _sim.add_event(state.changed)
-    var = await _SimAwaitable()
-    return var
+        _sim.add_event(state, state.changed)
+    state = await SimAwaitable()
+    return state
+
+
+async def resume(*events: tuple[State, Callable[[], bool]]) -> State:
+    """TODO(cjdrake): Write docstring."""
+    for state, cond in events:
+        _sim.add_event(state, cond)
+    state = await SimAwaitable()
+    return state
 
 
 def get_loop() -> Sim:
     """Return the event loop."""
     return _sim
 
 
 class _Schedule:
     """TODO(cjdrake): Write docstring."""
 
-    def __init__(self, func, region: Region):
+    def __init__(self, region: Region, func):
+        self._region = region
         assert inspect.iscoroutinefunction(func)
         self._func = func
-        self._region = region
 
     def __get__(self, obj, cls=None):
-        return (partial(self._func, obj), self._region)
+        return self._region, partial(self._func, obj)
 
 
 class initial(_Schedule):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, func):
         """TODO(cjdrake): Write docstring."""
-        super().__init__(func, Region(2))
+        super().__init__(Region(2), func)
 
 
 class always_ff(_Schedule):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, func):
         """TODO(cjdrake): Write docstring."""
-        super().__init__(func, Region(1))
+        super().__init__(Region(1), func)
 
 
 class always_comb(_Schedule):
     """TODO(cjdrake): Write docstring."""
 
     def __init__(self, func):
         """TODO(cjdrake): Write docstring."""
-        super().__init__(func, Region(0))
+        super().__init__(Region(0), func)
```

### Comparing `seqlogic-0.0.7/src/seqlogic/util.py` & `seqlogic-0.0.8/src/seqlogic/util.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.7/src/seqlogic.egg-info/PKG-INFO` & `seqlogic-0.0.8/src/seqlogic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.0.7
+Version: 0.0.8
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
 
 Sequential Logic (`seqlogic`) is a logic simulation library.
 It uses Python's `async` / `await` syntax to model time,
-and provides an N-dimensional `logicvec` data type for combinational logic.
+and provides an N-dimensional `bits` data type for combinational logic.
 
 The API design is a work in progress, and documentation has not started.
 See the `tests` directory for example usage.
 
 # Installing
 
 Sequential Logic is available on [PyPI](https://pypi.org):
```

### Comparing `seqlogic-0.0.7/src/seqlogic.egg-info/SOURCES.txt` & `seqlogic-0.0.8/src/seqlogic.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 README.md
 pyproject.toml
 src/seqlogic/__init__.py
 src/seqlogic/bits.py
 src/seqlogic/design.py
-src/seqlogic/enum.py
 src/seqlogic/hier.py
 src/seqlogic/lbool.py
 src/seqlogic/sim.py
 src/seqlogic/util.py
 src/seqlogic.egg-info/PKG-INFO
 src/seqlogic.egg-info/SOURCES.txt
 src/seqlogic.egg-info/dependency_links.txt
@@ -20,8 +19,9 @@
 tests/test_enum.py
 tests/test_fsm.py
 tests/test_gray.py
 tests/test_hier.py
 tests/test_lbool.py
 tests/test_lfsr.py
 tests/test_riscv.py
-tests/test_sim.py
+tests/test_sim.py
+tests/test_struct.py
```

### Comparing `seqlogic-0.0.7/tests/test_aes.py` & `seqlogic-0.0.8/tests/test_aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.7/tests/test_bits.py` & `seqlogic-0.0.8/tests/test_bits.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,122 +14,122 @@
     """Fix Me."""
     b = bits([W, F, T, X])
     assert b.shape == (4,)
 
 
 def test_not():
     """Test bits NOT method."""
-    b0 = bits("4bX10?")
-    assert str(~b0) == "bits(4bX01?)"
+    b0 = bits("4b-10X")
+    assert str(~b0) == "bits(4b-01X)"
 
     # NOT preserves the shape
     b1 = bits([bits("4b1010"), bits("4b0101")])
     assert str(~b1) == "bits([4b0101, 4b1010])"
 
 
 def test_nor():
     """Test bits NOR method."""
-    b0 = bits("16bXXXX_1111_0000_????")
-    b1 = bits("16bX10?_X10?_X10?_X10?")
-    assert str(b0.lnor(b1)) == "bits(16bX0X?_000?_X01?_????)"
+    b0 = bits("16b----_1111_0000_XXXX")
+    b1 = bits("16b-10X_-10X_-10X_-10X")
+    assert str(b0.lnor(b1)) == "bits(16b-0-X_000X_-01X_XXXX)"
 
 
 def test_or():
     """Test bits OR method."""
-    b0 = bits("16bXXXX_1111_0000_????")
-    b1 = bits("16bX10?_X10?_X10?_X10?")
-    assert str(b0 | b1) == "bits(16bX1X?_111?_X10?_????)"
+    b0 = bits("16b----_1111_0000_XXXX")
+    b1 = bits("16b-10X_-10X_-10X_-10X")
+    assert str(b0 | b1) == "bits(16b-1-X_111X_-10X_XXXX)"
 
 
 def test_nand():
     """Test bits NAND method."""
-    b0 = bits("16bXXXX_1111_0000_????")
-    b1 = bits("16bX10?_X10?_X10?_X10?")
-    assert str(b0.lnand(b1)) == "bits(16bXX1?_X01?_111?_????)"
+    b0 = bits("16b----_1111_0000_XXXX")
+    b1 = bits("16b-10X_-10X_-10X_-10X")
+    assert str(b0.lnand(b1)) == "bits(16b--1X_-01X_111X_XXXX)"
 
 
 def test_and():
     """Test bits AND method."""
-    b0 = bits("16bXXXX_1111_0000_????")
-    b1 = bits("16bX10?_X10?_X10?_X10?")
-    assert str(b0 & b1) == "bits(16bXX0?_X10?_000?_????)"
+    b0 = bits("16b----_1111_0000_XXXX")
+    b1 = bits("16b-10X_-10X_-10X_-10X")
+    assert str(b0 & b1) == "bits(16b--0X_-10X_000X_XXXX)"
 
 
 def test_xnor():
     """Test bits XNOR method."""
-    b0 = bits("16bXXXX_1111_0000_????")
-    b1 = bits("16bX10?_X10?_X10?_X10?")
-    assert str(b0.lxnor(b1)) == "bits(16bXXX?_X10?_X01?_????)"
+    b0 = bits("16b----_1111_0000_XXXX")
+    b1 = bits("16b-10X_-10X_-10X_-10X")
+    assert str(b0.lxnor(b1)) == "bits(16b---X_-10X_-01X_XXXX)"
 
 
 def test_xor():
     """Test bits XOR method."""
-    b0 = bits("16bXXXX_1111_0000_????")
-    b1 = bits("16bX10?_X10?_X10?_X10?")
-    assert str(b0 ^ b1) == "bits(16bXXX?_X01?_X10?_????)"
+    b0 = bits("16b----_1111_0000_XXXX")
+    b1 = bits("16b-10X_-10X_-10X_-10X")
+    assert str(b0 ^ b1) == "bits(16b---X_-01X_-10X_XXXX)"
 
 
 def test_uor():
     """Test bits unary OR method."""
-    assert bits("2b??").ulor() == W
-    assert bits("2b0?").ulor() == W
-    assert bits("2b1?").ulor() == W
-    assert bits("2bX?").ulor() == W
-    assert bits("2b?0").ulor() == W
+    assert bits("2bXX").ulor() == W
+    assert bits("2b0X").ulor() == W
+    assert bits("2b1X").ulor() == W
+    assert bits("2b-X").ulor() == W
+    assert bits("2bX0").ulor() == W
     assert bits("2b00").ulor() == F
     assert bits("2b10").ulor() == T
-    assert bits("2bX0").ulor() == X
-    assert bits("2b?1").ulor() == W
+    assert bits("2b-0").ulor() == X
+    assert bits("2bX1").ulor() == W
     assert bits("2b01").ulor() == T
     assert bits("2b11").ulor() == T
-    assert bits("2bX1").ulor() == T
-    assert bits("2b?X").ulor() == W
-    assert bits("2b0X").ulor() == X
-    assert bits("2b1X").ulor() == T
-    assert bits("2bXX").ulor() == X
+    assert bits("2b-1").ulor() == T
+    assert bits("2bX-").ulor() == W
+    assert bits("2b0-").ulor() == X
+    assert bits("2b1-").ulor() == T
+    assert bits("2b--").ulor() == X
 
 
 def test_uand():
     """Test bits unary AND method."""
-    assert bits("2b??").uland() == W
-    assert bits("2b0?").uland() == W
-    assert bits("2b1?").uland() == W
-    assert bits("2bX?").uland() == W
-    assert bits("2b?0").uland() == W
+    assert bits("2bXX").uland() == W
+    assert bits("2b0X").uland() == W
+    assert bits("2b1X").uland() == W
+    assert bits("2b-X").uland() == W
+    assert bits("2bX0").uland() == W
     assert bits("2b00").uland() == F
     assert bits("2b10").uland() == F
-    assert bits("2bX0").uland() == F
-    assert bits("2b?1").uland() == W
+    assert bits("2b-0").uland() == F
+    assert bits("2bX1").uland() == W
     assert bits("2b01").uland() == F
     assert bits("2b11").uland() == T
-    assert bits("2bX1").uland() == X
-    assert bits("2b?X").uland() == W
-    assert bits("2b0X").uland() == F
-    assert bits("2b1X").uland() == X
-    assert bits("2bXX").uland() == X
+    assert bits("2b-1").uland() == X
+    assert bits("2bX-").uland() == W
+    assert bits("2b0-").uland() == F
+    assert bits("2b1-").uland() == X
+    assert bits("2b--").uland() == X
 
 
 def test_uxor():
     """Test bits unary XOR method."""
-    assert bits("2b??").ulxor() == W
-    assert bits("2b0?").ulxor() == W
-    assert bits("2b1?").ulxor() == W
-    assert bits("2bX?").ulxor() == W
-    assert bits("2b?0").ulxor() == W
+    assert bits("2bXX").ulxor() == W
+    assert bits("2b0X").ulxor() == W
+    assert bits("2b1X").ulxor() == W
+    assert bits("2b-X").ulxor() == W
+    assert bits("2bX0").ulxor() == W
     assert bits("2b00").ulxor() == F
     assert bits("2b10").ulxor() == T
-    assert bits("2bX0").ulxor() == X
-    assert bits("2b?1").ulxor() == W
+    assert bits("2b-0").ulxor() == X
+    assert bits("2bX1").ulxor() == W
     assert bits("2b01").ulxor() == T
     assert bits("2b11").ulxor() == F
-    assert bits("2bX1").ulxor() == X
-    assert bits("2b?X").ulxor() == W
-    assert bits("2b0X").ulxor() == X
-    assert bits("2b1X").ulxor() == X
-    assert bits("2bXX").ulxor() == X
+    assert bits("2b-1").ulxor() == X
+    assert bits("2bX-").ulxor() == W
+    assert bits("2b0-").ulxor() == X
+    assert bits("2b1-").ulxor() == X
+    assert bits("2b--").ulxor() == X
 
 
 def test_zext():
     """Test bits zext method."""
     assert bits("4b1010").zext(4) == bits("8b0000_1010")
     # Zero extension on multi-dimensional array will flatten
     assert bits(["4b0000", "4b1111"]).zext(2) == bits("10b00_1111_0000")
@@ -333,15 +333,15 @@
         bits("8hdead")
 
     # Invalid input
     with pytest.raises(ValueError):
         bits("invalid")
 
     # Valid input
-    b = bits("4bX1_0?")
+    b = bits("4b-1_0X")
     assert b._v.data == 0b11_10_01_00
     b = bits("64hFeDc_Ba98_7654_3210")
     assert b._v.data == 0xAAA9_A6A5_9A99_9695_6A69_6665_5A59_5655
     b = bits("64hfEdC_bA98_7654_3210")
     assert b._v.data == 0xAAA9_A6A5_9A99_9695_6A69_6665_5A59_5655
 
 
@@ -426,18 +426,18 @@
     assert b0.size == 1
     assert b0._v.nbits == 2
     assert list(b0.flat) == [F]
 
     assert b0.flatten() == b0
 
     # Test __str__
-    assert str(bn) == "bits([?])"
+    assert str(bn) == "bits([X])"
     assert str(b0) == "bits([0])"
     assert str(b1) == "bits([1])"
-    assert str(bx) == "bits([X])"
+    assert str(bx) == "bits([-])"
 
     # Test __repr__
     assert repr(bn) == "bits((1,), 0b00)"
     assert repr(b0) == "bits((1,), 0b01)"
     assert repr(b1) == "bits((1,), 0b10)"
     assert repr(bx) == "bits((1,), 0b11)"
 
@@ -465,30 +465,30 @@
     assert b1.to_int() == -1
     with pytest.raises(ValueError):
         assert bx.to_uint()
 
 
 def test_rank1_str():
     """Test bits rank1 string input."""
-    b = bits("8bX10?_X10?")
+    b = bits("8b-10X_-10X")
     data = 0b11100100_11100100
     xs = [W, F, T, X] * 2
 
     # Test properties
     assert b.shape == (8,)
     assert b._v.data == data
     assert b.ndim == 1
     assert b.size == 8
     assert b._v.nbits == 16
     assert list(b.flat) == xs
 
     assert b.flatten() == b
 
     # Test __str__ and __repr__
-    assert str(b) == "bits(8bX10?_X10?)"
+    assert str(b) == "bits(8b-10X_-10X)"
     assert repr(b) == "bits((8,), 0b1110010011100100)"
 
     # Test __len__
     assert len(b) == 8
 
     # Test __iter__
     assert list(b) == xs
@@ -496,15 +496,15 @@
     # Test __getitem__
     assert b[0] == W
     assert b[1] == F
     assert b[6] == T
     assert b[7] == X
 
     # Test __eq__
-    assert b == bits("8bX10?_X10?")
+    assert b == bits("8b-10X_-10X")
     # Same data, different shape
     assert b != b.reshape((2, 4))
     with pytest.raises(ValueError):
         b.reshape((42,))
     # Different data, same shape
     assert b != bits("8b0000_0000")
 
@@ -521,105 +521,105 @@
     assert bits("4b1110").to_int() == -2
     assert bits("4b1111").to_int() == -1
 
 
 def test_rank1_logic():
     """Test bits function w/ rank1 logic input."""
     xs = [W, F, T, X]
-    b1 = bits("4bX10?")
+    b1 = bits("4b-10X")
     b2 = bits([0, 1, 0, 1])
 
     # Test properties
     assert b1.shape == (4,)
     assert b1._v.data == 0b11100100
     assert b1.ndim == 1
     assert b1.size == 4
     assert b1._v.nbits == 8
     assert list(b1.flat) == xs
 
     # Test __str__
-    assert str(b1) == "bits(4bX10?)"
+    assert str(b1) == "bits(4b-10X)"
     assert str(b2) == "bits(4b1010)"
 
     # Test __repr__
     assert repr(b1) == "bits((4,), 0b11100100)"
     assert repr(b2) == "bits((4,), 0b10011001)"
 
 
 def test_rank2_str():
     """Test bits function w/ rank2 str input."""
-    b = bits(["4bX10?", "4bX10?"])
+    b = bits(["4b-10X", "4b-10X"])
 
-    assert b.flatten() == bits("8bX10?_X10?")
+    assert b.flatten() == bits("8b-10X_-10X")
 
     # Test __str__
-    assert str(b) == "bits([4bX10?, 4bX10?])"
+    assert str(b) == "bits([4b-10X, 4b-10X])"
 
     # Test __repr__
     assert repr(b) == "bits((2, 4), 0b1110010011100100)"
 
 
 def test_rank2_vec():
     """Test bits function w/ rank2 bits input."""
-    b = bits([bits("4bX10?"), bits("4bX10?")])
+    b = bits([bits("4b-10X"), bits("4b-10X")])
 
     # Test __str__
-    assert str(b) == "bits([4bX10?, 4bX10?])"
+    assert str(b) == "bits([4b-10X, 4b-10X])"
 
     # Test __repr__
     assert repr(b) == "bits((2, 4), 0b1110010011100100)"
 
 
 def test_rank2_errors():
     """Test bits function rank2 errors."""
     # Mismatched str literal
     with pytest.raises(TypeError):
-        bits(["4bX10?", "3b10?"])
+        bits(["4b-10X", "3b10X"])
     # bits followed by some invalid type
     with pytest.raises(TypeError):
-        bits(["4bX10?", 42])
+        bits(["4b-10X", 42])
 
 
 R3VEC = """\
-bits([[4bX10?, 4bX10?],
-      [4bX10?, 4bX10?]])"""
+bits([[4b-10X, 4b-10X],
+      [4b-10X, 4b-10X]])"""
 
 
 def test_rank3_vec():
     """Test bits function w/ rank3 input."""
     b = bits(
         [
-            [bits("4bX10?"), bits("4bX10?")],
-            [bits("4bX10?"), bits("4bX10?")],
+            [bits("4b-10X"), bits("4b-10X")],
+            [bits("4b-10X"), bits("4b-10X")],
         ]
     )
 
-    assert b.flatten() == bits("16bX10?_X10?_X10?_X10?")
+    assert b.flatten() == bits("16b-10X_-10X_-10X_-10X")
 
     # Test __str__
     assert str(b) == R3VEC
 
     # Test __repr__
     assert repr(b) == "bits((2, 2, 4), 0b11100100111001001110010011100100)"
 
 
 R4VEC = """\
-bits([[[4bX10?, 4bX10?],
-       [4bX10?, 4bX10?]],
+bits([[[4b-10X, 4b-10X],
+       [4b-10X, 4b-10X]],
 
-      [[4bX10?, 4bX10?],
-       [4bX10?, 4bX10?]]])"""
+      [[4b-10X, 4b-10X],
+       [4b-10X, 4b-10X]]])"""
 
 
 def test_rank4_vec():
     """Test bits function w/ rank4 input."""
     b = bits(
         [
-            [[bits("4bX10?"), bits("4bX10?")], [bits("4bX10?"), bits("4bX10?")]],
-            [[bits("4bX10?"), bits("4bX10?")], [bits("4bX10?"), bits("4bX10?")]],
+            [[bits("4b-10X"), bits("4b-10X")], [bits("4b-10X"), bits("4b-10X")]],
+            [[bits("4b-10X"), bits("4b-10X")], [bits("4b-10X"), bits("4b-10X")]],
         ]
     )
 
     # Test __str__
     assert str(b) == R4VEC
 
     # Test __repr__
@@ -671,18 +671,18 @@
 
     b = rep(bits("2b00"), 4, flatten=False)
     assert b.shape == (4, 2)
 
 
 def test_consts():
     """Test bits constants."""
-    assert illogicals((8,)) == bits("8b????_????")
+    assert illogicals((8,)) == bits("8bXXXX_XXXX")
     assert zeros((8,)) == bits("8b0000_0000")
     assert ones((8,)) == bits("8b1111_1111")
-    assert xes((8,)) == bits("8bXXXX_XXXX")
+    assert xes((8,)) == bits("8b----_----")
 
 
 def test_slicing():
     """Test bits slicing behavior."""
     b = bits(
         [
             [bits("4b0000"), bits("4b0001"), bits("4b0010"), bits("4b0011")],
@@ -748,19 +748,19 @@
         b[0, 0, 0, 0]
     with pytest.raises(TypeError):
         b["invalid"]  # pyright: ignore[reportArgumentType]
 
 
 def test_countbits():
     """Test bits countbits methods."""
-    b = bits("8bX10?_X10?")
-    assert b._v.count_illogicals() == 2
+    b = bits("8b-10X_-10X")
+    assert b._v.count_xes() == 2
     assert b._v.count_zeros() == 2
     assert b._v.count_ones() == 2
-    assert b._v.count_unknowns() == 2
+    assert b._v.count_dcs() == 2
 
     assert bits("4b0000")._v.count_ones() == 0
     assert bits("4b0001")._v.count_ones() == 1
     assert bits("4b0011")._v.count_ones() == 2
     assert bits("4b0111")._v.count_ones() == 3
     assert bits("4b1111")._v.count_ones() == 4
 
@@ -771,11 +771,11 @@
     assert not bits("4b1101")._v.onehot()
 
     assert bits("4b0000")._v.onehot0()
     assert bits("4b1000")._v.onehot0()
     assert not bits("4b1010")._v.onehot0()
     assert not bits("4b1011")._v.onehot0()
 
-    assert not bits("4b0000")._v.has_unknown()
-    assert not bits("4b1111")._v.has_unknown()
-    assert bits("4b0X01")._v.has_unknown()
-    assert bits("4b01?1")._v.has_illogical()
+    assert not bits("4b0000")._v.has_dc()
+    assert not bits("4b1111")._v.has_dc()
+    assert bits("4b0-01")._v.has_dc()
+    assert bits("4b01X1")._v.has_x()
```

### Comparing `seqlogic-0.0.7/tests/test_fsm.py` & `seqlogic-0.0.8/tests/test_fsm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 """Example FSM implementation.
 
 Demonstrate usage of an enum.
 """
 
 from collections import defaultdict
 
-from seqlogic import Bit, Enum, Module, get_loop, notify
-from seqlogic.bits import F, T, X
-from seqlogic.enum import Enum as EnumVal
+from seqlogic import Bit, Enum, Module, get_loop
+from seqlogic.lbool import VecEnum, ones, xes, zeros
 from seqlogic.sim import Region
 
 from .common import p_clk, p_dff, p_rst
 
 # pyright: reportAttributeAccessIssue=false
 # pyright: reportReturnType=false
 
 
 loop = get_loop()
 
 
-class SeqDetect(EnumVal):
+class SeqDetect(VecEnum):
     """Sequence Detector state."""
 
     A = "2b00"
     B = "2b01"
     C = "2b10"
     D = "2b11"
 
 
 async def p_input(
     x: Bit,
     reset_n: Bit,
     clock: Bit,
 ):
-    """TODO(cjdrake): Write docstring."""
-    await notify(reset_n.negedge)
-    x.next = F
-
-    await notify(reset_n.posedge)
-    await notify(clock.posedge)
-    await notify(clock.posedge)
-    x.next = T  # A => B
-
-    await notify(clock.posedge)
-    x.next = T  # B => C
+    await reset_n.negedge()
+    x.next = zeros(1)
 
-    await notify(clock.posedge)
-    x.next = T  # C => D
+    await reset_n.posedge()
+    await clock.posedge()
+    await clock.posedge()
+    x.next = ones(1)  # A => B
 
-    await notify(clock.posedge)
-    x.next = T  # D => D
+    await clock.posedge()
+    x.next = ones(1)  # B => C
 
-    await notify(clock.posedge)
-    x.next = F  # D => A
+    await clock.posedge()
+    x.next = ones(1)  # C => D
+
+    await clock.posedge()
+    x.next = ones(1)  # D => D
+
+    await clock.posedge()
+    x.next = zeros(1)  # D => A
 
 
 def test_fsm():
     """Test a 3-bit LFSR."""
     loop.reset()
 
     top = Module(name="top")
@@ -90,118 +88,118 @@
                     return SeqDetect.D
                 else:
                     return SeqDetect.A
             case _:
                 return SeqDetect.X
 
     # Schedule input
-    loop.add_proc(p_input, Region(1), x, reset_n, clock)
+    loop.add_proc(Region(1), p_input, x, reset_n, clock)
 
     # Schedule LFSR
-    loop.add_proc(p_dff, Region(1), ps, ns, reset_n, SeqDetect.A, clock)
+    loop.add_proc(Region(1), p_dff, ps, ns, reset_n, SeqDetect.A, clock)
 
     # Schedule reset and clock
     # Note: Avoiding simultaneous reset/clock negedge/posedge on purpose
-    loop.add_proc(p_rst, Region(2), reset_n, init=T, phase1=6, phase2=10)
-    loop.add_proc(p_clk, Region(2), clock, init=F, shift=5, phase1=5, phase2=5)
+    loop.add_proc(Region(2), p_rst, reset_n, init=ones(1), phase1=6, phase2=10)
+    loop.add_proc(Region(2), p_clk, clock, init=zeros(1), shift=5, phase1=5, phase2=5)
 
     loop.run(until=100)
 
     exp = {
         # Initialize everything to X'es
         -1: {
-            reset_n: X,
-            clock: X,
-            x: X,
+            reset_n: xes(1),
+            clock: xes(1),
+            x: xes(1),
             ps: SeqDetect.X,
         },
         0: {
-            reset_n: T,
-            clock: F,
+            reset_n: ones(1),
+            clock: zeros(1),
         },
         # clock.posedge; reset_n = 1
         5: {
-            clock: T,
+            clock: ones(1),
         },
         # reset_n.negedge
         6: {
-            reset_n: F,
-            x: F,
+            reset_n: zeros(1),
+            x: zeros(1),
             ps: SeqDetect.A,
         },
         10: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge; reset_n = 0
         15: {
-            clock: T,
+            clock: ones(1),
         },
         # reset_n.posedge
         16: {
-            reset_n: T,
+            reset_n: ones(1),
         },
         20: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge; reset_n = 1
         25: {
-            clock: T,
+            clock: ones(1),
         },
         30: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge
         35: {
-            clock: T,
-            x: T,
+            clock: ones(1),
+            x: ones(1),
         },
         40: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge
         45: {
-            clock: T,
+            clock: ones(1),
             ps: SeqDetect.B,
         },
         50: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge
         55: {
-            clock: T,
+            clock: ones(1),
             ps: SeqDetect.C,
         },
         60: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge
         65: {
-            clock: T,
+            clock: ones(1),
             ps: SeqDetect.D,
         },
         70: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge
         75: {
-            clock: T,
-            x: F,
+            clock: ones(1),
+            x: zeros(1),
             # ps: D => D
         },
         80: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge
         85: {
-            clock: T,
+            clock: ones(1),
             ps: SeqDetect.A,
         },
         90: {
-            clock: F,
+            clock: zeros(1),
         },
         # clock.posedge
         95: {
-            clock: T,
+            clock: ones(1),
         },
     }
 
     assert waves == exp
```

### Comparing `seqlogic-0.0.7/tests/test_gray.py` & `seqlogic-0.0.8/tests/test_gray.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test Gray Code Algorithm."""
 
 from seqlogic.algorithms.gray import bin2gray, gray2bin
-from seqlogic.bits import uint2bits
+from seqlogic.lbool import uint2vec
 
 B2G_EXP = [
     0b0000,
     0b0001,
     0b0011,
     0b0010,
     0b0110,
@@ -22,14 +22,15 @@
     0b1000,
 ]
 
 
 def test_bin2gray():
     """Test bin2gray function."""
     for b, g in enumerate(B2G_EXP):
-        assert bin2gray(uint2bits(b, 4)).to_uint() == g
+        assert bin2gray(uint2vec(b, 4)).to_uint() == g
 
 
 def test_gray2bin():
     """Test gray2bin function."""
     for b, g in enumerate(B2G_EXP):
-        assert gray2bin(uint2bits(g, 4)).to_uint() == b
+        temp = gray2bin(uint2vec(g, 4)).to_uint()
+        assert temp == b
```

### Comparing `seqlogic-0.0.7/tests/test_hier.py` & `seqlogic-0.0.8/tests/test_hier.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.7/tests/test_lbool.py` & `seqlogic-0.0.8/tests/test_lbool.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,372 +4,366 @@
 # pylint: disable = protected-access
 
 import pytest
 
 from seqlogic import lbool
 from seqlogic.lbool import (
     Vec,
+    and_,
+    cat,
+    dcs,
+    implies,
     int2vec,
-    land,
-    limplies,
-    lnand,
-    lnor,
-    lnot,
-    lor,
-    lxnor,
-    lxor,
+    nand,
+    nor,
+    not_,
+    or_,
+    rep,
     uint2vec,
     vec,
+    xes,
+    xnor,
+    xor,
 )
 
-E = Vec(0, 0)
+E = Vec[0](0)
+F = vec(False)
+T = vec(True)
+
 
 LNOT = {
-    "?": "?",
+    "X": "X",
     "0": "1",
     "1": "0",
-    "X": "X",
+    "-": "-",
 }
 
 
 def test_vec():
-    """Test seqlogic.lbool.vec function."""
-    assert vec() == Vec(0, 0)
-    assert vec(None) == Vec(0, 0)
-    assert vec(False) == Vec(1, 0b01)
-    assert vec(True) == Vec(1, 0b10)
-    assert vec(0) == Vec(1, 0b01)
-    assert vec(1) == Vec(1, 0b10)
-    assert vec([False, True, 0, 1]) == Vec(4, 0b10_01_10_01)
+    assert vec() == Vec[0](0)
+    assert vec(None) == Vec[0](0)
+    assert vec(False) == Vec[1](0b01)
+    assert vec(True) == Vec[1](0b10)
+    assert vec(0) == Vec[1](0b01)
+    assert vec(1) == Vec[1](0b10)
+    assert vec([False, True, 0, 1]) == Vec[4](0b10_01_10_01)
 
     # Invalid input type
     with pytest.raises(TypeError):
         vec({"key": "val"})
 
 
 def test_lnot():
-    """Test seqlogic.lbool.lnot function."""
     for x, y in LNOT.items():
         x = lbool._from_char[x]
         y = lbool._from_char[y]
-        assert lnot(x) == y
+        assert not_(x) == y
 
 
-LNOR = {
-    "??": "?",
-    "?0": "?",
-    "?1": "?",
-    "?X": "?",
-    "0?": "?",
+NOR = {
+    "XX": "X",
+    "X0": "X",
+    "X1": "X",
+    "X-": "X",
+    "0X": "X",
     "00": "1",
     "01": "0",
-    "0X": "X",
-    "1?": "?",
+    "0-": "-",
+    "1X": "X",
     "10": "0",
     "11": "0",
-    "1X": "0",
-    "X?": "?",
-    "X0": "X",
-    "X1": "0",
-    "XX": "X",
+    "1-": "0",
+    "-X": "X",
+    "-0": "-",
+    "-1": "0",
+    "--": "-",
 }
 
 
 def test_lnor():
-    """Test seqlogic.lbool.lnor function."""
-    for xs, y in LNOR.items():
+    for xs, y in NOR.items():
         x0 = lbool._from_char[xs[0]]
         x1 = lbool._from_char[xs[1]]
         y = lbool._from_char[y]
-        assert lnor(x0, x1) == y
+        assert nor(x0, x1) == y
 
 
-LOR = {
-    "??": "?",
-    "?0": "?",
-    "?1": "?",
-    "?X": "?",
-    "0?": "?",
+OR = {
+    "XX": "X",
+    "X0": "X",
+    "X1": "X",
+    "X-": "X",
+    "0X": "X",
     "00": "0",
     "01": "1",
-    "0X": "X",
-    "1?": "?",
+    "0-": "-",
+    "1X": "X",
     "10": "1",
     "11": "1",
-    "1X": "1",
-    "X?": "?",
-    "X0": "X",
-    "X1": "1",
-    "XX": "X",
+    "1-": "1",
+    "-X": "X",
+    "-0": "-",
+    "-1": "1",
+    "--": "-",
 }
 
 
 def test_lor():
-    """Test seqlogic.lbool.lor function."""
-    for xs, y in LOR.items():
+    for xs, y in OR.items():
         x0 = lbool._from_char[xs[0]]
         x1 = lbool._from_char[xs[1]]
         y = lbool._from_char[y]
-        assert lor(x0, x1) == y
+        assert or_(x0, x1) == y
 
 
-LNAND = {
-    "??": "?",
-    "?0": "?",
-    "?1": "?",
-    "?X": "?",
-    "0?": "?",
+NAND = {
+    "XX": "X",
+    "X0": "X",
+    "X1": "X",
+    "X-": "X",
+    "0X": "X",
     "00": "1",
     "01": "1",
-    "0X": "1",
-    "1?": "?",
+    "0-": "1",
+    "1X": "X",
     "10": "1",
     "11": "0",
-    "1X": "X",
-    "X?": "?",
-    "X0": "1",
-    "X1": "X",
-    "XX": "X",
+    "1-": "-",
+    "-X": "X",
+    "-0": "1",
+    "-1": "-",
+    "--": "-",
 }
 
 
 def test_lnand():
-    """Test seqlogic.lbool.lnand function."""
-    for xs, y in LNAND.items():
+    for xs, y in NAND.items():
         x0 = lbool._from_char[xs[0]]
         x1 = lbool._from_char[xs[1]]
         y = lbool._from_char[y]
-        assert lnand(x0, x1) == y
+        assert nand(x0, x1) == y
 
 
-LAND = {
-    "??": "?",
-    "?0": "?",
-    "?1": "?",
-    "?X": "?",
-    "0?": "?",
+AND = {
+    "XX": "X",
+    "X0": "X",
+    "X1": "X",
+    "X-": "X",
+    "0X": "X",
     "00": "0",
     "01": "0",
-    "0X": "0",
-    "1?": "?",
+    "0-": "0",
+    "1X": "X",
     "10": "0",
     "11": "1",
-    "1X": "X",
-    "X?": "?",
-    "X0": "0",
-    "X1": "X",
-    "XX": "X",
+    "1-": "-",
+    "-X": "X",
+    "-0": "0",
+    "-1": "-",
+    "--": "-",
 }
 
 
 def test_land():
-    """Test seqlogic.lbool.land function."""
-    for xs, y in LAND.items():
+    for xs, y in AND.items():
         x0 = lbool._from_char[xs[0]]
         x1 = lbool._from_char[xs[1]]
         y = lbool._from_char[y]
-        assert land(x0, x1) == y
+        assert and_(x0, x1) == y
 
 
-LXNOR = {
-    "??": "?",
-    "?0": "?",
-    "?1": "?",
-    "?X": "?",
-    "0?": "?",
+XNOR = {
+    "XX": "X",
+    "X0": "X",
+    "X1": "X",
+    "X-": "X",
+    "0X": "X",
     "00": "1",
     "01": "0",
-    "0X": "X",
-    "1?": "?",
+    "0-": "-",
+    "1X": "X",
     "10": "0",
     "11": "1",
-    "1X": "X",
-    "X?": "?",
-    "X0": "X",
-    "X1": "X",
-    "XX": "X",
+    "1-": "-",
+    "-X": "X",
+    "-0": "-",
+    "-1": "-",
+    "--": "-",
 }
 
 
 def test_lxnor():
-    """Test seqlogic.lbool.lnand function."""
-    for xs, y in LXNOR.items():
+    for xs, y in XNOR.items():
         x0 = lbool._from_char[xs[0]]
         x1 = lbool._from_char[xs[1]]
         y = lbool._from_char[y]
-        assert lxnor(x0, x1) == y
+        assert xnor(x0, x1) == y
 
 
-LXOR = {
-    "??": "?",
-    "?0": "?",
-    "?1": "?",
-    "?X": "?",
-    "0?": "?",
+XOR = {
+    "XX": "X",
+    "X0": "X",
+    "X1": "X",
+    "X-": "X",
+    "0X": "X",
     "00": "0",
     "01": "1",
-    "0X": "X",
-    "1?": "?",
+    "0-": "-",
+    "1X": "X",
     "10": "1",
     "11": "0",
-    "1X": "X",
-    "X?": "?",
-    "X0": "X",
-    "X1": "X",
-    "XX": "X",
+    "1-": "-",
+    "-X": "X",
+    "-0": "-",
+    "-1": "-",
+    "--": "-",
 }
 
 
 def test_lxor():
-    """Test seqlogic.lbool.land function."""
-    for xs, y in LXOR.items():
+    for xs, y in XOR.items():
         x0 = lbool._from_char[xs[0]]
         x1 = lbool._from_char[xs[1]]
         y = lbool._from_char[y]
-        assert lxor(x0, x1) == y
+        assert xor(x0, x1) == y
 
 
-LIMPLIES = {
-    "??": "?",
-    "?0": "?",
-    "?1": "?",
-    "?X": "?",
-    "0?": "?",
+IMPLIES = {
+    "XX": "X",
+    "X0": "X",
+    "X1": "X",
+    "X-": "X",
+    "0X": "X",
     "00": "1",
     "01": "1",
-    "0X": "1",
-    "1?": "?",
+    "0-": "1",
+    "1X": "X",
     "10": "0",
     "11": "1",
-    "1X": "X",
-    "X?": "?",
-    "X0": "X",
-    "X1": "1",
-    "XX": "X",
+    "1-": "-",
+    "-X": "X",
+    "-0": "-",
+    "-1": "1",
+    "--": "-",
 }
 
 
 def test_limplies():
-    """Test seqlogic.lbool.limplies function."""
-    for xs, y in LIMPLIES.items():
+    for xs, y in IMPLIES.items():
         x0 = lbool._from_char[xs[0]]
         x1 = lbool._from_char[xs[1]]
         y = lbool._from_char[y]
-        assert limplies(x0, x1) == y
+        assert implies(x0, x1) == y
+
+
+def test_vec_cls_getitem():
+    vec_4 = Vec[4]
+    v = vec_4(42)  # pyright: ignore[reportCallIssue]
+    assert len(v) == 4 and v.data == 42
+    # Always return the same class instance
+    assert Vec[4] is vec_4
 
 
 def test_vec_repr():
-    """Test seqlogic.lbool.Vec.__repr__ method."""
-    assert repr(Vec(0, 0)) == "vec(0, 0b0)"
-    assert repr(Vec(4, 0b1110_0100)) == "vec(4, 0b11100100)"
+    assert repr(Vec[0](0)) == "Vec[0](0b0)"
+    assert repr(Vec[4](0b1110_0100)) == "Vec[4](0b11100100)"
 
 
 def test_vec_bool():
-    """Test seqlogic.lbool.Vec.__bool__ method."""
-    assert bool(Vec(0, 0)) is False
-    assert bool(Vec(1, 0b01)) is False
-    assert bool(Vec(1, 0b10)) is True
-    assert bool(Vec(4, 0b01_01_01_01)) is False
-    assert bool(Vec(4, 0b10_01_10_01)) is True
+    assert bool(Vec[0](0)) is False
+    assert bool(Vec[1](0b01)) is False
+    assert bool(Vec[1](0b10)) is True
+    assert bool(Vec[4](0b01_01_01_01)) is False
+    assert bool(Vec[4](0b10_01_10_01)) is True
     with pytest.raises(ValueError):
-        bool(Vec(4, 0b11_10_01_00))
+        bool(Vec[4](0b11_10_01_00))
 
 
 def test_vec_int():
-    """Test seqlogic.lbool.Vec.__int__ method."""
-    assert int(Vec(0, 0)) == 0
-    assert int(Vec(1, 0b01)) == 0
-    assert int(Vec(1, 0b10)) == -1
-    assert int(Vec(4, 0b01_01_01_01)) == 0
-    assert int(Vec(4, 0b10_01_10_01)) == -6
-    assert int(Vec(4, 0b01_10_01_10)) == 5
+    assert int(Vec[0](0)) == 0
+    assert int(Vec[1](0b01)) == 0
+    assert int(Vec[1](0b10)) == -1
+    assert int(Vec[4](0b01_01_01_01)) == 0
+    assert int(Vec[4](0b10_01_10_01)) == -6
+    assert int(Vec[4](0b01_10_01_10)) == 5
     with pytest.raises(ValueError):
-        int(Vec(4, 0b11_10_01_00))
+        int(Vec[4](0b11_10_01_00))
 
 
 def test_vec_eq():
-    """Test seqlogic.lbool.Vec.__eq__ method."""
-    assert Vec(0, 0) == Vec(0, 0)
-    assert Vec(4, 0b10_01_10_01) == Vec(4, 0b10_01_10_01)
-    assert Vec(4, 0b10_01_10_01) != Vec(4, 0b01_10_01_10)
-    assert Vec(4, 0b11_10_01_00) != "foo"
+    assert Vec[0](0) == Vec[0](0)
+    assert Vec[4](0b10_01_10_01) == Vec[4](0b10_01_10_01)
+    assert Vec[4](0b10_01_10_01) != Vec[4](0b01_10_01_10)
+    assert Vec[4](0b11_10_01_00) != "foo"
 
 
 def test_vec_hash():
-    """Test seqlogic.lbool.vec.__hash__ method."""
     s = set()
     s.add(lbool.uint2vec(0))
     s.add(lbool.uint2vec(1))
     s.add(lbool.uint2vec(2))
     s.add(lbool.uint2vec(3))
     s.add(lbool.uint2vec(1))
     s.add(lbool.uint2vec(2))
     assert len(s) == 4
 
 
 def test_vec_lnot():
-    """Test seqlogic.lbool.Vec.lnot method."""
-    x = Vec(4, 0b11_10_01_00)
-    assert x.lnot() == Vec(4, 0b11_01_10_00)
-    assert ~x == Vec(4, 0b11_01_10_00)
+    x = Vec[4](0b11_10_01_00)
+    assert x.not_() == Vec[4](0b11_01_10_00)
+    assert ~x == Vec[4](0b11_01_10_00)
 
 
 def test_vec_lnor():
-    """Test seqlogic.lbool.Vec.lnor method."""
-    x0 = Vec(16, 0b11111111_10101010_01010101_00000000)
-    x1 = Vec(16, 0b11100100_11100100_11100100_11100100)
-    assert x0.lnor(x1) == Vec(16, 0b11011100_01010100_11011000_00000000)
-    assert ~(x0 | x1) == Vec(16, 0b11011100_01010100_11011000_00000000)
+    x0 = Vec[16](0b11111111_10101010_01010101_00000000)
+    x1 = Vec[16](0b11100100_11100100_11100100_11100100)
+    assert x0.nor(x1) == Vec[16](0b11011100_01010100_11011000_00000000)
+    assert ~(x0 | x1) == Vec[16](0b11011100_01010100_11011000_00000000)
 
 
 def test_vec_lor():
-    """Test seqlogic.lbool.Vec.lor method."""
-    x0 = Vec(16, 0b11111111_10101010_01010101_00000000)
-    x1 = Vec(16, 0b11100100_11100100_11100100_11100100)
-    assert x0.lor(x1) == Vec(16, 0b11101100_10101000_11100100_00000000)
-    assert x0 | x1 == Vec(16, 0b11101100_10101000_11100100_00000000)
+    x0 = Vec[16](0b11111111_10101010_01010101_00000000)
+    x1 = Vec[16](0b11100100_11100100_11100100_11100100)
+    assert x0.or_(x1) == Vec[16](0b11101100_10101000_11100100_00000000)
+    assert x0 | x1 == Vec[16](0b11101100_10101000_11100100_00000000)
 
 
 def test_vec_lnand():
-    """Test seqlogic.lbool.Vec.lnand method."""
-    x0 = Vec(16, 0b11111111_10101010_01010101_00000000)
-    x1 = Vec(16, 0b11100100_11100100_11100100_11100100)
-    assert x0.lnand(x1) == Vec(16, 0b11111000_11011000_10101000_00000000)
-    assert ~(x0 & x1) == Vec(16, 0b11111000_11011000_10101000_00000000)
+    x0 = Vec[16](0b11111111_10101010_01010101_00000000)
+    x1 = Vec[16](0b11100100_11100100_11100100_11100100)
+    assert x0.nand(x1) == Vec[16](0b11111000_11011000_10101000_00000000)
+    assert ~(x0 & x1) == Vec[16](0b11111000_11011000_10101000_00000000)
 
 
 def test_vec_land():
-    """Test seqlogic.lbool.Vec.lnand method."""
-    x0 = Vec(16, 0b11111111_10101010_01010101_00000000)
-    x1 = Vec(16, 0b11100100_11100100_11100100_11100100)
-    assert x0.land(x1) == Vec(16, 0b11110100_11100100_01010100_00000000)
-    assert (x0 & x1) == Vec(16, 0b11110100_11100100_01010100_00000000)
+    x0 = Vec[16](0b11111111_10101010_01010101_00000000)
+    x1 = Vec[16](0b11100100_11100100_11100100_11100100)
+    assert x0.and_(x1) == Vec[16](0b11110100_11100100_01010100_00000000)
+    assert (x0 & x1) == Vec[16](0b11110100_11100100_01010100_00000000)
 
 
 def test_vec_lxnor():
-    """Test seqlogic.lbool.Vec.lxnor method."""
-    x0 = Vec(16, 0b11111111_10101010_01010101_00000000)
-    x1 = Vec(16, 0b11100100_11100100_11100100_11100100)
-    assert x0.lxnor(x1) == Vec(16, 0b11111100_11100100_11011000_00000000)
-    assert ~(x0 ^ x1) == Vec(16, 0b11111100_11100100_11011000_00000000)
+    x0 = Vec[16](0b11111111_10101010_01010101_00000000)
+    x1 = Vec[16](0b11100100_11100100_11100100_11100100)
+    assert x0.xnor(x1) == Vec[16](0b11111100_11100100_11011000_00000000)
+    assert ~(x0 ^ x1) == Vec[16](0b11111100_11100100_11011000_00000000)
 
 
 def test_vec_lxor():
-    """Test seqlogic.lbool.Vec.lxor method."""
-    x0 = Vec(16, 0b11111111_10101010_01010101_00000000)
-    x1 = Vec(16, 0b11100100_11100100_11100100_11100100)
-    assert x0.lxor(x1) == Vec(16, 0b11111100_11011000_11100100_00000000)
-    assert (x0 ^ x1) == Vec(16, 0b11111100_11011000_11100100_00000000)
+    x0 = Vec[16](0b11111111_10101010_01010101_00000000)
+    x1 = Vec[16](0b11100100_11100100_11100100_11100100)
+    assert x0.xor(x1) == Vec[16](0b11111100_11011000_11100100_00000000)
+    assert (x0 ^ x1) == Vec[16](0b11111100_11011000_11100100_00000000)
 
     # Vector length mismatch
     with pytest.raises(ValueError):
-        x0.lxor(Vec(8, 0b11111111_00000000))
+        x0.xor(Vec[8](0b11111111_00000000))
 
 
-ULOR = {
+UOR = {
     0b00_00: 0b00,
     0b01_00: 0b00,
     0b10_00: 0b00,
     0b11_00: 0b00,
     0b00_01: 0b00,
     0b01_01: 0b01,
     0b10_01: 0b10,
@@ -382,17 +376,16 @@
     0b01_11: 0b11,
     0b10_11: 0b10,
     0b11_11: 0b11,
 }
 
 
 def test_vec_ulor():
-    """Test seqlogic.lbool.Vec.ulor method."""
-    for k, v in ULOR.items():
-        assert Vec(2, k).ulor() == Vec(1, v)
+    for k, v in UOR.items():
+        assert Vec[2](k).uor() == Vec[1](v)
 
 
 UAND = {
     0b00_00: 0b00,
     0b01_00: 0b00,
     0b10_00: 0b00,
     0b11_00: 0b00,
@@ -408,17 +401,16 @@
     0b01_11: 0b01,
     0b10_11: 0b11,
     0b11_11: 0b11,
 }
 
 
 def test_vec_uand():
-    """Test seqlogic.lbool.Vec.uand method."""
     for k, v in UAND.items():
-        assert Vec(2, k).uland() == Vec(1, v)
+        assert Vec[2](k).uand() == Vec[1](v)
 
 
 UXNOR = {
     0b00_00: 0b00,
     0b01_00: 0b00,
     0b10_00: 0b00,
     0b11_00: 0b00,
@@ -434,17 +426,16 @@
     0b01_11: 0b11,
     0b10_11: 0b11,
     0b11_11: 0b11,
 }
 
 
 def test_vec_uxnor():
-    """Test seqlogic.lbool.Vec.uxnor method."""
     for k, v in UXNOR.items():
-        assert Vec(2, k).ulxnor() == Vec(1, v)
+        assert Vec[2](k).uxnor() == Vec[1](v)
 
 
 UXOR = {
     0b00_00: 0b00,
     0b01_00: 0b00,
     0b10_00: 0b00,
     0b11_00: 0b00,
@@ -460,15 +451,14 @@
     0b01_11: 0b11,
     0b10_11: 0b11,
     0b11_11: 0b11,
 }
 
 
 def test_vec_ult():
-    """Test seqlogic.lbool.Vec.ult method."""
     zero = uint2vec(0, 8)
     one = uint2vec(1, 8)
     two = uint2vec(2, 8)
     assert not zero.ult(zero)
     assert zero.ult(one)
     assert zero.ult(two)
     assert not one.ult(zero)
@@ -476,15 +466,14 @@
     assert one.ult(two)
     assert not two.ult(zero)
     assert not two.ult(one)
     assert not two.ult(two)
 
 
 def test_vec_slt():
-    """Test seqlogic.lbool.Vec.slt method."""
     n_one = int2vec(-1, 8)
     zero = int2vec(0, 8)
     one = int2vec(1, 8)
     assert not n_one.slt(n_one)
     assert n_one.slt(zero)
     assert n_one.slt(one)
     assert not zero.slt(n_one)
@@ -492,104 +481,212 @@
     assert zero.slt(one)
     assert not one.slt(n_one)
     assert not one.slt(zero)
     assert not one.slt(one)
 
 
 def test_vec_uxor():
-    """Test seqlogic.lbool.Vec.uxor method."""
     for k, v in UXOR.items():
-        assert Vec(2, k).ulxor() == Vec(1, v)
+        assert Vec[2](k).uxor() == Vec[1](v)
 
 
 def test_vec_zext():
-    """Test seqlogic.lbool.Vec.zext method."""
-    v = Vec(4, 0b10_01_10_01)
+    v = Vec[4](0b10_01_10_01)
     with pytest.raises(ValueError):
         v.zext(-1)
     assert v.zext(0) is v
-    assert v.zext(4) == Vec(8, 0b01_01_01_01_10_01_10_01)
+    assert v.zext(4) == Vec[8](0b01_01_01_01_10_01_10_01)
 
 
 def test_vec_sext():
-    """Test seqlogic.lbool.Vec.sext method."""
-    v1 = Vec(4, 0b10_01_10_01)
-    v2 = Vec(4, 0b01_10_01_10)
+    v1 = Vec[4](0b10_01_10_01)
+    v2 = Vec[4](0b01_10_01_10)
     with pytest.raises(ValueError):
         v1.sext(-1)
     assert v1.sext(0) is v1
-    assert v1.sext(4) == Vec(8, 0b10_10_10_10_10_01_10_01)
+    assert v1.sext(4) == Vec[8](0b10_10_10_10_10_01_10_01)
     assert v2.sext(0) is v2
-    assert v2.sext(4) == Vec(8, 0b01_01_01_01_01_10_01_10)
+    assert v2.sext(4) == Vec[8](0b01_01_01_01_01_10_01_10)
 
 
 def test_vec_lsh():
-    """Test seqlogic.lbool.Vec.lsh method."""
-    v = Vec(4, 0b10_10_10_10)
+    v = Vec[4](0b10_10_10_10)
     y, co = v.lsh(0)
     assert y is v and co == E
-    assert v.lsh(1) == (Vec(4, 0b10_10_10_01), Vec(1, 0b10))
-    assert v.lsh(2) == (Vec(4, 0b10_10_01_01), Vec(2, 0b10_10))
-    assert v << 2 == Vec(4, 0b10_10_01_01)
-    assert v.lsh(3) == (Vec(4, 0b10_01_01_01), Vec(3, 0b10_10_10))
-    assert v.lsh(4) == (Vec(4, 0b01_01_01_01), Vec(4, 0b10_10_10_10))
+    assert v.lsh(1) == (Vec[4](0b10_10_10_01), Vec[1](0b10))
+    assert v.lsh(2) == (Vec[4](0b10_10_01_01), Vec[2](0b10_10))
+    assert v << 2 == Vec[4](0b10_10_01_01)
+    assert v.lsh(3) == (Vec[4](0b10_01_01_01), Vec[3](0b10_10_10))
+    assert v.lsh(4) == (Vec[4](0b01_01_01_01), Vec[4](0b10_10_10_10))
 
     with pytest.raises(ValueError):
         v.lsh(-1)
     with pytest.raises(ValueError):
         v.lsh(5)
 
-    assert v.lsh(2, Vec(2, 0b01_10)) == (Vec(4, 0b10_10_01_10), Vec(2, 0b10_10))
+    assert v.lsh(2, Vec[2](0b01_10)) == (Vec[4](0b10_10_01_10), Vec[2](0b10_10))
     with pytest.raises(ValueError):
-        v.lsh(2, Vec(3, 0b01_01_01))
+        v.lsh(2, Vec[3](0b01_01_01))
 
 
 def test_vec_rsh():
-    """Test seqlogic.lbool.Vec.rsh method."""
-    v = Vec(4, 0b10_10_10_10)
+    v = Vec[4](0b10_10_10_10)
     y, co = v.rsh(0)
     assert y is v and co == E
-    assert v.rsh(1) == (Vec(4, 0b01_10_10_10), Vec(1, 0b10))
-    assert v.rsh(2) == (Vec(4, 0b01_01_10_10), Vec(2, 0b10_10))
-    assert v >> 2 == Vec(4, 0b01_01_10_10)
-    assert v.rsh(3) == (Vec(4, 0b01_01_01_10), Vec(3, 0b10_10_10))
-    assert v.rsh(4) == (Vec(4, 0b01_01_01_01), Vec(4, 0b10_10_10_10))
+    assert v.rsh(1) == (Vec[4](0b01_10_10_10), Vec[1](0b10))
+    assert v.rsh(2) == (Vec[4](0b01_01_10_10), Vec[2](0b10_10))
+    assert v >> 2 == Vec[4](0b01_01_10_10)
+    assert v.rsh(3) == (Vec[4](0b01_01_01_10), Vec[3](0b10_10_10))
+    assert v.rsh(4) == (Vec[4](0b01_01_01_01), Vec[4](0b10_10_10_10))
 
     with pytest.raises(ValueError):
         v.rsh(-1)
     with pytest.raises(ValueError):
         v.rsh(5)
 
-    assert v.rsh(2, Vec(2, 0b01_10)) == (Vec(4, 0b01_10_10_10), Vec(2, 0b10_10))
+    assert v.rsh(2, Vec[2](0b01_10)) == (Vec[4](0b01_10_10_10), Vec[2](0b10_10))
     with pytest.raises(ValueError):
-        v.rsh(2, Vec(3, 0b01_01_01))
+        v.rsh(2, Vec[3](0b01_01_01))
 
 
 def test_vec_arsh():
-    """Test seqlogic.lbool.Vec.arsh method."""
-    v = Vec(4, 0b10_10_10_10)
-    assert v.arsh(0) == (Vec(4, 0b10_10_10_10), E)
-    assert v.arsh(1) == (Vec(4, 0b10_10_10_10), Vec(1, 0b10))
-    assert v.arsh(2) == (Vec(4, 0b10_10_10_10), Vec(2, 0b10_10))
-    assert v.arsh(3) == (Vec(4, 0b10_10_10_10), Vec(3, 0b10_10_10))
-    assert v.arsh(4) == (Vec(4, 0b10_10_10_10), Vec(4, 0b10_10_10_10))
-
-    v = Vec(4, 0b01_10_10_10)
-    assert v.arsh(0) == (Vec(4, 0b01_10_10_10), E)
-    assert v.arsh(1) == (Vec(4, 0b01_01_10_10), Vec(1, 0b10))
-    assert v.arsh(2) == (Vec(4, 0b01_01_01_10), Vec(2, 0b10_10))
-    assert v.arsh(3) == (Vec(4, 0b01_01_01_01), Vec(3, 0b10_10_10))
-    assert v.arsh(4) == (Vec(4, 0b01_01_01_01), Vec(4, 0b01_10_10_10))
+    v = Vec[4](0b10_10_10_10)
+    assert v.arsh(0) == (Vec[4](0b10_10_10_10), E)
+    assert v.arsh(1) == (Vec[4](0b10_10_10_10), Vec[1](0b10))
+    assert v.arsh(2) == (Vec[4](0b10_10_10_10), Vec[2](0b10_10))
+    assert v.arsh(3) == (Vec[4](0b10_10_10_10), Vec[3](0b10_10_10))
+    assert v.arsh(4) == (Vec[4](0b10_10_10_10), Vec[4](0b10_10_10_10))
+
+    v = Vec[4](0b01_10_10_10)
+    assert v.arsh(0) == (Vec[4](0b01_10_10_10), E)
+    assert v.arsh(1) == (Vec[4](0b01_01_10_10), Vec[1](0b10))
+    assert v.arsh(2) == (Vec[4](0b01_01_01_10), Vec[2](0b10_10))
+    assert v.arsh(3) == (Vec[4](0b01_01_01_01), Vec[3](0b10_10_10))
+    assert v.arsh(4) == (Vec[4](0b01_01_01_01), Vec[4](0b01_10_10_10))
 
     with pytest.raises(ValueError):
         v.arsh(-1)
     with pytest.raises(ValueError):
         v.arsh(5)
 
 
+ADD_VALS = [
+    ("2b00", "2b00", F, "2b00", F, F),
+    ("2b00", "2b01", F, "2b01", F, F),
+    ("2b00", "2b10", F, "2b10", F, F),
+    ("2b00", "2b11", F, "2b11", F, F),
+    ("2b01", "2b00", F, "2b01", F, F),
+    ("2b01", "2b01", F, "2b10", F, T),  # overflow
+    ("2b01", "2b10", F, "2b11", F, F),
+    ("2b01", "2b11", F, "2b00", T, F),
+    ("2b10", "2b00", F, "2b10", F, F),
+    ("2b10", "2b01", F, "2b11", F, F),
+    ("2b10", "2b10", F, "2b00", T, T),  # overflow
+    ("2b10", "2b11", F, "2b01", T, T),  # overflow
+    ("2b11", "2b00", F, "2b11", F, F),
+    ("2b11", "2b01", F, "2b00", T, F),
+    ("2b11", "2b10", F, "2b01", T, T),  # overflow
+    ("2b11", "2b11", F, "2b10", T, F),
+    ("2b00", "2b00", T, "2b01", F, F),
+    ("2b00", "2b01", T, "2b10", F, T),  # overflow
+    ("2b00", "2b10", T, "2b11", F, F),
+    ("2b00", "2b11", T, "2b00", T, F),
+    ("2b01", "2b00", T, "2b10", F, T),  # overflow
+    ("2b01", "2b01", T, "2b11", F, T),  # overflow
+    ("2b01", "2b10", T, "2b00", T, F),
+    ("2b01", "2b11", T, "2b01", T, F),
+    ("2b10", "2b00", T, "2b11", F, F),
+    ("2b10", "2b01", T, "2b00", T, F),
+    ("2b10", "2b10", T, "2b01", T, T),  # overflow
+    ("2b10", "2b11", T, "2b10", T, F),
+    ("2b11", "2b00", T, "2b00", T, F),
+    ("2b11", "2b01", T, "2b01", T, F),
+    ("2b11", "2b10", T, "2b10", T, F),
+    ("2b11", "2b11", T, "2b11", T, F),
+]
+
+
+def test_vec_add():
+    """Test bits add method."""
+    for a, b, ci, s, co, v in ADD_VALS:
+        a, b, s = vec(a), vec(b), vec(s)
+        assert a.add(b, ci) == (s, co, v)
+
+
+def test_vec_addsubnegops():
+    """Test bits add/substract operators."""
+    assert vec("2b00") + vec("2b00") == vec("2b00")
+    assert vec("2b00") + vec("2b01") == vec("2b01")
+    assert vec("2b01") + vec("2b00") == vec("2b01")
+    assert vec("2b00") + vec("2b10") == vec("2b10")
+    assert vec("2b01") + vec("2b01") == vec("2b10")
+    assert vec("2b10") + vec("2b00") == vec("2b10")
+    assert vec("2b00") + vec("2b11") == vec("2b11")
+    assert vec("2b01") + vec("2b10") == vec("2b11")
+    assert vec("2b10") + vec("2b01") == vec("2b11")
+    assert vec("2b11") + vec("2b00") == vec("2b11")
+    assert vec("2b01") + vec("2b11") == vec("2b00")
+    assert vec("2b10") + vec("2b10") == vec("2b00")
+    assert vec("2b11") + vec("2b01") == vec("2b00")
+    assert vec("2b10") + vec("2b11") == vec("2b01")
+    assert vec("2b11") + vec("2b10") == vec("2b01")
+    assert vec("2b11") + vec("2b11") == vec("2b10")
+
+    assert vec("2b00") - vec("2b11") == vec("2b01")
+    assert vec("2b00") - vec("2b10") == vec("2b10")
+    assert vec("2b01") - vec("2b11") == vec("2b10")
+    assert vec("2b00") - vec("2b01") == vec("2b11")
+    assert vec("2b01") - vec("2b10") == vec("2b11")
+    assert vec("2b10") - vec("2b11") == vec("2b11")
+    assert vec("2b00") - vec("2b00") == vec("2b00")
+    assert vec("2b01") - vec("2b01") == vec("2b00")
+    assert vec("2b10") - vec("2b10") == vec("2b00")
+    assert vec("2b11") - vec("2b11") == vec("2b00")
+    assert vec("2b01") - vec("2b00") == vec("2b01")
+    assert vec("2b10") - vec("2b01") == vec("2b01")
+    assert vec("2b11") - vec("2b10") == vec("2b01")
+    assert vec("2b10") - vec("2b00") == vec("2b10")
+    assert vec("2b11") - vec("2b01") == vec("2b10")
+    assert vec("2b11") - vec("2b00") == vec("2b11")
+
+    assert -vec("3b000") == vec("3b000")
+    assert -vec("3b001") == vec("3b111")
+    assert -vec("3b111") == vec("3b001")
+    assert -vec("3b010") == vec("3b110")
+    assert -vec("3b110") == vec("3b010")
+    assert -vec("3b011") == vec("3b101")
+    assert -vec("3b101") == vec("3b011")
+    assert -vec("3b100") == vec("3b100")
+
+
+def test_count():
+    v = vec("8b-10X_-10X")
+    assert v.count_xes() == 2
+    assert v.count_zeros() == 2
+    assert v.count_ones() == 2
+    assert v.count_dcs() == 2
+
+    assert vec("4b0000").count_ones() == 0
+    assert vec("4b0001").count_ones() == 1
+    assert vec("4b0011").count_ones() == 2
+    assert vec("4b0111").count_ones() == 3
+    assert vec("4b1111").count_ones() == 4
+
+    assert not vec("4b0000").onehot()
+    assert vec("4b1000").onehot()
+    assert vec("4b0001").onehot()
+    assert not vec("4b1001").onehot()
+    assert not vec("4b1101").onehot()
+
+    assert vec("4b0000").onehot0()
+    assert vec("4b1000").onehot0()
+    assert not vec("4b1010").onehot0()
+    assert not vec("4b1011").onehot0()
+
+
 UINT2VEC_VALS = {
     0: "",
     1: "1b1",
     2: "2b10",
     3: "2b11",
     4: "3b100",
     5: "3b101",
@@ -615,15 +712,14 @@
     (4, 3): "3b100",
     (4, 4): "4b0100",
     (4, 5): "5b0_0100",
 }
 
 
 def test_uint2vec():
-    """Test seqlogic.lbool.uint2vec function."""
     # Negative inputs are invalid
     with pytest.raises(ValueError):
         uint2vec(-1)
 
     for i, s in UINT2VEC_VALS.items():
         v = uint2vec(i)
         assert str(v) == s
@@ -697,15 +793,14 @@
     (4, 4): "4b0100",
     (4, 5): "5b0_0100",
     (4, 6): "6b00_0100",
 }
 
 
 def test_int2vec():
-    """Test seqlogic.lbool.int2vec function."""
     for i, s in INT2VEC_VALS.items():
         v = int2vec(i)
         assert str(v) == s
         assert v.to_int() == i
 
     for (i, n), s in INT2VEC_N_VALS.items():
         v = int2vec(i, n)
@@ -731,15 +826,14 @@
     with pytest.raises(ValueError):
         int2vec(3, 2)
     with pytest.raises(ValueError):
         int2vec(4, 3)
 
 
 def test_lit2vec():
-    """Test parsing of vector string literals."""
     # literal doesn't match size
     with pytest.raises(ValueError):
         vec("4b1010_1010")
     with pytest.raises(ValueError):
         vec("8b1010")
     with pytest.raises(ValueError):
         vec("16hdead_beef")
@@ -747,50 +841,72 @@
         vec("8hdead")
 
     # Invalid input
     with pytest.raises(ValueError):
         vec("invalid")
 
     # Valid input
-    v = vec("4bX1_0?")
+    v = vec("4b-1_0X")
     assert v.data == 0b11_10_01_00
     v = vec("64hFeDc_Ba98_7654_3210")
     assert v.data == 0xAAA9_A6A5_9A99_9695_6A69_6665_5A59_5655
     v = vec("64hfEdC_bA98_7654_3210")
     assert v.data == 0xAAA9_A6A5_9A99_9695_6A69_6665_5A59_5655
 
 
 def test_vec_basic():
-    """Test seqlogic.lbool.Vec basic functionality."""
     # n is non-negative
     with pytest.raises(ValueError):
-        Vec(-1, 42)
+        Vec[-1](42)
 
     # data in [0, 2**nbits)
     with pytest.raises(ValueError):
-        Vec(4, -1)
+        Vec[4](-1)
     with pytest.raises(ValueError):
-        Vec(4, 2 ** (2 * 4))
+        Vec[4](2 ** (2 * 4))
 
-    v = Vec(4, 0b11_10_01_00)
+    v = Vec[4](0b11_10_01_00)
     assert len(v) == 4
 
-    assert v[3] == Vec(1, 0b11)
-    assert v[2] == Vec(1, 0b10)
-    assert v[1] == Vec(1, 0b01)
-    assert v[0] == Vec(1, 0b00)
-
-    assert v[0:1] == Vec(1, 0b00)
-    assert v[0:2] == Vec(2, 0b01_00)
-    assert v[0:3] == Vec(3, 0b10_01_00)
-    assert v[0:4] == Vec(4, 0b11_10_01_00)
-    assert v[1:2] == Vec(1, 0b01)
-    assert v[1:3] == Vec(2, 0b10_01)
-    assert v[1:4] == Vec(3, 0b11_10_01)
-    assert v[2:3] == Vec(1, 0b10)
-    assert v[2:4] == Vec(2, 0b11_10)
-    assert v[3:4] == Vec(1, 0b11)
+    assert v[3] == Vec[1](0b11)
+    assert v[2] == Vec[1](0b10)
+    assert v[1] == Vec[1](0b01)
+    assert v[0] == Vec[1](0b00)
+
+    assert v[0:1] == Vec[1](0b00)
+    assert v[0:2] == Vec[2](0b01_00)
+    assert v[0:3] == Vec[3](0b10_01_00)
+    assert v[0:4] == Vec[4](0b11_10_01_00)
+    assert v[1:2] == Vec[1](0b01)
+    assert v[1:3] == Vec[2](0b10_01)
+    assert v[1:4] == Vec[3](0b11_10_01)
+    assert v[2:3] == Vec[1](0b10)
+    assert v[2:4] == Vec[2](0b11_10)
+    assert v[3:4] == Vec[1](0b11)
 
     with pytest.raises(TypeError):
         v["invalid"]  # pyright: ignore[reportArgumentType]
 
-    assert list(v) == [Vec(1, 0b00), Vec(1, 0b01), Vec(1, 0b10), Vec(1, 0b11)]
+    assert list(v) == [Vec[1](0b00), Vec[1](0b01), Vec[1](0b10), Vec[1](0b11)]
+
+
+def test_cat():
+    v = vec("4b-10X")
+    assert cat() == vec()
+    assert cat(v) == v
+    assert cat(vec("2b0X"), vec("2b-1")) == vec("4b-10X")
+    assert cat(0, 1) == vec("2b10")
+
+    with pytest.raises(TypeError):
+        _ = cat(v, 42)
+
+
+def test_rep():
+    assert rep(vec("4b-10X"), 2) == vec("8b-10X_-10X")
+
+
+def test_misc():
+    assert str(xes(4)) == "4bXXXX"
+    assert str(dcs(4)) == "4b----"
+
+    with pytest.raises(ValueError):
+        _ = xes(-4)
```

### Comparing `seqlogic-0.0.7/tests/test_lfsr.py` & `seqlogic-0.0.8/tests/test_lfsr.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Example LFSR implementation."""
 
 from collections import defaultdict
 
 from seqlogic import Bit, Bits, Module, get_loop
-from seqlogic.bits import F, T, X, bits, cat
+from seqlogic.lbool import cat, ones, vec, xes, zeros
 from seqlogic.sim import Region
 
 from .common import p_clk, p_dff, p_rst
 
 loop = get_loop()
 
 
 class Top(Module):
     """Top level module."""
 
     def __init__(self):
-        """TODO(cjdrake): Write docstring."""
         super().__init__(name="top", parent=None)
         # Control
         self.reset_n = Bit(name="reset_n", parent=self)
         self.clock = Bit(name="clock", parent=self)
         # State
         self.q = Bits(name="q", parent=self, shape=(3,))
 
@@ -33,116 +32,116 @@
     top.dump_waves(waves, r".*")
 
     assert top.q.name == "q"
     assert top.q.qualname == "/top/q"
 
     def d():
         v = top.q.value
-        return cat([v[0] ^ v[2], v[:2]])
+        return cat(v[0] ^ v[2], v[:2])
 
-    reset_value = bits("3b100")
+    reset_value = vec("3b100")
 
     # Schedule LFSR
-    loop.add_proc(p_dff, Region(1), top.q, d, top.reset_n, reset_value, top.clock)
+    loop.add_proc(Region(1), p_dff, top.q, d, top.reset_n, reset_value, top.clock)
 
     # Schedule reset and clock
     # Note: Avoiding simultaneous reset/clock negedge/posedge on purpose
-    loop.add_proc(p_rst, Region(2), top.reset_n, init=T, phase1=6, phase2=10)
-    loop.add_proc(p_clk, Region(2), top.clock, init=F, shift=5, phase1=5, phase2=5)
+    loop.add_proc(Region(2), p_rst, top.reset_n, init=ones(1), phase1=6, phase2=10)
+    loop.add_proc(Region(2), p_clk, top.clock, init=zeros(1), shift=5, phase1=5, phase2=5)
 
     loop.run(until=100)
 
     exp = {
         # Initialize everything to X'es
         -1: {
-            top.reset_n: X,
-            top.clock: X,
-            top.q: bits("3bXXX"),
+            top.reset_n: xes(1),
+            top.clock: xes(1),
+            top.q: xes(3),
         },
         0: {
-            top.reset_n: T,
-            top.clock: F,
+            top.reset_n: ones(1),
+            top.clock: zeros(1),
         },
         # clock.posedge; reset_n = 1
         # q = xxx
         5: {
-            top.clock: T,
+            top.clock: ones(1),
         },
         # reset_n.negedge
         # q = reset_value
         6: {
-            top.reset_n: F,
-            top.q: bits("3b100"),
+            top.reset_n: zeros(1),
+            top.q: vec("3b100"),
         },
         10: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         # clock.posedge; reset_n = 0
         15: {
-            top.clock: T,
+            top.clock: ones(1),
         },
         # reset_n.posedge
         16: {
-            top.reset_n: T,
+            top.reset_n: ones(1),
         },
         20: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         # clock.posedge; reset_n = 1
         # q = 001
         25: {
-            top.clock: T,
-            top.q: bits("3b001"),
+            top.clock: ones(1),
+            top.q: vec("3b001"),
         },
         30: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         35: {
-            top.clock: T,
-            top.q: bits("3b011"),
+            top.clock: ones(1),
+            top.q: vec("3b011"),
         },
         40: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         45: {
-            top.clock: T,
-            top.q: bits("3b111"),
+            top.clock: ones(1),
+            top.q: vec("3b111"),
         },
         50: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         55: {
-            top.clock: T,
-            top.q: bits("3b110"),
+            top.clock: ones(1),
+            top.q: vec("3b110"),
         },
         60: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         65: {
-            top.clock: T,
-            top.q: bits("3b101"),
+            top.clock: ones(1),
+            top.q: vec("3b101"),
         },
         70: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         75: {
-            top.clock: T,
-            top.q: bits("3b010"),
+            top.clock: ones(1),
+            top.q: vec("3b010"),
         },
         80: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         # Repeat cycle
         85: {
-            top.clock: T,
-            top.q: bits("3b100"),
+            top.clock: ones(1),
+            top.q: vec("3b100"),
         },
         90: {
-            top.clock: F,
+            top.clock: zeros(1),
         },
         95: {
-            top.clock: T,
-            top.q: bits("3b001"),
+            top.clock: ones(1),
+            top.q: vec("3b001"),
         },
     }
 
     assert waves == exp
```

### Comparing `seqlogic-0.0.7/tests/test_riscv.py` & `seqlogic-0.0.8/tests/test_riscv.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,48 +5,46 @@
 
 Work In Progress
 The objective is to figure out seqlogic simulation style/semantics.
 We are not presently interested in the details of RISC-V.
 It merely serves as a non-trivial example design.
 """
 
+# pylint: disable = protected-access
+# pyright: reportAttributeAccessIssue=false
+
 from collections import defaultdict
 
 from seqlogic import get_loop, simify
-from seqlogic.bits import F, T, X, bits, uint2bits, xes, zeros
+from seqlogic.lbool import ones, uint2vec, vec, xes, zeros
 
-from .riscv.core.common.constants import AluOp, CtlAluA, CtlAluB, CtlPc
+from .riscv.core import AluOp, CtlAluA, CtlAluB, CtlPc
 from .riscv.core.singlecycle.top import Top
 
-# pyright: reportAttributeAccessIssue=false
-
-
 loop = get_loop()
 
 
-X32 = xes((32,))
-Z32 = zeros((32,))
+X32 = xes(32)
+Z32 = zeros(32)
 
-DEBUG_REG = bits("32hFFFF_FFF0")
+DEBUG_REG = vec("32hFFFF_FFF0")
 
 PASS, FAIL, TIMEOUT = 0, 1, 2
 
 
 def get_mem(name: str) -> list[int]:
-    """TODO(cjdrake): Write docstring."""
     text = []
     with open(name, encoding="utf-8") as f:
         for line in f:
             for part in line.split()[1:]:
                 text.append(int(part, base=16))
     return text
 
 
 def test_singlecycle_dump():
-    """TODO(cjdrake): Write docstring."""
     loop.reset()
     waves = defaultdict(dict)
 
     # Create module hierarchy
     top = Top(name="top")
 
     top.dump_waves(waves, r"/top/pc")
@@ -68,851 +66,720 @@
     top.dump_waves(waves, r"/top/core/datapath.data_mem_wr_data")
 
     simify(top)
 
     # Initialize instruction memory
     text = get_mem("tests/riscv/tests/add.text")
     for i, d in enumerate(text):
-        top.text_memory_bus.text_memory.mem.set_value(i, uint2bits(d, 32))
+        top.text_memory_bus.text_memory._mem.set_next(i, uint2vec(d, 32))
 
     loop.run(until=50)
 
     exp = {
         # Initialize everything to X'es
         -1: {
             # Top
-            top.pc: X32,
-            top.inst: X32,
+            top._pc: X32,
+            top._inst: X32,
             top.bus_addr: X32,
-            top.bus_wr_en: X,
+            top.bus_wr_en: xes(1),
             top.bus_wr_data: X32,
-            top.bus_rd_en: X,
+            top.bus_rd_en: xes(1),
             # Decode
             top.core.datapath.inst: X32,
-            top.core.datapath.inst_funct7: xes((7,)),
-            top.core.datapath.inst_funct3: xes((3,)),
-            top.core.datapath.inst_opcode: xes((7,)),
             top.core.datapath.immediate: X32,
             # Control
             top.core.datapath.alu_op_a_sel: CtlAluA.X,
             top.core.datapath.alu_op_b_sel: CtlAluB.X,
-            top.core.datapath.reg_writeback_sel: xes((3,)),
+            top.core.datapath.reg_writeback_sel: xes(3),
             # ALU
             top.core.datapath.alu_result: X32,
-            top.core.datapath.alu_result_equal_zero: xes((1,)),
+            top.core.datapath.alu_result_equal_zero: xes(1),
             top.core.datapath.alu_function: AluOp.X,
             top.core.datapath.alu_op_a: X32,
             top.core.datapath.alu_op_b: X32,
             # PC
             top.core.datapath.pc_next: X32,
             top.core.datapath.next_pc_sel: CtlPc.X,
             top.core.datapath.pc_plus_4: X32,
             top.core.datapath.pc_plus_immediate: X32,
-            top.core.datapath.pc_wr_en: X,
+            top.core.datapath.pc_wr_en: xes(1),
             top.core.datapath.pc: X32,
             # Regfile
-            top.core.datapath.regfile_wr_en: X,
-            top.core.datapath.inst_rd: xes((5,)),
+            top.core.datapath.regfile_wr_en: xes(1),
             top.core.datapath.wr_data: X32,
-            top.core.datapath.inst_rs1: xes((5,)),
             top.core.datapath.rs1_data: X32,
-            top.core.datapath.inst_rs2: xes((5,)),
             top.core.datapath.rs2_data: X32,
             # Data Mem
             top.core.datapath.data_mem_addr: X32,
             top.core.datapath.data_mem_wr_data: X32,
         },
         # @(posedge reset)
         5: {
-            top.pc: bits("32h0040_0000"),
-            top.inst: bits("32h0000_0093"),
+            top._pc: vec("32h0040_0000"),
+            top._inst: vec("32h0000_0093"),
             top.bus_addr: Z32,
-            top.bus_wr_en: F,
+            top.bus_wr_en: zeros(1),
             top.bus_wr_data: Z32,
-            top.bus_rd_en: F,
+            top.bus_rd_en: zeros(1),
             # Decode
-            top.core.datapath.inst: bits("32h0000_0093"),
-            top.core.datapath.inst_funct7: bits("7b000_0000"),
-            top.core.datapath.inst_funct3: bits("3b000"),
-            top.core.datapath.inst_opcode: bits("7b001_0011"),
+            top.core.datapath.inst: vec("32h0000_0093"),
             top.core.datapath.immediate: Z32,
             # Control
             top.core.datapath.alu_op_a_sel: CtlAluA.RS1,
             top.core.datapath.alu_op_b_sel: CtlAluB.IMM,
-            top.core.datapath.reg_writeback_sel: bits("3b000"),
+            top.core.datapath.reg_writeback_sel: vec("3b000"),
             # ALU
             top.core.datapath.alu_result: Z32,
-            top.core.datapath.alu_result_equal_zero: T,
+            top.core.datapath.alu_result_equal_zero: ones(1),
             top.core.datapath.alu_function: AluOp.ADD,
             top.core.datapath.alu_op_a: Z32,
             top.core.datapath.alu_op_b: Z32,
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0004"),
+            top.core.datapath.pc_next: vec("32h0040_0004"),
             top.core.datapath.next_pc_sel: CtlPc.PC4,
-            top.core.datapath.pc_plus_4: bits("32h0040_0004"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0000"),
-            top.core.datapath.pc_wr_en: T,
-            top.core.datapath.pc: bits("32h0040_0000"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0004"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0000"),
+            top.core.datapath.pc_wr_en: ones(1),
+            top.core.datapath.pc: vec("32h0040_0000"),
             # Regfile
-            top.core.datapath.regfile_wr_en: T,
-            top.core.datapath.inst_rd: bits("5b0_0001"),
+            top.core.datapath.regfile_wr_en: ones(1),
             top.core.datapath.wr_data: Z32,
-            top.core.datapath.inst_rs1: bits("5b0_0000"),
             top.core.datapath.rs1_data: Z32,
-            top.core.datapath.inst_rs2: bits("5b0_0000"),
             top.core.datapath.rs2_data: Z32,
             # Data Mem
             top.core.datapath.data_mem_addr: Z32,
             top.core.datapath.data_mem_wr_data: Z32,
         },
         # @(posedge clock)
         11: {
-            top.pc: bits("32h0040_0004"),
-            top.inst: bits("32h0000_0113"),
+            top._pc: vec("32h0040_0004"),
+            top._inst: vec("32h0000_0113"),
             # Decode
-            top.core.datapath.inst: bits("32h0000_0113"),
+            top.core.datapath.inst: vec("32h0000_0113"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0008"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0008"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0004"),
-            top.core.datapath.pc: bits("32h0040_0004"),
+            top.core.datapath.pc_next: vec("32h0040_0008"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0008"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0004"),
+            top.core.datapath.pc: vec("32h0040_0004"),
             # Regfile
-            top.core.datapath.inst_rd: bits("5b0_0010"),
         },
         # @(posedge clock)
         13: {
-            top.pc: bits("32h0040_0008"),
-            top.inst: bits("32h0020_81B3"),
+            top._pc: vec("32h0040_0008"),
+            top._inst: vec("32h0020_81B3"),
             # Decode
-            top.core.datapath.inst: bits("32h0020_81B3"),
-            top.core.datapath.inst_opcode: bits("7b011_0011"),
+            top.core.datapath.inst: vec("32h0020_81B3"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.RS2,
             # PC
-            top.core.datapath.pc_next: bits("32h0040_000C"),
-            top.core.datapath.pc_plus_4: bits("32h0040_000C"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0008"),
-            top.core.datapath.pc: bits("32h0040_0008"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b0_0011"),
-            top.core.datapath.inst_rs1: bits("5b0_0001"),
-            top.core.datapath.inst_rs2: bits("5b0_0010"),
+            top.core.datapath.pc_next: vec("32h0040_000C"),
+            top.core.datapath.pc_plus_4: vec("32h0040_000C"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0008"),
+            top.core.datapath.pc: vec("32h0040_0008"),
         },
         # @(posedge clock)
         15: {
-            top.pc: bits("32h0040_000C"),
-            top.inst: bits("32h0000_0E93"),
+            top._pc: vec("32h0040_000C"),
+            top._inst: vec("32h0000_0E93"),
             # Decode
-            top.core.datapath.inst: bits("32h0000_0E93"),
-            top.core.datapath.inst_opcode: bits("7b001_0011"),
+            top.core.datapath.inst: vec("32h0000_0E93"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.IMM,
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0010"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0010"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_000C"),
-            top.core.datapath.pc: bits("32h0040_000C"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b1_1101"),
-            top.core.datapath.inst_rs1: bits("5b0_0000"),
-            top.core.datapath.inst_rs2: bits("5b0_0000"),
+            top.core.datapath.pc_next: vec("32h0040_0010"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0010"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_000C"),
+            top.core.datapath.pc: vec("32h0040_000C"),
         },
         # @(posedge clock)
         17: {
-            top.pc: bits("32h0040_0010"),
-            top.inst: bits("32h0020_0E13"),
-            top.bus_addr: bits("32h0000_0002"),
-            # Decode
-            top.core.datapath.inst: bits("32h0020_0E13"),
-            top.core.datapath.immediate: bits("32h0000_0002"),
-            # ALU
-            top.core.datapath.alu_result: bits("32h0000_0002"),
-            top.core.datapath.alu_result_equal_zero: F,
-            top.core.datapath.alu_op_b: bits("32h0000_0002"),
-            # PC
-            top.core.datapath.pc_next: bits("32h0040_0014"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0014"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0012"),
-            top.core.datapath.pc: bits("32h0040_0010"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b1_1100"),
-            top.core.datapath.wr_data: bits("32h0000_0002"),
-            top.core.datapath.inst_rs2: bits("5b0_0010"),
+            top._pc: vec("32h0040_0010"),
+            top._inst: vec("32h0020_0E13"),
+            top.bus_addr: vec("32h0000_0002"),
+            # Decode
+            top.core.datapath.inst: vec("32h0020_0E13"),
+            top.core.datapath.immediate: vec("32h0000_0002"),
+            # ALU
+            top.core.datapath.alu_result: vec("32h0000_0002"),
+            top.core.datapath.alu_result_equal_zero: zeros(1),
+            top.core.datapath.alu_op_b: vec("32h0000_0002"),
+            # PC
+            top.core.datapath.pc_next: vec("32h0040_0014"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0014"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0012"),
+            top.core.datapath.pc: vec("32h0040_0010"),
+            # Regfile
+            top.core.datapath.wr_data: vec("32h0000_0002"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0002"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0002"),
         },
         # @(posedge clock)
         19: {
-            top.pc: bits("32h0040_0014"),
-            top.inst: bits("32h4DD1_9663"),
-            top.bus_addr: bits("32h0000_0001"),
-            # Decode
-            top.core.datapath.inst: bits("32h4DD1_9663"),
-            top.core.datapath.inst_funct7: bits("7b010_0110"),
-            top.core.datapath.inst_funct3: bits("3b001"),
-            top.core.datapath.inst_opcode: bits("7b110_0011"),
-            top.core.datapath.immediate: bits("32h0000_04CC"),
+            top._pc: vec("32h0040_0014"),
+            top._inst: vec("32h4DD1_9663"),
+            top.bus_addr: vec("32h0000_0001"),
+            # Decode
+            top.core.datapath.inst: vec("32h4DD1_9663"),
+            top.core.datapath.immediate: vec("32h0000_04CC"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.RS2,
             # ALU
-            top.core.datapath.alu_result: bits("32h0000_0001"),
+            top.core.datapath.alu_result: vec("32h0000_0001"),
             top.core.datapath.alu_function: AluOp.SEQ,
             top.core.datapath.alu_op_b: Z32,
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0018"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0018"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_04E0"),
-            top.core.datapath.pc: bits("32h0040_0014"),
-            # Regfile
-            top.core.datapath.regfile_wr_en: F,
-            top.core.datapath.inst_rd: bits("5b0_1100"),
-            top.core.datapath.wr_data: bits("32h0000_0001"),
-            top.core.datapath.inst_rs1: bits("5b0_0011"),
-            top.core.datapath.inst_rs2: bits("5b1_1101"),
+            top.core.datapath.pc_next: vec("32h0040_0018"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0018"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_04E0"),
+            top.core.datapath.pc: vec("32h0040_0014"),
+            # Regfile
+            top.core.datapath.regfile_wr_en: zeros(1),
+            top.core.datapath.wr_data: vec("32h0000_0001"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0001"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0001"),
         },
         # @(posedge clock)
         21: {
-            top.pc: bits("32h0040_0018"),
-            top.inst: bits("32h0010_0093"),
+            top._pc: vec("32h0040_0018"),
+            top._inst: vec("32h0010_0093"),
             # Decode
-            top.core.datapath.inst: bits("32h0010_0093"),
-            top.core.datapath.inst_funct7: bits("7b000_0000"),
-            top.core.datapath.inst_funct3: bits("3b000"),
-            top.core.datapath.inst_opcode: bits("7b001_0011"),
-            top.core.datapath.immediate: bits("32h0000_0001"),
+            top.core.datapath.inst: vec("32h0010_0093"),
+            top.core.datapath.immediate: vec("32h0000_0001"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.IMM,
             # ALU
             top.core.datapath.alu_function: AluOp.ADD,
-            top.core.datapath.alu_op_b: bits("32h0000_0001"),
+            top.core.datapath.alu_op_b: vec("32h0000_0001"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_001C"),
-            top.core.datapath.pc_plus_4: bits("32h0040_001C"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0019"),
-            top.core.datapath.pc: bits("32h0040_0018"),
-            # Regfile
-            top.core.datapath.regfile_wr_en: T,
-            top.core.datapath.inst_rd: bits("5b0_0001"),
-            top.core.datapath.inst_rs1: bits("5b0_0000"),
-            top.core.datapath.inst_rs2: bits("5b0_0001"),
+            top.core.datapath.pc_next: vec("32h0040_001C"),
+            top.core.datapath.pc_plus_4: vec("32h0040_001C"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0019"),
+            top.core.datapath.pc: vec("32h0040_0018"),
+            # Regfile
+            top.core.datapath.regfile_wr_en: ones(1),
         },
         # @(posedge clock)
         23: {
-            top.pc: bits("32h0040_001C"),
-            top.inst: bits("32h0010_0113"),
-            top.bus_wr_data: bits("32h0000_0100"),
+            top._pc: vec("32h0040_001C"),
+            top._inst: vec("32h0010_0113"),
+            top.bus_wr_data: vec("32h0000_0100"),
             # Decode
-            top.core.datapath.inst: bits("32h0010_0113"),
+            top.core.datapath.inst: vec("32h0010_0113"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0020"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0020"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_001D"),
-            top.core.datapath.pc: bits("32h0040_001C"),
+            top.core.datapath.pc_next: vec("32h0040_0020"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0020"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_001D"),
+            top.core.datapath.pc: vec("32h0040_001C"),
             # Regfile
-            top.core.datapath.inst_rd: bits("5b0_0010"),
-            top.core.datapath.rs2_data: bits("32h0000_0001"),
+            top.core.datapath.rs2_data: vec("32h0000_0001"),
             # Data Mem
-            top.core.datapath.data_mem_wr_data: bits("32h0000_0001"),
+            top.core.datapath.data_mem_wr_data: vec("32h0000_0001"),
         },
         # @(posedge clock)
         25: {
-            top.pc: bits("32h0040_0020"),
-            top.inst: bits("32h0020_81B3"),
-            top.bus_addr: bits("32h0000_0002"),
-            top.bus_wr_data: bits("32h0001_0000"),
+            top._pc: vec("32h0040_0020"),
+            top._inst: vec("32h0020_81B3"),
+            top.bus_addr: vec("32h0000_0002"),
+            top.bus_wr_data: vec("32h0001_0000"),
             # Decode
-            top.core.datapath.inst: bits("32h0020_81B3"),
-            top.core.datapath.inst_opcode: bits("7b011_0011"),
+            top.core.datapath.inst: vec("32h0020_81B3"),
             top.core.datapath.immediate: Z32,
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.RS2,
             # ALU
-            top.core.datapath.alu_result: bits("32h0000_0002"),
-            top.core.datapath.alu_op_a: bits("32h0000_0001"),
+            top.core.datapath.alu_result: vec("32h0000_0002"),
+            top.core.datapath.alu_op_a: vec("32h0000_0001"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0024"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0024"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0020"),
-            top.core.datapath.pc: bits("32h0040_0020"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b0_0011"),
-            top.core.datapath.wr_data: bits("32h0000_0002"),
-            top.core.datapath.inst_rs1: bits("5b0_0001"),
-            top.core.datapath.rs1_data: bits("32h0000_0001"),
-            top.core.datapath.inst_rs2: bits("5b0_0010"),
+            top.core.datapath.pc_next: vec("32h0040_0024"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0024"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0020"),
+            top.core.datapath.pc: vec("32h0040_0020"),
+            # Regfile
+            top.core.datapath.wr_data: vec("32h0000_0002"),
+            top.core.datapath.rs1_data: vec("32h0000_0001"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0002"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0002"),
         },
         # @(posedge clock)
         27: {
-            top.pc: bits("32h0040_0024"),
-            top.inst: bits("32h0020_0E93"),
+            top._pc: vec("32h0040_0024"),
+            top._inst: vec("32h0020_0E93"),
             # Decode
-            top.core.datapath.inst: bits("32h0020_0E93"),
-            top.core.datapath.inst_opcode: bits("7b001_0011"),
-            top.core.datapath.immediate: bits("32h0000_0002"),
+            top.core.datapath.inst: vec("32h0020_0E93"),
+            top.core.datapath.immediate: vec("32h0000_0002"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.IMM,
             # ALU
             top.core.datapath.alu_op_a: Z32,
-            top.core.datapath.alu_op_b: bits("32h0000_0002"),
+            top.core.datapath.alu_op_b: vec("32h0000_0002"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0028"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0028"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0026"),
-            top.core.datapath.pc: bits("32h0040_0024"),
+            top.core.datapath.pc_next: vec("32h0040_0028"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0028"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0026"),
+            top.core.datapath.pc: vec("32h0040_0024"),
             # Regfile
-            top.core.datapath.inst_rd: bits("5b1_1101"),
-            top.core.datapath.inst_rs1: bits("5b0_0000"),
             top.core.datapath.rs1_data: Z32,
         },
         # @(posedge clock)
         29: {
-            top.pc: bits("32h0040_0028"),
-            top.inst: bits("32h0030_0E13"),
-            top.bus_addr: bits("32h0000_0003"),
-            top.bus_wr_data: bits("32h0200_0000"),
-            # Decode
-            top.core.datapath.inst: bits("32h0030_0E13"),
-            top.core.datapath.immediate: bits("32h0000_0003"),
-            # ALU
-            top.core.datapath.alu_result: bits("32h0000_0003"),
-            top.core.datapath.alu_op_b: bits("32h0000_0003"),
-            # PC
-            top.core.datapath.pc_next: bits("32h0040_002C"),
-            top.core.datapath.pc_plus_4: bits("32h0040_002C"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_002B"),
-            top.core.datapath.pc: bits("32h0040_0028"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b1_1100"),
-            top.core.datapath.wr_data: bits("32h0000_0003"),
-            top.core.datapath.inst_rs2: bits("5b0_0011"),
-            top.core.datapath.rs2_data: bits("32h0000_0002"),
+            top._pc: vec("32h0040_0028"),
+            top._inst: vec("32h0030_0E13"),
+            top.bus_addr: vec("32h0000_0003"),
+            top.bus_wr_data: vec("32h0200_0000"),
+            # Decode
+            top.core.datapath.inst: vec("32h0030_0E13"),
+            top.core.datapath.immediate: vec("32h0000_0003"),
+            # ALU
+            top.core.datapath.alu_result: vec("32h0000_0003"),
+            top.core.datapath.alu_op_b: vec("32h0000_0003"),
+            # PC
+            top.core.datapath.pc_next: vec("32h0040_002C"),
+            top.core.datapath.pc_plus_4: vec("32h0040_002C"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_002B"),
+            top.core.datapath.pc: vec("32h0040_0028"),
+            # Regfile
+            top.core.datapath.wr_data: vec("32h0000_0003"),
+            top.core.datapath.rs2_data: vec("32h0000_0002"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0003"),
-            top.core.datapath.data_mem_wr_data: bits("32h0000_0002"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0003"),
+            top.core.datapath.data_mem_wr_data: vec("32h0000_0002"),
         },
         # @(posedge clock)
         31: {
-            top.pc: bits("32h0040_002C"),
-            top.inst: bits("32h4BD1_9A63"),
-            top.bus_addr: bits("32h0000_0001"),
-            top.bus_wr_data: bits("32h0000_0200"),
-            # Decode
-            top.core.datapath.inst: bits("32h4BD1_9A63"),
-            top.core.datapath.inst_funct7: bits("7b010_0101"),
-            top.core.datapath.inst_funct3: bits("3b001"),
-            top.core.datapath.inst_opcode: bits("7b110_0011"),
-            top.core.datapath.immediate: bits("32h0000_04B4"),
+            top._pc: vec("32h0040_002C"),
+            top._inst: vec("32h4BD1_9A63"),
+            top.bus_addr: vec("32h0000_0001"),
+            top.bus_wr_data: vec("32h0000_0200"),
+            # Decode
+            top.core.datapath.inst: vec("32h4BD1_9A63"),
+            top.core.datapath.immediate: vec("32h0000_04B4"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.RS2,
             # ALU
-            top.core.datapath.alu_result: bits("32h0000_0001"),
+            top.core.datapath.alu_result: vec("32h0000_0001"),
             top.core.datapath.alu_function: AluOp.SEQ,
-            top.core.datapath.alu_op_a: bits("32h0000_0002"),
-            top.core.datapath.alu_op_b: bits("32h0000_0002"),
+            top.core.datapath.alu_op_a: vec("32h0000_0002"),
+            top.core.datapath.alu_op_b: vec("32h0000_0002"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0030"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0030"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_04E0"),
-            top.core.datapath.pc: bits("32h0040_002C"),
-            # Regfile
-            top.core.datapath.regfile_wr_en: F,
-            top.core.datapath.inst_rd: bits("5b1_0100"),
-            top.core.datapath.wr_data: bits("32h0000_0001"),
-            top.core.datapath.inst_rs1: bits("5b0_0011"),
-            top.core.datapath.rs1_data: bits("32h0000_0002"),
-            top.core.datapath.inst_rs2: bits("5b1_1101"),
+            top.core.datapath.pc_next: vec("32h0040_0030"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0030"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_04E0"),
+            top.core.datapath.pc: vec("32h0040_002C"),
+            # Regfile
+            top.core.datapath.regfile_wr_en: zeros(1),
+            top.core.datapath.wr_data: vec("32h0000_0001"),
+            top.core.datapath.rs1_data: vec("32h0000_0002"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0001"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0001"),
         },
         # @(posedge clock)
         33: {
-            top.pc: bits("32h0040_0030"),
-            top.inst: bits("32h0030_0093"),
-            top.bus_addr: bits("32h0000_0003"),
-            top.bus_wr_data: bits("32h0200_0000"),
-            # Decode
-            top.core.datapath.inst: bits("32h0030_0093"),
-            top.core.datapath.inst_funct7: bits("7b000_0000"),
-            top.core.datapath.inst_funct3: bits("3b000"),
-            top.core.datapath.inst_opcode: bits("7b001_0011"),
-            top.core.datapath.immediate: bits("32h0000_0003"),
+            top._pc: vec("32h0040_0030"),
+            top._inst: vec("32h0030_0093"),
+            top.bus_addr: vec("32h0000_0003"),
+            top.bus_wr_data: vec("32h0200_0000"),
+            # Decode
+            top.core.datapath.inst: vec("32h0030_0093"),
+            top.core.datapath.immediate: vec("32h0000_0003"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.IMM,
             # ALU
-            top.core.datapath.alu_result: bits("32h0000_0003"),
+            top.core.datapath.alu_result: vec("32h0000_0003"),
             top.core.datapath.alu_function: AluOp.ADD,
             top.core.datapath.alu_op_a: Z32,
-            top.core.datapath.alu_op_b: bits("32h0000_0003"),
+            top.core.datapath.alu_op_b: vec("32h0000_0003"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0034"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0034"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0033"),
-            top.core.datapath.pc: bits("32h0040_0030"),
-            # Regfile
-            top.core.datapath.regfile_wr_en: T,
-            top.core.datapath.inst_rd: bits("5b0_0001"),
-            top.core.datapath.wr_data: bits("32h0000_0003"),
-            top.core.datapath.inst_rs1: bits("5b0_0000"),
+            top.core.datapath.pc_next: vec("32h0040_0034"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0034"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0033"),
+            top.core.datapath.pc: vec("32h0040_0030"),
+            # Regfile
+            top.core.datapath.regfile_wr_en: ones(1),
+            top.core.datapath.wr_data: vec("32h0000_0003"),
             top.core.datapath.rs1_data: Z32,
-            top.core.datapath.inst_rs2: bits("5b0_0011"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0003"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0003"),
         },
         # @(posedge clock)
         35: {
-            top.pc: bits("32h0040_0034"),
-            top.inst: bits("32h0070_0113"),
-            top.bus_addr: bits("32h0000_0007"),
+            top._pc: vec("32h0040_0034"),
+            top._inst: vec("32h0070_0113"),
+            top.bus_addr: vec("32h0000_0007"),
             top.bus_wr_data: Z32,
             # Decode
-            top.core.datapath.inst: bits("32h0070_0113"),
-            top.core.datapath.immediate: bits("32h0000_0007"),
+            top.core.datapath.inst: vec("32h0070_0113"),
+            top.core.datapath.immediate: vec("32h0000_0007"),
             # ALU
-            top.core.datapath.alu_result: bits("32h0000_0007"),
-            top.core.datapath.alu_op_b: bits("32h0000_0007"),
+            top.core.datapath.alu_result: vec("32h0000_0007"),
+            top.core.datapath.alu_op_b: vec("32h0000_0007"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0038"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0038"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_003B"),
-            top.core.datapath.pc: bits("32h0040_0034"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b0_0010"),
-            top.core.datapath.wr_data: bits("32h0000_0007"),
-            top.core.datapath.inst_rs2: bits("5b0_0111"),
+            top.core.datapath.pc_next: vec("32h0040_0038"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0038"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_003B"),
+            top.core.datapath.pc: vec("32h0040_0034"),
+            # Regfile
+            top.core.datapath.wr_data: vec("32h0000_0007"),
             top.core.datapath.rs2_data: Z32,
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0007"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0007"),
             top.core.datapath.data_mem_wr_data: Z32,
         },
         # @(posedge clock)
         37: {
-            top.pc: bits("32h0040_0038"),
-            top.inst: bits("32h0020_81B3"),
-            top.bus_addr: bits("32h0000_000A"),
-            top.bus_wr_data: bits("32h0007_0000"),
+            top._pc: vec("32h0040_0038"),
+            top._inst: vec("32h0020_81B3"),
+            top.bus_addr: vec("32h0000_000A"),
+            top.bus_wr_data: vec("32h0007_0000"),
             # Decode
-            top.core.datapath.inst: bits("32h0020_81B3"),
-            top.core.datapath.inst_opcode: bits("7b011_0011"),
+            top.core.datapath.inst: vec("32h0020_81B3"),
             top.core.datapath.immediate: Z32,
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.RS2,
             # ALU
-            top.core.datapath.alu_result: bits("32h0000_000A"),
-            top.core.datapath.alu_op_a: bits("32h0000_0003"),
+            top.core.datapath.alu_result: vec("32h0000_000A"),
+            top.core.datapath.alu_op_a: vec("32h0000_0003"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_003C"),
-            top.core.datapath.pc_plus_4: bits("32h0040_003C"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0038"),
-            top.core.datapath.pc: bits("32h0040_0038"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b0_0011"),
-            top.core.datapath.wr_data: bits("32h0000_000A"),
-            top.core.datapath.inst_rs1: bits("5b0_0001"),
-            top.core.datapath.rs1_data: bits("32h0000_0003"),
-            top.core.datapath.inst_rs2: bits("5b0_0010"),
-            top.core.datapath.rs2_data: bits("32h0000_0007"),
+            top.core.datapath.pc_next: vec("32h0040_003C"),
+            top.core.datapath.pc_plus_4: vec("32h0040_003C"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0038"),
+            top.core.datapath.pc: vec("32h0040_0038"),
+            # Regfile
+            top.core.datapath.wr_data: vec("32h0000_000A"),
+            top.core.datapath.rs1_data: vec("32h0000_0003"),
+            top.core.datapath.rs2_data: vec("32h0000_0007"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_000A"),
-            top.core.datapath.data_mem_wr_data: bits("32h0000_0007"),
+            top.core.datapath.data_mem_addr: vec("32h0000_000A"),
+            top.core.datapath.data_mem_wr_data: vec("32h0000_0007"),
         },
         # @(posedge clock)
         39: {
-            top.pc: bits("32h0040_003C"),
-            top.inst: bits("32h00A0_0E93"),
+            top._pc: vec("32h0040_003C"),
+            top._inst: vec("32h00A0_0E93"),
             top.bus_wr_data: Z32,
             # Decode
-            top.core.datapath.inst: bits("32h00A0_0E93"),
-            top.core.datapath.inst_opcode: bits("7b001_0011"),
-            top.core.datapath.immediate: bits("32h0000_000A"),
+            top.core.datapath.inst: vec("32h00A0_0E93"),
+            top.core.datapath.immediate: vec("32h0000_000A"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.IMM,
             # ALU
             top.core.datapath.alu_op_a: Z32,
-            top.core.datapath.alu_op_b: bits("32h0000_000A"),
+            top.core.datapath.alu_op_b: vec("32h0000_000A"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0040"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0040"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0046"),
-            top.core.datapath.pc: bits("32h0040_003C"),
+            top.core.datapath.pc_next: vec("32h0040_0040"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0040"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0046"),
+            top.core.datapath.pc: vec("32h0040_003C"),
             # Regfile
-            top.core.datapath.inst_rd: bits("5b1_1101"),
-            top.core.datapath.inst_rs1: bits("5b0_0000"),
             top.core.datapath.rs1_data: Z32,
-            top.core.datapath.inst_rs2: bits("5b0_1010"),
             top.core.datapath.rs2_data: Z32,
             # Data Mem
             top.core.datapath.data_mem_wr_data: Z32,
         },
         # @(posedge clock)
         41: {
-            top.pc: bits("32h0040_0040"),
-            top.inst: bits("32h0040_0E13"),
-            top.bus_addr: bits("32h0000_0004"),
-            # Decode
-            top.core.datapath.inst: bits("32h0040_0E13"),
-            top.core.datapath.immediate: bits("32h0000_0004"),
-            # ALU
-            top.core.datapath.alu_result: bits("32h0000_0004"),
-            top.core.datapath.alu_op_b: bits("32h0000_0004"),
-            # PC
-            top.core.datapath.pc_next: bits("32h0040_0044"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0044"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0044"),
-            top.core.datapath.pc: bits("32h0040_0040"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b1_1100"),
-            top.core.datapath.wr_data: bits("32h0000_0004"),
-            top.core.datapath.inst_rs2: bits("5b0_0100"),
+            top._pc: vec("32h0040_0040"),
+            top._inst: vec("32h0040_0E13"),
+            top.bus_addr: vec("32h0000_0004"),
+            # Decode
+            top.core.datapath.inst: vec("32h0040_0E13"),
+            top.core.datapath.immediate: vec("32h0000_0004"),
+            # ALU
+            top.core.datapath.alu_result: vec("32h0000_0004"),
+            top.core.datapath.alu_op_b: vec("32h0000_0004"),
+            # PC
+            top.core.datapath.pc_next: vec("32h0040_0044"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0044"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0044"),
+            top.core.datapath.pc: vec("32h0040_0040"),
+            # Regfile
+            top.core.datapath.wr_data: vec("32h0000_0004"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0004"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0004"),
         },
         # @(posedge clock)
         43: {
-            top.pc: bits("32h0040_0044"),
-            top.inst: bits("32h49D1_9E63"),
-            top.bus_addr: bits("32h0000_0001"),
-            top.bus_wr_data: bits("32h0000_0A00"),
-            # Decode
-            top.core.datapath.inst: bits("32h49D1_9E63"),
-            top.core.datapath.inst_funct7: bits("7b010_0100"),
-            top.core.datapath.inst_funct3: bits("3b001"),
-            top.core.datapath.inst_opcode: bits("7b110_0011"),
-            top.core.datapath.immediate: bits("32h0000_049C"),
+            top._pc: vec("32h0040_0044"),
+            top._inst: vec("32h49D1_9E63"),
+            top.bus_addr: vec("32h0000_0001"),
+            top.bus_wr_data: vec("32h0000_0A00"),
+            # Decode
+            top.core.datapath.inst: vec("32h49D1_9E63"),
+            top.core.datapath.immediate: vec("32h0000_049C"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.RS2,
             # ALU
-            top.core.datapath.alu_result: bits("32h0000_0001"),
+            top.core.datapath.alu_result: vec("32h0000_0001"),
             top.core.datapath.alu_function: AluOp.SEQ,
-            top.core.datapath.alu_op_a: bits("32h0000_000A"),
-            top.core.datapath.alu_op_b: bits("32h0000_000A"),
+            top.core.datapath.alu_op_a: vec("32h0000_000A"),
+            top.core.datapath.alu_op_b: vec("32h0000_000A"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0048"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0048"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_04E0"),
-            top.core.datapath.pc: bits("32h0040_0044"),
-            # Regfile
-            top.core.datapath.regfile_wr_en: F,
-            top.core.datapath.wr_data: bits("32h0000_0001"),
-            top.core.datapath.inst_rs1: bits("5b0_0011"),
-            top.core.datapath.rs1_data: bits("32h0000_000A"),
-            top.core.datapath.inst_rs2: bits("5b1_1101"),
-            top.core.datapath.rs2_data: bits("32h0000_000A"),
+            top.core.datapath.pc_next: vec("32h0040_0048"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0048"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_04E0"),
+            top.core.datapath.pc: vec("32h0040_0044"),
+            # Regfile
+            top.core.datapath.regfile_wr_en: zeros(1),
+            top.core.datapath.wr_data: vec("32h0000_0001"),
+            top.core.datapath.rs1_data: vec("32h0000_000A"),
+            top.core.datapath.rs2_data: vec("32h0000_000A"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32h0000_0001"),
-            top.core.datapath.data_mem_wr_data: bits("32h0000_000A"),
+            top.core.datapath.data_mem_addr: vec("32h0000_0001"),
+            top.core.datapath.data_mem_wr_data: vec("32h0000_000A"),
         },
         # @(posedge clock)
         45: {
-            top.pc: bits("32h0040_0048"),
-            top.inst: bits("32h0000_0093"),
+            top._pc: vec("32h0040_0048"),
+            top._inst: vec("32h0000_0093"),
             top.bus_addr: Z32,
             top.bus_wr_data: Z32,
             # Decode
-            top.core.datapath.inst: bits("32h0000_0093"),
-            top.core.datapath.inst_funct7: bits("7b000_0000"),
-            top.core.datapath.inst_funct3: bits("3b000"),
-            top.core.datapath.inst_opcode: bits("7b001_0011"),
+            top.core.datapath.inst: vec("32h0000_0093"),
             top.core.datapath.immediate: Z32,
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.IMM,
             # ALU
             top.core.datapath.alu_result: Z32,
-            top.core.datapath.alu_result_equal_zero: T,
+            top.core.datapath.alu_result_equal_zero: ones(1),
             top.core.datapath.alu_function: AluOp.ADD,
             top.core.datapath.alu_op_a: Z32,
             top.core.datapath.alu_op_b: Z32,
             # PC
-            top.core.datapath.pc_next: bits("32h0040_004C"),
-            top.core.datapath.pc_plus_4: bits("32h0040_004C"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0048"),
-            top.core.datapath.pc: bits("32h0040_0048"),
+            top.core.datapath.pc_next: vec("32h0040_004C"),
+            top.core.datapath.pc_plus_4: vec("32h0040_004C"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0048"),
+            top.core.datapath.pc: vec("32h0040_0048"),
             # Regfile
-            top.core.datapath.regfile_wr_en: T,
-            top.core.datapath.inst_rd: bits("5b0_0001"),
+            top.core.datapath.regfile_wr_en: ones(1),
             top.core.datapath.wr_data: Z32,
-            top.core.datapath.inst_rs1: bits("5b0_0000"),
             top.core.datapath.rs1_data: Z32,
-            top.core.datapath.inst_rs2: bits("5b0_0000"),
             top.core.datapath.rs2_data: Z32,
             # Data Mem
             top.core.datapath.data_mem_addr: Z32,
             top.core.datapath.data_mem_wr_data: Z32,
         },
         # @(posedge clock)
         47: {
-            top.pc: bits("32h0040_004C"),
-            top.inst: bits("32hFFFF_8137"),
+            top._pc: vec("32h0040_004C"),
+            top._inst: vec("32hFFFF_8137"),
             # Decode
-            top.core.datapath.inst: bits("32hFFFF_8137"),
-            top.core.datapath.inst_funct7: bits("7b111_1111"),
-            top.core.datapath.inst_opcode: bits("7b011_0111"),
-            top.core.datapath.immediate: bits("32hFFFF_8000"),
+            top.core.datapath.inst: vec("32hFFFF_8137"),
+            top.core.datapath.immediate: vec("32hFFFF_8000"),
             # Control
             top.core.datapath.alu_op_b_sel: CtlAluB.RS2,
-            top.core.datapath.reg_writeback_sel: bits("3b011"),
+            top.core.datapath.reg_writeback_sel: vec("3b011"),
             # PC
-            top.core.datapath.pc_next: bits("32h0040_0050"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0050"),
-            top.core.datapath.pc_plus_immediate: bits("32h003F_804C"),
-            top.core.datapath.pc: bits("32h0040_004C"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b0_0010"),
-            top.core.datapath.wr_data: bits("32hFFFF_8000"),
-            top.core.datapath.inst_rs1: bits("5b1_1111"),
-            top.core.datapath.inst_rs2: bits("5b1_1111"),
+            top.core.datapath.pc_next: vec("32h0040_0050"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0050"),
+            top.core.datapath.pc_plus_immediate: vec("32h003F_804C"),
+            top.core.datapath.pc: vec("32h0040_004C"),
+            # Regfile
+            top.core.datapath.wr_data: vec("32hFFFF_8000"),
         },
         # @(posedge clock)
         49: {
-            top.pc: bits("32h0040_0050"),
-            top.inst: bits("32h0020_81B3"),
-            top.bus_addr: bits("32hFFFF_8000"),
-            top.bus_wr_data: bits("32hFFFF_8000"),
-            # Decode
-            top.core.datapath.inst: bits("32h0020_81B3"),
-            top.core.datapath.inst_funct7: bits("7b000_0000"),
-            top.core.datapath.inst_opcode: bits("7b011_0011"),
+            top._pc: vec("32h0040_0050"),
+            top._inst: vec("32h0020_81B3"),
+            top.bus_addr: vec("32hFFFF_8000"),
+            top.bus_wr_data: vec("32hFFFF_8000"),
+            # Decode
+            top.core.datapath.inst: vec("32h0020_81B3"),
             top.core.datapath.immediate: Z32,
             # Control
-            top.core.datapath.reg_writeback_sel: bits("3b000"),
+            top.core.datapath.reg_writeback_sel: vec("3b000"),
             # ALU
-            top.core.datapath.alu_result: bits("32hFFFF_8000"),
-            top.core.datapath.alu_result_equal_zero: F,
-            top.core.datapath.alu_op_b: bits("32hFFFF_8000"),
+            top.core.datapath.alu_result: vec("32hFFFF_8000"),
+            top.core.datapath.alu_result_equal_zero: zeros(1),
+            top.core.datapath.alu_op_b: vec("32hFFFF_8000"),
             # Next PC
-            top.core.datapath.pc_next: bits("32h0040_0054"),
-            top.core.datapath.pc_plus_4: bits("32h0040_0054"),
-            top.core.datapath.pc_plus_immediate: bits("32h0040_0050"),
-            top.core.datapath.pc: bits("32h0040_0050"),
-            # Regfile
-            top.core.datapath.inst_rd: bits("5b0_0011"),
-            top.core.datapath.inst_rs1: bits("5b0_0001"),
-            top.core.datapath.inst_rs2: bits("5b0_0010"),
-            top.core.datapath.rs2_data: bits("32hFFFF_8000"),
+            top.core.datapath.pc_next: vec("32h0040_0054"),
+            top.core.datapath.pc_plus_4: vec("32h0040_0054"),
+            top.core.datapath.pc_plus_immediate: vec("32h0040_0050"),
+            top.core.datapath.pc: vec("32h0040_0050"),
+            # Regfile
+            top.core.datapath.rs2_data: vec("32hFFFF_8000"),
             # Data Mem
-            top.core.datapath.data_mem_addr: bits("32hFFFF_8000"),
-            top.core.datapath.data_mem_wr_data: bits("32hFFFF_8000"),
+            top.core.datapath.data_mem_addr: vec("32hFFFF_8000"),
+            top.core.datapath.data_mem_wr_data: vec("32hFFFF_8000"),
         },
     }
     assert waves == exp
 
 
 def run_riscv_test(name: str) -> int:
-    """TODO(cjdrake): Write docstring."""
     loop.reset()
 
     # Create module hierarchy
     top = Top(name="top")
 
     simify(top)
 
     # Initialize instruction memory
     text = get_mem(f"tests/riscv/tests/{name}.text")
     for i, d in enumerate(text):
-        top.text_memory_bus.text_memory.mem.set_value(i, uint2bits(d, 32))
+        top.text_memory_bus.text_memory._mem.set_next(i, uint2vec(d, 32))
 
     # Initialize data memory
     data = get_mem(f"tests/riscv/tests/{name}.data")
     for i, d in enumerate(data):
-        top.data_memory_bus.data_memory.mem.set_value(i, uint2bits(d, 32))
+        top.data_memory_bus.data_memory._mem.set_next(i, uint2vec(d, 32))
 
     # Run the simulation
     for _ in loop.iter(until=10000):
-        if top.bus_wr_en.value == T and top.bus_addr.value == DEBUG_REG:
-            if top.bus_wr_data.value == bits("32h0000_0001"):
+        if top.bus_wr_en.value == ones(1) and top.bus_addr.value == DEBUG_REG:
+            if top.bus_wr_data.value == vec("32h0000_0001"):
                 return PASS
             else:
                 return FAIL
     return TIMEOUT
 
 
 def test_singlecycle_add():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("add") == PASS
 
 
 def test_singlecycle_addi():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("addi") == PASS
 
 
 def test_singlecycle_and():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("and") == PASS
 
 
 def test_singlecycle_andi():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("andi") == PASS
 
 
 def test_singlecycle_auipc():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("auipc") == PASS
 
 
 def test_singlecycle_beq():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("beq") == PASS
 
 
 def test_singlecycle_bge():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("bge") == PASS
 
 
 def test_singlecycle_bgeu():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("bgeu") == PASS
 
 
 def test_singlecycle_blt():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("blt") == PASS
 
 
 def test_singlecycle_bltu():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("bltu") == PASS
 
 
 def test_singlecycle_bne():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("bne") == PASS
 
 
 def test_singlecycle_jal():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("jal") == PASS
 
 
 def test_singlecycle_jalr():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("jalr") == PASS
 
 
 def test_singlecycle_lb():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("lb") == PASS
 
 
 def test_singlecycle_lbu():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("lbu") == PASS
 
 
 def test_singlecycle_lh():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("lh") == PASS
 
 
 def test_singlecycle_lhu():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("lhu") == PASS
 
 
 def test_singlecycle_lui():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("lui") == PASS
 
 
 def test_singlecycle_lw():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("lw") == PASS
 
 
 def test_singlecycle_or():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("or") == PASS
 
 
 def test_singlecycle_ori():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("ori") == PASS
 
 
 def test_singlecycle_sb():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("sb") == PASS
 
 
 def test_singlecycle_sh():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("sh") == PASS
 
 
 def test_singlecycle_simple():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("simple") == PASS
 
 
 def test_singlecycle_sll():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("sll") == PASS
 
 
 def test_singlecycle_slli():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("slli") == PASS
 
 
 def test_singlecycle_slt():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("slt") == PASS
 
 
 def test_singlecycle_slti():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("slti") == PASS
 
 
 def test_singlecycle_sltiu():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("sltiu") == PASS
 
 
 def test_singlecycle_sltu():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("sltu") == PASS
 
 
 def test_singlecycle_sra():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("sra") == PASS
 
 
 def test_singlecycle_srai():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("srai") == PASS
 
 
 def test_singlecycle_srl():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("srl") == PASS
 
 
 def test_singlecycle_srli():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("srli") == PASS
 
 
 def test_singlecycle_sub():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("sub") == PASS
 
 
 def test_singlecycle_sw():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("sw") == PASS
 
 
 def test_singlecycle_xor():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("xor") == PASS
 
 
 def test_singlecycle_xori():
-    """TODO(cjdrake): Write docstring."""
     assert run_riscv_test("xori") == PASS
```

### Comparing `seqlogic-0.0.7/tests/test_sim.py` & `seqlogic-0.0.8/tests/test_sim.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 """Test seqlogic.sim module."""
 
 from collections import defaultdict
 
 import pytest
 
-from seqlogic.sim import Region, Singular, get_loop, notify, sleep
+from seqlogic import get_loop, sleep
+from seqlogic.sim import Region, SimAwaitable, Singular, State
 
 loop = get_loop()
 waves = defaultdict(dict)
 
 
 def _waves_add(time, var, val):
     waves[time][var] = val
 
 
 class Bool(Singular):
     """Variable that supports dumping to memory."""
 
     def __init__(self):
-        """TODO(cjdrake): Write docstring."""
         super().__init__(value=False)
-        _waves_add(self._sim.time(), self, self._value)
+        _waves_add(self._sim.time, self, self._value)
 
     def update(self):
-        """TODO(cjdrake): Write docstring."""
         if self.dirty():
-            _waves_add(self._sim.time(), self, self._next_value)
+            _waves_add(self._sim.time, self, self._next_value)
         super().update()
 
-    def posedge(self) -> bool:
-        """TODO(cjdrake): Write docstring."""
+    def is_posedge(self) -> bool:
         return not self._value and self._next_value
 
-    def negedge(self) -> bool:
-        """TODO(cjdrake): Write docstring."""
+    def is_negedge(self) -> bool:
         return self._value and not self._next_value
 
-    def edge(self) -> bool:
-        """TODO(cjdrake): Write docstring."""
-        return self.posedge() or self.negedge()
+    async def edge(self) -> State:
+        self._sim.add_event(self, lambda: self.is_posedge() or self.is_negedge())
+        state = await SimAwaitable()
+        return state
 
 
 HELLO_OUT = """\
 [2] Hello
 [4] World
 """
 
 
 def test_hello(capsys):
     """Test basic async/await hello world functionality."""
     loop.reset()
 
     async def hello():
         await sleep(2)
-        print(f"[{loop.time()}] Hello")
+        print(f"[{loop.time}] Hello")
         await sleep(2)
-        print(f"[{loop.time()}] World")
+        print(f"[{loop.time}] World")
 
-    loop.add_proc(hello, Region(2))
+    loop.add_proc(Region(2), hello)
 
     # Invalid run limit
     with pytest.raises(TypeError):
         loop.run("Invalid argument type")  # pyright: ignore[reportArgumentType]
 
     # Run until no events left
     loop.run()
@@ -82,32 +80,32 @@
         while True:
             await sleep(5)
             clk.next = not clk.value
 
     async def p_a():
         i = 0
         while True:
-            await notify(clk.edge)
+            await clk.edge()
             if i % 2 == 0:
                 a.next = not a.value
             else:
                 a.next = a.value
             i += 1
 
     async def p_b():
         i = 0
         while True:
-            await notify(clk.edge)
+            await clk.edge()
             if i % 3 == 0:
                 b.next = not b.value
             i += 1
 
-    loop.add_proc(p_clk, Region(2))
-    loop.add_proc(p_a, Region(1))
-    loop.add_proc(p_b, Region(1))
+    loop.add_proc(Region(2), p_clk)
+    loop.add_proc(Region(1), p_a)
+    loop.add_proc(Region(1), p_b)
 
     # Expected sim output
     exp = {
         -1: {clk: False, a: False, b: False},
         5: {clk: True, a: True, b: True},
         10: {clk: False},
         15: {clk: True, a: False},
@@ -145,32 +143,32 @@
         while True:
             await sleep(5)
             clk.next = not clk.value
 
     async def p_a():
         i = 0
         while True:
-            await notify(clk.edge)
+            await clk.edge()
             if i % 2 == 0:
                 a.next = not a.value
             else:
                 a.next = a.value
             i += 1
 
     async def p_b():
         i = 0
         while True:
-            await notify(clk.edge)
+            await clk.edge()
             if i % 3 == 0:
                 b.next = not b.value
             i += 1
 
-    loop.add_proc(p_clk, Region(2))
-    loop.add_proc(p_a, Region(1))
-    loop.add_proc(p_b, Region(1))
+    loop.add_proc(Region(2), p_clk)
+    loop.add_proc(Region(1), p_a)
+    loop.add_proc(Region(1), p_b)
 
     # Expected sim output
     exp = {
         -1: {clk: False, a: False, b: False},
         5: {clk: True, a: True, b: True},
         10: {clk: False},
         15: {clk: True, a: False},
```

