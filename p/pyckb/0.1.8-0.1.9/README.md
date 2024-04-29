# Comparing `tmp/pyckb-0.1.8.tar.gz` & `tmp/pyckb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyckb-0.1.8.tar", last modified: Wed Apr 10 07:01:22 2024, max compression
+gzip compressed data, was "pyckb-0.1.9.tar", last modified: Mon Apr 29 09:21:17 2024, max compression
```

## Comparing `pyckb-0.1.8.tar` & `pyckb-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-10 07:01:22.492136 pyckb-0.1.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-12-30 04:14:24.000000 pyckb-0.1.8/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-04-10 07:01:22.492136 pyckb-0.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2722 2024-04-10 03:25:41.000000 pyckb-0.1.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-10 07:01:22.488136 pyckb-0.1.8/ckb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      167 2024-02-26 07:22:12.000000 pyckb-0.1.8/ckb/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4369 2023-12-30 06:34:14.000000 pyckb-0.1.8/ckb/bech32.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4149 2024-04-09 03:33:20.000000 pyckb-0.1.8/ckb/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17356 2024-01-22 11:27:36.000000 pyckb-0.1.8/ckb/core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2024-01-22 07:26:45.000000 pyckb-0.1.8/ckb/ecdsa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3833 2024-01-22 11:27:41.000000 pyckb-0.1.8/ckb/molecule.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4413 2024-01-19 03:18:32.000000 pyckb-0.1.8/ckb/rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4268 2024-01-12 02:06:10.000000 pyckb-0.1.8/ckb/secp256k1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23788 2024-01-31 03:11:03.000000 pyckb-0.1.8/ckb/wallet.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-10 07:01:22.492136 pyckb-0.1.8/pyckb.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      377 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-10 07:01:22.000000 pyckb-0.1.8/pyckb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2024-04-10 06:59:09.000000 pyckb-0.1.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-10 07:01:22.492136 pyckb-0.1.8/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-10 07:01:22.492136 pyckb-0.1.8/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2254 2024-03-21 07:26:46.000000 pyckb-0.1.8/test/test_core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-01-12 02:25:22.000000 pyckb-0.1.8/test/test_ecdsa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-12-28 09:23:55.000000 pyckb-0.1.8/test/test_rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1791 2024-04-09 03:55:53.000000 pyckb-0.1.8/test/test_wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 09:21:17.949677 pyckb-0.1.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-12-30 04:14:24.000000 pyckb-0.1.9/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-04-29 09:21:17.949677 pyckb-0.1.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2722 2024-04-10 03:25:41.000000 pyckb-0.1.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 09:21:17.945677 pyckb-0.1.9/ckb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2024-04-29 09:12:52.000000 pyckb-0.1.9/ckb/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4637 2024-04-19 12:01:42.000000 pyckb-0.1.9/ckb/bech32m.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4149 2024-04-26 09:57:50.000000 pyckb-0.1.9/ckb/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17328 2024-04-29 09:13:36.000000 pyckb-0.1.9/ckb/core.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2024-04-29 09:13:08.000000 pyckb-0.1.9/ckb/denomination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2024-01-22 07:26:45.000000 pyckb-0.1.9/ckb/ecdsa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3833 2024-01-22 11:27:41.000000 pyckb-0.1.9/ckb/molecule.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2373 2024-04-23 08:43:17.000000 pyckb-0.1.9/ckb/rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4285 2024-04-26 12:19:31.000000 pyckb-0.1.9/ckb/secp256k1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23940 2024-04-29 09:14:31.000000 pyckb-0.1.9/ckb/wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 09:21:17.949677 pyckb-0.1.9/pyckb.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2024-04-29 09:19:50.000000 pyckb-0.1.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-29 09:21:17.949677 pyckb-0.1.9/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 09:21:17.949677 pyckb-0.1.9/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2254 2024-03-21 07:26:46.000000 pyckb-0.1.9/test/test_core.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-01-12 02:25:22.000000 pyckb-0.1.9/test/test_ecdsa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1245 2024-04-23 08:21:35.000000 pyckb-0.1.9/test/test_rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2024-04-29 09:17:31.000000 pyckb-0.1.9/test/test_wallet.py
```

### Comparing `pyckb-0.1.8/LICENSE` & `pyckb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.8/PKG-INFO` & `pyckb-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyckb
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for CKB
 Author-email: Mohanson <mohanson@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Mohanson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyckb-0.1.8/README.md` & `pyckb-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.8/ckb/config.py` & `pyckb-0.1.9/ckb/config.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.8/ckb/core.py` & `pyckb-0.1.9/ckb/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import ckb.bech32
