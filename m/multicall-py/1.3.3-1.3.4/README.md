# Comparing `tmp/multicall-py-1.3.3.tar.gz` & `tmp/multicall-py-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicall-py-1.3.3.tar", last modified: Tue Apr  9 03:26:32 2024, max compression
+gzip compressed data, was "multicall-py-1.3.4.tar", last modified: Mon Apr 29 00:53:15 2024, max compression
```

## Comparing `multicall-py-1.3.3.tar` & `multicall-py-1.3.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.435272 multicall-py-1.3.3/
--rw-r--r--   0 jsvisa     (501) staff       (20)     1064 2023-03-16 12:45:05.000000 multicall-py-1.3.3/LICENSE
--rw-r--r--   0 jsvisa     (501) staff       (20)       30 2023-03-16 12:45:05.000000 multicall-py-1.3.3/MANIFEST.in
--rw-r--r--   0 jsvisa     (501) staff       (20)     3328 2024-04-09 03:26:32.435006 multicall-py-1.3.3/PKG-INFO
--rw-r--r--   0 jsvisa     (501) staff       (20)     2227 2023-08-28 11:12:52.000000 multicall-py-1.3.3/README.md
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.427590 multicall-py-1.3.3/multicall/
--rw-r--r--   0 jsvisa     (501) staff       (20)      211 2024-04-09 03:24:37.000000 multicall-py-1.3.3/multicall/__init__.py
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.429871 multicall-py-1.3.3/multicall/__pycache__/
--rw-r--r--   0 jsvisa     (501) staff       (20)      378 2023-10-31 02:07:39.000000 multicall-py-1.3.3/multicall/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     1791 2023-10-31 02:07:39.000000 multicall-py-1.3.3/multicall/__pycache__/balance_call.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     2379 2023-10-31 02:07:39.000000 multicall-py-1.3.3/multicall/__pycache__/call.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     3672 2023-08-29 08:59:55.000000 multicall-py-1.3.3/multicall/__pycache__/eth_decode.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     4878 2023-08-29 08:59:55.000000 multicall-py-1.3.3/multicall/__pycache__/multicall.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     3453 2023-10-31 02:07:39.000000 multicall-py-1.3.3/multicall/__pycache__/signature.cpython-310.pyc
--rw-r--r--   0 jsvisa     (501) staff       (20)     1638 2023-10-31 02:03:51.000000 multicall-py-1.3.3/multicall/balance_call.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     2572 2023-09-12 08:34:46.000000 multicall-py-1.3.3/multicall/call.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3862 2023-09-12 08:15:04.000000 multicall-py-1.3.3/multicall/eth_decode.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     5009 2024-04-09 03:24:28.000000 multicall-py-1.3.3/multicall/multicall.py
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.432093 multicall-py-1.3.3/multicall/service/
--rw-r--r--   0 jsvisa     (501) staff       (20)      276 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/__init__.py
--rw-r--r--   0 jsvisa     (501) staff       (20)      708 2023-09-14 03:09:22.000000 multicall-py-1.3.3/multicall/service/base_token_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     4257 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/erc1155_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     2321 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/erc20_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3033 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/erc721_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     2933 2023-09-14 03:08:16.000000 multicall-py-1.3.3/multicall/service/ether_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3668 2023-03-16 12:45:05.000000 multicall-py-1.3.3/multicall/service/token_service.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3726 2023-09-12 09:45:50.000000 multicall-py-1.3.3/multicall/signature.py
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.433677 multicall-py-1.3.3/multicall_py.egg-info/
--rw-r--r--   0 jsvisa     (501) staff       (20)     3328 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/PKG-INFO
--rw-r--r--   0 jsvisa     (501) staff       (20)      936 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/SOURCES.txt
--rw-r--r--   0 jsvisa     (501) staff       (20)        1 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/dependency_links.txt
--rw-r--r--   0 jsvisa     (501) staff       (20)       24 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/requires.txt
--rw-r--r--   0 jsvisa     (501) staff       (20)       10 2024-04-09 03:26:32.000000 multicall-py-1.3.3/multicall_py.egg-info/top_level.txt
--rw-r--r--   0 jsvisa     (501) staff       (20)       38 2024-04-09 03:26:32.435499 multicall-py-1.3.3/setup.cfg
--rw-r--r--   0 jsvisa     (501) staff       (20)     1470 2024-04-09 03:24:44.000000 multicall-py-1.3.3/setup.py
-drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-09 03:26:32.434490 multicall-py-1.3.3/tests/
--rw-r--r--   0 jsvisa     (501) staff       (20)    16859 2023-09-08 03:13:01.000000 multicall-py-1.3.3/tests/test_eth_decode.py
--rw-r--r--   0 jsvisa     (501) staff       (20)     3080 2023-09-12 09:45:50.000000 multicall-py-1.3.3/tests/test_signature.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-29 00:53:15.740743 multicall-py-1.3.4/
+-rw-r--r--   0 jsvisa     (501) staff       (20)     1064 2023-03-16 12:45:05.000000 multicall-py-1.3.4/LICENSE
+-rw-r--r--   0 jsvisa     (501) staff       (20)       30 2023-03-16 12:45:05.000000 multicall-py-1.3.4/MANIFEST.in
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3440 2024-04-29 00:53:15.740608 multicall-py-1.3.4/PKG-INFO
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2227 2023-08-28 11:12:52.000000 multicall-py-1.3.4/README.md
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-29 00:53:15.737956 multicall-py-1.3.4/multicall/
+-rw-r--r--   0 jsvisa     (501) staff       (20)      211 2024-04-29 00:52:23.000000 multicall-py-1.3.4/multicall/__init__.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-29 00:53:15.738703 multicall-py-1.3.4/multicall/__pycache__/
+-rw-r--r--   0 jsvisa     (501) staff       (20)      378 2024-04-29 00:47:36.000000 multicall-py-1.3.4/multicall/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     1791 2023-10-31 02:07:39.000000 multicall-py-1.3.4/multicall/__pycache__/balance_call.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2379 2023-10-31 02:07:39.000000 multicall-py-1.3.4/multicall/__pycache__/call.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     5077 2024-04-29 00:49:29.000000 multicall-py-1.3.4/multicall/__pycache__/eth_decode.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     4842 2024-04-29 00:47:36.000000 multicall-py-1.3.4/multicall/__pycache__/multicall.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3453 2023-10-31 02:07:39.000000 multicall-py-1.3.4/multicall/__pycache__/signature.cpython-310.pyc
+-rw-r--r--   0 jsvisa     (501) staff       (20)     1638 2023-10-31 02:03:51.000000 multicall-py-1.3.4/multicall/balance_call.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2572 2023-09-12 08:34:46.000000 multicall-py-1.3.4/multicall/call.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     5574 2024-04-29 00:51:07.000000 multicall-py-1.3.4/multicall/eth_decode.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     5009 2024-04-09 03:24:28.000000 multicall-py-1.3.4/multicall/multicall.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-29 00:53:15.739549 multicall-py-1.3.4/multicall/service/
+-rw-r--r--   0 jsvisa     (501) staff       (20)      276 2023-03-16 12:45:05.000000 multicall-py-1.3.4/multicall/service/__init__.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)      708 2023-09-14 03:09:22.000000 multicall-py-1.3.4/multicall/service/base_token_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     4257 2023-03-16 12:45:05.000000 multicall-py-1.3.4/multicall/service/erc1155_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2321 2023-03-16 12:45:05.000000 multicall-py-1.3.4/multicall/service/erc20_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3033 2023-03-16 12:45:05.000000 multicall-py-1.3.4/multicall/service/erc721_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     2933 2023-09-14 03:08:16.000000 multicall-py-1.3.4/multicall/service/ether_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3668 2023-03-16 12:45:05.000000 multicall-py-1.3.4/multicall/service/token_service.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3726 2023-09-12 09:45:50.000000 multicall-py-1.3.4/multicall/signature.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-29 00:53:15.740141 multicall-py-1.3.4/multicall_py.egg-info/
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3440 2024-04-29 00:53:15.000000 multicall-py-1.3.4/multicall_py.egg-info/PKG-INFO
+-rw-r--r--   0 jsvisa     (501) staff       (20)      936 2024-04-29 00:53:15.000000 multicall-py-1.3.4/multicall_py.egg-info/SOURCES.txt
+-rw-r--r--   0 jsvisa     (501) staff       (20)        1 2024-04-29 00:53:15.000000 multicall-py-1.3.4/multicall_py.egg-info/dependency_links.txt
+-rw-r--r--   0 jsvisa     (501) staff       (20)       24 2024-04-29 00:53:15.000000 multicall-py-1.3.4/multicall_py.egg-info/requires.txt
+-rw-r--r--   0 jsvisa     (501) staff       (20)       10 2024-04-29 00:53:15.000000 multicall-py-1.3.4/multicall_py.egg-info/top_level.txt
+-rw-r--r--   0 jsvisa     (501) staff       (20)       38 2024-04-29 00:53:15.740789 multicall-py-1.3.4/setup.cfg
+-rw-r--r--   0 jsvisa     (501) staff       (20)     1580 2024-04-29 00:52:20.000000 multicall-py-1.3.4/setup.py
+drwxr-xr-x   0 jsvisa     (501) staff       (20)        0 2024-04-29 00:53:15.740432 multicall-py-1.3.4/tests/
+-rw-r--r--   0 jsvisa     (501) staff       (20)    16859 2023-09-08 03:13:01.000000 multicall-py-1.3.4/tests/test_eth_decode.py
+-rw-r--r--   0 jsvisa     (501) staff       (20)     3080 2023-09-12 09:45:50.000000 multicall-py-1.3.4/tests/test_signature.py
```

### Comparing `multicall-py-1.3.3/LICENSE` & `multicall-py-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/PKG-INFO` & `multicall-py-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: multicall-py
-Version: 1.3.3
+Version: 1.3.4
 Summary: Ethereum multiple contract/rpc calls
 Home-page: https://github.com/jsvisa/multicall.py
 Author: Wenbiao Zheng
 Author-email: delweng@gmail.com
 License: MIT
