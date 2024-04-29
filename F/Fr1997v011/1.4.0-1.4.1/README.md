# Comparing `tmp/Fr1997v011-1.4.0.tar.gz` & `tmp/Fr1997v011-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.4.0.tar", last modified: Sun Apr 28 08:18:45 2024, max compression
+gzip compressed data, was "Fr1997v011-1.4.1.tar", last modified: Sun Apr 28 08:52:37 2024, max compression
```

## Comparing `Fr1997v011-1.4.0.tar` & `Fr1997v011-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.136817 Fr1997v011-1.4.0/
-drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.121280 Fr1997v011-1.4.0/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-28 08:18:44.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-28 08:18:44.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 08:18:44.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-28 07:52:40.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-28 08:18:44.000000 Fr1997v011-1.4.0/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.0/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-28 08:18:45.134817 Fr1997v011-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-28 07:52:43.000000 Fr1997v011-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.123796 Fr1997v011-1.4.0/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.0/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.129797 Fr1997v011-1.4.0/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.0/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   172508 2024-04-28 08:18:42.000000 Fr1997v011-1.4.0/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:18:45.132800 Fr1997v011-1.4.0/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.0/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-28 08:18:45.136817 Fr1997v011-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-28 07:52:38.000000 Fr1997v011-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.595714 Fr1997v011-1.4.1/
+drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.586516 Fr1997v011-1.4.1/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-28 08:52:37.594615 Fr1997v011-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-28 08:52:37.000000 Fr1997v011-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.587615 Fr1997v011-1.4.1/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.1/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.590616 Fr1997v011-1.4.1/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.1/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   172506 2024-04-28 08:51:02.000000 Fr1997v011-1.4.1/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-28 08:52:37.592616 Fr1997v011-1.4.1/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.1/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-28 08:52:37.595714 Fr1997v011-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-28 08:52:34.000000 Fr1997v011-1.4.1/setup.py
```

### Comparing `Fr1997v011-1.4.0/LICENSE` & `Fr1997v011-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.0/README.md` & `Fr1997v011-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.4.0.tar.gz
+pip install dist/Fr1997v011-1.4.1.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.4.0/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.4.1/fr1997_mode/mode_func/all_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -4345,8 +4345,7 @@
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
 
-
```