+import ckb.bech32m
 import ckb.config
 import ckb.ecdsa
 import ckb.molecule
 import ckb.secp256k1
 import hashlib
 import json
 
-# 1 ckb = 10 ** 8 shannons
-shannon = 10 ** 8
 # https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0022-transaction-structure/0022-transaction-structure.md
 # The Type ID code cell uses a special type script hash, which is just the ascii codes in hex of the text TYPE_ID.
 type_id_code_hash = bytearray.fromhex('00000000000000000000000000000000000000000000000000545950455f4944')
 type_id_hash_type = 1
 
 
 def hash(data: bytearray):
@@ -155,36 +153,36 @@
             'args': f'0x{self.args.hex()}',
         }
 
     def hash(self):
         return hash(self.molecule())
 
 
-def address_encode(script: Script):
+def address_encode(script: Script) -> str:
     # See: https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0021-ckb-address-format/0021-ckb-address-format.md
     # See: https://github.com/rev-chaos/ckb-address-demo/blob/master/ckb_addr_test.py
     payload = bytearray()
     payload.append(0x00)
     # Append secp256k1 code hash
     payload.extend(script.code_hash)
     payload.append(script.hash_type)
     payload.extend(script.args)
-    return ckb.bech32.bech32_encode(
+    return ckb.bech32m.bech32m_encode(
         ckb.config.current.hrp,
-        ckb.bech32.convertbits(payload, 8, 5),
-        ckb.bech32.Encoding.BECH32M
+        ckb.bech32m.bech32m_re_arrange_5(payload),
     )
 
 
-def address_decode(address: str):
-    _, data, _ = ckb.bech32.bech32_decode(address)
-    data = bytearray(ckb.bech32.convertbits(data, 5, 8, False))
-    code_hash = data[1:33]
-    hash_type = data[33]
-    args = data[34:]
+def address_decode(addr: str) -> Script:
+    _, data = ckb.bech32m.bech32m_decode(addr)
+    payload = bytearray(ckb.bech32m.bech32m_re_arrange_8(data))
+    assert payload[0] == 0
+    code_hash = payload[1:33]
+    hash_type = payload[33]
+    args = payload[34:]
     return Script(code_hash, hash_type, args)
 
 
 class OutPoint:
     def __init__(self, tx_hash: bytearray, index: int):
         assert len(tx_hash) == 32
         self.tx_hash = tx_hash
```

### Comparing `pyckb-0.1.8/ckb/ecdsa.py` & `pyckb-0.1.9/ckb/ecdsa.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.8/ckb/molecule.py` & `pyckb-0.1.9/ckb/molecule.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.8/ckb/secp256k1.py` & `pyckb-0.1.9/ckb/secp256k1.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     #
     # https://www.cs.miami.edu/home/burt/learning/Csc609.142/ecdsa-cert.pdf
     # Don Johnson, Alfred Menezes and Scott Vanstone, The Elliptic Curve Digital Signature Algorithm (ECDSA)
     # 3.1 The Finite Field Fp
 
     p = 0
 
-    def __init__(self, x):
+    def __init__(self, x: int):
         self.x = x % self.p
 
     def __repr__(self):
         return f'Fp(0x{self.x:064x})'
 
     def __eq__(self, data):
         assert self.p == data.p
@@ -83,15 +83,15 @@
 
 A = Fq(0)
 B = Fq(7)
 
 
 class Pt:
 
-    def __init__(self, x, y):
+    def __init__(self, x: Fq, y: Fq):
         if x != Fq(0) or y != Fq(0):
             assert y ** 2 == x ** 3 + A * x + B
         self.x = x
         self.y = y
 
     def __repr__(self):
         return f'Pt({self.x}, {self.y})'
@@ -118,15 +118,15 @@
         x3 = s * s - x1 - x2
         y3 = s * (x1 - x3) - y1
         return Pt(x3, y3)
 
     def __sub__(self, data):
         return self + data.__neg__()
 
-    def __mul__(self, k):
+    def __mul__(self, k: Fr):
         # Point multiplication: Double-and-add
         # https://en.wikipedia.org/wiki/Elliptic_curve_point_multiplication
         n = k.x
         result = I
         addend = self
         while n:
             b = n & 1
```

### Comparing `pyckb-0.1.8/ckb/wallet.py` & `pyckb-0.1.9/ckb/wallet.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         for e in self.tx.raw.inputs:
             out_point = e.previous_output
             result = ckb.rpc.get_transaction('0x' + out_point.tx_hash.hex())
             origin = ckb.core.CellOutput.json_read(result['transaction']['outputs'][out_point.index])
             sender_capacity += origin.capacity
         for e in self.tx.raw.outputs:
             output_capacity += e.capacity
-        assert sender_capacity - output_capacity <= 1 * ckb.core.shannon
+        assert sender_capacity - output_capacity <= 1 * ckb.denomination.ckbytes
 
     def analyze_outputs_data(self):
         assert len(self.tx.raw.outputs) == len(self.tx.raw.outputs_data)
 
     def analyze_since(self):
         # Transaction since precondition
         # See https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0017-tx-valid-since/0017-tx-valid-since.md
@@ -100,15 +100,15 @@
             'script_type': 'lock',
             'filter': {
                 'script_len_range': ['0x0', '0x1']
             }
         })['capacity'], 16)
 
     def transfer(self, script: ckb.core.Script, capacity: int):