-Keywords: ethereum jsonrpc contract
+Keywords: ethereum jsonrpc contract multicall
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Multicall
```

### Comparing `multicall-py-1.3.3/README.md` & `multicall-py-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/__pycache__/balance_call.cpython-310.pyc` & `multicall-py-1.3.4/multicall/__pycache__/balance_call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/__pycache__/call.cpython-310.pyc` & `multicall-py-1.3.4/multicall/__pycache__/call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/__pycache__/multicall.cpython-310.pyc` & `multicall-py-1.3.4/multicall/__pycache__/multicall.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Aug 28 11:13:06 2023 UTC, .py size: 5058 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4281 ec64 c213 0000  o.......B..d....
+00000000: 6f0d 0d0a 0000 0000 ecb4 1466 9113 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a06 6400 6403 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6404 6c06 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
@@ -61,245 +61,243 @@
 000003c0: 1665 0f65 0e19 0064 1165 0f65 0e19 0066  .e.e...d.e.e...f
 000003d0: 0464 1764 1884 045a 1264 0a65 1364 0f65  .d.d...Z.d.e.d.e
 000003e0: 0d64 1165 1465 0f64 0164 0166 0319 0066  .d.e.e.d.d.f...f
 000003f0: 0664 1964 1a84 045a 1564 0153 0029 1dda  .d.d...Z.d.S.)..
 00000400: 094d 756c 7469 6361 6c6c 4eda 0c70 726f  .MulticallN..pro
 00000410: 7669 6465 725f 7572 69da 066c 6f67 6765  vider_uri..logge
 00000420: 72da 0773 6573 7369 6f6e 6304 0000 0000  r..sessionc.....
