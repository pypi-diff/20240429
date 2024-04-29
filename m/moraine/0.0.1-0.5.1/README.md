# Comparing `tmp/moraine-0.0.1.tar.gz` & `tmp/moraine-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moraine-0.0.1.tar", last modified: Sat Oct 21 01:09:00 2023, max compression
+gzip compressed data, was "moraine-0.5.1.tar", last modified: Mon Apr 29 02:27:45 2024, max compression
```

## Comparing `moraine-0.0.1.tar` & `moraine-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,40 @@
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2023-10-21 01:09:00.000000 moraine-0.0.1/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    11337 2023-04-27 10:12:58.000000 moraine-0.0.1/LICENSE
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      111 2023-04-27 10:12:58.000000 moraine-0.0.1/MANIFEST.in
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     1052 2023-10-21 01:09:00.000000 moraine-0.0.1/PKG-INFO
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      284 2023-10-21 01:04:48.000000 moraine-0.0.1/README.md
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)       22 2023-10-21 01:04:43.000000 moraine-0.0.1/moraine/__init__.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      357 2023-10-21 01:04:43.000000 moraine-0.0.1/moraine/_modidx.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      142 2023-10-21 01:04:43.000000 moraine-0.0.1/moraine/core.py
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     1052 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/PKG-INFO
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      324 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/SOURCES.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        1 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/dependency_links.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)       36 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/entry_points.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        1 2023-10-21 01:08:18.000000 moraine-0.0.1/moraine.egg-info/not-zip-safe
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        7 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/requires.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        8 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/top_level.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      949 2023-10-21 01:04:42.000000 moraine-0.0.1/settings.ini
--rw-rw-r--   0 kangl    (509674) kangl    (509674)       38 2023-10-21 01:09:00.000000 moraine-0.0.1/setup.cfg
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     2596 2023-04-27 10:12:58.000000 moraine-0.0.1/setup.py
+drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2024-04-29 02:27:45.000000 moraine-0.5.1/
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)    33253 2023-01-13 02:56:44.000000 moraine-0.5.1/LICENSE
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)      111 2023-01-13 02:56:44.000000 moraine-0.5.1/MANIFEST.in
+-rw-r--r--   0 kangl    (509674) kangl    (509674)     9344 2024-04-29 02:27:45.000000 moraine-0.5.1/PKG-INFO
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     8100 2024-04-29 02:09:02.000000 moraine-0.5.1/README.md
+drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine/
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)      191 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/__init__.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)    16297 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/_modidx.py
+drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2024-04-29 02:27:45.000000 moraine-0.5.1/moraine/cli/
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)      402 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/__init__.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     7175 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/co.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)    19775 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/load.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     2537 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/logging.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     2409 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/math.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)    26890 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/cli/pc.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     5740 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/pl.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)    22427 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/plot.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     2758 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/ps.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     7198 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/shp.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     2786 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/cli/transform.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     9136 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/co.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     4386 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/coord_.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)    12046 2024-04-29 02:13:21.000000 moraine-0.5.1/moraine/pc.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     1340 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/pl.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     6731 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/plot.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     2065 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/ps.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)    13999 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/rtree.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     3362 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/shp.py
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)      444 2024-04-29 02:13:22.000000 moraine-0.5.1/moraine/utils_.py
+drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/
+-rw-r--r--   0 kangl    (509674) kangl    (509674)     9344 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/PKG-INFO
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)      671 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/SOURCES.txt
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)        1 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/dependency_links.txt
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)       36 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/entry_points.txt
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)        1 2024-04-28 00:33:02.000000 moraine-0.5.1/moraine.egg-info/not-zip-safe
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)      200 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/requires.txt
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)        8 2024-04-29 02:27:44.000000 moraine-0.5.1/moraine.egg-info/top_level.txt
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     1317 2024-04-27 22:49:16.000000 moraine-0.5.1/settings.ini
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)       38 2024-04-29 02:27:45.000000 moraine-0.5.1/setup.cfg
+-rw-rw-r--   0 kangl    (509674) kangl    (509674)     2548 2023-01-13 02:56:44.000000 moraine-0.5.1/setup.py
```

### Comparing `moraine-0.0.1/setup.py` & `moraine-0.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
-import setuptools, shlex
+import setuptools
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
-config.read('settings.ini', encoding='utf-8')
+config.read('settings.ini')
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
 expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
 for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
 setup_cfg = {o:cfg[o] for o in cfg_keys}
 
 licenses = {
     'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
     'mit': ('MIT License', 'OSI Approved :: MIT License'),
     'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'gpl3': ('GNU General Public License v3.0 only', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
     'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
 py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
 
-requirements = shlex.split(cfg.get('requirements', ''))
-if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
+requirements = cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 dev_requirements = (cfg.get('dev_requirements') or '').split()
 
 setuptools.setup(
     name = cfg['lib_name'],
     license = lic[0],
@@ -41,15 +41,15 @@
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md', encoding='utf-8').read(),
+    long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     entry_points = {
         'console_scripts': cfg.get('console_scripts','').split(),
         'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
     },
     **setup_cfg)
```