-        assert capacity >= 61 * ckb.core.shannon
+        assert capacity >= 61 * ckb.denomination.ckbytes
         assert self.capacity() > capacity
         sender_capacity = 0
         accept_capacity = capacity
         accept_script = script
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
@@ -121,17 +121,17 @@
         for cell in itertools.islice(self.livecell(), 256):
             cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
-            if change_capacity >= 61 * ckb.core.shannon:
+            if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
-        assert change_capacity >= 61 * ckb.core.shannon
+        assert change_capacity >= 61 * ckb.denomination.ckbytes
         tx.raw.outputs[1].capacity = change_capacity
         sign_data = bytearray()
         sign_data.extend(tx.raw.hash())
         for witness in tx.witnesses:
             sign_data.extend(len(witness).to_bytes(8, 'little'))
             sign_data.extend(witness)
         sign_data = ckb.core.hash(sign_data)
@@ -169,15 +169,15 @@
         tx.witnesses[0] = ckb.core.WitnessArgs(sign, None, None).molecule()
         WalletTransactionAnalyzer(tx).analyze()
         hash = ckb.rpc.send_transaction(tx.json())
         return bytearray.fromhex(hash[2:])
 
     def script_deploy(self, script: ckb.core.Script, data: bytearray):
         sender_capacity = 0
-        accept_capacity = (61 + len(data)) * ckb.core.shannon
+        accept_capacity = (61 + len(data)) * ckb.denomination.ckbytes
         accept_script = script
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
         tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, None))
         tx.raw.outputs.append(ckb.core.CellOutput(change_capacity, change_script, None))
@@ -187,17 +187,17 @@
         for cell in itertools.islice(self.livecell(), 256):
             cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
-            if change_capacity >= 61 * ckb.core.shannon:
+            if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
-        assert change_capacity >= 61 * ckb.core.shannon
+        assert change_capacity >= 61 * ckb.denomination.ckbytes
         tx.raw.outputs[1].capacity = change_capacity
         sign_data = bytearray()
         sign_data.extend(tx.raw.hash())
         for witness in tx.witnesses:
             sign_data.extend(len(witness).to_bytes(8, 'little'))
             sign_data.extend(witness)
         sign_data = ckb.core.hash(sign_data)
@@ -205,15 +205,15 @@
         tx.witnesses[0] = ckb.core.WitnessArgs(sign, None, None).molecule()
         WalletTransactionAnalyzer(tx).analyze()
         hash = ckb.rpc.send_transaction(tx.json())
         return bytearray.fromhex(hash[2:])
 
     def script_deploy_type_id(self, script: ckb.core.Script, data: bytearray):
         sender_capacity = 0
