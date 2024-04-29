# Comparing `tmp/holytools-0.9.2.tar.gz` & `tmp/holytools-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holytools-0.9.2.tar", last modified: Fri Apr 26 15:22:23 2024, max compression
+gzip compressed data, was "holytools-0.9.3.tar", last modified: Mon Apr 29 12:31:23 2024, max compression
```

## Comparing `holytools-0.9.2.tar` & `holytools-0.9.3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.045792 holytools-0.9.2/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1072 2024-04-26 10:13:20.000000 holytools-0.9.2/LICENSE.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2790 2024-04-26 15:22:23.041792 holytools-0.9.2/PKG-INFO
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.017792 holytools-0.9.2/holytools/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.021792 holytools-0.9.2/holytools/abstract/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       81 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/abstract/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      704 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/abstract/enum.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.021792 holytools-0.9.2/holytools/abstract/serialization/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      139 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/abstract/serialization/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      805 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/abstract/serialization/dillable.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4388 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/abstract/serialization/jsondataclass.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      903 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/abstract/serialization/serializable.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.021792 holytools-0.9.2/holytools/abstract/tree/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       32 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/abstract/tree/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3393 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/abstract/tree/node.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.021792 holytools-0.9.2/holytools/configs/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       51 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/configs/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1846 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/configs/abstr.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2617 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/configs/impl.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.021792 holytools-0.9.2/holytools/crypto/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       42 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/crypto/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.021792 holytools-0.9.2/holytools/crypto/encrypt/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       41 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/crypto/encrypt/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2117 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/crypto/encrypt/aes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      262 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/crypto/encrypt/algo.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2041 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/crypto/encrypt/rsa.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.025792 holytools-0.9.2/holytools/crypto/hash/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       20 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/crypto/hash/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      828 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/crypto/hash/salt.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      643 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/crypto/hash/sha.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.025792 holytools-0.9.2/holytools/devtools/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.025792 holytools-0.9.2/holytools/devtools/inspection/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       93 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/inspection/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2790 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/inspection/module_inspect.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1354 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/inspection/type_inspect.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.025792 holytools-0.9.2/holytools/devtools/test/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       62 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/test/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2065 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/test/cases.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/test/configurable_unit.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4783 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/test/results.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4066 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/devtools/test/unit.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.025792 holytools-0.9.2/holytools/events/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      169 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/events/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1373 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/events/countdown.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      682 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/events/input_waiter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3133 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/events/task_scheduler.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/events/timer.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.025792 holytools-0.9.2/holytools/file/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       57 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.029792 holytools-0.9.2/holytools/file/mock/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1557 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/file_mock.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1024 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/mock.bin
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   171225 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/mock.csv
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   102796 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/mock.jpg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13264 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/mock.pdf
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2670 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/mock.png
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       89 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/mock.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)   775192 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/mock/mock.wav
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.033792 holytools-0.9.2/holytools/file/types/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      190 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/types/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1252 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/types/binary.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2152 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/types/file.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4855 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/types/image.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      950 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/file/types/plaintext.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.037792 holytools-0.9.2/holytools/fsys/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      116 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/fsys/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5213 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/fsys/fsys_node.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1821 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/fsys/location_manager.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2516 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/fsys/resource.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1715 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/fsys/save_manager.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.037792 holytools-0.9.2/holytools/hardware/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       91 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.037792 holytools-0.9.2/holytools/hardware/display/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       82 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/display/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2151 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/display/display.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3953 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/display/grid_draw.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3162 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/display/types.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.037792 holytools-0.9.2/holytools/hardware/input/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       84 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/input/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3207 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/input/keyboard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2137 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/input/mouse.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.037792 holytools-0.9.2/holytools/hardware/memory/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/memory/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3265 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/memory/drives.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      827 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/memory/ram.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2260 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/memory/usage.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.037792 holytools-0.9.2/holytools/hardware/microphone/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/microphone/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1385 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/hardware/microphone/recorder.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.041792 holytools-0.9.2/holytools/logging/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      149 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/logging/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3546 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/logging/customlogger.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1825 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/logging/interface.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      563 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/logging/log_settings.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.041792 holytools-0.9.2/holytools/network/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       87 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/network/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5058 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/network/adapter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      969 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/network/endpoint.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2221 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/network/ip.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.041792 holytools-0.9.2/holytools/userIO/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       31 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/userIO/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4140 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/userIO/cli.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1138 2024-04-26 10:49:47.000000 holytools-0.9.2/holytools/userIO/progr.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.041792 holytools-0.9.2/holytools/web/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/web/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1293 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/web/link_soup.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2145 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/web/search_engine.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3690 2024-04-26 10:13:20.000000 holytools-0.9.2/holytools/web/site_visitor.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-26 15:22:23.041792 holytools-0.9.2/holytools.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2790 2024-04-26 15:22:23.000000 holytools-0.9.2/holytools.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2947 2024-04-26 15:22:23.000000 holytools-0.9.2/holytools.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-26 15:22:23.000000 holytools-0.9.2/holytools.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      153 2024-04-26 15:22:23.000000 holytools-0.9.2/holytools.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       10 2024-04-26 15:22:23.000000 holytools-0.9.2/holytools.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-04-26 15:21:43.000000 holytools-0.9.2/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2072 2024-04-26 10:13:20.000000 holytools-0.9.2/readme.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      152 2024-04-26 10:13:20.000000 holytools-0.9.2/requirements.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-26 15:22:23.045792 holytools-0.9.2/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1072 2024-04-26 10:13:20.000000 holytools-0.9.3/LICENSE.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2818 2024-04-29 12:31:23.945153 holytools-0.9.3/PKG-INFO
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.933152 holytools-0.9.3/holytools/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.933152 holytools-0.9.3/holytools/abstract/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       81 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      704 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/enum.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/abstract/serialization/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      139 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/serialization/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      805 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/serialization/dillable.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4388 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/serialization/jsondataclass.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      903 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/serialization/serializable.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/abstract/tree/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       32 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/tree/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3393 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/abstract/tree/node.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/configs/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       51 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/configs/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1846 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/configs/abstr.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2617 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/configs/impl.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/crypto/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       42 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/crypto/encrypt/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       41 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/encrypt/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2117 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/encrypt/aes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      262 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/encrypt/algo.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2041 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/encrypt/rsa.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/crypto/hash/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       20 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/hash/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      828 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/hash/salt.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      643 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/crypto/hash/sha.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/devtools/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       45 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/devtools/inspection/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       93 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/inspection/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2790 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/inspection/module_inspect.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1354 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/inspection/type_inspect.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/devtools/test/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       62 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2065 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/cases.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/configurable_unit.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4783 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/results.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4066 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/devtools/test/unit.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/events/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      169 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1373 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/countdown.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      682 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/input_waiter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3133 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/task_scheduler.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/events/timer.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.937152 holytools-0.9.3/holytools/file/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       57 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/file/mock/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1557 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/file_mock.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1024 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.bin
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   171225 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.csv
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   102796 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.jpg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13264 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.pdf
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2670 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.png
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       89 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)   775192 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/mock/mock.wav
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/file/types/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      190 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1252 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/binary.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2152 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/file.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4855 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/image.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      950 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/file/types/plaintext.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/fsys/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      116 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5213 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/fsys_node.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1821 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/location_manager.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2516 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/resource.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1715 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/fsys/save_manager.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       91 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/display/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       82 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/display/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2151 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/display/display.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3953 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/display/grid_draw.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3162 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/display/types.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/input/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       84 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/input/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3207 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/input/keyboard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2137 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/input/mouse.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/memory/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/memory/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3265 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/memory/drives.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      827 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/memory/ram.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2260 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/memory/usage.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.941152 holytools-0.9.3/holytools/hardware/microphone/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/microphone/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1385 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/hardware/microphone/recorder.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools/logging/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      149 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/logging/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3546 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/logging/customlogger.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1825 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/logging/interface.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      563 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/logging/log_settings.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools/network/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       87 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/network/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5058 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/network/adapter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      969 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/network/endpoint.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2221 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/network/ip.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools/userIO/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       61 2024-04-29 12:23:52.000000 holytools-0.9.3/holytools/userIO/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4140 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/userIO/cli.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2319 2024-04-29 12:29:15.000000 holytools-0.9.3/holytools/userIO/progr.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools/web/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       92 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/web/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1293 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/web/link_soup.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2145 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/web/search_engine.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3690 2024-04-26 10:13:20.000000 holytools-0.9.3/holytools/web/site_visitor.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-29 12:31:23.945153 holytools-0.9.3/holytools.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2818 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2947 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      166 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       10 2024-04-29 12:31:23.000000 holytools-0.9.3/holytools.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      463 2024-04-29 12:31:01.000000 holytools-0.9.3/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2072 2024-04-26 10:13:20.000000 holytools-0.9.3/readme.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      166 2024-04-29 12:28:15.000000 holytools-0.9.3/requirements.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-29 12:31:23.945153 holytools-0.9.3/setup.cfg
```

### Comparing `holytools-0.9.2/LICENSE.txt` & `holytools-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/PKG-INFO` & `holytools-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holytools
-Version: 0.9.2
+Version: 0.9.3
 Summary: Collection of general python utilities for future projects
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
 Project-URL: repository, https://github.com/Somerandomguy10111/holytools
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: func_timeout
@@ -18,14 +18,15 @@
 Requires-Dist: PyYAML
 Requires-Dist: orjson
 Requires-Dist: mss
 Requires-Dist: screeninfo
 Requires-Dist: pynput
 Requires-Dist: pillow
 Requires-Dist: configobj
