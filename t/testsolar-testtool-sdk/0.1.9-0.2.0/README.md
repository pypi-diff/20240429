# Comparing `tmp/testsolar_testtool_sdk-0.1.9.tar.gz` & `tmp/testsolar-testtool-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar_testtool_sdk-0.1.9.tar", last modified: Mon Apr 15 08:46:20 2024, max compression
+gzip compressed data, was "testsolar-testtool-sdk-0.2.0.tar", last modified: Mon Apr 29 07:36:33 2024, max compression
```

## Comparing `testsolar_testtool_sdk-0.1.9.tar` & `testsolar-testtool-sdk-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.665649 testsolar_testtool_sdk-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-15 08:46:20.665649 testsolar_testtool_sdk-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:46:20.665649 testsolar_testtool_sdk-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/pipe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 08:46:20.000000 testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:46:20.661649 testsolar_testtool_sdk-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-15 08:45:56.000000 testsolar_testtool_sdk-0.1.9/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:33.042468 testsolar-testtool-sdk-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 07:36:33.042468 testsolar-testtool-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:36:33.042468 testsolar-testtool-sdk-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:33.038468 testsolar-testtool-sdk-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:33.038468 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:33.042468 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/model/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/model/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/pipe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:33.042468 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 07:36:33.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-29 07:36:33.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:36:33.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 07:36:33.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 07:36:33.000000 testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:36:33.042468 testsolar-testtool-sdk-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-29 07:36:09.000000 testsolar-testtool-sdk-0.2.0/tests/test_report.py
```

### Comparing `testsolar_testtool_sdk-0.1.9/LICENSE` & `testsolar-testtool-sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/model/testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/pipe_reader.py` & `testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/pipe_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import json
 import struct
-from typing import BinaryIO
+from typing import BinaryIO, Dict, Any
 
 from dacite import from_dict, Config
 
 from .model.load import LoadResult
 from .model.testresult import TestResult
 from .reporter import MAGIC_NUMBER
 
 
 # 从管道读取加载结果，仅供单元测试使用
 def read_load_result(pipe_io: BinaryIO) -> LoadResult:
     result_data = _read_model(pipe_io)
 
-    data_dict: dict = json.loads(result_data)
+    data_dict: Dict[Any, Any] = json.loads(result_data)
     re: LoadResult = from_dict(data_class=LoadResult, data=data_dict)
 
     return re
 
 
 # 从管道读取测试用例结果，仅供单元测试使用
 def read_test_result(pipe_io: BinaryIO) -> TestResult:
     result_data = _read_model(pipe_io)
 
-    data_dict: dict = json.loads(result_data)
+    data_dict: Dict[Any, Any] = json.loads(result_data)
     re: TestResult = from_dict(
         data_class=TestResult, data=data_dict, config=Config(check_types=False)
     )
     return re
 
 
 def _read_model(pipe_io: BinaryIO) -> str:
```

### Comparing `testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk/reporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import json
 import logging
 import os
 import struct
-from typing import Optional, BinaryIO
+from typing import Optional, BinaryIO, Any, Dict
 
 import portalocker
 
 from .model.encoder import DateTimeEncoder
 from .model.load import LoadResult
 from .model.testresult import TestResult
 
@@ -15,45 +15,45 @@
 MAGIC_NUMBER = 0x1234ABCD
 
 # 跟TestSolar uniSDK约定的管道上报文件描述符号
 PIPE_WRITER = 3
 
 
 class Reporter:
-    def __enter__(self):
+    def __enter__(self) -> 'Reporter':
         return self
 
     def __init__(self, pipe_io: Optional[BinaryIO] = None) -> None:
         """
         初始化报告工具类
         :param pipe_io: 可选的管道，用于测试
         """
         self.lock_file = "/tmp/testsolar_reporter.lock"
 
         if pipe_io:
             self.pipe_io = pipe_io
         else:
             self.pipe_io = os.fdopen(PIPE_WRITER, "wb")
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.close()
 
     def report_load_result(self, load_result: LoadResult) -> None:
         with portalocker.Lock(self.lock_file, timeout=60):
             self._send_json(dataclasses.asdict(load_result))
 
     def report_case_result(self, case_result: TestResult) -> None:
         with portalocker.Lock(self.lock_file, timeout=60):
             self._send_json(dataclasses.asdict(case_result))
 
     def close(self) -> None:
         if self.pipe_io:
             self.pipe_io.close()
 
-    def _send_json(self, result: dict) -> None:
+    def _send_json(self, result: Dict[Any, Any]) -> None:
         data = json.dumps(result, cls=DateTimeEncoder).encode("utf-8")
         length = len(data)
 
         # 将魔数写入管道
         self.pipe_io.write(struct.pack("<I", MAGIC_NUMBER))
 
         # 将 JSON 数据的长度写入管道
```

### Comparing `testsolar_testtool_sdk-0.1.9/src/testsolar_testtool_sdk.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-0.2.0/src/testsolar_testtool_sdk.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 src/testsolar_testtool_sdk/__init__.py
 src/testsolar_testtool_sdk/pipe_reader.py
-src/testsolar_testtool_sdk/py.typed
 src/testsolar_testtool_sdk/reporter.py
 src/testsolar_testtool_sdk.egg-info/PKG-INFO
 src/testsolar_testtool_sdk.egg-info/SOURCES.txt
 src/testsolar_testtool_sdk.egg-info/dependency_links.txt
 src/testsolar_testtool_sdk.egg-info/requires.txt
 src/testsolar_testtool_sdk.egg-info/top_level.txt
 src/testsolar_testtool_sdk/model/__init__.py
```

### Comparing `testsolar_testtool_sdk-0.1.9/tests/test_report.py` & `testsolar-testtool-sdk-0.2.0/tests/test_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
 
 def test_report_run_case_result():
     # 创建一个Reporter实例
     pipe_io = io.BytesIO()
     with Reporter(pipe_io=pipe_io) as reporter:
         # 创建五个LoadResult实例并发调用report_run_case_result方法
-        with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
+        with concurrent.futures.ThreadPoolExecutor(max_workers=3) as executor:
             send_action = partial(send_test_result, reporter)
             for i in range(5):
                 executor.submit(send_action)
 
         # 检查管道中的数据，确保每个用例的魔数和数据长度还有数据正确
         pipe_io.seek(0)
         r1: TestResult = read_test_result(pipe_io)
```