-        accept_capacity = (126 + len(data)) * ckb.core.shannon
+        accept_capacity = (126 + len(data)) * ckb.denomination.ckbytes
         accept_script = script
         accept_typeid = ckb.core.Script(ckb.core.type_id_code_hash, ckb.core.type_id_hash_type, bytearray([0] * 32))
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
         tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, accept_typeid))
@@ -224,17 +224,17 @@
         for cell in itertools.islice(self.livecell(), 256):
             cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
-            if change_capacity >= 61 * ckb.core.shannon:
+            if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
-        assert change_capacity >= 61 * ckb.core.shannon
+        assert change_capacity >= 61 * ckb.denomination.ckbytes
         # https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0022-transaction-structure/0022-transaction-structure.md#type-id
         tx.raw.outputs[0].type.args = ckb.core.hash(tx.raw.inputs[0].molecule() + bytearray([0] * 8))
         tx.raw.outputs[1].capacity = change_capacity
         sign_data = bytearray()
         sign_data.extend(tx.raw.hash())
         for witness in tx.witnesses:
             sign_data.extend(len(witness).to_bytes(8, 'little'))
@@ -248,15 +248,15 @@
 
     def script_update_type_id(self, script: ckb.core.Script, data: bytearray, out_point: ckb.core.OutPoint):
         result = ckb.rpc.get_transaction('0x' + out_point.tx_hash.hex())
         origin = ckb.core.CellOutput.json_read(result['transaction']['outputs'][out_point.index])
         assert origin.type.code_hash == ckb.core.type_id_code_hash
         assert origin.type.hash_type == ckb.core.type_id_hash_type
         sender_capacity = origin.capacity
-        accept_capacity = (126 + len(data)) * ckb.core.shannon
+        accept_capacity = (126 + len(data)) * ckb.denomination.ckbytes
         accept_script = script
         accept_typeid = origin.type
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
         tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.inputs.append(ckb.core.CellInput(0, out_point))
@@ -268,17 +268,17 @@
         for cell in itertools.islice(self.livecell(), 255):
             cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
-            if change_capacity >= 61 * ckb.core.shannon:
+            if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
-        assert change_capacity >= 61 * ckb.core.shannon
+        assert change_capacity >= 61 * ckb.denomination.ckbytes
         tx.raw.outputs[1].capacity = change_capacity
         sign_data = bytearray()
         sign_data.extend(tx.raw.hash())
         for witness in tx.witnesses:
             sign_data.extend(len(witness).to_bytes(8, 'little'))
             sign_data.extend(witness)
         sign_data = ckb.core.hash(sign_data)
@@ -286,15 +286,15 @@
         tx.witnesses[0] = ckb.core.WitnessArgs(sign, None, None).molecule()
         WalletTransactionAnalyzer(tx).analyze()
         hash = ckb.rpc.send_transaction(tx.json(), 'passthrough')
         return bytearray.fromhex(hash[2:])
 
     def dao_deposit(self, capacity: int):
         # https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0023-dao-deposit-withdraw/0023-dao-deposit-withdraw.md#deposit
