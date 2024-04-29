# Comparing `tmp/First_pypi-0.1.tar.gz` & `tmp/First_pypi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "First_pypi-0.1.tar", last modified: Mon Apr 29 06:52:04 2024, max compression
+gzip compressed data, was "First_pypi-0.2.tar", last modified: Mon Apr 29 07:04:12 2024, max compression
```

## Comparing `First_pypi-0.1.tar` & `First_pypi-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kushalbanda   (501) staff       (20)        0 2024-04-29 06:52:04.173891 First_pypi-0.1/
-drwxr-xr-x   0 kushalbanda   (501) staff       (20)        0 2024-04-29 06:52:04.173118 First_pypi-0.1/First_pypi.egg-info/
--rw-r--r--   0 kushalbanda   (501) staff       (20)       52 2024-04-29 06:52:04.000000 First_pypi-0.1/First_pypi.egg-info/PKG-INFO
--rw-r--r--   0 kushalbanda   (501) staff       (20)      204 2024-04-29 06:52:04.000000 First_pypi-0.1/First_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 kushalbanda   (501) staff       (20)        1 2024-04-29 06:52:04.000000 First_pypi-0.1/First_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 kushalbanda   (501) staff       (20)       15 2024-04-29 06:52:04.000000 First_pypi-0.1/First_pypi.egg-info/top_level.txt
--rw-r--r--   0 kushalbanda   (501) staff       (20)       52 2024-04-29 06:52:04.173770 First_pypi-0.1/PKG-INFO
--rw-r--r--   0 kushalbanda   (501) staff       (20)        0 2024-04-29 06:48:03.000000 First_pypi-0.1/README.md
-drwxr-xr-x   0 kushalbanda   (501) staff       (20)        0 2024-04-29 06:52:04.173485 First_pypi-0.1/pixegami_hello/
--rw-r--r--   0 kushalbanda   (501) staff       (20)       23 2024-04-29 06:48:43.000000 First_pypi-0.1/pixegami_hello/__init__.py
--rw-r--r--   0 kushalbanda   (501) staff       (20)       42 2024-04-29 06:48:23.000000 First_pypi-0.1/pixegami_hello/main.py
--rw-r--r--   0 kushalbanda   (501) staff       (20)       38 2024-04-29 06:52:04.173934 First_pypi-0.1/setup.cfg
--rw-r--r--   0 kushalbanda   (501) staff       (20)      226 2024-04-29 06:50:34.000000 First_pypi-0.1/setup.py
+drwxr-xr-x   0 kushalbanda   (501) staff       (20)        0 2024-04-29 07:04:12.467415 First_pypi-0.2/
+drwxr-xr-x   0 kushalbanda   (501) staff       (20)        0 2024-04-29 07:04:12.464316 First_pypi-0.2/First_pypi.egg-info/
+-rw-r--r--   0 kushalbanda   (501) staff       (20)       52 2024-04-29 07:04:12.000000 First_pypi-0.2/First_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 kushalbanda   (501) staff       (20)      241 2024-04-29 07:04:12.000000 First_pypi-0.2/First_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 kushalbanda   (501) staff       (20)        1 2024-04-29 07:04:12.000000 First_pypi-0.2/First_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 kushalbanda   (501) staff       (20)       56 2024-04-29 07:04:12.000000 First_pypi-0.2/First_pypi.egg-info/entry_points.txt
+-rw-r--r--   0 kushalbanda   (501) staff       (20)       15 2024-04-29 07:04:12.000000 First_pypi-0.2/First_pypi.egg-info/top_level.txt
+-rw-r--r--   0 kushalbanda   (501) staff       (20)       52 2024-04-29 07:04:12.467261 First_pypi-0.2/PKG-INFO
+-rw-r--r--   0 kushalbanda   (501) staff       (20)        0 2024-04-29 06:48:03.000000 First_pypi-0.2/README.md
+drwxr-xr-x   0 kushalbanda   (501) staff       (20)        0 2024-04-29 07:04:12.464646 First_pypi-0.2/pixegami_hello/
+-rw-r--r--   0 kushalbanda   (501) staff       (20)       23 2024-04-29 06:48:43.000000 First_pypi-0.2/pixegami_hello/__init__.py
+-rw-r--r--   0 kushalbanda   (501) staff       (20)       42 2024-04-29 06:48:23.000000 First_pypi-0.2/pixegami_hello/main.py
+-rw-r--r--   0 kushalbanda   (501) staff       (20)       38 2024-04-29 07:04:12.467469 First_pypi-0.2/setup.cfg
+-rw-r--r--   0 kushalbanda   (501) staff       (20)      348 2024-04-29 07:03:01.000000 First_pypi-0.2/setup.py
```

