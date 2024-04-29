# Comparing `tmp/nonebot_plugin_simulator_xiuxian-0.5.36.tar.gz` & `tmp/nonebot_plugin_simulator_xiuxian-0.5.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.36.tar", last modified: Sun Apr 28 20:26:44 2024, max compression
+gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.40.tar", last modified: Sun Apr 28 23:38:29 2024, max compression
```

## Comparing `nonebot_plugin_simulator_xiuxian-0.5.36.tar` & `nonebot_plugin_simulator_xiuxian-0.5.40.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 20:26:44.001444 nonebot_plugin_simulator_xiuxian-0.5.36/
--rw-rw-rw-   0        0        0     1089 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/LICENSE
--rw-rw-rw-   0        0        0     6672 2024-04-28 20:26:44.001444 nonebot_plugin_simulator_xiuxian-0.5.36/PKG-INFO
--rw-rw-rw-   0        0        0     5676 2024-04-27 18:59:32.000000 nonebot_plugin_simulator_xiuxian-0.5.36/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 20:26:43.986445 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/
--rw-rw-rw-   0        0        0     1352 2024-04-28 19:32:56.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/__init__.py
--rw-rw-rw-   0        0        0     1960 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/cd_manager.py
--rw-rw-rw-   0        0        0      361 2024-04-25 00:35:49.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/config.py
--rw-rw-rw-   0        0        0     2849 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/data_source.py
--rw-rw-rw-   0        0        0     1787 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/exp_util.py
--rw-rw-rw-   0        0        0     1354 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/help.py
--rw-rw-rw-   0        0        0     4430 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/item_json.py
--rw-rw-rw-   0        0        0    50728 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/player_fight.py
--rw-rw-rw-   0        0        0     8141 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/read_buff.py
--rw-rw-rw-   0        0        0     8555 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/utils.py
--rw-rw-rw-   0        0        0    54293 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
--rw-rw-rw-   0        0        0     5784 2024-04-25 00:26:19.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
--rw-rw-rw-   0        0        0      787 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
--rw-rw-rw-   0        0        0     2199 2024-04-25 14:18:36.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:26:44.000445 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian.egg-info/
--rw-rw-rw-   0        0        0     6672 2024-04-28 20:26:43.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      979 2024-04-28 20:26:43.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 20:26:43.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2024-04-28 20:26:43.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2024-04-28 20:26:43.000000 nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-28 20:26:44.005443 nonebot_plugin_simulator_xiuxian-0.5.36/setup.cfg
--rw-rw-rw-   0        0        0     1374 2024-04-28 20:26:30.000000 nonebot_plugin_simulator_xiuxian-0.5.36/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 23:38:29.702530 nonebot_plugin_simulator_xiuxian-0.5.40/
+-rw-rw-rw-   0        0        0     1089 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/LICENSE
+-rw-rw-rw-   0        0        0     6672 2024-04-28 23:38:29.702530 nonebot_plugin_simulator_xiuxian-0.5.40/PKG-INFO
+-rw-rw-rw-   0        0        0     5676 2024-04-27 18:59:32.000000 nonebot_plugin_simulator_xiuxian-0.5.40/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 23:38:29.690529 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/
+-rw-rw-rw-   0        0        0     1352 2024-04-28 19:32:56.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/__init__.py
+-rw-rw-rw-   0        0        0     1960 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/cd_manager.py
+-rw-rw-rw-   0        0        0      361 2024-04-25 00:35:49.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/config.py
+-rw-rw-rw-   0        0        0     2849 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/data_source.py
+-rw-rw-rw-   0        0        0     1787 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/exp_util.py
+-rw-rw-rw-   0        0        0     1354 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/help.py
+-rw-rw-rw-   0        0        0     4430 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/item_json.py
+-rw-rw-rw-   0        0        0    50728 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/player_fight.py
+-rw-rw-rw-   0        0        0     8141 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/read_buff.py
+-rw-rw-rw-   0        0        0     8555 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/utils.py
+-rw-rw-rw-   0        0        0    54293 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
+-rw-rw-rw-   0        0        0     5784 2024-04-25 00:26:19.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
+-rw-rw-rw-   0        0        0      787 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
+-rw-rw-rw-   0        0        0     2199 2024-04-25 14:18:36.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
+drwxrwxrwx   0        0        0        0 2024-04-28 23:38:29.702530 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian.egg-info/
+-rw-rw-rw-   0        0        0     6672 2024-04-28 23:38:29.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      979 2024-04-28 23:38:29.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 23:38:29.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2024-04-28 23:38:29.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-04-28 23:38:29.000000 nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-28 23:38:29.704490 nonebot_plugin_simulator_xiuxian-0.5.40/setup.cfg
+-rw-rw-rw-   0        0        0     1374 2024-04-28 23:38:24.000000 nonebot_plugin_simulator_xiuxian-0.5.40/setup.py
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/LICENSE` & `nonebot_plugin_simulator_xiuxian-0.5.40/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/PKG-INFO` & `nonebot_plugin_simulator_xiuxian-0.5.40/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_simulator_xiuxian
-Version: 0.5.36
+Version: 0.5.40
 Summary: 修仙
 Home-page: https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian
 Author: 甘城菜月
 Author-email: 2859385794@qq.com
 License: MIT license
 Platform: all
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 Requires-Dist: nonebot-plugin-apscheduler
 Requires-Dist: Pillow==9.5.0
 Requires-Dist: pydantic
 Requires-Dist: wcwidth
 Requires-Dist: ujson
 Requires-Dist: xiuxian-base
 Requires-Dist: xiuxian-bank