-00000430: 0000 0000 0000 0006 0000 0007 0000 0043  ...............C
-00000440: 0000 0073 6e00 0000 7c01 7c00 5f00 7c03  ...sn...|.|._.|.
-00000450: 6400 7500 722a 7401 6401 6402 6700 6403  d.u.r*t.d.d.g.d.
-00000460: a201 6404 6405 6702 6406 6407 8d05 7d04  ..d.d.g.d.d...}.
-00000470: 7402 6a03 6a04 7c04 6408 8d01 7d05 7405  t.j.j.|.d...}.t.
-00000480: 8300 7d03 7c03 a006 6409 7c05 a102 0100  ..}.|...d.|.....
-00000490: 7c03 a006 640a 7c05 a102 0100 7c03 7c00  |...d.|.....|.|.
-000004a0: 5f07 7c02 7033 7408 a009 740a a101 7c00  _.|.p3t...t...|.
-000004b0: 5f0b 6400 5300 290b 4ee9 0300 0000 e902  _.d.S.).N.......
-000004c0: 0000 0029 0569 ad01 0000 69f4 0100 0069  ...).i....i....i
-000004d0: f601 0000 69f7 0100 0069 f801 0000 da04  ....i....i......
-000004e0: 504f 5354 da03 4745 5446 2905 da05 746f  POST..GETF)...to
-000004f0: 7461 6cda 0e62 6163 6b6f 6666 5f66 6163  tal..backoff_fac
-00000500: 746f 72da 1073 7461 7475 735f 666f 7263  tor..status_forc
-00000510: 656c 6973 74da 0f61 6c6c 6f77 6564 5f6d  elist..allowed_m
-00000520: 6574 686f 6473 da1a 7265 7370 6563 745f  ethods..respect_
-00000530: 7265 7472 795f 6166 7465 725f 6865 6164  retry_after_head
-00000540: 6572 2901 da0b 6d61 785f 7265 7472 6965  er)...max_retrie
-00000550: 737a 0768 7474 703a 2f2f 7a08 6874 7470  sz.http://z.http
-00000560: 733a 2f2f 290c 7221 0000 0072 0400 0000  s://).r!...r....
-00000570: da08 7265 7175 6573 7473 da08 6164 6170  ..requests..adap
-00000580: 7465 7273 da0b 4854 5450 4164 6170 7465  ters..HTTPAdapte
-00000590: 7272 0500 0000 da05 6d6f 756e 7472 2300  rr......mountr#.
-000005a0: 0000 da07 6c6f 6767 696e 67da 0967 6574  ....logging..get
-000005b0: 4c6f 6767 6572 da08 5f5f 6e61 6d65 5f5f  Logger..__name__
-000005c0: 7222 0000 0029 06da 0473 656c 6672 2100  r"...)...selfr!.
-000005d0: 0000 7222 0000 0072 2300 0000 da05 7265  ..r"...r#.....re
-000005e0: 7472 79da 0761 6461 7074 6572 721d 0000  try..adapterr...
-000005f0: 0072 1d00 0000 721e 0000 00da 085f 5f69  .r....r......__i
-00000600: 6e69 745f 5f1b 0000 0073 1e00 0000 0606  nit__....s......
-00000610: 0801 0201 0201 0201 0601 0601 0201 06fb  ................
-00000620: 0e07 0601 0c01 0c01 0602 1401 7a12 4d75  ............z.Mu
-00000630: 6c74 6963 616c 6c2e 5f5f 696e 6974 5f5f  lticall.__init__
-00000640: 46e9 6400 0000 720f 0000 00da 0563 616c  F.d...r......cal
-00000650: 6c73 da07 6173 5f64 6963 74da 0c69 676e  ls..as_dict..ign
-00000660: 6f72 655f 6572 726f 72da 0862 6c6f 636b  ore_error..block
-00000670: 5f69 64da 0967 6173 5f6c 696d 6974 da0a  _id..gas_limit..
-00000680: 6261 7463 685f 7369 7a65 da0b 6d61 785f  batch_size..max_
-00000690: 776f 726b 6572 7372 1200 0000 6308 0000  workersr....c...
-000006a0: 0000 0000 0000 0000 000e 0000 000a 0000  ................
-000006b0: 0003 0000 0073 2601 0000 7c07 6401 6b04  .....s&...|.d.k.
-000006c0: 7308 4a00 6402 8301 8201 7400 6403 6404  s.J.d.....t.d.d.
-000006d0: 8400 7c01 4400 8301 8301 7d08 7401 7c08  ..|.D.....}.t.|.
-000006e0: 8301 7401 7c01 8301 6b03 721d 7402 6405  ..t.|...k.r.t.d.
-000006f0: 8301 8201 7403 8300 8900 7c07 6406 6b02  ....t.....|.d.k.
-00000700: 723f 7c00 a004 7c01 7c06 a102 4400 5d13  r?|...|.|...D.].
-00000710: 7d09 7c00 a005 7c09 7c04 7c05 a103 7d0a  }.|...|.|.|...}.
-00000720: 8800 a006 6407 6408 8400 7c0a 4400 8301  ....d.d...|.D...
-00000730: a101 0100 712a 6e3e 7407 7c07 8301 8f32  ....q*n>t.|....2
-00000740: 7d0b 6700 7d0c 7c00 a004 7c01 7c06 a102  }.g.}.|...|.|...
-00000750: 4400 5d0e 7d09 7c0c a008 7c0b a009 7c00  D.].}.|...|...|.
-00000760: 6a05 7c09 7c04 7c05 a104 a101 0100 714c  j.|.|.|.......qL
-00000770: 740a 7c0c 8301 4400 5d0e 7d0d 8800 a006  t.|...D.].}.....
-00000780: 6409 6408 8400 7c0d a00b a100 4400 8301  d.d...|.....D...
-00000790: a101 0100 715f 5700 6400 0400 0400 8303  ....q_W.d.......
-000007a0: 0100 6e08 3100 7378 7701 0100 0100 0100  ..n.1.sxw.......
-000007b0: 5900 0100 7c02 7289 8700 8701 6602 640a  Y...|.r.....f.d.
-000007c0: 6408 8408 7c01 4400 8301 5300 8700 8701  d...|.D...S.....
-000007d0: 6602 640b 640c 8408 7c01 4400 8301 5300  f.d.d...|.D...S.
-000007e0: 290d 4e72 0100 0000 7a20 6d61 785f 776f  ).Nr....z max_wo
-000007f0: 726b 6572 7320 6d75 7374 2062 6520 6e6f  rkers must be no
-00000800: 7420 6e65 6761 7469 7665 6301 0000 0000  t negativec.....
-00000810: 0000 0000 0000 0002 0000 0002 0000 0073  ...............s
-00000820: 0000 0073 1600 0000 8100 7c00 5d06 7d01  ...s......|.].}.
-00000830: 7c01 6a00 5600 0100 7102 6400 5300 2901  |.j.V...q.d.S.).
-00000840: 4e29 01da 0a72 6571 7565 7374 5f69 6429  N)...request_id)
-00000850: 02da 022e 30da 0463 616c 6c72 1d00 0000  ....0..callr....
-00000860: 721d 0000 0072 1e00 0000 da09 3c67 656e  r....r......<gen
-00000870: 6578 7072 3e3e 0000 0073 0400 0000 0280  expr>>...s......
-00000880: 1400 7a20 4d75 6c74 6963 616c 6c2e 6167  ..z Multicall.ag
-00000890: 672e 3c6c 6f63 616c 733e 2e3c 6765 6e65  g.<locals>.<gene
-000008a0: 7870 723e 7a29 7265 7175 6573 745f 6964  xpr>z)request_id
-000008b0: 2073 686f 756c 6420 6265 2075 6e69 7175   should be uniqu
-000008c0: 6520 666f 7220 6561 6368 2043 616c 6c72  e for each Callr
-000008d0: 0f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000008e0: 0002 0000 0004 0000 0053 0000 00f3 1600  .........S......
-000008f0: 0000 6900 7c00 5d07 7d01 7c01 6400 1900  ..i.|.].}.|.d...
-00000900: 7c01 9302 7102 5300 a901 da02 6964 721d  |...q.S.....idr.
-00000910: 0000 00a9 0272 4200 0000 da01 6572 1d00  .....rB.....er..
-00000920: 0000 721d 0000 0072 1e00 0000 da0a 3c64  ..r....r......<d
-00000930: 6963 7463 6f6d 703e 4600 0000 f302 0000  ictcomp>F.......
-00000940: 0016 007a 214d 756c 7469 6361 6c6c 2e61  ...z!Multicall.a
-00000950: 6767 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  gg.<locals>.<dic
-00000960: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
-00000970: 0000 0002 0000 0004 0000 0053 0000 0072  ...........S...r
-00000980: 4500 0000 7246 0000 0072 1d00 0000 7248  E...rF...r....rH
-00000990: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-000009a0: 0000 724a 0000 0052 0000 0072 4b00 0000  ..rJ...R...rK...
-000009b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000009c0: 0007 0000 0013 0000 0073 2200 0000 6900  .........s"...i.
-000009d0: 7c00 5d0d 7d01 7c01 6a00 7c01 a001 8800  |.].}.|.j.|.....
-000009e0: 7c01 6a00 1900 8801 a102 9302 7102 5300  |.j.........q.S.
-000009f0: 721d 0000 00a9 0272 4100 0000 da06 6465  r......rA.....de
-00000a00: 636f 6465 a902 7242 0000 00da 0163 a902  code..rB.....c..
-00000a10: 5a0a 6964 5f6f 7574 7075 7473 723c 0000  Z.id_outputsr<..
-00000a20: 0072 1d00 0000 721e 0000 0072 4a00 0000  .r....r....rJ...
-00000a30: 5500 0000 7308 0000 0006 0002 0214 ff06  U...s...........
-00000a40: ff63 0100 0000 0000 0000 0000 0000 0200  .c..............
-00000a50: 0000 0700 0000 1300 0000 7326 0000 0067  ..........s&...g
-00000a60: 007c 005d 0f7d 017c 016a 007c 01a0 0188  .|.].}.|.j.|....
-00000a70: 007c 016a 0019 0088 01a1 0264 009c 0291  .|.j.......d....
-00000a80: 0271 0253 0029 0129 0272 4100 0000 da06  .q.S.).).rA.....
-00000a90: 7265 7375 6c74 724c 0000 0072 4e00 0000  resultrL...rN...
-00000aa0: 7250 0000 0072 1d00 0000 721e 0000 00da  rP...r....r.....
-00000ab0: 0a3c 6c69 7374 636f 6d70 3e5a 0000 0073  .<listcomp>Z...s
-00000ac0: 0c00 0000 0600 0205 04fd 1001 04fe 06ff  ................
-00000ad0: 7a21 4d75 6c74 6963 616c 6c2e 6167 672e  z!Multicall.agg.
-00000ae0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000af0: 6d70 3e29 0cda 0373 6574 da03 6c65 6eda  mp>)...set..len.
-00000b00: 0a56 616c 7565 4572 726f 72da 0464 6963  .ValueError..dic
-00000b10: 74da 105f 7061 7274 6974 696f 6e5f 6361  t.._partition_ca
-00000b20: 6c6c 73da 0f6d 616b 655f 6261 7463 685f  lls..make_batch_
-00000b30: 6361 6c6c da06 7570 6461 7465 7202 0000  call..updater...
-00000b40: 00da 0661 7070 656e 64da 0673 7562 6d69  ...append..submi
-00000b50: 7472 0300 0000 7251 0000 0029 0e72 3500  tr....rQ...).r5.
-00000b60: 0000 723a 0000 0072 3b00 0000 723c 0000  ..r:...r;...r<..
-00000b70: 0072 3d00 0000 723e 0000 0072 3f00 0000  .r=...r>...r?...
-00000b80: 7240 0000 005a 0b72 6571 7565 7374 5f69  r@...Z.request_i
-00000b90: 6473 da05 6261 7463 68da 076f 7574 7075  ds..batch..outpu
-00000ba0: 7473 da08 6578 6563 7574 6f72 da07 6675  ts..executor..fu
-00000bb0: 7475 7265 73da 0666 7574 7572 6572 1d00  tures..futurer..
-00000bc0: 0000 7250 0000 0072 1e00 0000 da03 6167  ..rP...r......ag
-00000bd0: 6732 0000 0073 3a00 0000 100a 1202 1001  g2...s:.........
-00000be0: 0801 0602 0801 1001 0e01 1601 02fe 0a04  ................
-00000bf0: 0401 1001 0401 0401 0a01 02ff 06ff 0c06  ................
-00000c00: 1a01 02ff 1cf7 040c 0c01 0202 06fe 0c05  ................
-00000c10: 0205 06fb 7a0d 4d75 6c74 6963 616c 6c2e  ....z.Multicall.
-00000c20: 6167 6763 0400 0000 0000 0000 0000 0000  aggc............
-00000c30: 0600 0000 0600 0000 0300 0000 7350 0000  ............sP..
-00000c40: 0087 0087 0166 0264 0164 0284 087c 0144  .....f.d.d...|.D
-00000c50: 0083 017d 047c 00a0 007c 04a1 017d 0574  ...}.|...|...}.t
-00000c60: 017c 0583 0174 017c 0483 016b 0372 2674  .|...t.|...k.r&t
-00000c70: 0264 0374 017c 0483 019b 0064 0474 017c  .d.t.|.....d.t.|
-00000c80: 0583 019b 0064 059d 0583 0182 017c 0553  .....d.......|.S
-00000c90: 0029 064e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00000ca0: 0002 0000 0006 0000 0013 0000 0073 1800  .............s..
-00000cb0: 0000 6700 7c00 5d08 7d01 7c01 8800 8801  ..g.|.].}.|.....
-00000cc0: 6400 8d02 9102 7102 5300 2901 a902 723d  d.....q.S.)...r=
-00000cd0: 0000 0072 3e00 0000 721d 0000 0072 4e00  ...r>...r....rN.
-00000ce0: 0000 7262 0000 0072 1d00 0000 721e 0000  ..rb...r....r...
-00000cf0: 0072 5200 0000 6800 0000 7302 0000 0018  .rR...h...s.....
-00000d00: 007a 2d4d 756c 7469 6361 6c6c 2e6d 616b  .z-Multicall.mak
-00000d10: 655f 6261 7463 685f 6361 6c6c 2e3c 6c6f  e_batch_call.<lo
-00000d20: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00000d30: 7a0e 6d75 6c74 6963 616c 6c20 6861 7320  z.multicall has 
-00000d40: 7a13 2072 6571 7565 7374 732c 2062 7574  z. requests, but
-00000d50: 2067 6f74 207a 0a20 7265 7370 6f6e 7365   got z. response
-00000d60: 7329 03da 126d 616b 655f 6261 7463 685f  s)...make_batch_
-00000d70: 7265 7175 6573 7472 5400 0000 7255 0000  requestrT...rU..
-00000d80: 0029 0672 3500 0000 723a 0000 0072 3d00  .).r5...r:...r=.
-00000d90: 0000 723e 0000 0072 2e00 0000 725d 0000  ..r>...r....r]..
-00000da0: 0072 1d00 0000 7262 0000 0072 1e00 0000  .r....rb...r....
-00000db0: 7258 0000 0062 0000 0073 1200 0000 1406  rX...b...s......
-00000dc0: 0a01 1001 0201 0c01 0601 06ff 04ff 0404  ................
-00000dd0: 7a19 4d75 6c74 6963 616c 6c2e 6d61 6b65  z.Multicall.make
-00000de0: 5f62 6174 6368 5f63 616c 6c72 2e00 0000  _batch_callr....
-00000df0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-00000e00: 0006 0000 0043 0000 0073 8600 0000 7400  .....C...s....t.
-00000e10: 7c01 8301 6401 6b02 7208 6700 5300 7c00  |...d.k.r.g.S.|.
-00000e20: 6a01 a002 6402 7c00 6a03 7c01 a103 0100  j...d.|.j.|.....
-00000e30: 7c00 6a04 6a05 7c00 6a03 7400 7c01 8301  |.j.j.|.j.t.|...
-00000e40: 6403 6b04 721e 7c01 6e03 7c01 6401 1900  d.k.r.|.n.|.d...
-00000e50: 6404 8d02 7d02 7c00 6a01 a002 6405 7c00  d...}.|.j...d.|.
-00000e60: 6a03 7c01 7c02 a104 0100 7406 7c02 6a07  j.|.|.....t.|.j.
-00000e70: 6406 8d01 7d03 7408 7c03 8301 7d04 7400  d...}.t.|...}.t.
-00000e80: 7c01 8301 6403 6b04 7240 7c04 5300 7c04  |...d.k.r@|.S.|.
-00000e90: 6701 5300 2907 4e72 0100 0000 7a29 4d61  g.S.).Nr....z)Ma
-00000ea0: 6b69 6e67 2072 6571 7565 7374 2048 5454  king request HTT
-00000eb0: 502e 2055 5249 3a20 2573 2c20 5265 7175  P. URI: %s, Requ
-00000ec0: 6573 743a 2025 7372 0f00 0000 2901 7214  est: %sr....).r.
-00000ed0: 0000 007a 3947 6574 7469 6e67 2072 6573  ...z9Getting res
-00000ee0: 706f 6e73 6520 4854 5450 2e20 5552 493a  ponse HTTP. URI:
-00000ef0: 2025 732c 2052 6571 7565 7374 3a20 2573   %s, Request: %s
-00000f00: 2c20 5265 7370 6f6e 7365 3a20 2573 2901  , Response: %s).
-00000f10: da04 7465 7874 2909 7254 0000 0072 2200  ..text).rT...r".
-00000f20: 0000 da05 6465 6275 6772 2100 0000 7223  ....debugr!...r#
-00000f30: 0000 00da 0470 6f73 7472 0e00 0000 7264  .....postr....rd
-00000f40: 0000 0072 1f00 0000 2905 7235 0000 0072  ...r....).r5...r
-00000f50: 2e00 0000 da0c 7261 775f 7265 7370 6f6e  ......raw_respon
-00000f60: 7365 da0d 7465 7874 5f72 6573 706f 6e73  se..text_respons
-00000f70: 65da 0972 6573 706f 6e73 6573 721d 0000  e..responsesr...
-00000f80: 0072 1d00 0000 721e 0000 0072 6300 0000  .r....r....rc...
-00000f90: 7100 0000 732c 0000 000c 0104 0106 0202  q...s,..........
-00000fa0: 0104 0102 0104 fd06 0504 0116 0106 fe06  ................
-00000fb0: 0402 0104 0102 0102 0104 fc0c 0608 010c  ................
-00000fc0: 0104 0106 027a 1c4d 756c 7469 6361 6c6c  .....z.Multicall
-00000fd0: 2e6d 616b 655f 6261 7463 685f 7265 7175  .make_batch_requ
-00000fe0: 6573 7463 0300 0000 0000 0000 0000 0000  estc............
-00000ff0: 0500 0000 0400 0000 6300 0000 7352 0000  ........c...sR..
-00001000: 0081 0067 007d 037c 0144 005d 167d 047c  ...g.}.|.D.].}.|
-00001010: 03a0 007c 04a1 0101 007c 0264 016b 0472  ...|.....|.d.k.r
-00001020: 1b74 017c 0383 017c 026b 0572 1b7c 0356  .t.|...|.k.r.|.V
-00001030: 0001 0067 007d 0371 0574 017c 0383 0164  ...g.}.q.t.|...d
-00001040: 016b 0472 277c 0356 0001 0064 0053 0064  .k.r'|.V...d.S.d
-00001050: 0053 0029 024e 7201 0000 0029 0272 5a00  .S.).Nr....).rZ.
-00001060: 0000 7254 0000 0029 0572 3500 0000 723a  ..rT...).r5...r:
-00001070: 0000 0072 3f00 0000 725c 0000 00da 0469  ...r?...r\.....i
-00001080: 7465 6d72 1d00 0000 721d 0000 0072 1e00  temr....r....r..
-00001090: 0000 7257 0000 008b 0000 0073 1600 0000  ..rW.......s....
-000010a0: 0280 0403 0801 0a01 1401 0601 0401 0280  ................
-000010b0: 0c01 0a01 04ff 7a1a 4d75 6c74 6963 616c  ......z.Multical
-000010c0: 6c2e 5f70 6172 7469 7469 6f6e 5f63 616c  l._partition_cal
-000010d0: 6c73 2902 4e4e 2906 4646 4e4e 7239 0000  ls).NN).FFNNr9..
-000010e0: 0072 0f00 0000 2916 7234 0000 00da 0a5f  .r....).r4....._
-000010f0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00001100: 6c6e 616d 655f 5fda 0373 7472 7209 0000  lname__..strr...
-00001110: 0072 3200 0000 da06 4c6f 6767 6572 7205  .r2.....Loggerr.
-00001120: 0000 0072 3800 0000 720d 0000 0072 1000  ...r8...r....r..
-00001130: 0000 da04 626f 6f6c 7208 0000 00da 0369  ....boolr......i
-00001140: 6e74 7207 0000 0072 0600 0000 7261 0000  ntr....r....ra..
-00001150: 0072 5800 0000 7263 0000 0072 0b00 0000  .rX...rc...r....
-00001160: 720a 0000 0072 5700 0000 721d 0000 0072  r....rW...r....r
-00001170: 1d00 0000 721d 0000 0072 1e00 0000 7220  ....r....r....r 
-00001180: 0000 001a 0000 0073 6800 0000 0800 0204  .......sh.......
-00001190: 0201 04fc 0202 02fe 0803 02fd 0604 0afc  ................
-000011a0: 021a 0201 0201 0201 0201 0201 04f8 0602  ................
-000011b0: 02fe 0203 02fd 0204 02fc 0e05 02fb 0606  ................
-000011c0: 02fa 0207 02f9 0208 02f8 0e09 0af7 0233  ...............3
-000011d0: 0201 04fc 0602 02fe 0e03 02fd 0604 02fc  ................
-000011e0: 0605 0afb 1a0f 021a 0201 02ff 0201 02ff  ................
-000011f0: 0c02 0efe 7220 0000 0029 1b72 1400 0000  ....r ...).r....
-00001200: 7232 0000 00da 1263 6f6e 6375 7272 656e  r2.....concurren
-00001210: 742e 6675 7475 7265 7372 0200 0000 7203  t.futuresr....r.
-00001220: 0000 005a 1172 6571 7565 7374 732e 6164  ...Z.requests.ad
-00001230: 6170 7465 7273 722e 0000 005a 1275 726c  aptersr....Z.url
-00001240: 6c69 6233 2e75 7469 6c2e 7265 7472 7972  lib3.util.retryr
-00001250: 0400 0000 7205 0000 00da 0674 7970 696e  ....r......typin
-00001260: 6772 0600 0000 7207 0000 0072 0800 0000  gr....r....r....
-00001270: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00001280: 0c00 0000 da0f 636f 6c6c 6563 7469 6f6e  ......collection
-00001290: 732e 6162 6372 0d00 0000 5a15 6574 685f  s.abcr....Z.eth_
-000012a0: 7574 696c 732e 636f 6e76 6572 7369 6f6e  utils.conversion
-000012b0: 7372 0e00 0000 7243 0000 0072 1000 0000  sr....rC...r....
-000012c0: 726d 0000 0072 1f00 0000 7220 0000 0072  rm...r....r ...r
-000012d0: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
-000012e0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000012f0: 0073 1800 0000 0800 0801 1001 0801 0c01  .s..............
-00001300: 0c01 2401 0c01 0c02 0c02 1a03 120b       ..$...........
+00000430: 0000 0000 0000 0006 0000 0006 0000 0043  ...............C
+00000440: 0000 0073 6800 0000 7c01 7c00 5f00 7c03  ...sh...|.|._.|.
+00000450: 6400 7500 7227 7401 6401 6402 6700 6403  d.u.r't.d.d.g.d.
+00000460: a201 6404 6405 8d04 7d04 7402 6a03 6a04  ..d.d...}.t.j.j.
+00000470: 7c04 6406 8d01 7d05 7405 8300 7d03 7c03  |.d...}.t...}.|.
+00000480: a006 6407 7c05 a102 0100 7c03 a006 6408  ..d.|.....|...d.
+00000490: 7c05 a102 0100 7c03 7c00 5f07 7c02 7030  |.....|.|._.|.p0
+000004a0: 7408 a009 740a a101 7c00 5f0b 6400 5300  t...t...|._.d.S.
+000004b0: 2909 4ee9 0300 0000 e902 0000 0029 0569  ).N..........).i
+000004c0: ad01 0000 69f4 0100 0069 f601 0000 69f7  ....i....i....i.
+000004d0: 0100 0069 f801 0000 4629 04da 0574 6f74  ...i....F)...tot
+000004e0: 616c da0e 6261 636b 6f66 665f 6661 6374  al..backoff_fact
+000004f0: 6f72 da10 7374 6174 7573 5f66 6f72 6365  or..status_force
+00000500: 6c69 7374 da1a 7265 7370 6563 745f 7265  list..respect_re
+00000510: 7472 795f 6166 7465 725f 6865 6164 6572  try_after_header
+00000520: 2901 da0b 6d61 785f 7265 7472 6965 737a  )...max_retriesz
+00000530: 0768 7474 703a 2f2f 7a08 6874 7470 733a  .http://z.https:
+00000540: 2f2f 290c 7221 0000 0072 0400 0000 da08  //).r!...r......
+00000550: 7265 7175 6573 7473 da08 6164 6170 7465  requests..adapte
+00000560: 7273 da0b 4854 5450 4164 6170 7465 7272  rs..HTTPAdapterr
+00000570: 0500 0000 da05 6d6f 756e 7472 2300 0000  ......mountr#...
+00000580: da07 6c6f 6767 696e 67da 0967 6574 4c6f  ..logging..getLo
+00000590: 6767 6572 da08 5f5f 6e61 6d65 5f5f 7222  gger..__name__r"
+000005a0: 0000 0029 06da 0473 656c 6672 2100 0000  ...)...selfr!...
+000005b0: 7222 0000 0072 2300 0000 da05 7265 7472  r"...r#.....retr
+000005c0: 79da 0761 6461 7074 6572 721d 0000 0072  y..adapterr....r
+000005d0: 1d00 0000 721e 0000 00da 085f 5f69 6e69  ....r......__ini
+000005e0: 745f 5f1b 0000 0073 1c00 0000 0606 0801  t__....s........
+000005f0: 0201 0201 0201 0601 0201 06fc 0e06 0601  ................
+00000600: 0c01 0c01 0602 1401 7a12 4d75 6c74 6963  ........z.Multic
+00000610: 616c 6c2e 5f5f 696e 6974 5f5f 46e9 6400  all.__init__F.d.
+00000620: 0000 720f 0000 00da 0563 616c 6c73 da07  ..r......calls..
+00000630: 6173 5f64 6963 74da 0c69 676e 6f72 655f  as_dict..ignore_
+00000640: 6572 726f 72da 0862 6c6f 636b 5f69 64da  error..block_id.
+00000650: 0967 6173 5f6c 696d 6974 da0a 6261 7463  .gas_limit..batc
+00000660: 685f 7369 7a65 da0b 6d61 785f 776f 726b  h_size..max_work
+00000670: 6572 7372 1200 0000 6308 0000 0000 0000  ersr....c.......
+00000680: 0000 0000 000e 0000 000a 0000 0003 0000  ................
+00000690: 0073 2601 0000 7c07 6401 6b04 7308 4a00  .s&...|.d.k.s.J.
+000006a0: 6402 8301 8201 7400 6403 6404 8400 7c01  d.....t.d.d...|.
+000006b0: 4400 8301 8301 7d08 7401 7c08 8301 7401  D.....}.t.|...t.
+000006c0: 7c01 8301 6b03 721d 7402 6405 8301 8201  |...k.r.t.d.....
+000006d0: 7403 8300 8900 7c07 6406 6b02 723f 7c00  t.....|.d.k.r?|.
+000006e0: a004 7c01 7c06 a102 4400 5d13 7d09 7c00  ..|.|...D.].}.|.
+000006f0: a005 7c09 7c04 7c05 a103 7d0a 8800 a006  ..|.|.|...}.....
+00000700: 6407 6408 8400 7c0a 4400 8301 a101 0100  d.d...|.D.......
+00000710: 712a 6e3e 7407 7c07 8301 8f32 7d0b 6700  q*n>t.|....2}.g.
+00000720: 7d0c 7c00 a004 7c01 7c06 a102 4400 5d0e  }.|...|.|...D.].
+00000730: 7d09 7c0c a008 7c0b a009 7c00 6a05 7c09  }.|...|...|.j.|.
+00000740: 7c04 7c05 a104 a101 0100 714c 740a 7c0c  |.|.......qLt.|.
+00000750: 8301 4400 5d0e 7d0d 8800 a006 6409 6408  ..D.].}.....d.d.
+00000760: 8400 7c0d a00b a100 4400 8301 a101 0100  ..|.....D.......
+00000770: 715f 5700 6400 0400 0400 8303 0100 6e08  q_W.d.........n.
+00000780: 3100 7378 7701 0100 0100 0100 5900 0100  1.sxw.......Y...
+00000790: 7c02 7289 8700 8701 6602 640a 6408 8408  |.r.....f.d.d...
+000007a0: 7c01 4400 8301 5300 8700 8701 6602 640b  |.D...S.....f.d.
+000007b0: 640c 8408 7c01 4400 8301 5300 290d 4e72  d...|.D...S.).Nr
+000007c0: 0100 0000 7a20 6d61 785f 776f 726b 6572  ....z max_worker
+000007d0: 7320 6d75 7374 2062 6520 6e6f 7420 6e65  s must be not ne
+000007e0: 6761 7469 7665 6301 0000 0000 0000 0000  gativec.........
+000007f0: 0000 0002 0000 0002 0000 0073 0000 0073  ...........s...s
+00000800: 1600 0000 8100 7c00 5d06 7d01 7c01 6a00  ......|.].}.|.j.
+00000810: 5600 0100 7102 6400 5300 2901 4e29 01da  V...q.d.S.).N)..
+00000820: 0a72 6571 7565 7374 5f69 6429 02da 022e  .request_id)....
+00000830: 30da 0463 616c 6c72 1d00 0000 721d 0000  0..callr....r...
+00000840: 0072 1e00 0000 da09 3c67 656e 6578 7072  .r......<genexpr
+00000850: 3e3d 0000 0073 0400 0000 0280 1400 7a20  >=...s........z 
+00000860: 4d75 6c74 6963 616c 6c2e 6167 672e 3c6c  Multicall.agg.<l
+00000870: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+00000880: 7a29 7265 7175 6573 745f 6964 2073 686f  z)request_id sho
+00000890: 756c 6420 6265 2075 6e69 7175 6520 666f  uld be unique fo
+000008a0: 7220 6561 6368 2043 616c 6c72 0f00 0000  r each Callr....
+000008b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000008c0: 0004 0000 0053 0000 00f3 1600 0000 6900  .....S........i.
+000008d0: 7c00 5d07 7d01 7c01 6400 1900 7c01 9302  |.].}.|.d...|...
+000008e0: 7102 5300 a901 da02 6964 721d 0000 00a9  q.S.....idr.....
+000008f0: 0272 3f00 0000 da01 6572 1d00 0000 721d  .r?.....er....r.
+00000900: 0000 0072 1e00 0000 da0a 3c64 6963 7463  ...r......<dictc
+00000910: 6f6d 703e 4500 0000 f302 0000 0016 007a  omp>E..........z
+00000920: 214d 756c 7469 6361 6c6c 2e61 6767 2e3c  !Multicall.agg.<
+00000930: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+00000940: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
+00000950: 0000 0004 0000 0053 0000 0072 4200 0000  .......S...rB...
+00000960: 7243 0000 0072 1d00 0000 7245 0000 0072  rC...r....rE...r
+00000970: 1d00 0000 721d 0000 0072 1e00 0000 7247  ....r....r....rG
+00000980: 0000 0051 0000 0072 4800 0000 6301 0000  ...Q...rH...c...
+00000990: 0000 0000 0000 0000 0002 0000 0007 0000  ................
+000009a0: 0013 0000 0073 2200 0000 6900 7c00 5d0d  .....s"...i.|.].
+000009b0: 7d01 7c01 6a00 7c01 a001 8800 7c01 6a00  }.|.j.|.....|.j.
+000009c0: 1900 8801 a102 9302 7102 5300 721d 0000  ........q.S.r...
+000009d0: 00a9 0272 3e00 0000 da06 6465 636f 6465  ...r>.....decode
+000009e0: a902 723f 0000 00da 0163 a902 5a0a 6964  ..r?.....c..Z.id
+000009f0: 5f6f 7574 7075 7473 7239 0000 0072 1d00  _outputsr9...r..
+00000a00: 0000 721e 0000 0072 4700 0000 5400 0000  ..r....rG...T...
+00000a10: 7308 0000 0006 0002 0214 ff06 ff63 0100  s............c..
+00000a20: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00000a30: 0000 1300 0000 7326 0000 0067 007c 005d  ......s&...g.|.]
+00000a40: 0f7d 017c 016a 007c 01a0 0188 007c 016a  .}.|.j.|.....|.j
+00000a50: 0019 0088 01a1 0264 009c 0291 0271 0253  .......d.....q.S
+00000a60: 0029 0129 0272 3e00 0000 da06 7265 7375  .).).r>.....resu
+00000a70: 6c74 7249 0000 0072 4b00 0000 724d 0000  ltrI...rK...rM..
+00000a80: 0072 1d00 0000 721e 0000 00da 0a3c 6c69  .r....r......<li
+00000a90: 7374 636f 6d70 3e59 0000 0073 0c00 0000  stcomp>Y...s....
+00000aa0: 0600 0205 04fd 1001 04fe 06ff 7a21 4d75  ............z!Mu
+00000ab0: 6c74 6963 616c 6c2e 6167 672e 3c6c 6f63  lticall.agg.<loc
+00000ac0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
+00000ad0: 0cda 0373 6574 da03 6c65 6eda 0a56 616c  ...set..len..Val
+00000ae0: 7565 4572 726f 72da 0464 6963 74da 105f  ueError..dict.._
+00000af0: 7061 7274 6974 696f 6e5f 6361 6c6c 73da  partition_calls.
+00000b00: 0f6d 616b 655f 6261 7463 685f 6361 6c6c  .make_batch_call
+00000b10: da06 7570 6461 7465 7202 0000 00da 0661  ..updater......a
+00000b20: 7070 656e 64da 0673 7562 6d69 7472 0300  ppend..submitr..
+00000b30: 0000 724e 0000 0029 0e72 3200 0000 7237  ..rN...).r2...r7
+00000b40: 0000 0072 3800 0000 7239 0000 0072 3a00  ...r8...r9...r:.
+00000b50: 0000 723b 0000 0072 3c00 0000 723d 0000  ..r;...r<...r=..
+00000b60: 005a 0b72 6571 7565 7374 5f69 6473 da05  .Z.request_ids..
+00000b70: 6261 7463 68da 076f 7574 7075 7473 da08  batch..outputs..
+00000b80: 6578 6563 7574 6f72 da07 6675 7475 7265  executor..future
+00000b90: 73da 0666 7574 7572 6572 1d00 0000 724d  s..futurer....rM
+00000ba0: 0000 0072 1e00 0000 da03 6167 6731 0000  ...r......agg1..
+00000bb0: 0073 3a00 0000 100a 1202 1001 0801 0602  .s:.............
+00000bc0: 0801 1001 0e01 1601 02fe 0a04 0401 1001  ................
+00000bd0: 0401 0401 0a01 02ff 06ff 0c06 1a01 02ff  ................
+00000be0: 1cf7 040c 0c01 0202 06fe 0c05 0205 06fb  ................
+00000bf0: 7a0d 4d75 6c74 6963 616c 6c2e 6167 6763  z.Multicall.aggc
+00000c00: 0400 0000 0000 0000 0000 0000 0600 0000  ................
+00000c10: 0600 0000 0300 0000 7350 0000 0087 0087  ........sP......
+00000c20: 0166 0264 0164 0284 087c 0144 0083 017d  .f.d.d...|.D...}
+00000c30: 047c 00a0 007c 04a1 017d 0574 017c 0583  .|...|...}.t.|..
+00000c40: 0174 017c 0483 016b 0372 2674 0264 0374  .t.|...k.r&t.d.t
+00000c50: 017c 0483 019b 0064 0474 017c 0583 019b  .|.....d.t.|....
+00000c60: 0064 059d 0583 0182 017c 0553 0029 064e  .d.......|.S.).N
+00000c70: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000c80: 0006 0000 0013 0000 0073 1800 0000 6700  .........s....g.
+00000c90: 7c00 5d08 7d01 7c01 8800 8801 6400 8d02  |.].}.|.....d...
+00000ca0: 9102 7102 5300 2901 a902 723a 0000 0072  ..q.S.)...r:...r
+00000cb0: 3b00 0000 721d 0000 0072 4b00 0000 725f  ;...r....rK...r_
+00000cc0: 0000 0072 1d00 0000 721e 0000 0072 4f00  ...r....r....rO.
+00000cd0: 0000 6700 0000 7302 0000 0018 007a 2d4d  ..g...s......z-M
+00000ce0: 756c 7469 6361 6c6c 2e6d 616b 655f 6261  ulticall.make_ba
+00000cf0: 7463 685f 6361 6c6c 2e3c 6c6f 6361 6c73  tch_call.<locals
+00000d00: 3e2e 3c6c 6973 7463 6f6d 703e 7a0e 6d75  >.<listcomp>z.mu
+00000d10: 6c74 6963 616c 6c20 6861 7320 7a13 2072  lticall has z. r
+00000d20: 6571 7565 7374 732c 2062 7574 2067 6f74  equests, but got
+00000d30: 207a 0a20 7265 7370 6f6e 7365 7329 03da   z. responses)..
+00000d40: 126d 616b 655f 6261 7463 685f 7265 7175  .make_batch_requ
+00000d50: 6573 7472 5100 0000 7252 0000 0029 0672  estrQ...rR...).r
+00000d60: 3200 0000 7237 0000 0072 3a00 0000 723b  2...r7...r:...r;
+00000d70: 0000 0072 2b00 0000 725a 0000 0072 1d00  ...r+...rZ...r..
+00000d80: 0000 725f 0000 0072 1e00 0000 7255 0000  ..r_...r....rU..
+00000d90: 0061 0000 0073 1200 0000 1406 0a01 1001  .a...s..........
+00000da0: 0201 0c01 0601 06ff 04ff 0404 7a19 4d75  ............z.Mu
+00000db0: 6c74 6963 616c 6c2e 6d61 6b65 5f62 6174  lticall.make_bat
+00000dc0: 6368 5f63 616c 6c72 2b00 0000 6302 0000  ch_callr+...c...
+00000dd0: 0000 0000 0000 0000 0005 0000 0006 0000  ................
+00000de0: 0043 0000 0073 8600 0000 7400 7c01 8301  .C...s....t.|...
+00000df0: 6401 6b02 7208 6700 5300 7c00 6a01 a002  d.k.r.g.S.|.j...
+00000e00: 6402 7c00 6a03 7c01 a103 0100 7c00 6a04  d.|.j.|.....|.j.
+00000e10: 6a05 7c00 6a03 7400 7c01 8301 6403 6b04  j.|.j.t.|...d.k.
+00000e20: 721e 7c01 6e03 7c01 6401 1900 6404 8d02  r.|.n.|.d...d...
+00000e30: 7d02 7c00 6a01 a002 6405 7c00 6a03 7c01  }.|.j...d.|.j.|.
+00000e40: 7c02 a104 0100 7406 7c02 6a07 6406 8d01  |.....t.|.j.d...
+00000e50: 7d03 7408 7c03 8301 7d04 7400 7c01 8301  }.t.|...}.t.|...
+00000e60: 6403 6b04 7240 7c04 5300 7c04 6701 5300  d.k.r@|.S.|.g.S.
+00000e70: 2907 4e72 0100 0000 7a29 4d61 6b69 6e67  ).Nr....z)Making
+00000e80: 2072 6571 7565 7374 2048 5454 502e 2055   request HTTP. U
+00000e90: 5249 3a20 2573 2c20 5265 7175 6573 743a  RI: %s, Request:
+00000ea0: 2025 7372 0f00 0000 2901 7214 0000 007a   %sr....).r....z
+00000eb0: 3947 6574 7469 6e67 2072 6573 706f 6e73  9Getting respons
+00000ec0: 6520 4854 5450 2e20 5552 493a 2025 732c  e HTTP. URI: %s,
+00000ed0: 2052 6571 7565 7374 3a20 2573 2c20 5265   Request: %s, Re
+00000ee0: 7370 6f6e 7365 3a20 2573 2901 da04 7465  sponse: %s)...te
+00000ef0: 7874 2909 7251 0000 0072 2200 0000 da05  xt).rQ...r".....
+00000f00: 6465 6275 6772 2100 0000 7223 0000 00da  debugr!...r#....
+00000f10: 0470 6f73 7472 0e00 0000 7261 0000 0072  .postr....ra...r
+00000f20: 1f00 0000 2905 7232 0000 0072 2b00 0000  ....).r2...r+...
+00000f30: da0c 7261 775f 7265 7370 6f6e 7365 da0d  ..raw_response..
+00000f40: 7465 7874 5f72 6573 706f 6e73 65da 0972  text_response..r
+00000f50: 6573 706f 6e73 6573 721d 0000 0072 1d00  esponsesr....r..
+00000f60: 0000 721e 0000 0072 6000 0000 7000 0000  ..r....r`...p...
+00000f70: 732c 0000 000c 0104 0106 0202 0104 0102  s,..............
+00000f80: 0104 fd06 0504 0116 0106 fe06 0402 0104  ................
+00000f90: 0102 0102 0104 fc0c 0608 010c 0104 0106  ................
+00000fa0: 027a 1c4d 756c 7469 6361 6c6c 2e6d 616b  .z.Multicall.mak
+00000fb0: 655f 6261 7463 685f 7265 7175 6573 7463  e_batch_requestc
+00000fc0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00000fd0: 0400 0000 6300 0000 7352 0000 0081 0067  ....c...sR.....g
+00000fe0: 007d 037c 0144 005d 167d 047c 03a0 007c  .}.|.D.].}.|...|
+00000ff0: 04a1 0101 007c 0264 016b 0472 1b74 017c  .....|.d.k.r.t.|
+00001000: 0383 017c 026b 0572 1b7c 0356 0001 0067  ...|.k.r.|.V...g
+00001010: 007d 0371 0574 017c 0383 0164 016b 0472  .}.q.t.|...d.k.r
+00001020: 277c 0356 0001 0064 0053 0064 0053 0029  '|.V...d.S.d.S.)
+00001030: 024e 7201 0000 0029 0272 5700 0000 7251  .Nr....).rW...rQ
+00001040: 0000 0029 0572 3200 0000 7237 0000 0072  ...).r2...r7...r
+00001050: 3c00 0000 7259 0000 00da 0469 7465 6d72  <...rY.....itemr
+00001060: 1d00 0000 721d 0000 0072 1e00 0000 7254  ....r....r....rT
+00001070: 0000 008a 0000 0073 1600 0000 0280 0403  .......s........
+00001080: 0801 0a01 1401 0601 0401 0280 0c01 0a01  ................
+00001090: 04ff 7a1a 4d75 6c74 6963 616c 6c2e 5f70  ..z.Multicall._p
+000010a0: 6172 7469 7469 6f6e 5f63 616c 6c73 2902  artition_calls).
+000010b0: 4e4e 2906 4646 4e4e 7236 0000 0072 0f00  NN).FFNNr6...r..
+000010c0: 0000 2916 7231 0000 00da 0a5f 5f6d 6f64  ..).r1.....__mod
+000010d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000010e0: 655f 5fda 0373 7472 7209 0000 0072 2f00  e__..strr....r/.
+000010f0: 0000 da06 4c6f 6767 6572 7205 0000 0072  ....Loggerr....r
+00001100: 3500 0000 720d 0000 0072 1000 0000 da04  5...r....r......
+00001110: 626f 6f6c 7208 0000 00da 0369 6e74 7207  boolr......intr.
+00001120: 0000 0072 0600 0000 725e 0000 0072 5500  ...r....r^...rU.
+00001130: 0000 7260 0000 0072 0b00 0000 720a 0000  ..r`...r....r...
+00001140: 0072 5400 0000 721d 0000 0072 1d00 0000  .rT...r....r....
+00001150: 721d 0000 0072 1e00 0000 7220 0000 001a  r....r....r ....
+00001160: 0000 0073 6800 0000 0800 0204 0201 04fc  ...sh...........
+00001170: 0202 02fe 0803 02fd 0604 0afc 0219 0201  ................
+00001180: 0201 0201 0201 0201 04f8 0602 02fe 0203  ................
+00001190: 02fd 0204 02fc 0e05 02fb 0606 02fa 0207  ................
+000011a0: 02f9 0208 02f8 0e09 0af7 0233 0201 04fc  ...........3....
+000011b0: 0602 02fe 0e03 02fd 0604 02fc 0605 0afb  ................
+000011c0: 1a0f 021a 0201 02ff 0201 02ff 0c02 0efe  ................
+000011d0: 7220 0000 0029 1b72 1400 0000 722f 0000  r ...).r....r/..
+000011e0: 00da 1263 6f6e 6375 7272 656e 742e 6675  ...concurrent.fu
+000011f0: 7475 7265 7372 0200 0000 7203 0000 005a  turesr....r....Z
+00001200: 1172 6571 7565 7374 732e 6164 6170 7465  .requests.adapte
+00001210: 7273 722b 0000 005a 1275 726c 6c69 6233  rsr+...Z.urllib3
+00001220: 2e75 7469 6c2e 7265 7472 7972 0400 0000  .util.retryr....
+00001230: 7205 0000 00da 0674 7970 696e 6772 0600  r......typingr..
+00001240: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00001250: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00001260: da0f 636f 6c6c 6563 7469 6f6e 732e 6162  ..collections.ab
+00001270: 6372 0d00 0000 5a15 6574 685f 7574 696c  cr....Z.eth_util
+00001280: 732e 636f 6e76 6572 7369 6f6e 7372 0e00  s.conversionsr..
+00001290: 0000 7240 0000 0072 1000 0000 726a 0000  ..r@...r....rj..
+000012a0: 0072 1f00 0000 7220 0000 0072 1d00 0000  .r....r ...r....
+000012b0: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
+000012c0: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
+000012d0: 0000 0800 0801 1001 0801 0c01 0c01 2401  ..............$.
+000012e0: 0c01 0c02 0c02 1a03 120b                 ..........
```

### Comparing `multicall-py-1.3.3/multicall/__pycache__/signature.cpython-310.pyc` & `multicall-py-1.3.4/multicall/__pycache__/signature.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/balance_call.py` & `multicall-py-1.3.4/multicall/balance_call.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/call.py` & `multicall-py-1.3.4/multicall/call.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/eth_decode.py` & `multicall-py-1.3.4/multicall/eth_decode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,62 @@
-from typing import List, Dict, Tuple
+from itertools import chain
+from typing import List, Dict, Tuple, Optional, Any
 from eth_abi.abi import decode
 from eth_utils.abi import collapse_if_tuple
 
 
