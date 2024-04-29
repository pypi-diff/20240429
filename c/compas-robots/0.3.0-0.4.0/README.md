# Comparing `tmp/compas_robots-0.3.0.tar.gz` & `tmp/compas_robots-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_robots-0.3.0.tar", last modified: Tue Feb 20 10:12:33 2024, max compression
+gzip compressed data, was "compas_robots-0.4.0.tar", last modified: Mon Apr 29 15:46:36 2024, max compression
```

## Comparing `compas_robots-0.3.0.tar` & `compas_robots-0.4.0.tar`

### file list

```diff
@@ -1,79 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.454964 compas_robots-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-20 10:12:23.000000 compas_robots-0.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-20 10:12:23.000000 compas_robots-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-20 10:12:23.000000 compas_robots-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-20 10:12:23.000000 compas_robots-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-20 10:12:33.454964 compas_robots-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-20 10:12:23.000000 compas_robots-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-20 10:12:23.000000 compas_robots-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-20 10:12:23.000000 compas_robots-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-20 10:12:33.454964 compas_robots-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-20 10:12:23.000000 compas_robots-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.430965 compas_robots-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.434965 compas_robots-0.3.0/src/compas_robots/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.434965 compas_robots-0.3.0/src/compas_robots/blender/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/blender/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.434965 compas_robots-0.3.0/src/compas_robots/blender/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/blender/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/blender/scene/robotmodelobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.430965 compas_robots-0.3.0/src/compas_robots/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.430965 compas_robots-0.3.0/src/compas_robots/data/ur_description/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.430965 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.430965 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.438964 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/
--rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/base.stl
--rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/forearm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/shoulder.stl
--rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/upperarm.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist1.stl
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist2.stl
--rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist3.stl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.450965 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/
--rw-r--r--   0 runner    (1001) docker     (127)   193387 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/base.obj
--rw-r--r--   0 runner    (1001) docker     (127)  1960914 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/forearm.obj
--rw-r--r--   0 runner    (1001) docker     (127)  1308382 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/shoulder.obj
--rw-r--r--   0 runner    (1001) docker     (127)  2936777 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/upperarm.obj
--rw-r--r--   0 runner    (1001) docker     (127)  1354955 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist1.obj
--rw-r--r--   0 runner    (1001) docker     (127)  1352873 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist2.obj
--rw-r--r--   0 runner    (1001) docker     (127)   164202 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist3.obj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.450965 compas_robots-0.3.0/src/compas_robots/data/ur_description/urdf/
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/data/ur_description/urdf/ur5.urdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.450965 compas_robots-0.3.0/src/compas_robots/files/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/files/urdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.450965 compas_robots-0.3.0/src/compas_robots/ghpython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/ghpython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.450965 compas_robots-0.3.0/src/compas_robots/ghpython/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/ghpython/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/ghpython/scene/robotmodelobject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.450965 compas_robots-0.3.0/src/compas_robots/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/model/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/model/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/model/link.py
--rw-r--r--   0 runner    (1001) docker     (127)    39083 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/model/robot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/model/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.450965 compas_robots-0.3.0/src/compas_robots/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/resources/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/resources/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/resources/mesh_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.454964 compas_robots-0.3.0/src/compas_robots/rhino/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/rhino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/rhino/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.454964 compas_robots-0.3.0/src/compas_robots/rhino/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/rhino/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/rhino/scene/robotmodelobject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.454964 compas_robots-0.3.0/src/compas_robots/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-02-20 10:12:23.000000 compas_robots-0.3.0/src/compas_robots/scene/baserobotmodelobject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:12:33.434965 compas_robots-0.3.0/src/compas_robots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-20 10:12:33.000000 compas_robots-0.3.0/src/compas_robots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-20 10:12:33.000000 compas_robots-0.3.0/src/compas_robots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 10:12:33.000000 compas_robots-0.3.0/src/compas_robots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 10:12:33.000000 compas_robots-0.3.0/src/compas_robots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-20 10:12:33.000000 compas_robots-0.3.0/src/compas_robots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-20 10:12:33.000000 compas_robots-0.3.0/src/compas_robots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-29 15:46:24.000000 compas_robots-0.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-29 15:46:24.000000 compas_robots-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-29 15:46:24.000000 compas_robots-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-29 15:46:24.000000 compas_robots-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-29 15:46:36.945388 compas_robots-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-29 15:46:24.000000 compas_robots-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-29 15:46:24.000000 compas_robots-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 15:46:24.000000 compas_robots-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 15:46:36.949388 compas_robots-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-29 15:46:24.000000 compas_robots-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.921388 compas_robots-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.925388 compas_robots-0.4.0/src/compas_robots/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.929388 compas_robots-0.4.0/src/compas_robots/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/blender/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.929388 compas_robots-0.4.0/src/compas_robots/blender/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/blender/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/blender/scene/robotmodelobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20730 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.921388 compas_robots-0.4.0/src/compas_robots/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.925388 compas_robots-0.4.0/src/compas_robots/data/ur_description/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.925388 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.925388 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.929388 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/
+-rw-r--r--   0 runner    (1001) docker     (127)    28984 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/base.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    52584 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/forearm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    33784 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/shoulder.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    58884 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/upperarm.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist2.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist3.stl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.941388 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)   193387 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/base.obj
+-rw-r--r--   0 runner    (1001) docker     (127)  1960914 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/forearm.obj
+-rw-r--r--   0 runner    (1001) docker     (127)  1308382 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/shoulder.obj
+-rw-r--r--   0 runner    (1001) docker     (127)  2936777 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/upperarm.obj
+-rw-r--r--   0 runner    (1001) docker     (127)  1354955 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist1.obj
+-rw-r--r--   0 runner    (1001) docker     (127)  1352873 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist2.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   164202 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist3.obj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.941388 compas_robots-0.4.0/src/compas_robots/data/ur_description/urdf/
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/data/ur_description/urdf/ur5.urdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.941388 compas_robots-0.4.0/src/compas_robots/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/files/urdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/ghpython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/ghpython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/ghpython/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/ghpython/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/ghpython/scene/robotmodelobject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/model/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/model/joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/model/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39083 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/model/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/model/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/resources/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/resources/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/resources/mesh_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/rhino/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/rhino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/rhino/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/rhino/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/rhino/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/rhino/scene/robotmodelobject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/scene/baserobotmodelobject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.945388 compas_robots-0.4.0/src/compas_robots/viewer/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/viewer/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-04-29 15:46:24.000000 compas_robots-0.4.0/src/compas_robots/viewer/scene/robotmodelobject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:46:36.929388 compas_robots-0.4.0/src/compas_robots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-29 15:46:36.000000 compas_robots-0.4.0/src/compas_robots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-29 15:46:36.000000 compas_robots-0.4.0/src/compas_robots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:46:36.000000 compas_robots-0.4.0/src/compas_robots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:46:36.000000 compas_robots-0.4.0/src/compas_robots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 15:46:36.000000 compas_robots-0.4.0/src/compas_robots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 15:46:36.000000 compas_robots-0.4.0/src/compas_robots.egg-info/top_level.txt
```

### Comparing `compas_robots-0.3.0/CHANGELOG.md` & `compas_robots-0.4.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0] 2024-04-29
+
+### Added
+
+* Added support for `compas_viewer`
+
+### Changed
+
+### Removed
+
+
 ## [0.3.0] 2024-02-20
 
 ### Added
 
 ### Changed
 
 * Moved private methods `_get_file_format` and `_mesh_import` to `compas_robots.resources` and made them public (`get_file_format` and `mesh_import`).
