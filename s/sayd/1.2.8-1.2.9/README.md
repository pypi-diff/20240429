# Comparing `tmp/sayd-1.2.8.tar.gz` & `tmp/sayd-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayd-1.2.8.tar", max compression
+gzip compressed data, was "sayd-1.2.9.tar", max compression
```

## Comparing `sayd-1.2.8.tar` & `sayd-1.2.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     9162 2024-02-15 13:25:05.307996 sayd-1.2.8/LICENSE
--rw-r--r--   0        0        0     3188 2024-02-15 13:33:19.661726 sayd-1.2.8/README.rst
--rw-r--r--   0        0        0     1424 2024-03-02 18:23:39.129282 sayd-1.2.8/pyproject.toml
--rw-r--r--   0        0        0      846 2024-03-02 18:23:39.129282 sayd-1.2.8/sayd/__init__.py
--rw-r--r--   0        0        0     2261 2022-08-23 22:18:53.021755 sayd-1.2.8/sayd/__main__.py
--rw-r--r--   0        0        0    14910 2022-09-01 18:18:12.006951 sayd-1.2.8/sayd/_client.py
--rw-r--r--   0        0        0    20592 2022-09-01 18:18:12.006951 sayd-1.2.8/sayd/_server.py
--rw-r--r--   0        0        0        0 2022-08-18 08:33:25.453468 sayd-1.2.8/sayd/py.typed
--rw-r--r--   0        0        0     4114 2024-03-02 18:24:16.905920 sayd-1.2.8/setup.py
--rw-r--r--   0        0        0     4389 2024-03-02 18:24:16.906388 sayd-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     9162 2024-04-28 17:36:56.664918 sayd-1.2.9/LICENSE
+-rw-r--r--   0        0        0      542 2024-04-28 22:14:31.180132 sayd-1.2.9/NOTICE
+-rw-r--r--   0        0        0     3188 2024-04-28 22:14:31.180132 sayd-1.2.9/README.rst
+-rw-r--r--   0        0        0     1325 2024-04-28 22:14:31.180132 sayd-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0      777 2024-04-28 22:14:31.180132 sayd-1.2.9/sayd/__init__.py
+-rw-r--r--   0        0        0     2192 2024-04-28 22:14:31.180132 sayd-1.2.9/sayd/__main__.py
+-rw-r--r--   0        0        0    14856 2024-04-28 22:14:31.180132 sayd-1.2.9/sayd/_client.py
+-rw-r--r--   0        0        0    20538 2024-04-28 22:14:31.180132 sayd-1.2.9/sayd/_server.py
+-rw-r--r--   0        0        0        0 2024-04-28 17:36:56.668918 sayd-1.2.9/sayd/py.typed
+-rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 sayd-1.2.9/PKG-INFO
```

### Comparing `sayd-1.2.8/LICENSE` & `sayd-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sayd-1.2.8/README.rst` & `sayd-1.2.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This library was developed with simplicity and performance in mind, with modern practices of Python development.
 
 `Documentation Reference <https://sayd.readthedocs.io>`_
 
 
 Install
 -------
-Works on Python 3.7.4+.
+Works on Python 3.8.0+.
 
 .. code-block:: bash
 
     pip install sayd
 
 
 Development
