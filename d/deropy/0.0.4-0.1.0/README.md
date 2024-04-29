# Comparing `tmp/deropy-0.0.4.tar.gz` & `tmp/deropy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.0.4.tar", last modified: Thu Apr 18 15:06:22 2024, max compression
+gzip compressed data, was "deropy-0.1.0.tar", last modified: Mon Apr 29 09:18:41 2024, max compression
```

## Comparing `deropy-0.0.4.tar` & `deropy-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:22.512145 deropy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-18 15:06:22.512145 deropy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-18 15:06:14.000000 deropy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:22.512145 deropy-0.0.4/deropy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:14.000000 deropy-0.0.4/deropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:22.512145 deropy-0.0.4/deropy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:14.000000 deropy-0.0.4/deropy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-18 15:06:14.000000 deropy-0.0.4/deropy/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 15:06:14.000000 deropy-0.0.4/deropy/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-18 15:06:14.000000 deropy-0.0.4/deropy/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 15:06:14.000000 deropy-0.0.4/deropy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:06:22.512145 deropy-0.0.4/deropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-18 15:06:22.000000 deropy-0.0.4/deropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 15:06:22.000000 deropy-0.0.4/deropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:06:22.000000 deropy-0.0.4/deropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 15:06:22.000000 deropy-0.0.4/deropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 15:06:22.000000 deropy-0.0.4/deropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 15:06:22.000000 deropy-0.0.4/deropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:06:22.512145 deropy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-18 15:06:14.000000 deropy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:41.652305 deropy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-29 09:18:41.652305 deropy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-29 09:18:37.000000 deropy-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:41.640305 deropy-0.1.0/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:41.640305 deropy-0.1.0/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/commands/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:41.644305 deropy-0.1.0/deropy/dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/Smartcontract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/Wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:41.648305 deropy-0.1.0/deropy/dvm/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/AddressRaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/AddressString.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/AssetValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Atoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Blid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/BlockHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/BlockTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Dero.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/DeroValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/HexDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/IsAddressValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Itoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/MapDelete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/MapExists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/MapGet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/MapStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Panic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Scid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/SendAssetToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/SendDeroToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Sha3256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Strlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Substr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/Txid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/UpdateScCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/dvm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-29 09:18:37.000000 deropy-0.1.0/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:41.652305 deropy-0.1.0/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-29 09:18:41.000000 deropy-0.1.0/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-29 09:18:41.000000 deropy-0.1.0/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:18:41.000000 deropy-0.1.0/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 09:18:41.000000 deropy-0.1.0/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 09:18:41.000000 deropy-0.1.0/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 09:18:41.000000 deropy-0.1.0/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:18:41.652305 deropy-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 09:18:37.000000 deropy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:18:41.648305 deropy-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-29 09:18:37.000000 deropy-0.1.0/tests/test_compute_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-29 09:18:37.000000 deropy-0.1.0/tests/test_map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-29 09:18:37.000000 deropy-0.1.0/tests/test_storage_functions.py
```

### Comparing `deropy-0.0.4/PKG-INFO` & `deropy-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.0.4
+Version: 0.1.0
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: click==8.0.4
-Requires-Dist: requests==2.27.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: python-dotenv==0.20.0
 Requires-Dist: InquirerPy==0.3.4
+Requires-Dist: pycryptodome==3.20.0
 
 # DEROPY
 
 Deropy is a toolbox for creating, managing and testing DERO smart contracts.
 
 # Roadmap
 
@@ -47,47 +48,64 @@
   - [x] Variable assignement
   - [x] Mathematic operator
   - [x] Comparison operator
   - [x] If block
   - [ ] While loop :fire:
   - [ ] For loop ?
 
-## Installation
+**future version**
+- template support for standard smart-contract
+- NFT collection builder
+  - g45-c + g45-nft automatic deployment 
+- API builder for any SC already deployed on chain
 
+# Installation
+
+## Directly from the python public repositry
 ```bash
 pip install deropy
+deropy configure 
+```
+
+## From sources
+```bash
+git clone https://github.com/dero-hyperbolic/deropy.git
+cd deropy
+pip install .
+deropy configure
 ```
 
 ## Quick Start
 
