# Comparing `tmp/common-tools-ai-bnq-0.1.2.tar.gz` & `tmp/common-tools-ai-bnq-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.1.2.tar", last modified: Fri Apr 26 04:22:01 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.1.3.tar", last modified: Mon Apr 29 05:59:23 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.1.2.tar` & `common-tools-ai-bnq-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 04:22:01.570863 common-tools-ai-bnq-0.1.2/
--rw-rw-rw-   0        0        0     2598 2024-04-26 04:22:01.569766 common-tools-ai-bnq-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2236 2024-04-24 02:51:54.000000 common-tools-ai-bnq-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 04:22:01.547120 common-tools-ai-bnq-0.1.2/bnq_py_core/
--rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.1.2/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     1090 2024-04-26 04:02:02.000000 common-tools-ai-bnq-0.1.2/bnq_py_core/cos_connect.py
--rw-rw-rw-   0        0        0     4664 2024-04-25 12:17:36.000000 common-tools-ai-bnq-0.1.2/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3274 2024-04-26 04:19:35.000000 common-tools-ai-bnq-0.1.2/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.1.2/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.2/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-04-26 04:22:01.568675 common-tools-ai-bnq-0.1.2/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0     2598 2024-04-26 04:22:01.000000 common-tools-ai-bnq-0.1.2/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-04-26 04:22:01.000000 common-tools-ai-bnq-0.1.2/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 04:22:01.000000 common-tools-ai-bnq-0.1.2/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-26 04:22:01.000000 common-tools-ai-bnq-0.1.2/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-26 04:22:01.000000 common-tools-ai-bnq-0.1.2/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 04:22:01.570863 common-tools-ai-bnq-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-04-26 04:21:54.000000 common-tools-ai-bnq-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:59:23.061529 common-tools-ai-bnq-0.1.3/
+-rw-rw-rw-   0        0        0     2598 2024-04-29 05:59:23.060528 common-tools-ai-bnq-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2236 2024-04-24 02:51:54.000000 common-tools-ai-bnq-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 05:59:23.043530 common-tools-ai-bnq-0.1.3/bnq_py_core/
+-rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     1090 2024-04-26 04:02:02.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/cos_connect.py
+-rw-rw-rw-   0        0        0     4617 2024-04-29 05:56:47.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3274 2024-04-26 04:19:35.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.3/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:59:23.059536 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0     2598 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 05:59:22.000000 common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 05:59:23.061529 common-tools-ai-bnq-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-04-29 05:59:08.000000 common-tools-ai-bnq-0.1.3/setup.py
```

### Comparing `common-tools-ai-bnq-0.1.2/PKG-INFO` & `common-tools-ai-bnq-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.2
+Version: 0.1.3
 Summary: Common tools of AI module for BNQ
 Author: BNQ
 Description-Content-Type: text/markdown
 Requires-Dist: structlog==23.1.0
 Requires-Dist: concurrent-log-handler==0.9.22
 Requires-Dist: nacos-sdk-python==0.1.12
 Requires-Dist: PyYAML==6.0.1
```

### Comparing `common-tools-ai-bnq-0.1.2/README.md` & `common-tools-ai-bnq-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.2/bnq_py_core/cos_connect.py` & `common-tools-ai-bnq-0.1.3/bnq_py_core/cos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.2/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.1.3/bnq_py_core/logger_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         """初始化log模块
 
         Returns:
 
         """
         if self.log_record_path is None:
             # 获取根目录路径，并创建日志文件夹
-            # self.log_record_path = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "log")
-            raise ValueError("log_dir is None")
+            self.log_record_path = os.path.join(os.getcwd(), "logs")
+            # raise ValueError("log_dir is None")
 
         pathlib.Path(self.log_record_path).mkdir(parents=True, exist_ok=True)
         log_filename = os.path.join(self.log_record_path, self.__filename)
         logging.config.dictConfig({
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
```

### Comparing `common-tools-ai-bnq-0.1.2/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.1.3/bnq_py_core/nacos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.2/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.1.3/bnq_py_core/read_conf_from_ini.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.2/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.1.3/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.2/common_tools_ai_bnq.egg-info/PKG-INFO` & `common-tools-ai-bnq-0.1.3/common_tools_ai_bnq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.2
+Version: 0.1.3
 Summary: Common tools of AI module for BNQ
 Author: BNQ
 Description-Content-Type: text/markdown
 Requires-Dist: structlog==23.1.0
 Requires-Dist: concurrent-log-handler==0.9.22
 Requires-Dist: nacos-sdk-python==0.1.12
 Requires-Dist: PyYAML==6.0.1
```

### Comparing `common-tools-ai-bnq-0.1.2/setup.py` & `common-tools-ai-bnq-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.22',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
```