```

### Comparing `sayd-1.2.8/pyproject.toml` & `sayd-1.2.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sayd"
-version = "1.2.8"
+version = "1.2.9"
 description = "A performant asynchronous communication protocol in pure Python."
 authors = ["LW016"]
 readme = "README.rst"
 repository = "https://github.com/lw016/sayd"
 keywords = ["network", "protocol", "communication"]
 license = "Apache-2.0"
 classifiers=[
@@ -25,27 +25,27 @@
 
 
 [tool.poetry.scripts]
 sayd = "sayd.__main__:execute"
 
 
 [tool.poetry.dependencies]
-python = ">=3.7.4,<4.0.0"
+python = ">=3.8.0,<4.0.0"
 
 typer = "0.4.1"
-pyOpenSSL = "22.0.0"
+pyOpenSSL = "24.1.0"
 
-uvloop = {version="0.17.0", optional=true, markers="sys_platform != 'win32'"}
-ujson = {version="5.6.0", optional=true}
-rich = {version="12.5.1", optional=true}
+uvloop = "0.17.0"
+ujson = "5.6.0"
+rich = "12.5.1"
 
 
 [tool.poetry.dev-dependencies]
-types-ujson = "5.2.0"
-types-pyOpenSSL = "22.0.3"
+types-ujson = "5.6.0.0"
+types-pyOpenSSL = "24.1.0.20240425"
 
 tox = "3.8.0"
 mypy = "0.950"
 pylint = "2.14.0"
 bandit = "1.7.4" 
 pytest = "7.1.2"
 pytest-asyncio = "0.18.3"
```

### Comparing `sayd-1.2.8/sayd/__init__.py` & `sayd-1.2.9/sayd/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Sayd package."""
 
-# Copyright 2022 LW016 (GPG FINGERPRINT 33CA C1E8 EC4C 0B31 73AE  DD8B 31A5 35D1 2844 39ED)
+# Copyright 2022 LW016
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 # http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __all__ = ("SaydServer", "SaydClient")
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 
 __author__ = "LW016"
 __license__ = "Apache License, Version 2.0"
 
 
 from ._server import SaydServer
 from ._client import SaydClient
```

### Comparing `sayd-1.2.8/sayd/__main__.py` & `sayd-1.2.9/sayd/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """CLI utility to generate self-signed certificates."""
 
-# Copyright 2022 LW016 (GPG FINGERPRINT 33CA C1E8 EC4C 0B31 73AE  DD8B 31A5 35D1 2844 39ED)
+# Copyright 2022 LW016
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 # http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sayd-1.2.8/sayd/_client.py` & `sayd-1.2.9/sayd/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Client implementation."""
 
-# Copyright 2022 LW016 (GPG FINGERPRINT 33CA C1E8 EC4C 0B31 73AE  DD8B 31A5 35D1 2844 39ED)
+# Copyright 2022 LW016
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 # http://www.apache.org/licenses/LICENSE-2.0
 
@@ -34,15 +34,15 @@
 try:
     import ujson as json
 
 except ImportError:
     import json # type: ignore
 
 try:
-    from uvloop import install as tune
+    from uvloop import install as tune # type: ignore
 
 except ImportError:
     pass
 
 
 class SaydClient:
     """Client class.
```

### Comparing `sayd-1.2.8/sayd/_server.py` & `sayd-1.2.9/sayd/_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Server implementation."""
 
-# Copyright 2022 LW016 (GPG FINGERPRINT 33CA C1E8 EC4C 0B31 73AE  DD8B 31A5 35D1 2844 39ED)
+# Copyright 2022 LW016
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 # http://www.apache.org/licenses/LICENSE-2.0
 
@@ -35,15 +35,15 @@
 try:
     import ujson as json
 
 except ImportError:
     import json # type: ignore
 
 try:
-    from uvloop import install as tune
+    from uvloop import install as tune # type: ignore
 
 except ImportError:
     pass
 
 
 class SaydServer:
     """Server class.
```

### Comparing `sayd-1.2.8/setup.py` & `sayd-1.2.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,195 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sayd
+Version: 1.2.9
+Summary: A performant asynchronous communication protocol in pure Python.
+Home-page: https://github.com/lw016/sayd
+License: Apache-2.0
+Keywords: network,protocol,communication
+Author: LW016
+Requires-Python: >=3.8.0,<4.0.0
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Android
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: pyOpenSSL (==24.1.0)
+Requires-Dist: rich (==12.5.1)
+Requires-Dist: typer (==0.4.1)
+Requires-Dist: ujson (==5.6.0)
+Requires-Dist: uvloop (==0.17.0)
+Project-URL: Repository, https://github.com/lw016/sayd
+Description-Content-Type: text/x-rst
 
-packages = \
-['sayd']
+Sayd
+====
+*A performant asynchronous communication protocol in pure Python.*
 
-package_data = \
-{'': ['*']}
+This library was developed with simplicity and performance in mind, with modern practices of Python development.
 
-install_requires = \
-['pyOpenSSL==22.0.0', 'typer==0.4.1']
-
-entry_points = \
-{'console_scripts': ['sayd = sayd.__main__:execute']}
-
-setup_kwargs = {
-    'name': 'sayd',
-    'version': '1.2.8',
-    'description': 'A performant asynchronous communication protocol in pure Python.',
-    'long_description': 'Sayd\n====\n*A performant asynchronous communication protocol in pure Python.*\n\nThis library was developed with simplicity and performance in mind, with modern practices of Python development.\n\n`Documentation Reference <https://sayd.readthedocs.io>`_\n\n\nInstall\n-------\nWorks on Python 3.7.4+.\n\n.. code-block:: bash\n\n    pip install sayd\n\n\nDevelopment\n-----------\nYou need to have installed `poetry <https://github.com/python-poetry/poetry>`_ for dependencies management (`how to <https://python-poetry.org/docs/#installation>`_).\n\n.. code-block:: bash\n\n    git clone https://github.com/lw016/sayd\n    cd sayd\n    poetry install\n\n\nRun tests\n^^^^^^^^^\n.. code-block:: bash\n\n    poetry run tox -e tests\n\nBuild docs\n^^^^^^^^^^\n.. code-block:: bash\n\n    poetry run tox -e docs\n\n\nFeatures\n--------\n- Client and server implementations\n- Reliable TCP persistent connection\n- Auto reconnection *(client)*\n- Multiple asynchronous connections *(server)*\n- Blacklist of clients *(server)*\n- TLS encryption\n- Proxy Protocol V2 support *(server)*\n- Data transmitted as dictionaries *(json)*\n- Broadcast *(server)*\n- Remote function callbacks\n- Built-in CLI utility to generate self-signed certificates\n\n\nRoadmap\n-------\n- Add support to Unix socket\n- Implement TLS certificate authentication\n\n\nCLI\n---\nThe built-in CLI utility (*sayd*) can be used to generate self-signed certificates to encrypt the connection.\n\n.. code-block:: bash\n\n    sayd --help\n\n\nUsage example\n-------------\nServer\n^^^^^^\n.. code-block:: python\n\n    import logging\n    import asyncio\n\n    from sayd import SaydServer\n\n\n    logging.basicConfig(\n            format="[%(name)s][%(levelname)s] %(asctime)s - %(message)s",\n            datefmt="%Y/%m/%d %H:%M:%S"\n            )\n\n    logger = logging.getLogger("SERVER")\n    logger.setLevel(logging.INFO)\n\n\n    server = SaydServer(logger=logger)\n\n\n    @server.callback("message")\n    async def msg(address: tuple, instance: str, data: dict) -> dict:\n        return {"greetings": "Hello from server!"}\n\n\n    async def main() -> None:\n        await server.start()\n        \n        \n        while True:\n            result = await server.call("msg", {"greetings": "Hi!"}) # Broadcast call.\n            print(result)\n\n            await asyncio.sleep(1)\n        \n        \n        await server.stop()\n\n\n    if __name__ == "__main__":\n        asyncio.run(main())\n\nClient\n^^^^^^\n.. code-block:: python\n\n    import logging\n    import asyncio\n\n    from sayd import SaydClient\n\n\n    logging.basicConfig(\n            format="[%(name)s][%(levelname)s] %(asctime)s - %(message)s",\n            datefmt="%Y/%m/%d %H:%M:%S"\n            )\n\n    logger = logging.getLogger("CLIENT")\n    logger.setLevel(logging.INFO)\n\n\n    client = SaydClient(logger=logger)\n\n\n    @client.callback("msg")\n    async def msg(instance: str, data: dict) -> dict:\n        return {"greetings": "Hello from client!"}\n\n\n    async def main() -> None:\n        await client.start()\n\n\n        while True:\n            result = await client.call("message", {"greetings": "Hi!"})\n            print(result)\n\n            await asyncio.sleep(1)\n\n        \n        await client.stop()\n\n\n    if __name__ == "__main__":\n        asyncio.run(main())\n',
-    'author': 'LW016',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/lw016/sayd',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.4,<4.0.0',
-}
+`Documentation Reference <https://sayd.readthedocs.io>`_
 
 
-setup(**setup_kwargs)
+Install
+-------
+Works on Python 3.8.0+.
+
+.. code-block:: bash
+
+    pip install sayd
+
+
+Development
+-----------
+You need to have installed `poetry <https://github.com/python-poetry/poetry>`_ for dependencies management (`how to <https://python-poetry.org/docs/#installation>`_).
+
+.. code-block:: bash
+
+    git clone https://github.com/lw016/sayd
+    cd sayd
+    poetry install
+
+
+Run tests
+^^^^^^^^^
+.. code-block:: bash
+
+    poetry run tox -e tests
+
+Build docs
+^^^^^^^^^^
+.. code-block:: bash
+
+    poetry run tox -e docs
+
+
+Features
+--------
+- Client and server implementations
+- Reliable TCP persistent connection
+- Auto reconnection *(client)*
+- Multiple asynchronous connections *(server)*
+- Blacklist of clients *(server)*
+- TLS encryption
+- Proxy Protocol V2 support *(server)*
+- Data transmitted as dictionaries *(json)*
+- Broadcast *(server)*
+- Remote function callbacks
+- Built-in CLI utility to generate self-signed certificates
+
+
+Roadmap
+-------
+- Add support to Unix socket
+- Implement TLS certificate authentication
+
+
+CLI
+---
+The built-in CLI utility (*sayd*) can be used to generate self-signed certificates to encrypt the connection.
+
+.. code-block:: bash
+
+    sayd --help
+
+
+Usage example
+-------------
+Server
+^^^^^^
+.. code-block:: python
+
+    import logging
+    import asyncio
+
+    from sayd import SaydServer
+
+
+    logging.basicConfig(
+            format="[%(name)s][%(levelname)s] %(asctime)s - %(message)s",
+            datefmt="%Y/%m/%d %H:%M:%S"
+            )
+
+    logger = logging.getLogger("SERVER")
+    logger.setLevel(logging.INFO)
+
+
+    server = SaydServer(logger=logger)
+
+
+    @server.callback("message")
+    async def msg(address: tuple, instance: str, data: dict) -> dict:
+        return {"greetings": "Hello from server!"}
+
+
+    async def main() -> None:
+        await server.start()
+        
+        
+        while True:
+            result = await server.call("msg", {"greetings": "Hi!"}) # Broadcast call.
+            print(result)
+
+            await asyncio.sleep(1)
+        
+        
+        await server.stop()
+
+
+    if __name__ == "__main__":
+        asyncio.run(main())
+
+Client
+^^^^^^
+.. code-block:: python
+
+    import logging
+    import asyncio
+
+    from sayd import SaydClient
+
+
+    logging.basicConfig(
+            format="[%(name)s][%(levelname)s] %(asctime)s - %(message)s",
+            datefmt="%Y/%m/%d %H:%M:%S"
+            )
+
+    logger = logging.getLogger("CLIENT")
+    logger.setLevel(logging.INFO)
+
+
+    client = SaydClient(logger=logger)
+
+
+    @client.callback("msg")
+    async def msg(instance: str, data: dict) -> dict:
+        return {"greetings": "Hello from client!"}
+
+
+    async def main() -> None:
+        await client.start()
+
+
+        while True:
+            result = await client.call("message", {"greetings": "Hi!"})
+            print(result)
+
+            await asyncio.sleep(1)
+
+        
+        await client.stop()
+
+
+    if __name__ == "__main__":
+        asyncio.run(main())
+
```