```

### Comparing `compas_robots-0.3.0/LICENSE` & `compas_robots-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/PKG-INFO` & `compas_robots-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_robots
-Version: 0.3.0
+Version: 0.4.0
 Summary: Basic infrastructure for working with robots in COMPAS.
 Home-page: https://github.com/compas-dev/compas_robots
 Author: Gonzalo Casas
 Author-email: casas@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_robots-0.3.0/README.md` & `compas_robots-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/pyproject.toml` & `compas_robots-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/setup.py` & `compas_robots-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="compas_robots",
-    version="0.3.0",
+    version="0.4.0",
     description="Basic infrastructure for working with robots in COMPAS.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/compas-dev/compas_robots",
     author="Gonzalo Casas",
     author_email="casas@arch.ethz.ch",
     license="MIT license",
```

### Comparing `compas_robots-0.3.0/src/compas_robots/__init__.py` & `compas_robots-0.4.0/src/compas_robots/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import os
 
 __author__ = ["Gonzalo Casas"]
 __copyright__ = "COMPAS Association"
 __license__ = "MIT License"
 __email__ = "casas@arch.ethz.ch"
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 
 from .configuration import Configuration
 from .model.robot import RobotModel
 from .model.tool import ToolModel
 
 HERE = os.path.dirname(__file__)