+Requires-Dist: progressbar2
 
 ## Holytools
 A collection of general utilities in various very general areas that aim for simplicity in use. 
 Functionalities include:
 
 - object serialization -> holytools.abstract.serialization
 - fileIO and mock files -> holytools.file
```

### Comparing `holytools-0.9.2/holytools/abstract/enum.py` & `holytools-0.9.3/holytools/abstract/enum.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/abstract/serialization/dillable.py` & `holytools-0.9.3/holytools/abstract/serialization/dillable.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/abstract/serialization/jsondataclass.py` & `holytools-0.9.3/holytools/abstract/serialization/jsondataclass.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/abstract/serialization/serializable.py` & `holytools-0.9.3/holytools/abstract/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/abstract/tree/node.py` & `holytools-0.9.3/holytools/abstract/tree/node.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/configs/abstr.py` & `holytools-0.9.3/holytools/configs/abstr.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/configs/impl.py` & `holytools-0.9.3/holytools/configs/impl.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/crypto/encrypt/aes.py` & `holytools-0.9.3/holytools/crypto/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/crypto/encrypt/rsa.py` & `holytools-0.9.3/holytools/crypto/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/crypto/hash/salt.py` & `holytools-0.9.3/holytools/crypto/hash/salt.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/crypto/hash/sha.py` & `holytools-0.9.3/holytools/crypto/hash/sha.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/devtools/inspection/module_inspect.py` & `holytools-0.9.3/holytools/devtools/inspection/module_inspect.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/devtools/inspection/type_inspect.py` & `holytools-0.9.3/holytools/devtools/inspection/type_inspect.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/devtools/test/cases.py` & `holytools-0.9.3/holytools/devtools/test/cases.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/devtools/test/results.py` & `holytools-0.9.3/holytools/devtools/test/results.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/devtools/test/unit.py` & `holytools-0.9.3/holytools/devtools/test/unit.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/events/countdown.py` & `holytools-0.9.3/holytools/events/countdown.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/events/input_waiter.py` & `holytools-0.9.3/holytools/events/input_waiter.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/events/task_scheduler.py` & `holytools-0.9.3/holytools/events/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/mock/file_mock.py` & `holytools-0.9.3/holytools/file/mock/file_mock.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/mock/mock.csv` & `holytools-0.9.3/holytools/file/mock/mock.csv`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/mock/mock.jpg` & `holytools-0.9.3/holytools/file/mock/mock.jpg`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/mock/mock.pdf` & `holytools-0.9.3/holytools/file/mock/mock.pdf`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/mock/mock.png` & `holytools-0.9.3/holytools/file/mock/mock.png`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/mock/mock.wav` & `holytools-0.9.3/holytools/file/mock/mock.wav`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/types/binary.py` & `holytools-0.9.3/holytools/file/types/binary.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/types/file.py` & `holytools-0.9.3/holytools/file/types/file.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/types/image.py` & `holytools-0.9.3/holytools/file/types/image.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/file/types/plaintext.py` & `holytools-0.9.3/holytools/file/types/plaintext.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/fsys/fsys_node.py` & `holytools-0.9.3/holytools/fsys/fsys_node.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/fsys/location_manager.py` & `holytools-0.9.3/holytools/fsys/location_manager.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/fsys/resource.py` & `holytools-0.9.3/holytools/fsys/resource.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/fsys/save_manager.py` & `holytools-0.9.3/holytools/fsys/save_manager.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/display/display.py` & `holytools-0.9.3/holytools/hardware/display/display.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/display/grid_draw.py` & `holytools-0.9.3/holytools/hardware/display/grid_draw.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/display/types.py` & `holytools-0.9.3/holytools/hardware/display/types.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/input/keyboard.py` & `holytools-0.9.3/holytools/hardware/input/keyboard.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/input/mouse.py` & `holytools-0.9.3/holytools/hardware/input/mouse.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/memory/drives.py` & `holytools-0.9.3/holytools/hardware/memory/drives.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/memory/ram.py` & `holytools-0.9.3/holytools/hardware/memory/ram.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/memory/usage.py` & `holytools-0.9.3/holytools/hardware/memory/usage.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/hardware/microphone/recorder.py` & `holytools-0.9.3/holytools/hardware/microphone/recorder.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/logging/customlogger.py` & `holytools-0.9.3/holytools/logging/customlogger.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/logging/interface.py` & `holytools-0.9.3/holytools/logging/interface.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/logging/log_settings.py` & `holytools-0.9.3/holytools/logging/log_settings.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/network/adapter.py` & `holytools-0.9.3/holytools/network/adapter.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/network/endpoint.py` & `holytools-0.9.3/holytools/network/endpoint.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/network/ip.py` & `holytools-0.9.3/holytools/network/ip.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/userIO/cli.py` & `holytools-0.9.3/holytools/userIO/cli.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/web/link_soup.py` & `holytools-0.9.3/holytools/web/link_soup.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/web/search_engine.py` & `holytools-0.9.3/holytools/web/search_engine.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools/web/site_visitor.py` & `holytools-0.9.3/holytools/web/site_visitor.py`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/holytools.egg-info/PKG-INFO` & `holytools-0.9.3/holytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holytools
-Version: 0.9.2
+Version: 0.9.3
 Summary: Collection of general python utilities for future projects
 Author-email: Daniel Hollarek <daniel.hollarek@googlemail.com>
 Project-URL: repository, https://github.com/Somerandomguy10111/holytools
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: func_timeout
@@ -18,14 +18,15 @@
 Requires-Dist: PyYAML
 Requires-Dist: orjson
 Requires-Dist: mss
 Requires-Dist: screeninfo
 Requires-Dist: pynput
 Requires-Dist: pillow
 Requires-Dist: configobj
+Requires-Dist: progressbar2
 
 ## Holytools
 A collection of general utilities in various very general areas that aim for simplicity in use. 
 Functionalities include:
 
 - object serialization -> holytools.abstract.serialization
 - fileIO and mock files -> holytools.file
```

### Comparing `holytools-0.9.2/holytools.egg-info/SOURCES.txt` & `holytools-0.9.3/holytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `holytools-0.9.2/readme.md` & `holytools-0.9.3/readme.md`

 * *Files identical despite different names*