-        assert capacity >= 102 * ckb.core.shannon
+        assert capacity >= 102 * ckb.denomination.ckbytes
         assert self.capacity() > capacity
         sender_capacity = 0
         accept_capacity = capacity
         accept_script = self.script
         accept_typeid = ckb.core.Script(
             ckb.config.current.script.dao.code_hash,
             ckb.config.current.script.dao.hash_type,
@@ -313,17 +313,17 @@
         for cell in itertools.islice(self.livecell(), 256):
             cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
-            if change_capacity >= 61 * ckb.core.shannon:
+            if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
-        assert change_capacity >= 61 * ckb.core.shannon
+        assert change_capacity >= 61 * ckb.denomination.ckbytes
         tx.raw.outputs[1].capacity = change_capacity
         sign_data = bytearray()
         sign_data.extend(tx.raw.hash())
         for witness in tx.witnesses:
             sign_data.extend(len(witness).to_bytes(8, 'little'))
             sign_data.extend(witness)
         sign_data = ckb.core.hash(sign_data)
@@ -360,17 +360,17 @@
         for cell in itertools.islice(self.livecell(), 255):
             cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
-            if change_capacity >= 61 * ckb.core.shannon:
+            if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
-        assert change_capacity >= 61 * ckb.core.shannon
+        assert change_capacity >= 61 * ckb.denomination.ckbytes
         tx.raw.outputs[1].capacity = change_capacity
         sign_data = bytearray()
         sign_data.extend(tx.raw.hash())
         for witness in tx.witnesses:
             sign_data.extend(len(witness).to_bytes(8, 'little'))
             sign_data.extend(witness)
         sign_data = ckb.core.hash(sign_data)
@@ -402,15 +402,15 @@
         extract_since_delay = math.ceil((prepare_block_epoch_float - deposit_block_epoch_float) / 180) * 180
         extract_since_epoch = ckb.core.epoch_encode(
             deposit_block_epoch[0] + extract_since_delay,
             deposit_block_epoch[1],
             deposit_block_epoch[2],
         )
         extract_since = 0x2000000000000000 + extract_since_epoch
-        occupy_capacity = 102 * ckb.core.shannon
+        occupy_capacity = 102 * ckb.denomination.ckbytes
         sender_capacity = (origin.capacity - occupy_capacity) * prepare_dao_ar // deposit_dao_ar + occupy_capacity
         accept_capacity = 0
         accept_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
         tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.dao.cell_dep))
         tx.raw.header_deps.append(deposit_block_hash)
```

### Comparing `pyckb-0.1.8/pyckb.egg-info/PKG-INFO` & `pyckb-0.1.9/pyckb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyckb
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for CKB
 Author-email: Mohanson <mohanson@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Mohanson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyckb-0.1.8/test/test_core.py` & `pyckb-0.1.9/test/test_core.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.8/test/test_ecdsa.py` & `pyckb-0.1.9/test/test_ecdsa.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.8/test/test_rpc.py` & `pyckb-0.1.9/test/test_rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,13 +23,17 @@
         ckb.config.current.script.secp256k1_blake160.hash_type,
         bytearray.fromhex(args)
     )
     search = {'script': script.json(), 'script_type': 'lock'}
     assert int(ckb.rpc.get_cells_capacity(search)['capacity'], 16) >= 0
 
 
+def test_get_current_epoch():
+    assert int(ckb.rpc.get_current_epoch()['number'], 0) >= 0
+
+
 def test_get_indexer_tip():
     assert int(ckb.rpc.get_indexer_tip()['block_number'], 16) >= 0
 
 
 def test_get_tip_block_numner():
     assert int(ckb.rpc.get_tip_block_number(), 16) >= 0
```

### Comparing `pyckb-0.1.8/test/test_wallet.py` & `pyckb-0.1.9/test/test_wallet.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def test_wallet_transfer():
     ckb.config.upgrade('http://127.0.0.1:8114')
     ckb.config.current = ckb.config.develop
     user = ckb.wallet.Wallet(1)
     mate = ckb.wallet.Wallet(2)
-    capacity = 100 * ckb.core.shannon
+    capacity = 100 * ckb.denomination.ckbytes
     capacity_old = mate.capacity()
     hash = user.transfer(mate.script, capacity)
     ckb.rpc.wait(f'0x{hash.hex()}')
     capacity_new = mate.capacity()
     assert capacity_new - capacity_old == capacity
     hash = mate.transfer_all(user.script)
     ckb.rpc.wait(f'0x{hash.hex()}')
@@ -42,11 +42,11 @@
     ckb.rpc.wait(f'0x{hash.hex()}')
 
 
 def test_wallet_dao():
     ckb.config.upgrade('http://127.0.0.1:8114')
     ckb.config.current = ckb.config.develop
     user = ckb.wallet.Wallet(1)
-    hash = user.dao_deposit(200 * ckb.core.shannon)
+    hash = user.dao_deposit(200 * ckb.denomination.ckbytes)
     ckb.rpc.wait(f'0x{hash.hex()}')
     hash = user.dao_prepare(ckb.core.OutPoint(hash, 0))
     ckb.rpc.wait(f'0x{hash.hex()}')
```