-**If the simulator is running** the followin
-the following command will:
+```bash
+deropy deploy -g path/to/sc.bas
+```
+
+this command will:
+
+**If the simulator is running**
 - Deploy your smart contract to the simulator
 - Create a new SC.py file in the current directory with the correct SCID.
 - A new tests/test_sc.py file in the current directory.
 
 **If the simulator is not running** the Smart Contract will not be deployed
 
 SC.py will contain a class that allow you to call every function implemented in your smart contract
 test_sc.py will contain a test class that provide you with a basic test skeleton for every function implemented in your smart contract
 
-```bash
-deropy deploy -g path/to/sc.bas
-```
-
-### Usage in a python script or terminal
+## Usage in a python script or terminal
 ```python
 from SC import SC
 sc = SC()
 sc.function_to_invoke(param1, param2)
 >>> {'jsonrpc': '2.0', 'id': '1', 'result': {'txid': '861fbb04b475fb94de9ba...'}}
 ```
 
 ## Commands
 
 | Command | Description |
 | --- | --- |
 | `deropy configure` | Install the autocomplete script |
-| `deropy deploy` | Compile a DERO smart contract |
-| `deropy generate` | Test a DERO smart contract |
+| `deropy deploy` | deploy a DERO smart contract |
+| `deropy generate` | Convert a DERO smart contract into a python API|
```

### Comparing `deropy-0.0.4/README.md` & `deropy-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -31,47 +31,64 @@
   - [x] Variable assignement
   - [x] Mathematic operator
   - [x] Comparison operator
   - [x] If block
   - [ ] While loop :fire:
   - [ ] For loop ?
 
-## Installation
+**future version**
+- template support for standard smart-contract
+- NFT collection builder
+  - g45-c + g45-nft automatic deployment 
+- API builder for any SC already deployed on chain
 
+# Installation
+
+## Directly from the python public repositry
 ```bash
 pip install deropy
+deropy configure 
+```
+
+## From sources
+```bash
+git clone https://github.com/dero-hyperbolic/deropy.git
+cd deropy
+pip install .
+deropy configure
 ```
 
 ## Quick Start
 
-**If the simulator is running** the followin
-the following command will:
+```bash
+deropy deploy -g path/to/sc.bas
+```
+
+this command will:
+
+**If the simulator is running**
 - Deploy your smart contract to the simulator
 - Create a new SC.py file in the current directory with the correct SCID.
 - A new tests/test_sc.py file in the current directory.
 
 **If the simulator is not running** the Smart Contract will not be deployed
 
 SC.py will contain a class that allow you to call every function implemented in your smart contract
 test_sc.py will contain a test class that provide you with a basic test skeleton for every function implemented in your smart contract
 
-```bash
-deropy deploy -g path/to/sc.bas
-```
-
-### Usage in a python script or terminal
+## Usage in a python script or terminal
 ```python
 from SC import SC
 sc = SC()
 sc.function_to_invoke(param1, param2)
 >>> {'jsonrpc': '2.0', 'id': '1', 'result': {'txid': '861fbb04b475fb94de9ba...'}}
 ```
 
 ## Commands
 
 | Command | Description |
 | --- | --- |
 | `deropy configure` | Install the autocomplete script |
-| `deropy deploy` | Compile a DERO smart contract |
-| `deropy generate` | Test a DERO smart contract |
+| `deropy deploy` | deploy a DERO smart contract |
+| `deropy generate` | Convert a DERO smart contract into a python API|
```

### Comparing `deropy-0.0.4/deropy/commands/configure.py` & `deropy-0.1.0/deropy/commands/configure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 import click
 import logging
 
+
 @click.command('configure')
 def configure():
     _install_autocomplete()
 
+
 def _configure():
     _install_autocomplete()
 
+
 def _install_autocomplete():
     os.makedirs(os.path.join(os.path.expanduser('~'), '.deropy'), exist_ok=True)
 
     bashrc_path = os.path.join(os.path.expanduser('~'), '.bashrc')
     if os.path.isfile(bashrc_path):
         logging.info('Installing bash autocomplete')
         cmd_str = '~/.deropy/deropy_complete.bash'
@@ -32,10 +35,11 @@
 
         if _check_exist_in_file(cmd_str, rc_file):
             return
 
         os.system(f'_DEROPY_COMPLETE=zsh_source deropy > {cmd_str}')
         os.system(f'echo ". {cmd_str}" >> ~/.zshrc')
 
+
 def _check_exist_in_file(sentence: str, filepath: str):
     with open(filepath, 'r') as file:
-        return any(sentence in line for line in file.readlines())
+        return any(sentence in line for line in file.readlines())
```

### Comparing `deropy-0.0.4/deropy/commands/deploy.py` & `deropy-0.1.0/deropy/commands/deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import requests
 import click
-import json
 
 from deropy.commands.generate import _generate_class, _generate_tests
 
+
 @click.command('deploy')
 @click.argument('file', type=click.Path())
 @click.option('-g', '--generate', is_flag=True, help='Generate the SC file')
 def deploy(file, generate):
     sc_txid = _deploy(file)
     click.echo(f'Transaction ID: {sc_txid}')
 
     if generate:
         _generate_class(file, sc_txid)
         _generate_tests(file)
 
+
 def _deploy(file: str):
     with open(file, 'r') as f:
         data = f.read()
 
     url = 'http://127.0.0.1:30000/install_sc'
     response = requests.post(url, data.encode())
 
     data = response.json()
-    return data['txid']
+    return data['txid']
```

### Comparing `deropy-0.0.4/deropy/commands/generate.py` & `deropy-0.1.0/deropy/commands/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import click
-import json
 import os
 
+
 @click.command('generate')
 @click.argument('file', type=click.Path())
 @click.option('-s', '--scid', type=str, help='The SCID of the smart contract', default='')
 def generate(file, scid):
     _generate_class(file, scid)
     _generate_tests(file)
 
-# def generate_tests(functions):
-#     file_content = _read_bas(file)
-#     functions = _parse_function(file_content)
-
-#     os.mak
 
 def _generate_tests(file):
     file_content = _read_bas(file)
     functions = _parse_function(file_content)
 
     lines = ['from SC import SC']
     lines += ['import unittest']
@@ -30,20 +25,21 @@
 
     for f, p in functions.items():
         test_method = _generate_test_method(f, p)
         lines.extend(test_method)
 
     os.makedirs('tests', exist_ok=True)
     with open('tests/test_SC.py', 'w') as f:
-        for l in lines:
-            f.write(f'{l}\n')
+        for line in lines:
+            f.write(f'{line}\n')
+
 
 def _generate_test_method(f_name, p):
     lines = [f'\n    def test_{_camelCase_to_snake_case(f_name)}(self):']
-    
+
     # Create a parameter map
     if len(p) != 0:
         lines += ['        params = {']
         for k, v in p.items():
             lines += [f'            "{k}": {_SC_type_to_python_fake(v)},']
         lines += ['        }']
         lines += ['']
@@ -72,17 +68,14 @@
     lines += ['        sc_content = self.sc.read()']
     lines += ['']
 
     # Create the assertion
     lines += ['        # ---- Your test here']
     lines += ['        self.assertEqual(1, 1)']
 
-
-
-
     return lines
 
 
 def _generate_class(file: str, scid: str):
     file_content = _read_bas(file)
     functions = _parse_function(file_content)
 
@@ -98,98 +91,101 @@
     for f, p in functions.items():
         scinvoce_method = _generate_method_scinvoce(f, p)
         transfer2_method = _generate_method_transfer2(f, p)
         lines.extend(scinvoce_method)
         lines.extend(transfer2_method)
 
     with open('SC.py', 'w') as f:
-        for l in lines:
-            f.write(f'{l}\n')
+        for line in lines:
+            f.write(f'{line}\n')
+
 
 def _read_bas(path: str) -> str:
     with open(path, 'r') as f:
         return f.readlines()
-    
+
+
 def _parse_function(lines: list) -> dict:
     def get_function_name(line: str) -> str:
         return line[9:].split('(')[0]
-    
+
     def get_function_parameters(line: str) -> list:
         output = dict()
         parameters = line[9:].split('(')[1].split(')')[0].split(',')
         if len(parameters) == 1 and parameters[0] == '':
             return output
-        
+
         for p in parameters:
             p = p.strip()
             output[p.split()[0]] = p.split()[1]
-        
+
         return output
 
     functions = {}
     for line in lines:
-        if "Function " in line and not "End Function" in line:
+        if "Function " in line and "End Function" not in line:
             function_name = get_function_name(line)
 
             if not function_name[0].isupper():
                 continue
 
             parameters = get_function_parameters(line)
             functions[function_name] = parameters
 
     return functions
 
+
 def _generate_read_method(scid):