-def collapse_if_tuple_with_name(abi: Dict) -> str:
+def collapse_if_tuple_with_name(abi: Dict[str, Any], is_event=False) -> str:
     """
     Converts a tuple from a dict to a parenthesized list of its types.
     Copy from eth_utils.abi
 
+    >>> from eth_utils.abi import collapse_if_tuple
     >>> collapse_if_tuple(
     ...     {
     ...         'components': [
     ...             {'name': 'anAddress', 'type': 'address'},
     ...             {'name': 'anInt', 'type': 'uint256'},
     ...             {'name': 'someBytes', 'type': 'bytes'},
     ...         ],
     ...         'type': 'tuple',
     ...     }
     ... )
+    '(address,uint256,bytes)'
+
+    >>> collapse_if_tuple_with_name(
+    ...     {
+    ...         'components': [
+    ...             {'name': 'anAddress', 'type': 'address'},
+    ...             {'name': 'anInt', 'type': 'uint256'},
+    ...             {'name': 'someBytes', 'type': 'bytes'},
+    ...         ],
+    ...         'type': 'tuple',
+    ...     }
+    ... )
     '(address anAddress, uint256 anInt, bytes someBytes)'
     """
     typ = abi["type"]
-    nam = abi.get("name", "?__?")
     if not isinstance(typ, str):
         raise TypeError(
-            f"The 'type' must be a string, but got {type} of type {type(typ)}"
+            "The 'type' must be a string, but got %r of type %s" % (typ, type(typ))
         )
     elif not typ.startswith("tuple"):
