# Comparing `tmp/parthenon_utils-0.0.2.tar.gz` & `tmp/parthenon_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parthenon_utils-0.0.2.tar", last modified: Fri Apr 26 21:46:56 2024, max compression
+gzip compressed data, was "parthenon_utils-0.0.4.tar", last modified: Mon Apr 29 17:36:57 2024, max compression
```

## Comparing `parthenon_utils-0.0.2.tar` & `parthenon_utils-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 21:46:56.104604 parthenon_utils-0.0.2/
--rw-rw-rw-   0        0        0       99 2024-04-26 21:46:56.102566 parthenon_utils-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-26 21:46:56.062349 parthenon_utils-0.0.2/parthenon_utils/
--rw-rw-rw-   0        0        0      264 2024-04-26 21:40:29.000000 parthenon_utils-0.0.2/parthenon_utils/__init__.py
--rw-rw-rw-   0        0        0    28590 2024-04-26 21:40:29.000000 parthenon_utils-0.0.2/parthenon_utils/builder.py
--rw-rw-rw-   0        0        0     5689 2024-04-26 21:40:36.000000 parthenon_utils-0.0.2/parthenon_utils/controller.py
--rw-rw-rw-   0        0        0    11296 2024-04-26 21:40:36.000000 parthenon_utils-0.0.2/parthenon_utils/encrypter.py
--rw-rw-rw-   0        0        0    15284 2024-04-26 21:40:36.000000 parthenon_utils-0.0.2/parthenon_utils/logger.py
--rw-rw-rw-   0        0        0      436 2024-04-26 21:40:29.000000 parthenon_utils-0.0.2/parthenon_utils/nologger.py
-drwxrwxrwx   0        0        0        0 2024-04-26 21:46:56.098564 parthenon_utils-0.0.2/parthenon_utils.egg-info/
--rw-rw-rw-   0        0        0       99 2024-04-26 21:46:55.000000 parthenon_utils-0.0.2/parthenon_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-04-26 21:46:56.000000 parthenon_utils-0.0.2/parthenon_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 21:46:55.000000 parthenon_utils-0.0.2/parthenon_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-26 21:46:55.000000 parthenon_utils-0.0.2/parthenon_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-26 21:46:55.000000 parthenon_utils-0.0.2/parthenon_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 21:46:56.105565 parthenon_utils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      211 2024-04-26 21:41:32.000000 parthenon_utils-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:36:57.557883 parthenon_utils-0.0.4/
+-rw-rw-rw-   0        0        0       99 2024-04-29 17:36:57.553969 parthenon_utils-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 17:36:57.520198 parthenon_utils-0.0.4/parthenon_utils/
+-rw-rw-rw-   0        0        0       59 2024-04-29 17:26:25.000000 parthenon_utils-0.0.4/parthenon_utils/__init__.py
+-rw-rw-rw-   0        0        0    28567 2024-04-29 17:26:25.000000 parthenon_utils-0.0.4/parthenon_utils/builder.py
+-rw-rw-rw-   0        0        0     5666 2024-04-29 17:26:25.000000 parthenon_utils-0.0.4/parthenon_utils/controller.py
+-rw-rw-rw-   0        0        0    11200 2024-04-29 17:30:01.000000 parthenon_utils-0.0.4/parthenon_utils/encrypter.py
+-rw-rw-rw-   0        0        0    15288 2024-04-29 17:26:25.000000 parthenon_utils-0.0.4/parthenon_utils/logger.py
+-rw-rw-rw-   0        0        0      413 2024-04-29 17:26:26.000000 parthenon_utils-0.0.4/parthenon_utils/nologger.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:36:57.550138 parthenon_utils-0.0.4/parthenon_utils.egg-info/
+-rw-rw-rw-   0        0        0       99 2024-04-29 17:36:57.000000 parthenon_utils-0.0.4/parthenon_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-04-29 17:36:57.000000 parthenon_utils-0.0.4/parthenon_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:36:57.000000 parthenon_utils-0.0.4/parthenon_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-29 17:36:57.000000 parthenon_utils-0.0.4/parthenon_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 17:36:57.000000 parthenon_utils-0.0.4/parthenon_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:36:57.558065 parthenon_utils-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      211 2024-04-29 17:36:28.000000 parthenon_utils-0.0.4/setup.py
```

### Comparing `parthenon_utils-0.0.2/parthenon_utils/builder.py` & `parthenon_utils-0.0.4/parthenon_utils/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 
 __author__ = 'Miguel Freire Couy'
 __credits__ = ['Miguel Freire Couy']
-__version__ = '0.0.1'
 __maintainer__ = 'Miguel Freire Couy'
 __email__ = 'miguel.couy@outlook.com'
 __status__ = 'Production'
 
 from pathlib import Path
 from typing import Callable, Union, Optional, List, Dict
 from datetime import datetime
```

### Comparing `parthenon_utils-0.0.2/parthenon_utils/controller.py` & `parthenon_utils-0.0.4/parthenon_utils/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 
 __author__ = 'Miguel Freire Couy'
 __credits__ = ['Miguel Freire Couy']
-__version__ = '0.0.1'
 __maintainer__ = 'Miguel Freire Couy'
 __email__ = 'miguel.couy@Ooutlook.com'
 __status__ = 'Production'
 
 from pathlib import Path
 from typing import Union, Optional
 import datetime as dt
```

### Comparing `parthenon_utils-0.0.2/parthenon_utils/encrypter.py` & `parthenon_utils-0.0.4/parthenon_utils/encrypter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# -*- coding: utf-8 -*-
+
 __author__ = 'Miguel Freire Couy'
 __credits__ = ['Miguel Freire Couy']
-__version__ = '0.0.1'
 __maintainer__ = 'Miguel Freire Couy'
 __email__ = 'miguel.couy@Ooutlook.com'
 __status__ = 'Production'
 
 from cryptography.fernet import Fernet, InvalidToken
 from typing import Union, Optional
 from functools import wraps
@@ -56,18 +57,16 @@
         
         if isinstance(self.key, (str, bytes)):
             self.key = Fernet(self.key)
 
         elif isinstance(self.key, Fernet):
             self.key = self.key
 
-        else:
-           raise TypeError(
-               "The key must be a string, bytes, or a Fernet object."
-            )
+        else: pass
+        
 
     @staticmethod
     def generate_key(as_bytes: bool = False) -> Union[str, bytes]:
         """
         Generates a new Fernet key and returns it either as a bytes object or a
         base64-encoded string.
```

### Comparing `parthenon_utils-0.0.2/parthenon_utils/logger.py` & `parthenon_utils-0.0.4/parthenon_utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# -*- coding: utf-8 -*-
+
 __author__ = 'Miguel Freire Couy'
 __credits__ = ['Miguel Freire Couy']
-__version__ = '0.0.1'
 __maintainer__ = 'Miguel Freire Couy'
 __email__ = 'miguel.couy@Ooutlook.com'
 __status__ = 'Production'
 
 import logging
 from logging.handlers import RotatingFileHandler
 from sys import stderr
```