@@ -41,10 +41,11 @@
 
 
 __all__ = ["Configuration", "RobotModel", "ToolModel", "get"]
 
 __all_plugins__ = [
     "compas_robots.blender.scene",
     "compas_robots.ghpython.scene",
+    "compas_robots.viewer.scene",
     "compas_robots.rhino.scene",
     "compas_robots.rhino.install",
 ]
```

### Comparing `compas_robots-0.3.0/src/compas_robots/blender/scene/robotmodelobject.py` & `compas_robots-0.4.0/src/compas_robots/blender/scene/robotmodelobject.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/configuration.py` & `compas_robots-0.4.0/src/compas_robots/configuration.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/base.stl` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/base.stl`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/forearm.stl` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/forearm.stl`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/shoulder.stl` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/shoulder.stl`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/upperarm.stl` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/upperarm.stl`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist1.stl` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist1.stl`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist2.stl` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist2.stl`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist3.stl` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/collision/wrist3.stl`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/base.obj` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/base.obj`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/forearm.obj` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/forearm.obj`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/shoulder.obj` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/shoulder.obj`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/upperarm.obj` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/upperarm.obj`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist1.obj` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist1.obj`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist2.obj` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist2.obj`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist3.obj` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/meshes/ur5/visual/wrist3.obj`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/data/ur_description/urdf/ur5.urdf` & `compas_robots-0.4.0/src/compas_robots/data/ur_description/urdf/ur5.urdf`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/files/urdf.py` & `compas_robots-0.4.0/src/compas_robots/files/urdf.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/ghpython/scene/robotmodelobject.py` & `compas_robots-0.4.0/src/compas_robots/ghpython/scene/robotmodelobject.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/model/__init__.py` & `compas_robots-0.4.0/src/compas_robots/model/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/model/base.py` & `compas_robots-0.4.0/src/compas_robots/model/base.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/model/geometry.py` & `compas_robots-0.4.0/src/compas_robots/model/geometry.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/model/joint.py` & `compas_robots-0.4.0/src/compas_robots/model/joint.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/model/link.py` & `compas_robots-0.4.0/src/compas_robots/model/link.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/model/robot.py` & `compas_robots-0.4.0/src/compas_robots/model/robot.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/model/tool.py` & `compas_robots-0.4.0/src/compas_robots/model/tool.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/resources/basic.py` & `compas_robots-0.4.0/src/compas_robots/resources/basic.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/resources/github.py` & `compas_robots-0.4.0/src/compas_robots/resources/github.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/resources/mesh_importer.py` & `compas_robots-0.4.0/src/compas_robots/resources/mesh_importer.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/rhino/scene/robotmodelobject.py` & `compas_robots-0.4.0/src/compas_robots/rhino/scene/robotmodelobject.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots/scene/baserobotmodelobject.py` & `compas_robots-0.4.0/src/compas_robots/scene/baserobotmodelobject.py`

 * *Files identical despite different names*

### Comparing `compas_robots-0.3.0/src/compas_robots.egg-info/PKG-INFO` & `compas_robots-0.4.0/src/compas_robots.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas-robots
-Version: 0.3.0
+Version: 0.4.0
 Summary: Basic infrastructure for working with robots in COMPAS.
 Home-page: https://github.com/compas-dev/compas_robots
 Author: Gonzalo Casas
 Author-email: casas@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_robots-0.3.0/src/compas_robots.egg-info/SOURCES.txt` & `compas_robots-0.4.0/src/compas_robots.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -50,8 +50,11 @@
 src/compas_robots/resources/github.py
 src/compas_robots/resources/mesh_importer.py
 src/compas_robots/rhino/__init__.py
 src/compas_robots/rhino/install.py
 src/compas_robots/rhino/scene/__init__.py
 src/compas_robots/rhino/scene/robotmodelobject.py
 src/compas_robots/scene/__init__.py
-src/compas_robots/scene/baserobotmodelobject.py
+src/compas_robots/scene/baserobotmodelobject.py
+src/compas_robots/viewer/__init__.py
+src/compas_robots/viewer/scene/__init__.py
+src/compas_robots/viewer/scene/robotmodelobject.py
```