-        return f"{typ} {nam}"
+        return "{indexed}{typ} {name}".format(
+            indexed="index " if is_event is True and abi.get("indexed") is True else "",
+            typ=typ,
+            name=abi.get("name", ""),
+        )
 
-    delimited = ", ".join(collapse_if_tuple(c) for c in abi["components"])
+    delimited = ", ".join(collapse_if_tuple_with_name(c) for c in abi["components"])
     # Whatever comes after "tuple" is the array dims.  The ABI spec states that
     # this will have the form "", "[]", or "[k]".
     array_dim = typ[5:]
-    collapsed = "({}){} ".format(delimited, array_dim)
+    collapsed = "({delimited}){array_dim}{name}".format(
+        delimited=delimited, array_dim=array_dim, name=abi.get("name", "")
+    )
 
     return collapsed
 
 
 def zip_if_tuple(abi: Dict, value) -> Dict:
     typ = abi["type"]
     name = abi["name"]
@@ -90,15 +109,15 @@
     parameter = {}
     for idx, value in enumerate(decoded):
         parameter.update(zip_if_tuple(inputs[idx], value))
 
     return func_text, parameter
 
 
-def eth_decode_log(event_abi: Dict, topics: List[str], data):
+def eth_decode_log(event_abi: Dict, topics: List[str], data: str) -> Tuple:
     if "name" not in event_abi or event_abi.get("type") != "event":
         return (None, None)
 
     # rewrite the indexed columns first
     indexed, normal = [], []
     if "inputs" in event_abi:
         for input in event_abi.get("inputs", []):