-        return [
-            '    def read(self):',
-            '        url = "http://127.0.0.1:20000/json_rpc"',
-            '        payload = {',
-            '            "jsonrpc": "2.0",',
-            '            "id": "1",',
-            '            "method": "DERO.GetSC",',
-            '            "params": {',
-            f'                "scid": "{scid}",',
-            '                "code": True,',
-            '                "variables": True',
-            '            }',
-            '        }',
-            '        response = requests.post(url, data=json.dumps(payload), headers=self.headers)',
-            '        print(response.json())',
-            '        return response.json()'
-        ]
-        return lines
+    return [
+        '    def read(self):',
+        '        url = "http://127.0.0.1:20000/json_rpc"',
+        '        payload = {',
+        '            "jsonrpc": "2.0",',
+        '            "id": "1",',
+        '            "method": "DERO.GetSC",',
+        '            "params": {',
+        f'                "scid": "{scid}",',
+        '                "code": True,',
+        '                "variables": True',
+        '            }',
+        '        }',
+        '        response = requests.post(url, data=json.dumps(payload), headers=self.headers)',
+        '        print(response.json())',
+        '        return response.json()'
+    ]
+
 
 def _generate_method_scinvoce(f_name, p):
     # create the method definition
     method_parameters = ''
     for k, v in p.items():
         method_parameters += f'{k}:{_SC_type_to_python_type(v)}, '
     method_parameters = method_parameters[:-2]
 
     if len(method_parameters) == 0:
         lines = [f'\n    def {_camelCase_to_snake_case(f_name)}(self):']
     else:
         lines = [f'\n    def {_camelCase_to_snake_case(f_name)}(self, {method_parameters}):']
 
     scrpc = [
-        f'                    "sc_rpc": [',
+        '                    "sc_rpc": [',
         '                        {',
-        f'                            "name": "entrypoint",',
-        f'                            "datatype": "S",',
+        '                            "name": "entrypoint",',
+        '                            "datatype": "S",',
         f'                            "value": "{f_name}"',
         '                        },',
     ]
 
     for k, v in p.items():
         scrpc += [
-             '                        {',
+            '                        {',
             f'                            "name": "{k}",',
             f'                            "datatype": "{_SC_type_to_jsonrpc(v)}",',
             f'                            "value": {k}',
-             '                        },',
+            '                        },',
         ]
 
     payload = [
         '        payload = {',
         '                "jsonrpc": "2.0",',
         '                "id": "1",',
         '                "method": "scinvoke",',
@@ -200,46 +196,47 @@
     payload += scrpc
     payload += [
         '                    ]',
         '                }',
         '            }',
     ]
     lines.extend(payload)
-    lines += [f'        response = requests.post(self.url, data=json.dumps(payload), headers=self.headers)']
-    lines += [f'        print(response.json())']
+    lines += ['        response = requests.post(self.url, data=json.dumps(payload), headers=self.headers)']
+    lines += ['        print(response.json())']
     return lines
 
+
 def _generate_method_transfer2(f_name, p):
     # create the method definition
     method_parameters = ''
     for k, v in p.items():
         method_parameters += f'{k}:{_SC_type_to_python_type(v)}, '
     method_parameters = method_parameters[:-2]
 
     if len(method_parameters) == 0:
         lines = [f'\n    def {_camelCase_to_snake_case(f_name)}_fee(self, fee: int):']
     else:
         lines = [f'\n    def {_camelCase_to_snake_case(f_name)}_fee(self, fee: int, {method_parameters}):']
 
     scrpc = [
-        f'                    "sc_rpc": [',
+        '                    "sc_rpc": [',
         '                        {',
-        f'                            "name": "entrypoint",',
-        f'                            "datatype": "S",',
+        '                            "name": "entrypoint",',
+        '                            "datatype": "S",',
         f'                            "value": "{f_name}"',
         '                        },',
     ]
 
     for k, v in p.items():
         scrpc += [
-             '                        {',
+            '                        {',
             f'                            "name": "{k}",',
             f'                            "datatype": "{_SC_type_to_jsonrpc(v)}",',
             f'                            "value": {k}',
-             '                        },',
+            '                        },',
         ]
 
     payload = [
         '        payload = {',
         '                "jsonrpc": "2.0",',
         '                "id": "1",',
         '                "method": "transfer",',
@@ -251,37 +248,40 @@
     payload += scrpc
     payload += [
         '                    ]',
         '                }',
         '            }',
     ]
     lines.extend(payload)
-    lines += [f'        response = requests.post(self.url, data=json.dumps(payload), headers=self.headers)']
-    lines += [f'        print(response.json())']
+    lines += ['        response = requests.post(self.url, data=json.dumps(payload), headers=self.headers)']
+    lines += ['        print(response.json())']
     return lines
 
+
 def _SC_type_to_python_type(t: str):
     if t == 'String':
         return 'str'
-    
+
     if t == 'Uint64':
         return 'int'
     raise RuntimeError(f'type [{t}] do not exist in DERO')
 
+
 def _SC_type_to_python_fake(t: str):
     if t == 'String':
         return '"string"'
-    
+
     if t == 'Uint64':
         return '1'
     raise RuntimeError(f'type [{t}] do not exist in DERO')
 
+
 def _SC_type_to_jsonrpc(t: str):
     if t == "String":
         return "S"
     if t == "Uint64":
         return "U"
     raise RuntimeError(f'type {t} do not exist in DERO')
 
+
 def _camelCase_to_snake_case(name: str) -> str:
     return ''.join(['_' + i.lower() if i.isupper() else i for i in name]).lstrip('_')
-
```

### Comparing `deropy-0.0.4/deropy.egg-info/PKG-INFO` & `deropy-0.1.0/deropy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.0.4
+Version: 0.1.0
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: click==8.0.4
-Requires-Dist: requests==2.27.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: python-dotenv==0.20.0
 Requires-Dist: InquirerPy==0.3.4
+Requires-Dist: pycryptodome==3.20.0
 
 # DEROPY
 
 Deropy is a toolbox for creating, managing and testing DERO smart contracts.
 
 # Roadmap
 
@@ -47,47 +48,64 @@
   - [x] Variable assignement
   - [x] Mathematic operator
   - [x] Comparison operator
   - [x] If block
   - [ ] While loop :fire:
   - [ ] For loop ?
 
-## Installation
+**future version**
+- template support for standard smart-contract
+- NFT collection builder
+  - g45-c + g45-nft automatic deployment 
+- API builder for any SC already deployed on chain
 
+# Installation
+
+## Directly from the python public repositry
 ```bash
 pip install deropy
+deropy configure 
+```
+
+## From sources
+```bash
+git clone https://github.com/dero-hyperbolic/deropy.git
+cd deropy
+pip install .
+deropy configure
 ```
 
 ## Quick Start
 
-**If the simulator is running** the followin
-the following command will:
+```bash
+deropy deploy -g path/to/sc.bas
+```
+
+this command will:
+
+**If the simulator is running**
 - Deploy your smart contract to the simulator
 - Create a new SC.py file in the current directory with the correct SCID.
 - A new tests/test_sc.py file in the current directory.
 
 **If the simulator is not running** the Smart Contract will not be deployed
 
 SC.py will contain a class that allow you to call every function implemented in your smart contract
 test_sc.py will contain a test class that provide you with a basic test skeleton for every function implemented in your smart contract
 
-```bash
-deropy deploy -g path/to/sc.bas
-```
-
-### Usage in a python script or terminal
+## Usage in a python script or terminal
 ```python
 from SC import SC
 sc = SC()
 sc.function_to_invoke(param1, param2)
 >>> {'jsonrpc': '2.0', 'id': '1', 'result': {'txid': '861fbb04b475fb94de9ba...'}}
 ```
 
 ## Commands
 
 | Command | Description |
 | --- | --- |
 | `deropy configure` | Install the autocomplete script |
-| `deropy deploy` | Compile a DERO smart contract |
-| `deropy generate` | Test a DERO smart contract |
+| `deropy deploy` | deploy a DERO smart contract |
+| `deropy generate` | Convert a DERO smart contract into a python API|
```

### Comparing `deropy-0.0.4/setup.py` & `deropy-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.0.4',
+    version=os.getenv('DEROPY_VERSION') or '0.1.0',
     url='https://github.com/dero-hyperbolic/deropy.git',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'click==8.0.4',
-        'requests==2.27.1',
+        'requests==2.31.0',
         'coloredlogs==15.0.1',
         'pyperclip==1.8.2',
         'python-dotenv==0.20.0',
         'InquirerPy==0.3.4',
+        'pycryptodome==3.20.0',
     ],
     include_package_data=True,
     package_data={},
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
```