-Requires-Dist: xiuxian-base
+Requires-Dist: xiuxian-back
 Requires-Dist: xiuxian-boss
 Requires-Dist: xiuxian-buff
 Requires-Dist: xiuxian-info
 Requires-Dist: xiuxian-mixelixir
 Requires-Dist: xiuxian-rift
 Requires-Dist: xiuxian-sect
 Requires-Dist: xiuxian-work
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_simulator_xiuxian Version: 0.5.36
+Metadata-Version: 2.1 Name: nonebot_plugin_simulator_xiuxian Version: 0.5.40
 Summary: ä¿®ä» Home-page: https://github.com/luoyefufeng/
 nonebot_plugin_simulator_xiuxian Author: çåèæ Author-email:
 2859385794@qq.com License: MIT license Platform: all Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-Dist:
 nonebot-adapter-onebot Requires-Dist: wget Requires-Dist: nonebot-plugin-
 apscheduler Requires-Dist: Pillow==9.5.0 Requires-Dist: pydantic Requires-Dist:
 wcwidth Requires-Dist: ujson Requires-Dist: xiuxian-base Requires-Dist:
-xiuxian-bank Requires-Dist: xiuxian-base Requires-Dist: xiuxian-boss Requires-
+xiuxian-bank Requires-Dist: xiuxian-back Requires-Dist: xiuxian-boss Requires-
 Dist: xiuxian-buff Requires-Dist: xiuxian-info Requires-Dist: xiuxian-mixelixir
 Requires-Dist: xiuxian-rift Requires-Dist: xiuxian-sect Requires-Dist: xiuxian-
 work
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
              # ä¿®ä»1.0 _â¨ QQç¾¤èä¿®ä»æå­æ¸¸æâ¨_ ð§¬
                 æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½ï¼ð
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/README.md` & `nonebot_plugin_simulator_xiuxian-0.5.40/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/__init__.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/cd_manager.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/cd_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/data_source.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/exp_util.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/exp_util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/help.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/item_json.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/item_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/player_fight.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/player_fight.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/read_buff.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/read_buff.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/utils.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/xiuxian_config.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/xiuxian_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_simulator_xiuxian
-Version: 0.5.36
+Version: 0.5.40
 Summary: 修仙
 Home-page: https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian
 Author: 甘城菜月
 Author-email: 2859385794@qq.com
 License: MIT license
 Platform: all
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 Requires-Dist: nonebot-plugin-apscheduler
 Requires-Dist: Pillow==9.5.0
 Requires-Dist: pydantic
 Requires-Dist: wcwidth
 Requires-Dist: ujson
 Requires-Dist: xiuxian-base
 Requires-Dist: xiuxian-bank
-Requires-Dist: xiuxian-base
+Requires-Dist: xiuxian-back
 Requires-Dist: xiuxian-boss
 Requires-Dist: xiuxian-buff
 Requires-Dist: xiuxian-info
 Requires-Dist: xiuxian-mixelixir
 Requires-Dist: xiuxian-rift
 Requires-Dist: xiuxian-sect
 Requires-Dist: xiuxian-work
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_simulator_xiuxian Version: 0.5.36
+Metadata-Version: 2.1 Name: nonebot_plugin_simulator_xiuxian Version: 0.5.40
 Summary: ä¿®ä» Home-page: https://github.com/luoyefufeng/
 nonebot_plugin_simulator_xiuxian Author: çåèæ Author-email:
 2859385794@qq.com License: MIT license Platform: all Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-Dist:
 nonebot-adapter-onebot Requires-Dist: wget Requires-Dist: nonebot-plugin-
 apscheduler Requires-Dist: Pillow==9.5.0 Requires-Dist: pydantic Requires-Dist:
 wcwidth Requires-Dist: ujson Requires-Dist: xiuxian-base Requires-Dist:
-xiuxian-bank Requires-Dist: xiuxian-base Requires-Dist: xiuxian-boss Requires-
+xiuxian-bank Requires-Dist: xiuxian-back Requires-Dist: xiuxian-boss Requires-
 Dist: xiuxian-buff Requires-Dist: xiuxian-info Requires-Dist: xiuxian-mixelixir
 Requires-Dist: xiuxian-rift Requires-Dist: xiuxian-sect Requires-Dist: xiuxian-
 work
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
              # ä¿®ä»1.0 _â¨ QQç¾¤èä¿®ä»æå­æ¸¸æâ¨_ ð§¬
                 æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½ï¼ð
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt` & `nonebot_plugin_simulator_xiuxian-0.5.40/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.36/setup.py` & `nonebot_plugin_simulator_xiuxian-0.5.40/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_namespace_packages,find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='nonebot_plugin_simulator_xiuxian',
-    version='0.5.36',
+    version='0.5.40',
     description='修仙',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='甘城菜月',
     author_email='2859385794@qq.com',
     license='MIT license',
     include_package_data=True,
@@ -19,15 +19,15 @@
                       "nonebot-plugin-apscheduler",
                       "Pillow==9.5.0",
                       "pydantic",
                       "wcwidth",
                       "ujson",
                       "xiuxian-base",
                       "xiuxian-bank",
-                      "xiuxian-base",
+                      "xiuxian-back",
                       "xiuxian-boss",
                       "xiuxian-buff",
                       "xiuxian-info",
                       "xiuxian-mixelixir",
                       "xiuxian-rift",
                       "xiuxian-sect",
                       "xiuxian-work"],
```