@@ -108,7 +127,37 @@
                 normal.append(collapse_if_tuple(input))
     indexed_values = decode(
         indexed, bytes(bytearray.fromhex("".join(e[2:] for e in topics[1:])))
     )
     data_values = decode(normal, bytes(bytearray.fromhex(data[2:])))
 
     return indexed_values, data_values
+
+
+def eth_decode_log_as_dict(abi: Dict, topics: List[str], data: str) -> Optional[Dict]:
+    indexed_values, data_values = eth_decode_log(abi, topics, data)
+    if None in (indexed_values, data_values):
+        return None
+
+    indexed_names, data_names = [], []
+    byte_names = []
+    if "inputs" in abi:
+        for _in in abi.get("inputs", []):
+            name = _in["name"]
+            if _in.get("indexed") is True:
+                indexed_names.append(name)
+            else:
+                data_names.append(name)
+            if _in["type"].startswith("byte"):
+                byte_names.append(name)
+
+    parameter = dict(
+        chain(zip(indexed_names, indexed_values), zip(data_names, data_values))
+    )
+    for key in byte_names:
+        val = parameter[key]
+        if isinstance(val, tuple):
+            parameter[key] = tuple([e.hex() for e in val])
+        elif isinstance(val, bytes):
+            parameter[key] = val.hex()
+
+    return parameter
```

### Comparing `multicall-py-1.3.3/multicall/multicall.py` & `multicall-py-1.3.4/multicall/multicall.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/service/base_token_service.py` & `multicall-py-1.3.4/multicall/service/base_token_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/service/erc1155_service.py` & `multicall-py-1.3.4/multicall/service/erc1155_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/service/erc20_service.py` & `multicall-py-1.3.4/multicall/service/erc20_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/service/erc721_service.py` & `multicall-py-1.3.4/multicall/service/erc721_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/service/ether_service.py` & `multicall-py-1.3.4/multicall/service/ether_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/service/token_service.py` & `multicall-py-1.3.4/multicall/service/token_service.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall/signature.py` & `multicall-py-1.3.4/multicall/signature.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/multicall_py.egg-info/PKG-INFO` & `multicall-py-1.3.4/multicall_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: multicall-py
-Version: 1.3.3
+Version: 1.3.4
 Summary: Ethereum multiple contract/rpc calls
 Home-page: https://github.com/jsvisa/multicall.py
 Author: Wenbiao Zheng
 Author-email: delweng@gmail.com
 License: MIT
-Keywords: ethereum jsonrpc contract
+Keywords: ethereum jsonrpc contract multicall
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Multicall
```

### Comparing `multicall-py-1.3.3/multicall_py.egg-info/SOURCES.txt` & `multicall-py-1.3.4/multicall_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/setup.py` & `multicall-py-1.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 setup(
     name="multicall-py",
-    version="1.3.3",
+    version="1.3.4",
     description="Ethereum multiple contract/rpc calls",
     long_description=open(os.path.join(here, "README.md")).read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
@@ -20,18 +20,20 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    keywords="ethereum jsonrpc contract",
+    keywords="ethereum jsonrpc contract multicall",
     author="Wenbiao Zheng",
     author_email="delweng@gmail.com",
     url="https://github.com/jsvisa/multicall.py",
     license="MIT",
     packages=find_packages(include=["multicall"]),
     include_package_data=True,
     python_requires=">=3.6",
```

### Comparing `multicall-py-1.3.3/tests/test_eth_decode.py` & `multicall-py-1.3.4/tests/test_eth_decode.py`

 * *Files identical despite different names*

### Comparing `multicall-py-1.3.3/tests/test_signature.py` & `multicall-py-1.3.4/tests/test_signature.py`

 * *Files identical despite different names*

